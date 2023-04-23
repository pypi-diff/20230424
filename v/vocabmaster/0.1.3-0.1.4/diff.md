# Comparing `tmp/vocabmaster-0.1.3.tar.gz` & `tmp/vocabmaster-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.3.tar", last modified: Sun Apr 23 18:11:53 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.4.tar", last modified: Sun Apr 23 23:23:47 2023, max compression
```

## Comparing `vocabmaster-0.1.3.tar` & `vocabmaster-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.3/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2560 2023-04-23 17:55:42.000000 vocabmaster-0.1.3/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 18:11:40.000000 vocabmaster-0.1.3/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.865177 vocabmaster-0.1.3/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.3/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18018 2023-04-23 18:08:54.000000 vocabmaster-0.1.3/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.3/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.3/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.3/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.3/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 18:11:53.875177 vocabmaster-0.1.3/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2693 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 18:11:53.000000 vocabmaster-0.1.3/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.4/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2594 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2461 2023-04-23 22:56:29.000000 vocabmaster-0.1.4/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 23:22:55.000000 vocabmaster-0.1.4/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.4/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18244 2023-04-23 23:21:09.000000 vocabmaster-0.1.4/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.4/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.4/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.4/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.4/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2594 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.3/LICENSE` & `vocabmaster-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.3/PKG-INFO` & `vocabmaster-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.3
+Version: 0.1.4
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
@@ -55,28 +55,26 @@
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
-You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
-
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.bash
+source /path/to/vocabmaster/completion/_complete_vocabmaster.bash
 ```
 
 #### For zsh:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.zsh
+source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
```

### Comparing `vocabmaster-0.1.3/README.md` & `vocabmaster-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,28 +48,26 @@
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
-You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
-
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.bash
+source /path/to/vocabmaster/completion/_complete_vocabmaster.bash
 ```
 
 #### For zsh:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.zsh
+source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
```

### Comparing `vocabmaster-0.1.3/setup.py` & `vocabmaster-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.3/vocabmaster/cli.py` & `vocabmaster-0.1.4/vocabmaster/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,17 @@
         )
         click.echo(f"Run '{BOLD}vocabmaster add --help{RESET}' for more information.")
         return
 
     # Show untranslated words count if `--count` is used, then exit.
     if count:
         try:
-            number_words = len(csv_handler.get_words_to_translate(translations_filepath))
+            number_words = len(
+                csv_handler.get_words_to_translate(translations_filepath)
+            )
             click.echo(f"Number of words to translate: {BLUE}{number_words}{RESET}")
         except Exception as error:
             click.echo(f"{GREEN}Status:{RESET} {error}")
         return
 
     # Check for OpenAI API key
     if not openai_api_key_exists():
@@ -200,18 +202,21 @@
 @vocabmaster.command()
 def anki():
     """
     Generate an Anki deck from your vocabulary list.
 
     The Anki deck will be saved in the same folder as your vocabulary list.
     """
-    language_to_learn, mother_tongue = config_handler.get_default_language_pair()
+    language_to_learn = config_handler.get_default_language_pair()["language_to_learn"]
+    mother_tongue = config_handler.get_default_language_pair()["mother_tongue"]
+
     translations_filepath, anki_filepath = setup_files(
         setup_dir(), language_to_learn, mother_tongue
     )
+
     generate_anki_deck(translations_filepath, anki_filepath)
 
 
 @vocabmaster.command()
 def setup():
     """
     Set up a new language pair.
@@ -270,15 +275,17 @@
     else:
         print_default_language_pair()
 
         if click.confirm("Do you want to set this language pair as the default?"):
             if click.confirm(
                 f"{RED}Are you sure?{RESET} This will overwrite the current default 🚨"
             ):
-                config_handler.set_default_language_pair(language_to_learn, mother_tongue)
+                config_handler.set_default_language_pair(
+                    language_to_learn, mother_tongue
+                )
             click.echo()
             click.echo("This language pair has been set as the default ✅")
             click.echo(f"{BLUE}The new default language pair is:{RESET}")
 
             # Get the new default language pair by reinitalizing the variables to avoid confusion
             default_language_to_learn = config_handler.get_default_language_pair()[
                 "language_to_learn"
@@ -334,15 +341,15 @@
     Example usage:
     'vocabmaster config default'
 
     Example usage:
     'vocabmaster config key'
     """
     # the directory where the translations and Anki decks are stored,
-    #Example usage:
+    # Example usage:
     #'vocabmaster config dir'
     pass
 
 
 @config.command("default")
 def config_default_language_pair():
     """
@@ -364,15 +371,17 @@
     if choice.isdigit():
         idx = int(choice) - 1
         if 0 <= idx < len(config_handler.get_all_language_pairs()):
             # Set the language pair as the default
             language_to_learn = config_handler.get_all_language_pairs()[idx][
                 "language_to_learn"
             ]
-            mother_tongue = config_handler.get_all_language_pairs()[idx]["mother_tongue"]
+            mother_tongue = config_handler.get_all_language_pairs()[idx][
+                "mother_tongue"
+            ]
             config_handler.set_default_language_pair(language_to_learn, mother_tongue)
             click.echo(
                 f"{BOLD}{language_to_learn}:{mother_tongue}{RESET} {GREEN} has been set"
                 f" as the default language pair{RESET} ✅"
             )
         else:
             # The user entered a number that is out of range
@@ -399,16 +408,16 @@
         config_handler.set_default_language_pair(language_to_learn, mother_tongue)
         click.echo(
             f"{BOLD}{language_to_learn}:{mother_tongue}{RESET} {GREEN} has been set as"
             f" the default language pair{RESET} ✅"
         )
 
 
-#@config.command("dir")
-#def config_dir():
+# @config.command("dir")
+# def config_dir():
 #    """
 #    Set the directory where the list and the Anki deck are stored.
 #    """
 #    custom_app_data_dir = click.prompt("Enter the path for the new directory", type=str)
 #    setup_dir(custom_app_data_dir)
 
 
@@ -417,15 +426,16 @@
     """
     Set the OpenAI API key.
     """
     if openai_api_key_exists():
         click.echo(f"{GREEN}OpenAI API key found!{RESET}")
         click.echo()
         click.echo(
-            f"You can use '{BOLD}vocabmaster translate{RESET}' to generate translations."
+            f"You can use '{BOLD}vocabmaster translate{RESET}' to generate"
+            " translations."
         )
         click.echo()
         click.echo(
             "If you only want to generate your Anki deck, you can use"
             f" '{BOLD}vocabmaster anki{RESET}'."
         )
     if not openai_api_key_exists():
@@ -442,15 +452,17 @@
         "You can generate API keys in the OpenAI web interface. See"
         " https://platform.openai.com/account/api-keys for details."
     )
     click.echo()
     if platform.system() == "Windows":
         click.echo(f"Then, you can set it up by running `setx OPENAI_API_KEY your_key`")
     else:
-        click.echo(f"Then, you can set it up by running `export OPENAI_API_KEY=YOUR_KEY`")
+        click.echo(
+            f"Then, you can set it up by running `export OPENAI_API_KEY=YOUR_KEY`"
+        )
     return
 
 
 @vocabmaster.command()
 def show():
     """
     Show all the language pairs that have been set up.
@@ -521,16 +533,16 @@
     for idx, language_pair in enumerate(language_pairs, start=1):
         click.echo(
             f"{idx}."
             f" {language_pair['language_to_learn']}:{language_pair['mother_tongue']}"
         )
     click.echo()
 
+
 vocabmaster.add_command(config)
 vocabmaster.add_command(anki)
 vocabmaster.add_command(translate)
 vocabmaster.add_command(add)
 vocabmaster.add_command(anki)
 vocabmaster.add_command(default)
 vocabmaster.add_command(show)
 vocabmaster.add_command(tokens)
-
```

### Comparing `vocabmaster-0.1.3/vocabmaster/config_handler.py` & `vocabmaster-0.1.4/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.3/vocabmaster/csv_handler.py` & `vocabmaster-0.1.4/vocabmaster/csv_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.3/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.4/vocabmaster/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.3/vocabmaster/utils.py` & `vocabmaster-0.1.4/vocabmaster/utils.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.3/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.4/vocabmaster.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.3
+Version: 0.1.4
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
@@ -55,28 +55,26 @@
 
 ```
 pipx install vocabmaster
 ```
 
 ### Shell Completion
 
-You should have autocompletion after the installation. If that's not the case, you can follow the instructions below.
-
 To enable shell completion for bash or zsh, source the completion file (see the `completion` folder) related to your shell by adding the following line to your `.bashrc` or `.zshrc` file:
 
 #### For bash:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.bash
+source /path/to/vocabmaster/completion/_complete_vocabmaster.bash
 ```
 
 #### For zsh:
 
 ```
-source /path/to/vocabmaster/completion/vocabmaster.zsh
+source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
```


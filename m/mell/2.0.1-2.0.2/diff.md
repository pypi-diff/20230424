# Comparing `tmp/mell-2.0.1.tar.gz` & `tmp/mell-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.1.tar", last modified: Sun Apr 23 00:43:24 2023, max compression
+gzip compressed data, was "mell-2.0.2.tar", last modified: Mon Apr 24 00:31:38 2023, max compression
```

## Comparing `mell-2.0.1.tar` & `mell-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/
--rw-rw-r--   0 diego     (1000) diego     (1000)    10046 2023-04-23 00:43:24.591577 mell-2.0.1/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     9594 2023-04-23 00:43:10.000000 mell-2.0.1/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/mell/
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-22 21:31:52.000000 mell-2.0.1/mell/__init__.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    15036 2023-04-23 00:37:24.000000 mell-2.0.1/mell/main.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-23 00:43:24.591577 mell-2.0.1/mell.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)    10046 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      218 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-23 00:43:24.000000 mell-2.0.1/mell.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-23 00:43:24.591577 mell-2.0.1/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)     1062 2023-04-23 00:38:25.000000 mell-2.0.1/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.185941 mell-2.0.2/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    14237 2023-04-24 00:31:38.185941 mell-2.0.2/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    13785 2023-04-24 00:03:39.000000 mell-2.0.2/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.181941 mell-2.0.2/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-22 21:31:52.000000 mell-2.0.2/mell/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      238 2023-04-24 00:31:32.000000 mell-2.0.2/mell/consts.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    21618 2023-04-24 00:30:51.000000 mell-2.0.2/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.181941 mell-2.0.2/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    14237 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      233 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-24 00:31:38.185941 mell-2.0.2/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-23 13:44:11.000000 mell-2.0.2/setup.py
```

### Comparing `mell-2.0.1/PKG-INFO` & `mell-2.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,242 +1,340 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Metaprogramming Logic Layer designed to generate anything from template files
 Home-page: https://github.com/diegofps/pywup
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: full
 
 # Mell
 
-Mell is a Metaprogramming Logic Layer designer to generate anything from template files.
+Mell is a Metaprogramming Logic Layer designed to generate anything from template files. 
 
 # Why do I need this?
 
-There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that I use mell. So far, I have used its concept in the following situations:
+There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that you may want to use mell. So far, I have used it in the following situations:
 
-* Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes present in the language.
-* Generating database model classes. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
-* Generating resumes to send to job applications. I use latex to generate my resume, instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source which I compile to PDF.
+* Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
+* Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
+* Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
-Conceptually, you may use mell in two directions. A metadata being used with multiple styles, representing different projections of the same thing, or a single style being used by multiple metadata, creating different things with the same look. 
+Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
-As an example, consider the situation that we have metadata describing a mobile app and our style can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on another platform, an Apple app perhaps.
+As an example, consider the situation that we have metadata describing a mobile app and a style that can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on different platforms, like an IOS app.
 
 
 # When should I not use this?
 
-I don't recommend using this if you are not confortable programming in the language you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just repeating with a few different parameters. These few parameters will become your metadata.
+I don't recommend using this if you are not confortable programming in the stack you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just the same with a few different parameters. These few parameters will likely become your metadata when you use mell.
 
-You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to which of them is better depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime.
+You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
 # Concepts
 
 To use this library you must understand a few concepts. These are:
 
 * `metadata:` These is data describing what we want to generate. We use json format for it.
-* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, and plugins.
+* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, plugins, and logic rules.
 * `generated folder:` This is where the rendered files will be saved and you must never change these files. However, you may want to execute or compile them if you are generating a webserver or a latex template, for instance. 
-* `template:` These are models with missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
-* `static:` These are files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
-* `asset:` These are files used by your logic layer but that are not automatically used by mell.
+
+A style is composed of the following concepts:
+
+* `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
+* `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
+* `asset:` files used by your style that are not automatically used by mell.
 * `plugin:` Scripts that will be executed by mell. These usually access the files in the asset folder.
+* `logic:` Scripts that will be executed in order by mell. These are used to validate and extend the metadata.
 
-# Folder structure
+# Basic folder structure
 
 The following table describes the folders used by mell.
 
 | Folder  | Description | 
 |-------------|-------------|
 | \<root\> | The base folder that contains all folders described here |
 | \<root\>/style | The base folder for template, static, plugin, and asset |
 | \<root\>/generate | this will hold the generated data, never edit this folder |
 | \<root\>/meta | holds all metadata as json files |
 | \<root\>/style/template | holds the template files that will be automatically rendered and written to the generated folder |
 | \<root\>/style/static | contains static files that will be copied as they are to the generate folder |
 | \<root\>/style/plugin | contains scripts that will be executed by mell. Use these to render multiple files from templates in the asset folder |
 | \<root\>/style/asset | contains template and other files that are not automatically used by mell. They may be used by plugins or other tools |
+| \<root\>/style/logic | contains scripts used automatically executed by mell to transform the metadata |
 
-# How to install / uninstall it?
+If you want to create a new project using this structure with the root folder named testing_mell, you can use the following command.
 
+```shell
+mell --new testing_mell
 ```
+
+# How to install / uninstall it?
+
+```shell
 # To install
 pip install mell
 
 # To upgrade
 pip install --upgrade mell
 
 # To uninstall
 pip uninstall mell
 ```
 
-# Give me Examples!
+After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your $PATH variable includes the local bin directory that pip uses; (2) install it in a virtual environment, like virtualenv; or (3) try to install it at the system level, running pip as root;
 
-## Using the template folder
+# Generating Hello Worlds
 
 This will demonstrate how to use mell in a simple use case, changing the language for a static interface. You may be thinking now, "what a naive example, most web frameworks have much more powerful internationalization tools and I would never use it for that". Indeed, me neither. I used this in my resumes in latex, though. By doing this I had a different metadata for each place I would apply, some in portuguese, some in english, some specific for each position. Another benefit is that I could update the resume by changing only a single file. I could generate old ones again, they had their own metadata, and so on.
 
-Create a new mell project and enter it.
+## Step 1. Create a new mell project
+
+Execute the following command to create the standard structure.
 
 ```shell
 mell --new template_test
 cd template_test
 ```
 
-Create the file `<root>/template/main.py` with the following content.
+Now, we will create a second style, named `style2`. We will make `style` render a program that prints a message using python and `style2` will render a program that prints a message using cpp.
 
-```python
-print(|= meta["message"] =|)
+```shell
+mell --new-style style2
 ```
 
-Create the file `<root>/meta/pt.json` with the following content.
+## Step 2. Create the metadata files
+
+This is the content for `<root>/meta/en.json`.
 
 ```json
-{ "message": "Olá Mundo" }
+{
+    "message": "Hello World"
+}
 ```
 
-Create the file `./meta/en.json` with the following content.
+This is the content for `<root>/meta/pt.json`.
 
 ```json
-{ "message": "Hello World" }
+{
+    "message": "Olá Mundo" 
+}
 ```
 
-Inside the `<root>` folder, execute the following command. The parameter pt is the name of the metadata file we want to use, that is, `<root>/meta/pt.json`.
+## Step 3. Create the contents for style and style2
 
-```shell
-mell pt
+This is the content for `<root>/style/template/main.py`:
+
+```python
+print("|= meta.message =|")
 ```
 
-Mell will generate the following file in `./generate/main.py`.
+This is the content for `<root>/style2/template/main.cpp`.
 
-```python
-print("Olá Mundo")
+```shell
+#include <iostream>
+
+int main()
+{
+    std::cout << "|= meta.message =|" << std::endl;
+    return 0;
+}
 ```
 
-Now, execute the following command:
+## Step 4. Generating the programs
+
+If we only pass the metadata name to mell, it will use the default folders for style and generate folder. The following program will use the metadata file `<root>/meta/en.json`, the style folder `<root>/style`, and render everything to `<root>/generate`.
 
 ```shell
+# This must be executed inside the <root> folder
 mell en
 ```
 
-This time, mell will generate the following file in `./generate/main.py`.
+The command above will generate the following content in `<root>/generate/main.py`
 
 ```shell
 print("Hello World")
 ```
 
-## Using the plugin folder
+The following is the program generated if we execute `mell pt`.
 
-This example will use a metadata to generate a bunch of letters, each addressed to a different client. We will use a plugin because the number of clients is defined on a list inside the metadata. Therefore, we will use a single template file inside the asset folder and the plugin will generate multiple files in the output. A similar approach could be used to generate model classes for an ORM, for instance.
-
-Create a new mell project and enter it.
-
-```shell
-mell --new plugin_test
-cd plugin_test
+```python
+print("Olá Mundo")
 ```
 
-Create a file in `plugin_test/style/asset/letter.txt` with the following content.
+To generate the cpp program we need to tell mell to use the style in style2. This can be done with the following command.
 
+```shell
+# This must be executed inside the <root> folder
+mell --style style2 en
 ```
-Dear |= meta["name"] =|,
 
-As you have added the item |= meta["product"] =| on your wishlist, I am here to tell you that this item is now available with a discount of |= meta["discount"] =|. 
+The command above will generate the following content in `<root>/generate/main.cpp`
 
-If this is still of your interest, you can check it [here](|= meta["product_url"] =|). If you want to see or manage your entire wishlist you may click [here](http://shopping.com/wishlist).
+```cpp
+#include <iostream>
 
-Best Regards,
-Bot
+int main()
+{
+    std::cout << "Hello World" << std::endl;
+    return 0;
+}
 ```
 
-Create a file in `plugin_test/style/plugin/example_plugin.py` with the following content.
+The following is the program generated if we execute `mell --style style2 pt`.
 
-```python
-def main(inflater, meta):
-    for i, item in enumerate(meta["clients"]):
-        inflater.inflateAsset("letter.txt", item, to_file=f"examples/letter_{i}.txt")
-```
+```cpp
+#include <iostream>
 
-Create a file in `plugin_test/meta/data.json` with the following content.
-```json
+int main()
 {
-    "clients": [
-        {
-            "name": "Diego",
-            "product": "Tablet",
-            "discount": "50%",
-            "product_url": "http://shopping.com/item/12345"
-        },
-        {
-            "name": "Pedro",
-            "product": "Microscope",
-            "discount": "10%",
-            "product_url": "http://shopping.com/item/54321"
-        },
-        {
-            "name": "Jéssica",
-            "product": "Professional Easel",
-            "discount": "10%",
-            "product_url": "http://shopping.com/item/21543"
-        }
-    ]
+    std::cout << "Olá Mundo" << std::endl;
+    return 0;
 }
 ```
 
-Now, inside the `<root>` folder, execute the following command:
+## Step 5. Improving the structure
+
+If you pretend to use just one style, the default folder name is fine, but for multiple style it is better to rename and put them into something more representative, like `styles/cpp` and `styles/python`. You may also want to save the output to different output folders. You can do this using the parameter `--generate`. The following is an example of all four combinations using the new style structure.
 
 ```shell
-mell data
-```
+# Create new folders to keep our styles
+mkdir styles
 
-Three files will be generated in `<root>/generate/examples`. The first file is `letter_0.txt`, containing the following content. The remaining files contain similar content, but with their remaining data:
+# Rename the style folders
+mv style styles/python
+mv style2 styles/cpp
+
+# Generate the programs and save them in different folders
+mell --style styles/cpp --generate generates/cpp/en en
+mell --style styles/cpp --generate generates/cpp/pt pt
+mell --style styles/python --generate generates/python/en en
+mell --style styles/python --generate generates/python/pt pt
+```
+
+This is how the project looks like in the end.
+
+```perl
+.
+├── generates
+│   ├── cpp
+│   │   ├── en
+│   │   │   └── main.cpp
+│   │   └── pt
+│   │       └── main.cpp
+│   └── python
+│       ├── en
+│       │   └── main.py
+│       └── pt
+│           └── main.py
+├── meta
+│   ├── en.json
+│   └── pt.json
+└── styles
+    ├── cpp
+    │   ├── asset
+    │   ├── plugin
+    │   ├── static
+    │   └── template
+    │       └── main.cpp
+    └── python
+        ├── asset
+        ├── plugin
+        ├── static
+        └── template
+            └── main.py
+```
+
+# The Pipeline
+
+Sometimes it is important to understand the order in which the operations are executed. The list below describe these operations in their standard order.
+
+1. Load metadata
+1. Execute logic scripts
+1. Actions to generate the output:
+>4. Clean output folder [clean]
+>1. Copy static files [static]
+>1. Render templates and copy them to output [template]
+>1. Execute plugin scripts [plugin]
 
-```
-Dear Diego,
+Loading the metadata and executing the logic scripts is always executed first and can't be changed. The list of actions to generate the output, though, can be modified or canceled. To modify the list of actions we use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
 
-As you have added the item Tablet on your wishlist, I am here to tell you that this item is now available with a discount of 50%. 
+```shell
+# These two calls are the same
+mell --do clean --do static --do template --do plugin data
+mell data
+
+# This will only generate output files based on the template folder
+mell --do template data
 
-If this is still of your interest, you can check it [here](http://shopping.com/item/12345). If you want to see or manage your entire wishlist you may click [here](http://shopping.com/wishlist).
+# This will only clean the generated folder
+mell --do clean data
 
-Best Regards,
-Bot
+# The word 'nothing' is a special keyword. It will not do any action but will still load the metadata and execute logic scripts. This is useful when used with -v (verose mode) or --show-metadata (display the metadata after executing the logic scripts).
+mell --do nothing data
+mell --do nothing -v data
+mell --do nothing --show-metadata data
 ```
 
-## Special Command Options
+# Tutorials
+
+* [Metadata](https://github.com/diegofps/mell/blob/main/docs/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
+* [Template](https://github.com/diegofps/mell/blob/main/docs/template.md) - Explains the template syntax and how to customize it;
+* [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
+* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend extend the input metadata, generating more metadata and preventing complex rules in template files.
+
+# List of useful command options
 
 These are a few examples of common operations.
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
 mell --new project_name
 
 # This will create a folder named style2 with the recommended style folder structure (use it inside the root directory to keep things organized)
 mell --new-style project_name
 
+# Create a new plugin file as <root>/style/plugin/plugin_name.py
+mell --new-plugin plugin_name
+
+# Create a new logic file as <root>/style/logic/<timestamp>.logic_name.py
+mell --new-logic logic_name
+
+# Display the version number and exit
+mell --version
+
 # Display more info during execution (verbose mode)
 mell -v en
 
 # Display less info during execution (quiet mode)
 mell -q en
 
 # Specify what we want to generate
-mell -d clean -d static -d template -d plugin en
+mell --do clean --do static --do template --do plugin en
 
 # Only clean the output folder
-mell -d clean en
+mell --do clean en
 
 # Only generate files from templates
-mell -d template en
+mell --do template en
 
 # Specify a different style folder. This will make mell use the folders template, asset, plugin, and static that inside it.
 mell --style style2 en
+
+# Specify a different generate folder. This is useful if you have multiple styles and want to generate different things on different folders.
+mell --generate generate2 en
+
+# An example with custom style names, distinct output folders and two metadata files. We are assuming the style folders are on local directory and named python and cpp.
+mell --style styles/python --generate generates/python/en en
+mell --style styles/python --generate generates/python/pt pt
+mell --style styles/cpp --generate generates/cpp/en en
+mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
 # Source Code
 
 The source code is available [here](https://github.com/diegofps/mell)
```

### Comparing `mell-2.0.1/mell.egg-info/PKG-INFO` & `mell-2.0.2/mell.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,242 +1,340 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Metaprogramming Logic Layer designed to generate anything from template files
 Home-page: https://github.com/diegofps/pywup
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: full
 
 # Mell
 
-Mell is a Metaprogramming Logic Layer designer to generate anything from template files.
+Mell is a Metaprogramming Logic Layer designed to generate anything from template files. 
 
 # Why do I need this?
 
-There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that I use mell. So far, I have used its concept in the following situations:
+There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that you may want to use mell. So far, I have used it in the following situations:
 
-* Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes present in the language.
-* Generating database model classes. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
-* Generating resumes to send to job applications. I use latex to generate my resume, instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source which I compile to PDF.
+* Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
+* Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
+* Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
-Conceptually, you may use mell in two directions. A metadata being used with multiple styles, representing different projections of the same thing, or a single style being used by multiple metadata, creating different things with the same look. 
+Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
-As an example, consider the situation that we have metadata describing a mobile app and our style can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on another platform, an Apple app perhaps.
+As an example, consider the situation that we have metadata describing a mobile app and a style that can render an Android app. We could change the metadata and generate different Android apps, or we could change the style and render the same app on different platforms, like an IOS app.
 
 
 # When should I not use this?
 
-I don't recommend using this if you are not confortable programming in the language you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just repeating with a few different parameters. These few parameters will become your metadata.
+I don't recommend using this if you are not confortable programming in the stack you are generating code to, as the template files may elevate your project complexity. This works better if are at a point where you feel like everything is just the same with a few different parameters. These few parameters will likely become your metadata when you use mell.
 
-You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to which of them is better depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime.
+You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
 # Concepts
 
 To use this library you must understand a few concepts. These are:
 
 * `metadata:` These is data describing what we want to generate. We use json format for it.
-* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, and plugins.
+* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, plugins, and logic rules.
 * `generated folder:` This is where the rendered files will be saved and you must never change these files. However, you may want to execute or compile them if you are generating a webserver or a latex template, for instance. 
-* `template:` These are models with missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
-* `static:` These are files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
-* `asset:` These are files used by your logic layer but that are not automatically used by mell.
+
+A style is composed of the following concepts:
+
+* `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
+* `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
+* `asset:` files used by your style that are not automatically used by mell.
 * `plugin:` Scripts that will be executed by mell. These usually access the files in the asset folder.
+* `logic:` Scripts that will be executed in order by mell. These are used to validate and extend the metadata.
 
-# Folder structure
+# Basic folder structure
 
 The following table describes the folders used by mell.
 
 | Folder  | Description | 
 |-------------|-------------|
 | \<root\> | The base folder that contains all folders described here |
 | \<root\>/style | The base folder for template, static, plugin, and asset |
 | \<root\>/generate | this will hold the generated data, never edit this folder |
 | \<root\>/meta | holds all metadata as json files |
 | \<root\>/style/template | holds the template files that will be automatically rendered and written to the generated folder |
 | \<root\>/style/static | contains static files that will be copied as they are to the generate folder |
 | \<root\>/style/plugin | contains scripts that will be executed by mell. Use these to render multiple files from templates in the asset folder |
 | \<root\>/style/asset | contains template and other files that are not automatically used by mell. They may be used by plugins or other tools |
+| \<root\>/style/logic | contains scripts used automatically executed by mell to transform the metadata |
 
-# How to install / uninstall it?
+If you want to create a new project using this structure with the root folder named testing_mell, you can use the following command.
 
+```shell
+mell --new testing_mell
 ```
+
+# How to install / uninstall it?
+
+```shell
 # To install
 pip install mell
 
 # To upgrade
 pip install --upgrade mell
 
 # To uninstall
 pip uninstall mell
 ```
 
-# Give me Examples!
+After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your $PATH variable includes the local bin directory that pip uses; (2) install it in a virtual environment, like virtualenv; or (3) try to install it at the system level, running pip as root;
 
-## Using the template folder
+# Generating Hello Worlds
 
 This will demonstrate how to use mell in a simple use case, changing the language for a static interface. You may be thinking now, "what a naive example, most web frameworks have much more powerful internationalization tools and I would never use it for that". Indeed, me neither. I used this in my resumes in latex, though. By doing this I had a different metadata for each place I would apply, some in portuguese, some in english, some specific for each position. Another benefit is that I could update the resume by changing only a single file. I could generate old ones again, they had their own metadata, and so on.
 
-Create a new mell project and enter it.
+## Step 1. Create a new mell project
+
+Execute the following command to create the standard structure.
 
 ```shell
 mell --new template_test
 cd template_test
 ```
 
-Create the file `<root>/template/main.py` with the following content.
+Now, we will create a second style, named `style2`. We will make `style` render a program that prints a message using python and `style2` will render a program that prints a message using cpp.
 
-```python
-print(|= meta["message"] =|)
+```shell
+mell --new-style style2
 ```
 
-Create the file `<root>/meta/pt.json` with the following content.
+## Step 2. Create the metadata files
+
+This is the content for `<root>/meta/en.json`.
 
 ```json
-{ "message": "Olá Mundo" }
+{
+    "message": "Hello World"
+}
 ```
 
-Create the file `./meta/en.json` with the following content.
+This is the content for `<root>/meta/pt.json`.
 
 ```json
-{ "message": "Hello World" }
+{
+    "message": "Olá Mundo" 
+}
 ```
 
-Inside the `<root>` folder, execute the following command. The parameter pt is the name of the metadata file we want to use, that is, `<root>/meta/pt.json`.
+## Step 3. Create the contents for style and style2
 
-```shell
-mell pt
+This is the content for `<root>/style/template/main.py`:
+
+```python
+print("|= meta.message =|")
 ```
 
-Mell will generate the following file in `./generate/main.py`.
+This is the content for `<root>/style2/template/main.cpp`.
 
-```python
-print("Olá Mundo")
+```shell
+#include <iostream>
+
+int main()
+{
+    std::cout << "|= meta.message =|" << std::endl;
+    return 0;
+}
 ```
 
-Now, execute the following command:
+## Step 4. Generating the programs
+
+If we only pass the metadata name to mell, it will use the default folders for style and generate folder. The following program will use the metadata file `<root>/meta/en.json`, the style folder `<root>/style`, and render everything to `<root>/generate`.
 
 ```shell
+# This must be executed inside the <root> folder
 mell en
 ```
 
-This time, mell will generate the following file in `./generate/main.py`.
+The command above will generate the following content in `<root>/generate/main.py`
 
 ```shell
 print("Hello World")
 ```
 
-## Using the plugin folder
+The following is the program generated if we execute `mell pt`.
 
-This example will use a metadata to generate a bunch of letters, each addressed to a different client. We will use a plugin because the number of clients is defined on a list inside the metadata. Therefore, we will use a single template file inside the asset folder and the plugin will generate multiple files in the output. A similar approach could be used to generate model classes for an ORM, for instance.
-
-Create a new mell project and enter it.
-
-```shell
-mell --new plugin_test
-cd plugin_test
+```python
+print("Olá Mundo")
 ```
 
-Create a file in `plugin_test/style/asset/letter.txt` with the following content.
+To generate the cpp program we need to tell mell to use the style in style2. This can be done with the following command.
 
+```shell
+# This must be executed inside the <root> folder
+mell --style style2 en
 ```
-Dear |= meta["name"] =|,
 
-As you have added the item |= meta["product"] =| on your wishlist, I am here to tell you that this item is now available with a discount of |= meta["discount"] =|. 
+The command above will generate the following content in `<root>/generate/main.cpp`
 
-If this is still of your interest, you can check it [here](|= meta["product_url"] =|). If you want to see or manage your entire wishlist you may click [here](http://shopping.com/wishlist).
+```cpp
+#include <iostream>
 
-Best Regards,
-Bot
+int main()
+{
+    std::cout << "Hello World" << std::endl;
+    return 0;
+}
 ```
 
-Create a file in `plugin_test/style/plugin/example_plugin.py` with the following content.
+The following is the program generated if we execute `mell --style style2 pt`.
 
-```python
-def main(inflater, meta):
-    for i, item in enumerate(meta["clients"]):
-        inflater.inflateAsset("letter.txt", item, to_file=f"examples/letter_{i}.txt")
-```
+```cpp
+#include <iostream>
 
-Create a file in `plugin_test/meta/data.json` with the following content.
-```json
+int main()
 {
-    "clients": [
-        {
-            "name": "Diego",
-            "product": "Tablet",
-            "discount": "50%",
-            "product_url": "http://shopping.com/item/12345"
-        },
-        {
-            "name": "Pedro",
-            "product": "Microscope",
-            "discount": "10%",
-            "product_url": "http://shopping.com/item/54321"
-        },
-        {
-            "name": "Jéssica",
-            "product": "Professional Easel",
-            "discount": "10%",
-            "product_url": "http://shopping.com/item/21543"
-        }
-    ]
+    std::cout << "Olá Mundo" << std::endl;
+    return 0;
 }
 ```
 
-Now, inside the `<root>` folder, execute the following command:
+## Step 5. Improving the structure
+
+If you pretend to use just one style, the default folder name is fine, but for multiple style it is better to rename and put them into something more representative, like `styles/cpp` and `styles/python`. You may also want to save the output to different output folders. You can do this using the parameter `--generate`. The following is an example of all four combinations using the new style structure.
 
 ```shell
-mell data
-```
+# Create new folders to keep our styles
+mkdir styles
 
-Three files will be generated in `<root>/generate/examples`. The first file is `letter_0.txt`, containing the following content. The remaining files contain similar content, but with their remaining data:
+# Rename the style folders
+mv style styles/python
+mv style2 styles/cpp
+
+# Generate the programs and save them in different folders
+mell --style styles/cpp --generate generates/cpp/en en
+mell --style styles/cpp --generate generates/cpp/pt pt
+mell --style styles/python --generate generates/python/en en
+mell --style styles/python --generate generates/python/pt pt
+```
+
+This is how the project looks like in the end.
+
+```perl
+.
+├── generates
+│   ├── cpp
+│   │   ├── en
+│   │   │   └── main.cpp
+│   │   └── pt
+│   │       └── main.cpp
+│   └── python
+│       ├── en
+│       │   └── main.py
+│       └── pt
+│           └── main.py
+├── meta
+│   ├── en.json
+│   └── pt.json
+└── styles
+    ├── cpp
+    │   ├── asset
+    │   ├── plugin
+    │   ├── static
+    │   └── template
+    │       └── main.cpp
+    └── python
+        ├── asset
+        ├── plugin
+        ├── static
+        └── template
+            └── main.py
+```
+
+# The Pipeline
+
+Sometimes it is important to understand the order in which the operations are executed. The list below describe these operations in their standard order.
+
+1. Load metadata
+1. Execute logic scripts
+1. Actions to generate the output:
+>4. Clean output folder [clean]
+>1. Copy static files [static]
+>1. Render templates and copy them to output [template]
+>1. Execute plugin scripts [plugin]
 
-```
-Dear Diego,
+Loading the metadata and executing the logic scripts is always executed first and can't be changed. The list of actions to generate the output, though, can be modified or canceled. To modify the list of actions we use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
 
-As you have added the item Tablet on your wishlist, I am here to tell you that this item is now available with a discount of 50%. 
+```shell
+# These two calls are the same
+mell --do clean --do static --do template --do plugin data
+mell data
+
+# This will only generate output files based on the template folder
+mell --do template data
 
-If this is still of your interest, you can check it [here](http://shopping.com/item/12345). If you want to see or manage your entire wishlist you may click [here](http://shopping.com/wishlist).
+# This will only clean the generated folder
+mell --do clean data
 
-Best Regards,
-Bot
+# The word 'nothing' is a special keyword. It will not do any action but will still load the metadata and execute logic scripts. This is useful when used with -v (verose mode) or --show-metadata (display the metadata after executing the logic scripts).
+mell --do nothing data
+mell --do nothing -v data
+mell --do nothing --show-metadata data
 ```
 
-## Special Command Options
+# Tutorials
+
+* [Metadata](https://github.com/diegofps/mell/blob/main/docs/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
+* [Template](https://github.com/diegofps/mell/blob/main/docs/template.md) - Explains the template syntax and how to customize it;
+* [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
+* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend extend the input metadata, generating more metadata and preventing complex rules in template files.
+
+# List of useful command options
 
 These are a few examples of common operations.
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
 mell --new project_name
 
 # This will create a folder named style2 with the recommended style folder structure (use it inside the root directory to keep things organized)
 mell --new-style project_name
 
+# Create a new plugin file as <root>/style/plugin/plugin_name.py
+mell --new-plugin plugin_name
+
+# Create a new logic file as <root>/style/logic/<timestamp>.logic_name.py
+mell --new-logic logic_name
+
+# Display the version number and exit
+mell --version
+
 # Display more info during execution (verbose mode)
 mell -v en
 
 # Display less info during execution (quiet mode)
 mell -q en
 
 # Specify what we want to generate
-mell -d clean -d static -d template -d plugin en
+mell --do clean --do static --do template --do plugin en
 
 # Only clean the output folder
-mell -d clean en
+mell --do clean en
 
 # Only generate files from templates
-mell -d template en
+mell --do template en
 
 # Specify a different style folder. This will make mell use the folders template, asset, plugin, and static that inside it.
 mell --style style2 en
+
+# Specify a different generate folder. This is useful if you have multiple styles and want to generate different things on different folders.
+mell --generate generate2 en
+
+# An example with custom style names, distinct output folders and two metadata files. We are assuming the style folders are on local directory and named python and cpp.
+mell --style styles/python --generate generates/python/en en
+mell --style styles/python --generate generates/python/pt pt
+mell --style styles/cpp --generate generates/cpp/en en
+mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
 # Source Code
 
 The source code is available [here](https://github.com/diegofps/mell)
```


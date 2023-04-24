# Comparing `tmp/ascii-cli-0.1.3.tar.gz` & `tmp/ascii-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.1.3.tar", last modified: Thu Apr 20 08:26:36 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.4.tar", last modified: Mon Apr 24 02:56:17 2023, max compression
```

## Comparing `ascii-cli-0.1.3.tar` & `ascii-cli-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.560652 ascii-cli-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2566 2023-04-20 08:26:36.559648 ascii-cli-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-04-20 07:43:25.000000 ascii-cli-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.544648 ascii-cli-0.1.3/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0     2566 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-20 08:26:36.000000 ascii-cli-0.1.3/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 08:26:36.560652 ascii-cli-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-04-20 08:26:03.000000 ascii-cli-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:26:36.556647 ascii-cli-0.1.3/src/
--rw-rw-rw-   0        0        0       20 2023-04-20 06:52:26.000000 ascii-cli-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0     1229 2023-04-20 08:21:27.000000 ascii-cli-0.1.3/src/__main__.py
--rw-rw-rw-   0        0        0     4017 2023-04-20 07:00:43.000000 ascii-cli-0.1.3/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.409306 ascii-cli-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2541 2023-04-24 02:56:17.407318 ascii-cli-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2044 2023-04-24 02:50:58.000000 ascii-cli-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.395301 ascii-cli-0.1.4/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0     2541 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:56:17.409306 ascii-cli-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-04-24 02:55:11.000000 ascii-cli-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.405334 ascii-cli-0.1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 06:05:45.000000 ascii-cli-0.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-04-24 02:47:45.000000 ascii-cli-0.1.4/src/__main__.py
+-rw-rw-rw-   0        0        0     3116 2023-04-24 02:42:00.000000 ascii-cli-0.1.4/src/func.py
```

### Comparing `ascii-cli-0.1.3/LICENSE` & `ascii-cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.3/PKG-INFO` & `ascii-cli-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,14 @@
 
 # Command Line ASCII Art Generator
 
 ASCII-cli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
 
 ---
 
-## TODO
-
-- Colour
-- UI
-
----
-
 ## Installation & Building
 
 ### PIP
 
 The easiest way to install ASCII-CLI is by using the [PyPI library](https://pypi.org/project/ascii-cli/).
 You can run `pip install ascii-cli` on any command-line with Python3 in order to install it.
 
@@ -37,28 +30,30 @@
 
 If you are unable to use the PyPI library you can access ASCII-CLI by going to our [releases page](https://github.com/mrq-andras/ascii-cli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\ascii-cli`
 
 ---
 
 ## Usage
 
-`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] path/to/your/image`
+`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
 Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
 Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
 Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
-If you have downloaded the application through pip input the following command in the terminal:  
+If you have downloaded the application through pip input the following command in the terminal:
 `ascii-cli --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI  
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI
 `.\path\to\ascii-cli.exe --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
 This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
 
 Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
 
+---
+
 ## License
 
 See [`LICENSE`](./LICENSE)
```

### Comparing `ascii-cli-0.1.3/README.md` & `ascii-cli-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 # Command Line ASCII Art Generator
 
 ASCII-cli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
 
 ---
 
-## TODO
-
-- Colour
-- UI
-
----
-
 ## Installation & Building
 
 ### PIP
 
 The easiest way to install ASCII-CLI is by using the [PyPI library](https://pypi.org/project/ascii-cli/).
 You can run `pip install ascii-cli` on any command-line with Python3 in order to install it.
 
@@ -22,28 +15,30 @@
 
 If you are unable to use the PyPI library you can access ASCII-CLI by going to our [releases page](https://github.com/mrq-andras/ascii-cli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\ascii-cli`
 
 ---
 
 ## Usage
 
-`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] path/to/your/image`
+`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
 Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
 Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
 Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
-If you have downloaded the application through pip input the following command in the terminal:  
+If you have downloaded the application through pip input the following command in the terminal:
 `ascii-cli --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI  
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI
 `.\path\to\ascii-cli.exe --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
 This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
 
 Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
 
+---
+
 ## License
 
 See [`LICENSE`](./LICENSE)
```

### Comparing `ascii-cli-0.1.3/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.1.4/ascii_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,14 @@
 
 # Command Line ASCII Art Generator
 
 ASCII-cli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
 
 ---
 
-## TODO
-
-- Colour
-- UI
-
----
-
 ## Installation & Building
 
 ### PIP
 
 The easiest way to install ASCII-CLI is by using the [PyPI library](https://pypi.org/project/ascii-cli/).
 You can run `pip install ascii-cli` on any command-line with Python3 in order to install it.
 
@@ -37,28 +30,30 @@
 
 If you are unable to use the PyPI library you can access ASCII-CLI by going to our [releases page](https://github.com/mrq-andras/ascii-cli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\ascii-cli`
 
 ---
 
 ## Usage
 
-`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] path/to/your/image`
+`ascii-cli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
 Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
 Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
 Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
-If you have downloaded the application through pip input the following command in the terminal:  
+If you have downloaded the application through pip input the following command in the terminal:
 `ascii-cli --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI  
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCII-CLI
 `.\path\to\ascii-cli.exe --width 40 --height 17 --set 1 --random True path\to\input.jpg`
 
 This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
 
 Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
 
+---
+
 ## License
 
 See [`LICENSE`](./LICENSE)
```

### Comparing `ascii-cli-0.1.3/setup.py` & `ascii-cli-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     package_data={'src': ['func.py']},
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `ascii-cli-0.1.3/src/__main__.py` & `ascii-cli-0.1.4/src/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
-from src.func import convert_to_ascii
+from func import convert_to_ascii
+from func import print_cmd
 
 
-def main():
+def arguments():
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
         description="Converts an image to ASCII art.")
     parser.add_argument("path", metavar="path", type=str,
                         help="The path to the image")
     parser.add_argument("--width", type=int, default=62,
@@ -19,13 +20,15 @@
                         help="Character set is scrambled")
     parser.add_argument("--invert", type=bool, default=False,
                         help="Output is inverted")
     parser.add_argument("--darkness", type=int, default=100,
                         help="Darkness of line-art")
     args = parser.parse_args()
 
+    # print out the chosen options
+    print_cmd(args)
     # call the conversion function from ascii.py
     convert_to_ascii(args)
 
 
 if __name__ == '__main__':
-    main()
+    arguments()
```


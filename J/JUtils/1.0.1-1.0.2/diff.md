# Comparing `tmp/JUtils-1.0.1.tar.gz` & `tmp/JUtils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JUtils-1.0.1.tar", last modified: Mon Apr 24 19:21:37 2023, max compression
+gzip compressed data, was "JUtils-1.0.2.tar", last modified: Mon Apr 24 19:25:14 2023, max compression
```

## Comparing `JUtils-1.0.1.tar` & `JUtils-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:21:37.676481 JUtils-1.0.1/
--rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     8852 2023-04-24 19:21:37.676481 JUtils-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8406 2023-04-24 19:19:37.000000 JUtils-1.0.1/README.md
--rw-rw-rw-   0        0        0      522 2023-04-24 19:21:17.000000 JUtils-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 19:21:37.676481 JUtils-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:21:37.652923 JUtils-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:21:37.662961 JUtils-1.0.1/src/JUtils/
--rw-rw-rw-   0        0        0     1721 2023-04-24 19:19:36.000000 JUtils-1.0.1/src/JUtils/AutoDoc.py
--rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-1.0.1/src/JUtils/JArr.py
--rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-1.0.1/src/JUtils/JColors.py
--rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-1.0.1/src/JUtils/JConst.py
--rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-1.0.1/src/JUtils/JConv.py
--rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-1.0.1/src/JUtils/JNum.py
--rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-1.0.1/src/JUtils/JOut.py
--rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-1.0.1/src/JUtils/JStr.py
--rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-1.0.1/src/JUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:21:37.675482 JUtils-1.0.1/src/JUtils.egg-info/
--rw-rw-rw-   0        0        0     8852 2023-04-24 19:21:37.000000 JUtils-1.0.1/src/JUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-04-24 19:21:37.000000 JUtils-1.0.1/src/JUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:21:37.000000 JUtils-1.0.1/src/JUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 19:21:37.000000 JUtils-1.0.1/src/JUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.685768 JUtils-1.0.2/
+-rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8894 2023-04-24 19:25:14.684769 JUtils-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8448 2023-04-24 19:24:15.000000 JUtils-1.0.2/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-24 19:24:44.000000 JUtils-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:25:14.685768 JUtils-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.661541 JUtils-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.672258 JUtils-1.0.2/src/JUtils/
+-rw-rw-rw-   0        0        0     1723 2023-04-24 19:24:12.000000 JUtils-1.0.2/src/JUtils/AutoDoc.py
+-rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-1.0.2/src/JUtils/JArr.py
+-rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-1.0.2/src/JUtils/JColors.py
+-rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-1.0.2/src/JUtils/JConst.py
+-rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-1.0.2/src/JUtils/JConv.py
+-rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-1.0.2/src/JUtils/JNum.py
+-rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-1.0.2/src/JUtils/JOut.py
+-rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-1.0.2/src/JUtils/JStr.py
+-rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-1.0.2/src/JUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.683768 JUtils-1.0.2/src/JUtils.egg-info/
+-rw-rw-rw-   0        0        0     8894 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/top_level.txt
```

### Comparing `JUtils-1.0.1/LICENSE` & `JUtils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/PKG-INFO` & `JUtils-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -47,67 +47,72 @@
     Examples:
         >>> IterComp([1, 2, 3], [1, 2, 3])
         True
         >>> IterComp([1, 2, 3], [1, 2, 4])
         False
         >>> IterComp([1, 2, 3], [1, 2])
         None
-    .```
+    .
+```
 - **flt2d**
 ```
     Flatten a list of lists into a single list. Only for 2d lists, because the inner items should not be flattened.
     
     Parameters:
         arr (list): The list of lists to be flattened.
         
     Returns:
         list: The resulting flattened list.
         
     Example:
         >>> flt([[(), ()], [(), ()]])
         [(), (), (), (), (), ()]
-    .```
+    .
+```
 - **overlp**
 ```
     Checks if elements in l1 and l2 share any same elements
 
     Parameters:
         l1 (list): a list of elements
         l2 (list): a list of elements
 
     Returns:
         bool: if there are any overlaps between l1 and l2
-    .```
+    .
+```
 - **segm**
 ```
     Divide a list into sublists of a specified size.
     
     Parameters:
         arr (list): The list to be divided into sublists.
         n (int): The size of each sublist.
         
     Returns:
         list: A list of sublists, where each sublist contains 'n' elements.
         
     Example:
         >>> segm([1, 1, 1, 1, 1, 1], 2)
         [[1, 1], [1, 1], [1, 1]]
-    .```
+    .
+```
 # JColors
 Color constants importable by name.
 ```py
 from JUtils.JColors import *
 ```
 
 - **randColor**
 ```Returns a random color
     
     Returns:
         tuple: A 3-tuple of integers representing the red, green, and blue components of the color.
-    .```
+    .
+```
 # JConst
 Constants for keeping code clean.
 ```py
 from JUtils.JConst import *
 ```
 
 # JConv
@@ -121,96 +126,104 @@
 
     Args:
         x (float): The x-coordinate.
         y (float): The y-coordinate.
 
     Returns:
         tuple: Polar coordinates (th, r), where r is the distance fromthe origin and th is the angle in degrees.
-    .```
+    .
+```
 - **deg2rad**
 ```Converts an angle in degrees to radians.
 
     Parameters:
         deg (float): An angle in degrees.
 
     Returns:
         float: The equivalent angle in radians.
-    .```
+    .
+```
 - **hex2asc**
 ```
     Convert a string of hexadecimal characters to a string of ASCII characters.
     
     Parameters:
         hx (str): The string of hexadecimal characters to be converted.
         
     Returns:
         str: The resulting string of ASCII characters.
     
     Example:
         >>> hex2asc('0000ff')
         '048048048048102102' #048 048 048 048 102 102
-    .```
+    .
+```
 - **hex2rgb**
 ```
     Convert a hexadecimal string representation to an RGB tuple.
 
     Parameters:
     hx (str): A hexadecimal string representation of an RGB color, in the form '#RRGGBB'.
 
     Returns:
     tuple: An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Example:
     >>> hex2rgb('#ff00ff')
     (255, 0, 255)
-    .```
+    .
+```
 - **pol2cart**
 ```Converts polar coordinates to Cartesian coordinates.
 
     Args:
         ang (float): An angle in degrees.
         r (float): The distance from the origin.
 
     Returns:
         tuple: A tuple of the Cartesian coordinates (x, y).
-    .```
+    .
+```
 - **rad2deg**
 ```Converts an angle in radians to degrees.
 
     Parameters:
         rad (float): An angle in radians.
 
     Returns:
         float: The equivalent angle in degrees.
-    .```
+    .
+```
 - **rgb2gray**
 ```
     Converts an RGB color tuple to a grayscale integer value using the luminosity method.
     
     Args:
         rgb (tuple): A tuple containing 3 integers representing the RGB color values. The values
                      should be in the range of 0-255, inclusive.
                      
     Returns:
         int: The grayscale integer value representing the given RGB color tuple.
-    .```
+    .
+```
 - **rgb2hex**
 ```
     Convert an RGB tuple to a hexadecimal string representation.
 
     Parameters:
     rgb (tuple): An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Returns:
     str: A hexadecimal string representation of the input RGB tuple, in the form '#RRGGBB'.
 
     Example:
     >>> rgb_to_hex((255, 0, 255))
     '#ff00ff'
-    .```
+    .
+```
 # JNum
 Functions for handling numbers.
 ```py
 from JUtils.JNum import *
 ```
 
 - **contain**
@@ -220,53 +233,58 @@
         n (float): The number to be clamped.
         limDown (float): The lower bound of the range.
         limUp (float): The upper bound of the range.
 
     Returns:
         'n' if it is within the range, or the nearest bound if 'n' is outside
         the range.
-    .```
+    .
+```
 - **sTup2Tup**
 ```
     Turns the given string of a tuple to a tuple object.
 
     Parameters:
         s: A tuple in string form.
 
     Returns:
         The tuple as a tuple object.
-    .```
+    .
+```
 - **sgn**
 ```Returns the sign of a number.
 
     Parameters:
         n: An int/float number.
 
     Returns:
         An int representing the sign of 'n'. 1 if 'n' is positive, -1 if 'n'
         is negative, and 0 if 'n' is zero.
-    .```
+    .
+```
 # JOut
 Functions for handling console output.
 ```py
 from JUtils.JOut import *
 ```
 
 - **delayPrint**
 ```Prints the given string with a slight delay after each character.
 
     Parameters:
         s: A string.
-    .```
+    .
+```
 - **printn**
 ```Prints the given arguments, with newlines before and after (works with multiple args like print)
     
     Parameters:
         *args: The arguments to print.
-    .```
+    .
+```
 # JStr
 Functions for string analysing and modification.
 ```py
 from JUtils.JStr import *
 ```
 
 - **listPath**
@@ -274,15 +292,16 @@
     Just like os.listdir(), but with appended path.
     
     Args:
         d: The path to list.
         
     Returns:
         list: A list of paths of files and directories in the given path.
-    .```
+    .
+```
 - **locBrac**
 ```
     Finds the index of the closing bracket that matches the opening bracket at the given index in the given string.
 
     Parameters:
         string (str): The input string.
         brac (str): The bracket character | Possible are ( [ { <
@@ -294,26 +313,28 @@
     Example:
         >>> locBrac('[hello[world]]', '[', 0)
         13
         >>> locBrac('<hello<world>>', '<', 6)
         12
         >>> locBrac('{hello}world}', '{', 0)
         -1
-    .```
+    .
+```
 - **multiCenter**
 ```
     Centers the text in a string by padding spaces on either side of each line.
     
     Args:
         s (str): The input string to center.
         l (int): The desired width of the centered string.
         
     Returns:
         str: The centered string. Each line is padded with spaces on either side to center the text. If
              a line already has an odd number of characters, the extra space is added to the right
              side of the line.
-    .```
+    .
+```
 \
 \
 \
 This Package is not under active development, i will update it every now and then if i find a new function to add.
 Please consider emailing me at: [jan@seifert-online.de](mailto:jan@seifert-online.de) if you got any suggestions for improvement.
```

### Comparing `JUtils-1.0.1/README.md` & `JUtils-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,67 +35,72 @@
     Examples:
         >>> IterComp([1, 2, 3], [1, 2, 3])
         True
         >>> IterComp([1, 2, 3], [1, 2, 4])
         False
         >>> IterComp([1, 2, 3], [1, 2])
         None
-    .```
+    .
+```
 - **flt2d**
 ```
     Flatten a list of lists into a single list. Only for 2d lists, because the inner items should not be flattened.
     
     Parameters:
         arr (list): The list of lists to be flattened.
         
     Returns:
         list: The resulting flattened list.
         
     Example:
         >>> flt([[(), ()], [(), ()]])
         [(), (), (), (), (), ()]
-    .```
+    .
+```
 - **overlp**
 ```
     Checks if elements in l1 and l2 share any same elements
 
     Parameters:
         l1 (list): a list of elements
         l2 (list): a list of elements
 
     Returns:
         bool: if there are any overlaps between l1 and l2
-    .```
+    .
+```
 - **segm**
 ```
     Divide a list into sublists of a specified size.
     
     Parameters:
         arr (list): The list to be divided into sublists.
         n (int): The size of each sublist.
         
     Returns:
         list: A list of sublists, where each sublist contains 'n' elements.
         
     Example:
         >>> segm([1, 1, 1, 1, 1, 1], 2)
         [[1, 1], [1, 1], [1, 1]]
-    .```
+    .
+```
 # JColors
 Color constants importable by name.
 ```py
 from JUtils.JColors import *
 ```
 
 - **randColor**
 ```Returns a random color
     
     Returns:
         tuple: A 3-tuple of integers representing the red, green, and blue components of the color.
-    .```
+    .
+```
 # JConst
 Constants for keeping code clean.
 ```py
 from JUtils.JConst import *
 ```
 
 # JConv
@@ -109,96 +114,104 @@
 
     Args:
         x (float): The x-coordinate.
         y (float): The y-coordinate.
 
     Returns:
         tuple: Polar coordinates (th, r), where r is the distance fromthe origin and th is the angle in degrees.
-    .```
+    .
+```
 - **deg2rad**
 ```Converts an angle in degrees to radians.
 
     Parameters:
         deg (float): An angle in degrees.
 
     Returns:
         float: The equivalent angle in radians.
-    .```
+    .
+```
 - **hex2asc**
 ```
     Convert a string of hexadecimal characters to a string of ASCII characters.
     
     Parameters:
         hx (str): The string of hexadecimal characters to be converted.
         
     Returns:
         str: The resulting string of ASCII characters.
     
     Example:
         >>> hex2asc('0000ff')
         '048048048048102102' #048 048 048 048 102 102
-    .```
+    .
+```
 - **hex2rgb**
 ```
     Convert a hexadecimal string representation to an RGB tuple.
 
     Parameters:
     hx (str): A hexadecimal string representation of an RGB color, in the form '#RRGGBB'.
 
     Returns:
     tuple: An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Example:
     >>> hex2rgb('#ff00ff')
     (255, 0, 255)
-    .```
+    .
+```
 - **pol2cart**
 ```Converts polar coordinates to Cartesian coordinates.
 
     Args:
         ang (float): An angle in degrees.
         r (float): The distance from the origin.
 
     Returns:
         tuple: A tuple of the Cartesian coordinates (x, y).
-    .```
+    .
+```
 - **rad2deg**
 ```Converts an angle in radians to degrees.
 
     Parameters:
         rad (float): An angle in radians.
 
     Returns:
         float: The equivalent angle in degrees.
-    .```
+    .
+```
 - **rgb2gray**
 ```
     Converts an RGB color tuple to a grayscale integer value using the luminosity method.
     
     Args:
         rgb (tuple): A tuple containing 3 integers representing the RGB color values. The values
                      should be in the range of 0-255, inclusive.
                      
     Returns:
         int: The grayscale integer value representing the given RGB color tuple.
-    .```
+    .
+```
 - **rgb2hex**
 ```
     Convert an RGB tuple to a hexadecimal string representation.
 
     Parameters:
     rgb (tuple): An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Returns:
     str: A hexadecimal string representation of the input RGB tuple, in the form '#RRGGBB'.
 
     Example:
     >>> rgb_to_hex((255, 0, 255))
     '#ff00ff'
-    .```
+    .
+```
 # JNum
 Functions for handling numbers.
 ```py
 from JUtils.JNum import *
 ```
 
 - **contain**
@@ -208,53 +221,58 @@
         n (float): The number to be clamped.
         limDown (float): The lower bound of the range.
         limUp (float): The upper bound of the range.
 
     Returns:
         'n' if it is within the range, or the nearest bound if 'n' is outside
         the range.
-    .```
+    .
+```
 - **sTup2Tup**
 ```
     Turns the given string of a tuple to a tuple object.
 
     Parameters:
         s: A tuple in string form.
 
     Returns:
         The tuple as a tuple object.
-    .```
+    .
+```
 - **sgn**
 ```Returns the sign of a number.
 
     Parameters:
         n: An int/float number.
 
     Returns:
         An int representing the sign of 'n'. 1 if 'n' is positive, -1 if 'n'
         is negative, and 0 if 'n' is zero.
-    .```
+    .
+```
 # JOut
 Functions for handling console output.
 ```py
 from JUtils.JOut import *
 ```
 
 - **delayPrint**
 ```Prints the given string with a slight delay after each character.
 
     Parameters:
         s: A string.
-    .```
+    .
+```
 - **printn**
 ```Prints the given arguments, with newlines before and after (works with multiple args like print)
     
     Parameters:
         *args: The arguments to print.
-    .```
+    .
+```
 # JStr
 Functions for string analysing and modification.
 ```py
 from JUtils.JStr import *
 ```
 
 - **listPath**
@@ -262,15 +280,16 @@
     Just like os.listdir(), but with appended path.
     
     Args:
         d: The path to list.
         
     Returns:
         list: A list of paths of files and directories in the given path.
-    .```
+    .
+```
 - **locBrac**
 ```
     Finds the index of the closing bracket that matches the opening bracket at the given index in the given string.
 
     Parameters:
         string (str): The input string.
         brac (str): The bracket character | Possible are ( [ { <
@@ -282,26 +301,28 @@
     Example:
         >>> locBrac('[hello[world]]', '[', 0)
         13
         >>> locBrac('<hello<world>>', '<', 6)
         12
         >>> locBrac('{hello}world}', '{', 0)
         -1
-    .```
+    .
+```
 - **multiCenter**
 ```
     Centers the text in a string by padding spaces on either side of each line.
     
     Args:
         s (str): The input string to center.
         l (int): The desired width of the centered string.
         
     Returns:
         str: The centered string. Each line is padded with spaces on either side to center the text. If
              a line already has an odd number of characters, the extra space is added to the right
              side of the line.
-    .```
+    .
+```
 \
 \
 \
 This Package is not under active development, i will update it every now and then if i find a new function to add.
 Please consider emailing me at: [jan@seifert-online.de](mailto:jan@seifert-online.de) if you got any suggestions for improvement.
```

### Comparing `JUtils-1.0.1/pyproject.toml` & `JUtils-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JUtils"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jan Seifert", email="jan@seifert-online.de" },
 ]
 description = "Package containing various utility functions i needed now and then, that i wanted to share"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `JUtils-1.0.1/src/JUtils/AutoDoc.py` & `JUtils-1.0.2/src/JUtils/AutoDoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     readme += f"## {str(count)}. [{package}](#{foldername}.{package})\n"
     count += 1
 readme += "\n"
 
 for package, info in dataStruct[foldername].items():
     readme += f"# {package}\n{info['doc']}.\n```py\nfrom {foldername}.{package} import *\n```\n\n"
     for func, funcINFO in info["funcs"].items():
-        readme += f"- **{func}**\n```{funcINFO}.```\n"
+        readme += f"- **{func}**\n```{funcINFO}.\n```\n"
 with open("ModuleEnd.txt", "r") as f3:
     readme += f3.read()
 
 #print(readme)
 #######################################################
 
 if os.path.exists("README.md"):
```

### Comparing `JUtils-1.0.1/src/JUtils/JArr.py` & `JUtils-1.0.2/src/JUtils/JArr.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils/JColors.py` & `JUtils-1.0.2/src/JUtils/JColors.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils/JConv.py` & `JUtils-1.0.2/src/JUtils/JConv.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils/JNum.py` & `JUtils-1.0.2/src/JUtils/JNum.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils/JOut.py` & `JUtils-1.0.2/src/JUtils/JOut.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils/JStr.py` & `JUtils-1.0.2/src/JUtils/JStr.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.1/src/JUtils.egg-info/PKG-INFO` & `JUtils-1.0.2/src/JUtils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -47,67 +47,72 @@
     Examples:
         >>> IterComp([1, 2, 3], [1, 2, 3])
         True
         >>> IterComp([1, 2, 3], [1, 2, 4])
         False
         >>> IterComp([1, 2, 3], [1, 2])
         None
-    .```
+    .
+```
 - **flt2d**
 ```
     Flatten a list of lists into a single list. Only for 2d lists, because the inner items should not be flattened.
     
     Parameters:
         arr (list): The list of lists to be flattened.
         
     Returns:
         list: The resulting flattened list.
         
     Example:
         >>> flt([[(), ()], [(), ()]])
         [(), (), (), (), (), ()]
-    .```
+    .
+```
 - **overlp**
 ```
     Checks if elements in l1 and l2 share any same elements
 
     Parameters:
         l1 (list): a list of elements
         l2 (list): a list of elements
 
     Returns:
         bool: if there are any overlaps between l1 and l2
-    .```
+    .
+```
 - **segm**
 ```
     Divide a list into sublists of a specified size.
     
     Parameters:
         arr (list): The list to be divided into sublists.
         n (int): The size of each sublist.
         
     Returns:
         list: A list of sublists, where each sublist contains 'n' elements.
         
     Example:
         >>> segm([1, 1, 1, 1, 1, 1], 2)
         [[1, 1], [1, 1], [1, 1]]
-    .```
+    .
+```
 # JColors
 Color constants importable by name.
 ```py
 from JUtils.JColors import *
 ```
 
 - **randColor**
 ```Returns a random color
     
     Returns:
         tuple: A 3-tuple of integers representing the red, green, and blue components of the color.
-    .```
+    .
+```
 # JConst
 Constants for keeping code clean.
 ```py
 from JUtils.JConst import *
 ```
 
 # JConv
@@ -121,96 +126,104 @@
 
     Args:
         x (float): The x-coordinate.
         y (float): The y-coordinate.
 
     Returns:
         tuple: Polar coordinates (th, r), where r is the distance fromthe origin and th is the angle in degrees.
-    .```
+    .
+```
 - **deg2rad**
 ```Converts an angle in degrees to radians.
 
     Parameters:
         deg (float): An angle in degrees.
 
     Returns:
         float: The equivalent angle in radians.
-    .```
+    .
+```
 - **hex2asc**
 ```
     Convert a string of hexadecimal characters to a string of ASCII characters.
     
     Parameters:
         hx (str): The string of hexadecimal characters to be converted.
         
     Returns:
         str: The resulting string of ASCII characters.
     
     Example:
         >>> hex2asc('0000ff')
         '048048048048102102' #048 048 048 048 102 102
-    .```
+    .
+```
 - **hex2rgb**
 ```
     Convert a hexadecimal string representation to an RGB tuple.
 
     Parameters:
     hx (str): A hexadecimal string representation of an RGB color, in the form '#RRGGBB'.
 
     Returns:
     tuple: An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Example:
     >>> hex2rgb('#ff00ff')
     (255, 0, 255)
-    .```
+    .
+```
 - **pol2cart**
 ```Converts polar coordinates to Cartesian coordinates.
 
     Args:
         ang (float): An angle in degrees.
         r (float): The distance from the origin.
 
     Returns:
         tuple: A tuple of the Cartesian coordinates (x, y).
-    .```
+    .
+```
 - **rad2deg**
 ```Converts an angle in radians to degrees.
 
     Parameters:
         rad (float): An angle in radians.
 
     Returns:
         float: The equivalent angle in degrees.
-    .```
+    .
+```
 - **rgb2gray**
 ```
     Converts an RGB color tuple to a grayscale integer value using the luminosity method.
     
     Args:
         rgb (tuple): A tuple containing 3 integers representing the RGB color values. The values
                      should be in the range of 0-255, inclusive.
                      
     Returns:
         int: The grayscale integer value representing the given RGB color tuple.
-    .```
+    .
+```
 - **rgb2hex**
 ```
     Convert an RGB tuple to a hexadecimal string representation.
 
     Parameters:
     rgb (tuple): An RGB tuple with 3 integers between 0 and 255, inclusive, representing the red, green, and blue values.
 
     Returns:
     str: A hexadecimal string representation of the input RGB tuple, in the form '#RRGGBB'.
 
     Example:
     >>> rgb_to_hex((255, 0, 255))
     '#ff00ff'
-    .```
+    .
+```
 # JNum
 Functions for handling numbers.
 ```py
 from JUtils.JNum import *
 ```
 
 - **contain**
@@ -220,53 +233,58 @@
         n (float): The number to be clamped.
         limDown (float): The lower bound of the range.
         limUp (float): The upper bound of the range.
 
     Returns:
         'n' if it is within the range, or the nearest bound if 'n' is outside
         the range.
-    .```
+    .
+```
 - **sTup2Tup**
 ```
     Turns the given string of a tuple to a tuple object.
 
     Parameters:
         s: A tuple in string form.
 
     Returns:
         The tuple as a tuple object.
-    .```
+    .
+```
 - **sgn**
 ```Returns the sign of a number.
 
     Parameters:
         n: An int/float number.
 
     Returns:
         An int representing the sign of 'n'. 1 if 'n' is positive, -1 if 'n'
         is negative, and 0 if 'n' is zero.
-    .```
+    .
+```
 # JOut
 Functions for handling console output.
 ```py
 from JUtils.JOut import *
 ```
 
 - **delayPrint**
 ```Prints the given string with a slight delay after each character.
 
     Parameters:
         s: A string.
-    .```
+    .
+```
 - **printn**
 ```Prints the given arguments, with newlines before and after (works with multiple args like print)
     
     Parameters:
         *args: The arguments to print.
-    .```
+    .
+```
 # JStr
 Functions for string analysing and modification.
 ```py
 from JUtils.JStr import *
 ```
 
 - **listPath**
@@ -274,15 +292,16 @@
     Just like os.listdir(), but with appended path.
     
     Args:
         d: The path to list.
         
     Returns:
         list: A list of paths of files and directories in the given path.
-    .```
+    .
+```
 - **locBrac**
 ```
     Finds the index of the closing bracket that matches the opening bracket at the given index in the given string.
 
     Parameters:
         string (str): The input string.
         brac (str): The bracket character | Possible are ( [ { <
@@ -294,26 +313,28 @@
     Example:
         >>> locBrac('[hello[world]]', '[', 0)
         13
         >>> locBrac('<hello<world>>', '<', 6)
         12
         >>> locBrac('{hello}world}', '{', 0)
         -1
-    .```
+    .
+```
 - **multiCenter**
 ```
     Centers the text in a string by padding spaces on either side of each line.
     
     Args:
         s (str): The input string to center.
         l (int): The desired width of the centered string.
         
     Returns:
         str: The centered string. Each line is padded with spaces on either side to center the text. If
              a line already has an odd number of characters, the extra space is added to the right
              side of the line.
-    .```
+    .
+```
 \
 \
 \
 This Package is not under active development, i will update it every now and then if i find a new function to add.
 Please consider emailing me at: [jan@seifert-online.de](mailto:jan@seifert-online.de) if you got any suggestions for improvement.
```


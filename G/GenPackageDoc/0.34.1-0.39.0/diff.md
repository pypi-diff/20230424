# Comparing `tmp/GenPackageDoc-0.34.1.tar.gz` & `tmp/GenPackageDoc-0.39.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenPackageDoc-0.34.1.tar", last modified: Mon Nov 14 16:02:24 2022, max compression
+gzip compressed data, was "GenPackageDoc-0.39.0.tar", last modified: Mon Apr 24 14:18:03 2023, max compression
```

## Comparing `GenPackageDoc-0.34.1.tar` & `GenPackageDoc-0.39.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:02:24.368610 GenPackageDoc-0.34.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:02:24.364610 GenPackageDoc-0.34.1/GenPackageDoc/
--rw-r--r--   0 runner    (1001) docker     (121)    39386 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/CDocBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/CInterface.py
--rw-r--r--   0 runner    (1001) docker     (121)    24429 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/CPackageDocConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     7831 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/CPatterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     7491 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/CSourceParser.py
--rw-r--r--   0 runner    (1001) docker     (121)   264870 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/GenPackageDoc.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:02:24.368610 GenPackageDoc-0.34.1/GenPackageDoc/styles/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/styles/admonitions.sty
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/styles/common.sty
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/styles/pandoc.sty
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/styles/preamble.tex
--rw-r--r--   0 runner    (1001) docker     (121)    11838 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/styles/robotframeworkaio.sty
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/GenPackageDoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 16:02:24.364610 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-11-14 16:02:24.000000 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-14 16:02:24.000000 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 16:02:24.000000 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-14 16:02:24.000000 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-14 16:02:24.000000 GenPackageDoc-0.34.1/GenPackageDoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-11-14 16:02:24.368610 GenPackageDoc-0.34.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 16:02:24.368610 GenPackageDoc-0.34.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9149 2022-11-14 16:00:06.000000 GenPackageDoc-0.34.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc/
+-rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CDocBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CPackageDocConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CPatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CSourceParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283914 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/GenPackageDoc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/admonitions.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/common.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/pandoc.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/preamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/robotframeworkaio.sty
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/setup.py
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/CDocBuilder.py` & `GenPackageDoc-0.39.0/GenPackageDoc/CDocBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # **************************************************************************************************************
 #
 # CDocBuilder.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 04.11.2022
+# 06.01.2023
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
 Python module containing all methods to generate tex sources.
 """
 
@@ -69,15 +69,15 @@
       """
 Constructor of class ``CDocBuilder``.
 
 * ``oPackageDocConfig``
 
   / *Condition*: required / *Type*: CPackageDocConfig() /
 
-  GenPackageDoc configuration containing static and dynamic configuration values.
+  **GenPackageDoc** configuration containing static and dynamic configuration values.
       """
 
       sMethod = "CDocBuilder.__init__"
 
       if oPackageDocConfig is None:
          bSuccess = None
          sResult  = "oPackageDocConfig is None"
@@ -239,17 +239,22 @@
          sLine = sLine.replace(self.__dictPlaceholder['newline'], r"\newline")
 
          # To handle ambiguous names of methods, classes and methods, the original names (= document headlines)
          # are replaced by the full scopes. We will not run into trouble any more when Pandoc creates labels out of the headlines
          # when converting the rst source code to LaTeX code.
          # Here we have to undo this replacement: We replace the full scope string in every section and subsection by the original headline.
 
+         # Pandoc adds ligatures in some cases: '--' -> '-\/-'. We do not need them. They have to be removed before we search for sKey,
+         # because sKey does not contain these ligatures.
+         if "section{" in sLine:
+            sLine = sLine.replace(r'\/', '')
+
          for sKey in self.__dictScopes:
             # sKey is full scope string
-            # value of sKey is original headline
+            # value of sKey is original headline (= original name of function, class or method)
             sSearch  = "section{" + sKey + "}" # this includes 'subsection'
             sReplace = "section{" + self.__dictScopes[sKey] + "}"
             sReplace = sReplace.replace('_', r'\_') # LaTeX requires this masking
             sLine = sLine.replace(sSearch, sReplace)
 
          listLinesProcessed.append(sLine)
 
@@ -613,30 +618,33 @@
                   listLinesRST.append("")
                   if sClassDocString is not None:
                      listLinesRST.append(sClassDocString)
 
 
                   for dictMethod in listofdictMethods:
                      sMethodName = dictMethod['sMethodName']
-                     sMethodScope = f"{sModuleFileScope}-{sClassName}-{sMethodName}"
-                     sMethodScope = self.__ConvertToScopeFormat(sMethodScope)
-                     sMethodHeadline = f"Method: {sMethodName}"
+                     bIsKeyword  = dictMethod['bIsKeyword']
+                     sIdentifier = "Method"
+                     if bIsKeyword is True:
+                        sIdentifier = "Keyword"
+                     sMethodHeadline = f"{sIdentifier}: {sMethodName}"
+                     sMethodScope    = f"{sModuleFileScope}-{sClassName}-{sMethodName}"
+                     sMethodScope    = self.__ConvertToScopeFormat(sMethodScope)
                      self.__dictScopes[sMethodScope] = sMethodHeadline
 
-                     sMethodDocString = dictMethod['sMethodDocString']
-
-                     print(f"    - Method : '{sMethodName}' / scope: '{sMethodScope}'")
+                     print(f"    - {sIdentifier} : '{sMethodName}' / scope: '{sMethodScope}'")
 
                      # tmp mapping
                      sMethodHeadline = sMethodScope
 
                      listLinesRST.append(sMethodHeadline)
                      sMethodHeadlineUnderline = len(sMethodHeadline)*"-"
                      listLinesRST.append(sMethodHeadlineUnderline)
                      listLinesRST.append("")
+                     sMethodDocString = dictMethod['sMethodDocString']
                      if sMethodDocString is not None:
                         listLinesRST.append(sMethodDocString)
 
                # eof for dictClass in listofdictClasses:
 
                print()
 
@@ -787,17 +795,19 @@
       oPatterns = CPatterns()
 
       # 1. autodefined sty file (containing runtime informations)
       sAutodefinedFile = f"{sBuildFolder}/styles/autodefined.sty"
       oAutodefinedFile = CFile(sAutodefinedFile)
       sAutodefinedHeader = oPatterns.GetAutodefinedHeader(time.strftime('%d.%m.%Y - %H:%M:%S'))
       oAutodefinedFile.Write(sAutodefinedHeader)
-      sCommand = r"\newcommand{\repo}{" + self.__dictPackageDocConfig['REPOSITORYNAME'] + "}"
+      REPOSITORYNAME = self.__dictPackageDocConfig['REPOSITORYNAME'].replace("_", r"\_")
+      sCommand = r"\newcommand{\repo}{\textbf{" + REPOSITORYNAME + "}}"
       oAutodefinedFile.Write(sCommand)
-      sCommand = r"\newcommand{\pkg}{" + self.__dictPackageDocConfig['PACKAGENAME'] + "}"
+      PACKAGENAME = self.__dictPackageDocConfig['PACKAGENAME'].replace("_", r"\_")
+      sCommand = r"\newcommand{\pkg}{\textbf{" + PACKAGENAME + "}}"
       oAutodefinedFile.Write(sCommand)
       oAutodefinedFile.Write()
       del oAutodefinedFile
 
       # 2. main tex file
       sDocumentationTeXFileName = self.__dictPackageDocConfig['DOCUMENT']['OUTPUTFILENAME']
       sMainTexFile = f"{sBuildFolder}/{sDocumentationTeXFileName}"
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/CInterface.py` & `GenPackageDoc-0.39.0/GenPackageDoc/CInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 #
 # **************************************************************************************************************
 #
 # CInterface.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 28.06.2022
+# 21.11.2022
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
-Python module containing an interface for ``GenPackageDoc``. This interface can be used to get access to the
-LaTeX stylesheets that are part of the ``GenPackageDoc`` installation.
+Python module containing an interface for **GenPackageDoc**. This interface can be used to get access to the
+LaTeX stylesheets that are part of the **GenPackageDoc** installation.
 """
 
 # --------------------------------------------------------------------------------------------------------------
 
 import os, sys, time
 import colorama as col
 
@@ -67,24 +67,24 @@
    # eof def __init__(self, oRepositoryConfig=None):
 
    def __del__(self):
       pass
 
    def GetLaTeXStyles(self, sDestination=None):
       """
-The LaTeX stylesheets are part of the installation of ``GenPackageDoc``. In case of anyone else than ``GenPackageDoc``
+The LaTeX stylesheets are part of the installation of **GenPackageDoc**. In case of anyone else than **GenPackageDoc**
 needs these stylesheets, this method can be used to copy them to any other folder.
 
 **Arguments:**
 
 * ``sDestination``
 
   / *Condition*: required / *Type*: str /
 
-  Path and name of a folder in which the styles folder from ``GenPackageDoc`` will be copied.
+  Path and name of a folder in which the styles folder from **GenPackageDoc** will be copied.
 
 **Returns:**
 
 * ``bSuccess``
 
   / *Type*: bool /
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/CPackageDocConfig.py` & `GenPackageDoc-0.39.0/GenPackageDoc/CPackageDocConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 # **************************************************************************************************************
 #
 # CPackageDocConfig.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 31.08.2022
+# 17.03.2023
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
-Python module containing the configuration for GenPackageDoc. This includes the repository configurantion
+Python module containing the configuration for **GenPackageDoc**. This includes the repository configurantion
 and command line values.
 """
 
 # --------------------------------------------------------------------------------------------------------------
 
 import os, sys, time, platform, json, argparse
 import colorama as col
@@ -46,14 +46,19 @@
 COLBW = col.Style.BRIGHT + col.Fore.WHITE
 
 SUCCESS = 0
 ERROR   = 1
 
 # --------------------------------------------------------------------------------------------------------------
 
+def printerror(sMsg):
+    sys.stderr.write(COLBR + f"Error: {sMsg}!\n")
+
+# --------------------------------------------------------------------------------------------------------------
+
 class CPackageDocConfig():
 
    def __init__(self, oRepositoryConfig=None):
       """
 Constructor of class ``CPackageDocConfig``.
 
 Responsible for:
@@ -63,15 +68,15 @@
 * Resolve placeholders used in packagedoc configuration
 * Prepare runtime variables
 
 * ``oRepositoryConfig``
 
   / *Condition*: required / *Type*: CRepositoryConfig() /
 
-  GenPackageDoc configuration containing static and dynamic configuration values (this includes the
+  **GenPackageDoc** configuration containing static and dynamic configuration values (this includes the
   Repository configuration).
       """
 
       sMethod = "CPackageDocConfig.__init__"
 
       self.__dictPackageDocConfig = None  # self.__dictConfig
 
@@ -164,14 +169,18 @@
       # required
       if 'CONTROL' in dictJsonValues:
          self.__dictPackageDocConfig['CONTROL']  = dictJsonValues['CONTROL']
       else:
          bSuccess = None
          sResult  = f"Missing key 'CONTROL' within '{sDocumentationProjectConfigFile}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
+      # ==============================================================================================================
+      # 21.11.2022 Feature 'INCLUDEPRIVATE' switched off. TODO: needs several bugfixes
+      self.__dictPackageDocConfig['CONTROL']['INCLUDEPRIVATE'] = False
+      # ==============================================================================================================
       bSuccess, sResult = self.__CheckElements(('INCLUDEPRIVATE','INCLUDEUNDOCUMENTED','STRICT'), self.__dictPackageDocConfig['CONTROL'].keys(), "subkey")
       if bSuccess is not True:
          sResult = sResult + f"\nWhile reading from '{sDocumentationProjectConfigFile}'"
          raise Exception(CString.FormatResult(sMethod, bSuccess, sResult))
 
       # required
       if 'TOC' in dictJsonValues:
@@ -439,16 +448,17 @@
 
    def Get(self, sName=None):
       """
 Returns the configuration value belonging to a key name.
       """
       if ( (sName is None) or (sName not in self.__dictPackageDocConfig) ):
          print()
-         printerror(f"Error: Configuration parameter '{sName}' not existing!")
+         printerror(f"Configuration parameter '{sName}' not existing")
          # from here it's standard output:
+         print()
          print("Use instead one of:")
          self.PrintConfigKeys()
          return None # returning 'None' in case of key is not existing !!!
       else:
          return self.__dictPackageDocConfig[sName]
    # eof def Get(self, sName=None):
 
@@ -459,15 +469,15 @@
       """
       return self.__dictPackageDocConfig
    # eof def GetConfig(self):
 
 
    def __GetCmdLineArgs(self):
       """
-Get values fom command linwe and add them to GenPackageDoc configuration. Already existing configuration values will be overwritten.
+Get values fom command linwe and add them to **GenPackageDoc** configuration. Already existing configuration values will be overwritten.
       """
 
       sMethod = "CPackageDocConfig.__GetCmdLineArgs"
 
       bSuccess = False
       sResult  = "UNKNOWN"
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/CPatterns.py` & `GenPackageDoc-0.39.0/GenPackageDoc/CPatterns.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/CSourceParser.py` & `GenPackageDoc-0.39.0/GenPackageDoc/CSourceParser.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # **************************************************************************************************************
 #
 # CSourceParser.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 16.06.2022
+# 21.11.2022
 #
 # --------------------------------------------------------------------------------------------------------------
 
 """
 Python module containing all methods to parse the documentation content of Python source files.
 """
 
@@ -58,15 +58,15 @@
 
 * ``sFile``
 
   / *Condition*: required / *Type*: str /
 
   Path and name of a single Python module.
 
-* ``bIncludePrivate``
+* ``bIncludePrivate`` (currently not active, is ``False``)
 
   / *Condition*: optional / *Type*: bool / *Default*: False /
 
   If ``False``: private methods are skipped, otherwise they are included in documentation.
 
 * ``bIncludeUndocumented``
 
@@ -164,28 +164,38 @@
 
             listofdictMethods = []
 
             for subnode in node.body:
                if isinstance(subnode, ast.FunctionDef):
                   sMethodName = f"{subnode.name}"
                   sMethodDocString = ast.get_docstring(subnode)
+
+                  # is keyword?
+                  bIsKeyword = False
+                  for decorator in subnode.decorator_list:
+                     if hasattr(decorator, 'id'):
+                        if decorator.id == "keyword":
+                           bIsKeyword = True
+                           break
+
                   bTakeIt = True
                   if bIncludePrivate is False:
                      if sMethodName.startswith('_'):
                         # is private
                         bTakeIt = False
                   # eof if bIncludePrivate is False:
                   if bIncludeUndocumented is False:
                      if sMethodDocString is None:
                         # is undocumented
                         bTakeIt = False
                   # eof if bIncludeUndocumented is False:
                   if bTakeIt is True:
                      dictMethod = {}
-                     dictMethod['sMethodName'] = sMethodName
+                     dictMethod['sMethodName']      = sMethodName
+                     dictMethod['bIsKeyword']       = bIsKeyword
                      dictMethod['sMethodDocString'] = sMethodDocString
                      listofdictMethods.append(dictMethod)
                   # eof if bTakeIt is True
                # eof if isinstance(subnode, ast.FunctionDef):
             # eof for subnode in node.body:
 
             dictClass['listofdictMethods'] = listofdictMethods
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/GenPackageDoc.pdf` & `GenPackageDoc-0.39.0/GenPackageDoc/GenPackageDoc.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 16% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 GenPackageDoc
-v. 0.34.1
+v. 0.39.0
 Holger Queckenstedt
-09.11.2022
+06.01.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -214,17 +214,18 @@
 B
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
 Introduction
-The Python package GenPackageDoc generates the documentation of Python modules. The content of this documentation is taken out of the docstrings of functions, classes and their methods.
-It is possible to extend the documentation by the content of additional files either in reStructuredText (RST) format
-or in LaTeX format.
+The Python package GenPackageDoc generates the documentation of Python modules. The content of this documentation is taken out of the docstrings of functions, classes and their methods. All docstrings have to be written in
+reStructuredText (RST) format, that is a certain markdown dialect.
+It is possible to extend the documentation by the content of additional files either in reStructuredText format or in
+LaTeX format.
 The documentation is generated in four steps:
 1. Files in LaTeX format are taken over immediately.
 2. Files in reStructuredText format are converted to LaTeX files.
 3. All docstrings of all Python modules in the package are converted to LaTeX files.
 4. All LaTeX files together are converted to a single PDF document. This requires a separately installed LaTeX
 distribution (recommended: TeX Live). A LaTeX distribution is not part of GenPackageDoc and has to be
 installed separately!
@@ -237,16 +238,16 @@
 out of Python sources that are stored within a repository, and therefore we have dependencies to the structure of the
 repository. For example: Configuration files with values that are specific for a repository, should not be installed.
 Such a specific configuration value is e.g. the name of the package or the name of the PDF document.
 The impact is: There is a deep relationship between the repository containing the sources to be documented, and the
 sources and the configuration of GenPackageDoc itself. Therefore some manual preparations are necessary to use
 GenPackageDoc also in other repositories.
 How to do this is explained in detail in the next chapters.
-The outcome of all preparations of GenPackageDoc in your own repository is a PDF document like the one you are
-currently reading.
+The outcome of all preparations of GenPackageDoc in your own repository is a PDF document like the one you
+are currently reading.
 
 1
 
 CHAPTER 2. DESCRIPTION
 
 Chapter 2
 
@@ -263,16 +264,16 @@
 Contains the repository configuration (e.g. the name of the package, the name of the repository, the author,
 and more ...).
 This folder is specific for the repository.
 • Folder additions
 Contains additionally needed sources like setup related class definitions and sources, that are imported from
 other repositories - to make this repository stand alone
 • Folder packagedoc
-Contains all package documentation related files, e.g. the GenPackageDoc configuration, additional input files
-and the generated documentation itself.
+Contains all package documentation related files, e.g. the GenPackageDoc configuration, additional input
+files and the generated documentation itself.
 This folder is specific for the documentation.
 • Repository root folder
 – genpackagedoc.py
 Python script to start the documentation build
 – setup.py
 Python script to install the package sources. This includes the execution of genpackagedoc.py. Therefore building the documentation is part of the installation process.
 – dump repository config.py
@@ -543,19 +544,18 @@
 RST syntax rules. To avoid a needless indentation of the text within the resulting PDF document and to avoid
 further unwanted side effects caused by improper indentations, it is strongly required to start at least the first
 line of a docstring text within the first column! And this first line is the reference for the indentation of further
 lines of the current docstring. The indentation of these further lines depends on the RST syntax element that
 is used here.
 • In RST also blank lines are part of the syntax!
 Why is a proper indentation of the docstrings so much important?
-The contents of all doctrings of a Python module will be merged to one single RST document (internally by
-GenPackageDoc). In this single RST document we do not have separated docstring lines any more. We have
-one text! And we have a relationship between previous lines and following lines in this text. The indentation of these
-previous and following lines must fit together – accordingly to the RST syntax rules. Otherwise we either get syntax
-issues during computation or we get text with a layout that does not fit to our expectation.
+The contents of all doctrings of a Python module will be merged to one single RST document (internally by GenPackageDoc). In this single RST document we do not have separated docstring lines any more. We have one text!
+And we have a relationship between previous lines and following lines in this text. The indentation of these previous
+and following lines must fit together – accordingly to the RST syntax rules. Otherwise we either get syntax issues
+during computation or we get text with a layout that does not fit to our expectation.
 Please be attentive while typing your documentation in RST format!
 
 2.7.2
 
 Syntax extensions
 
 GenPackageDoc extends the RST syntax by the following topics:
@@ -802,15 +802,15 @@
 Method: ParseSourceFile
 
 The method ParseSourceFile parses the content of a Python module.
 Arguments:
 • sFile
 / Condition: required / Type: str /
 Path and name of a single Python module.
-• bIncludePrivate
+• bIncludePrivate (currently not active, is False)
 / Condition: optional / Type: bool / Default: False /
 If False: private methods are skipped, otherwise they are included in documentation.
 • bIncludeUndocumented
 / Condition: optional / Type: bool / Default: True /
 If True: also classes and methods without docstring are listed in the documentation (together with a hint that
 information is not available), otherwise they are skipped.
 Returns:
@@ -839,19 +839,19 @@
 
 Name
 
 GenPackageDoc
 
 Version
 
-0.34.1
+0.39.0
 
 Date
 
-09.11.2022
+06.01.2023
 
 Description
 
 Documentation builder for Python packages
 
 Package URL
 
@@ -1100,15 +1100,47 @@
 package)
 0.34.0
 
 07.11.2022
 
 Introduced auto defined LaTeX style file containing mnemotechnical commands
 to type the repository name and the package name
+0.35.0
+
+16.11.2022
+
+Layout settings of some LaTeX commands adapted:
+- Repository name and package name in bold
+- Inline code and inline listings in clearer colors
+0.36.0
+
+17.11.2022
+
+Brightness of all listings colors reduced to 45% (both text boxes and inline)
+0.37.0
+
+21.11.2022
+
+- LaTeX style adaptions and bugfixes
+- Introduced LaTeX commands Python log and pylog
+- Added keyword decorator detection
+- Feature ’INCLUDEPRIVATE’ temporarily switched off (requires bugfixes)
+0.38.0
+
+30.11.2022
+
+Removed harming ligatures that were added by Pandoc automatically to LaTeX
+code in case of multiple minus characters in names
+0.39.0
+
+06.01.2023
+
+Added masking of underlines in case of the content of \repo or \pkg contain
+underlines (masking required by LaTeX).
 
 GenPackageDoc.pdf
-Created at 10.11.2022 - 16:35:58
-by GenPackageDoc v. 0.34.1
+Created at 06.01.2023 - 15:11:02
+by GenPackageDoc v. 0.39.0
 
 19
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/__init__.py` & `GenPackageDoc-0.39.0/GenPackageDoc/__init__.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/styles/admonitions.sty` & `GenPackageDoc-0.39.0/GenPackageDoc/styles/admonitions.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/styles/common.sty` & `GenPackageDoc-0.39.0/GenPackageDoc/styles/common.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/styles/pandoc.sty` & `GenPackageDoc-0.39.0/GenPackageDoc/styles/pandoc.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/styles/preamble.tex` & `GenPackageDoc-0.39.0/GenPackageDoc/styles/preamble.tex`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/styles/robotframeworkaio.sty` & `GenPackageDoc-0.39.0/GenPackageDoc/styles/robotframeworkaio.sty`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,50 @@
 %
 % --------------------------------------------------------------------------------------------------------------
 %
 % robotframeworkaio.sty
 %
 % includes:
 % - RobotFramework AIO code and console listings
-% - Python for RobotFramework AIO code
+% - Python code and console listings
 %
-% 22.08.2022
+% 21.11.2022
 %
 % --------------------------------------------------------------------------------------------------------------
 
 \usepackage{listings}
 \usepackage{expl3,xparse}
 
 % ----------------------------------------------------------------------- %
 %
 % framework names
 %
 \newcommand{\rfwcore}{Robot Framework}
 \newcommand{\rfw}{RobotFramework AIO}
 % ----------------------------------------------------------------------- %
 
+% ----------------------------------------------------------------------- %
+%
+% tabulator and test results
+%
+\newcommand{\tab}{\phantom{x}\hspace{3ex}}
+
+\newcommand{\unknown}{\textcolor{blue}{unknown}}
+\newcommand{\aborted}{\textcolor{gray}{aborted}}
+\newcommand{\passed}{\textcolor{ForestGreen}{passed}}
+\newcommand{\failed}{\textcolor{red}{failed}}
+
+% deprecated (but still in use)
+\newcommand{\ifalignrcode}{\hspace{2pt}}
+\newcommand{\iftab}{\phantom{x}\hspace{3ex}}
+\newcommand{\ifunknown}[1]{\textcolor{blue}{#1}}
+\newcommand{\ifaborted}[1]{\textcolor{gray}{#1}}
+\newcommand{\ifpassed}[1]{\textcolor{ForestGreen}{#1}}
+\newcommand{\iffailed}[1]{\textcolor{red}{#1}}
+\newcommand{\ifnotice}[1]{\textbf{\textcolor{red}{#1}}}
 
 % ----------------------------------------------------------------------- %
 
 % !!! TODO: After switching von MiKTeX to Texlive it should be checked if the following fix is still needed !!!
 
 %lstlinebgrd needs this fix to run with current listings version provided by MiKTeX
 \makeatletter
@@ -119,25 +138,33 @@
 \begin{boxsyn_template}
 {\color{black!30!white} Robot Syntax}
 \ttfamily #1
 \end{boxsyn_template}
 }
 
 %
-%  style definitions for Robot code listings and log listings
+%  style definitions for Robot and Python code listings and log listings
 %
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 
-\definecolor{color_code_background}{RGB}{255, 239, 222}
-\definecolor{color_code_frame}{RGB}{255, 222, 189}
-\definecolor{color_code_highlight}{RGB}{255, 222, 189}
-
-\definecolor{color_log_background}{RGB}{222, 231, 247}
-\definecolor{color_log_frame}{RGB}{189, 206, 231}
-\definecolor{color_log_highlight}{RGB}{189, 206, 231}
+% color definitions
+\definecolor{color_def_code_background}{RGB}{255, 239, 222}
+\definecolor{color_def_code_frame}{RGB}{255, 222, 189}
+\definecolor{color_def_code_highlight}{RGB}{255, 222, 189}
+\definecolor{color_def_log_background}{RGB}{222, 231, 247}
+\definecolor{color_def_log_frame}{RGB}{189, 206, 231}
+\definecolor{color_def_log_highlight}{RGB}{189, 206, 231}
+
+% brightness
+\colorlet{color_code_background}{color_def_code_background!45!white}
+\colorlet{color_code_frame}{color_def_code_frame!45!white}
+\colorlet{color_code_highlight}{color_def_code_highlight!45!white}
+\colorlet{color_log_background}{color_def_log_background!45!white}
+\colorlet{color_log_frame}{color_def_log_frame!45!white}
+\colorlet{color_log_highlight}{color_def_log_highlight!45!white}
 
 %
 %  \hlcode command and \hllog command
 %  for highlighting specific lines in code and log listings
 %
 \ExplSyntaxOn
 \NewDocumentCommand \hlcode { O{color_code_highlight} O{color_code_background } m }
@@ -158,15 +185,15 @@
 \newcommand{\inlinecomment}[1]{\color{col_comment}\normalfont$\langle$\textit{#1}$\rangle$}
 
 
 %
 % environment for robot code listings
 %
 \lstdefinelanguage{Robot_code}{
-      alsoletter={-,[,],{,},$,@,\%},
+      alsoletter={-,[,],{,},$,@,\%,\&},
       basicstyle=\ttfamily\small,
       columns=fixed,
       showstringspaces=false,
       frame=single,
       framesep=5pt,
       breaklines=true,
       breakatwhitespace=true,
@@ -211,14 +238,15 @@
       keywordstyle=[2]\color{col_flowcontrol},
       comment=[l][\color{col_comment}]{\#},
       commentstyle=\color{col_comment}\upshape,
       moredelim=[s][\color{col_section}]{***}{***},
       moredelim=[s][\color{ForestGreen}]{$\{}{\}},
       moredelim=[s][\color{ForestGreen}]{@\{}{\}},
       moredelim=[s][\color{ForestGreen}]{\%\{}{\}},
+      moredelim=[s][\color{ForestGreen}]{\&\{}{\}},
       morestring=*[b]{"},
       morestring=[s][\color{gray}]{<}{>},
       stringstyle=\color{red},
       identifierstyle=\color{blue},
       rulesepcolor=\color{color_code_frame},
       rulecolor=\color{color_code_frame},
       backgroundcolor=\color{color_code_background},
@@ -241,14 +269,15 @@
    \efbox[margin=2pt,
          linewidth=1pt,
          linecolor=color_code_frame,
          backgroundcolor=color_code_background,
          font=\ttfamily\small]{\lstinline[language=Robot_code]!#1!}
 }
 
+
 %
 % environment for robot log listings
 %
 \lstdefinelanguage{Robot_log}{
       alsoletter=-,
       basicstyle=\ttfamily\small,
       columns=fixed,
@@ -263,19 +292,21 @@
       escapeinside={<}{>},
       captionpos=b,
       moredelim=[is][\bfseries]{[*}{*]},
       morestring=[m][\color{red}]{'},
       morestring=[m][\color{red}]{"},
       stringstyle=\color{red},
       identifierstyle=\color{black},
-      keywordstyle=\color{darkblue},   
+      keywordstyle=\color{blue},   
       morekeywords=[1]{PASS, passed},
       morekeywords=[2]{FAIL, failed},
+      morekeywords=[3]{UNKNOWN, unknown},
       keywordstyle=[1]\color{ForestGreen},
       keywordstyle=[2]\color{red},
+      keywordstyle=[3]\color{blue},
       rulesepcolor=\color{color_log_frame},
       rulecolor=\color{color_log_frame},
       backgroundcolor=\color{color_log_background},
       columns=fixed,
       keepspaces=true,
       abovecaptionskip=15pt
 }
@@ -293,23 +324,14 @@
    \efbox[margin=2pt,
          linewidth=1pt,
          linecolor=color_log_frame,
          backgroundcolor=color_log_background,
          font=\ttfamily\small]{\lstinline[language=Robot_log]!#1!}
 }
 
-
-
-\newcommand{\ifalignrcode}{\hspace{2pt}}
-\newcommand{\iftab}{\phantom{x}\hspace{3ex}}
-\newcommand{\ifunknown}[1]{\textcolor{blue}{#1}}
-\newcommand{\ifaborted}[1]{\textcolor{gray}{#1}}
-\newcommand{\ifpassed}[1]{\textcolor{ForestGreen}{#1}}
-\newcommand{\iffailed}[1]{\textcolor{red}{#1}}
-\newcommand{\ifnotice}[1]{\textbf{\textcolor{red}{#1}}}
 \usepackage{multirow}
 
 % use for flowchart drawing
 \usetikzlibrary{shapes.geometric, arrows}
 \tikzstyle{startstop} = [rectangle, rounded corners, minimum width=3cm, minimum height=0.8cm,text centered, draw=black, fill=red!30]
 \tikzstyle{io} = [trapezium, trapezium left angle=70, trapezium right angle=110, minimum width=3cm, minimum height=0.8cm, text centered, draw=black, fill=blue!30, text width=3cm]
 \tikzstyle{process} = [rectangle, minimum width=3cm, minimum height=0.8cm, text centered, draw=black, fill=orange!30, text width=4cm]
@@ -367,9 +389,60 @@
    \efbox[margin=2pt,
          linewidth=1pt,
          linecolor=color_code_frame,
          backgroundcolor=color_code_background,
          font=\ttfamily\small]{\lstinline[language=Python_code]!#1!}
 }
 
+%
+% environment for Python log listings
+%
+\lstdefinelanguage{Python_log}{
+      alsoletter=-,
+      basicstyle=\ttfamily\small,
+      columns=fixed,
+      showstringspaces=false,
+      commentstyle=\color{gray}\upshape,
+      frame=single,
+      framesep=5pt,
+      breaklines=true,
+      breakatwhitespace=true,
+      prebreak=\mbox{\textcolor{Red}{$\hookleftarrow$}\space},
+      postbreak=\mbox{\textcolor{ForestGreen}{$\hookrightarrow$}\space},
+      escapeinside={<}{>},
+      captionpos=b,
+      moredelim=[is][\bfseries]{[*}{*]},
+      morestring=[m][\color{red}]{'},
+      morestring=[m][\color{red}]{"},
+      stringstyle=\color{red},
+      identifierstyle=\color{black},
+      keywordstyle=\color{blue},   
+      morekeywords=[1]{PASS, passed},
+      morekeywords=[2]{FAIL, failed},
+      morekeywords=[3]{UNKNOWN, unknown},
+      keywordstyle=[1]\color{ForestGreen},
+      keywordstyle=[2]\color{red},
+      keywordstyle=[3]\color{blue},
+      rulesepcolor=\color{color_log_frame},
+      rulecolor=\color{color_log_frame},
+      backgroundcolor=\color{color_log_background},
+      columns=fixed,
+      keepspaces=true,
+      abovecaptionskip=15pt
+}
 
+\lstnewenvironment{pythonlog}[1][]{%
+   \lstset{%
+      xleftmargin=5pt,
+      xrightmargin=5pt,
+      alsolanguage=Python_log,
+      #1
+   }
+}{}
 
+\newcommand{\plog}[1]{
+   \efbox[margin=2pt,
+         linewidth=1pt,
+         linecolor=color_log_frame,
+         backgroundcolor=color_log_background,
+         font=\ttfamily\small]{\lstinline[language=Python_log]!#1!}
+}
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc/version.py` & `GenPackageDoc-0.39.0/GenPackageDoc/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of GenPackageDoc
 #
-VERSION      = "0.34.1"
-VERSION_DATE = "09.11.2022"
+VERSION      = "0.39.0"
+VERSION_DATE = "06.01.2023"
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc.egg-info/PKG-INFO` & `GenPackageDoc-0.39.0/GenPackageDoc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.34.1
+Version: 0.39.0
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,85 +16,85 @@
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 GenPackageDoc Description
 =========================
 
-The Python package `GenPackageDoc` generates the documentation of Python
-modules. The content of this documentation is taken out of the
+The Python package **GenPackageDoc** generates the documentation of
+Python modules. The content of this documentation is taken out of the
 docstrings of functions, classes and their methods.
 
 It is possible to extend the documentation by the content of additional
 files either in reStructuredText (RST) format or in LaTeX format.
 
 The documentation is generated in four steps:
 
 1.  Files in LaTeX format are taken over immediately.
 2.  Files in reStructuredText format are converted to LaTeX files.
 3.  All docstrings of all Python modules in the package are converted to
     LaTeX files.
 4.  All LaTeX files together are converted to a single PDF document.
     This requires a separately installed LaTeX distribution
     (recommended: TeX Live). A LaTeX distribution is **not** part of
-    `GenPackageDoc` and has to be installed separately!
+    **GenPackageDoc** and has to be installed separately!
 
 How to install
 --------------
 
-`GenPackageDoc` can be installed in two different ways.
+**GenPackageDoc** can be installed in two different ways.
 
 1.  Installation via PyPi (recommended for users)
 
-    ``` {.sourceCode .}
+    ``` {.}
     pip install GenPackageDoc
     ```
 
     [GenPackageDoc in PyPi](https://pypi.org/project/GenPackageDoc/)
 
 2.  Installation via GitHub (recommended for developers)
 
     Clone the **python-genpackagedoc** repository to your machine.
 
-    ``` {.sourceCode .}
+    ``` {.}
     git clone https://github.com/test-fullautomation/python-genpackagedoc.git
     ```
 
     [GenPackageDoc in
     GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
 
-    Use the following command to install `GenPackageDoc`:
+    Use the following command to install **GenPackageDoc**:
 
-    ``` {.sourceCode .}
+    ``` {.}
     setup.py install
     ```
 
 How to use
 ----------
 
-`GenPackageDoc` provides a toolchain to generate documentation out of
-Python sources that are stored within a repository. `GenPackageDoc` is
+**GenPackageDoc** provides a toolchain to generate documentation out of
+Python sources that are stored within a repository. **GenPackageDoc** is
 also designed to be able to consider setup informations of a repository.
 
 The impact is: There is a deep relationship between the repository
 containing the sources to be documented, and the sources and the
-configuration of `GenPackageDoc` itself. Therefore `GenPackageDoc` needs
-to be configured to get to know about things like the path to the
+configuration of **GenPackageDoc** itself. Therefore **GenPackageDoc**
+needs to be configured to get to know about things like the path to the
 package sources and the desired name of the generated documentation PDF
 file.
 
-`GenPackageDoc` is able to use it\'s own sources to document itself.
+**GenPackageDoc** is able to use it\'s own sources to document itself.
 Therefore the complete [GenPackageDoc
 repository](https://github.com/test-fullautomation/python-genpackagedoc)
 can be used as example about about writing a package documentation.
 
 At the end of all preparations you will get for your own repository a
 PDF document that will look like this:
 [GenPackageDoc.pdf](https://github.com/test-fullautomation/python-genpackagedoc/blob/develop/GenPackageDoc/GenPackageDoc.pdf)
-(that is the detailed documentation of `GenPackageDoc`).
+(that is the detailed documentation of **GenPackageDoc**).
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to [Thomas
 Pollerspöck](mailto:Thomas.Pollerspoeck@de.bosch.com)
```

### Comparing `GenPackageDoc-0.34.1/GenPackageDoc.egg-info/SOURCES.txt` & `GenPackageDoc-0.39.0/GenPackageDoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/LICENSE` & `GenPackageDoc-0.39.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.34.1/PKG-INFO` & `GenPackageDoc-0.39.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.34.1
+Version: 0.39.0
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,85 +16,85 @@
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 GenPackageDoc Description
 =========================
 
-The Python package `GenPackageDoc` generates the documentation of Python
-modules. The content of this documentation is taken out of the
+The Python package **GenPackageDoc** generates the documentation of
+Python modules. The content of this documentation is taken out of the
 docstrings of functions, classes and their methods.
 
 It is possible to extend the documentation by the content of additional
 files either in reStructuredText (RST) format or in LaTeX format.
 
 The documentation is generated in four steps:
 
 1.  Files in LaTeX format are taken over immediately.
 2.  Files in reStructuredText format are converted to LaTeX files.
 3.  All docstrings of all Python modules in the package are converted to
     LaTeX files.
 4.  All LaTeX files together are converted to a single PDF document.
     This requires a separately installed LaTeX distribution
     (recommended: TeX Live). A LaTeX distribution is **not** part of
-    `GenPackageDoc` and has to be installed separately!
+    **GenPackageDoc** and has to be installed separately!
 
 How to install
 --------------
 
-`GenPackageDoc` can be installed in two different ways.
+**GenPackageDoc** can be installed in two different ways.
 
 1.  Installation via PyPi (recommended for users)
 
-    ``` {.sourceCode .}
+    ``` {.}
     pip install GenPackageDoc
     ```
 
     [GenPackageDoc in PyPi](https://pypi.org/project/GenPackageDoc/)
 
 2.  Installation via GitHub (recommended for developers)
 
     Clone the **python-genpackagedoc** repository to your machine.
 
-    ``` {.sourceCode .}
+    ``` {.}
     git clone https://github.com/test-fullautomation/python-genpackagedoc.git
     ```
 
     [GenPackageDoc in
     GitHub](https://github.com/test-fullautomation/python-genpackagedoc)
 
-    Use the following command to install `GenPackageDoc`:
+    Use the following command to install **GenPackageDoc**:
 
-    ``` {.sourceCode .}
+    ``` {.}
     setup.py install
     ```
 
 How to use
 ----------
 
-`GenPackageDoc` provides a toolchain to generate documentation out of
-Python sources that are stored within a repository. `GenPackageDoc` is
+**GenPackageDoc** provides a toolchain to generate documentation out of
+Python sources that are stored within a repository. **GenPackageDoc** is
 also designed to be able to consider setup informations of a repository.
 
 The impact is: There is a deep relationship between the repository
 containing the sources to be documented, and the sources and the
-configuration of `GenPackageDoc` itself. Therefore `GenPackageDoc` needs
-to be configured to get to know about things like the path to the
+configuration of **GenPackageDoc** itself. Therefore **GenPackageDoc**
+needs to be configured to get to know about things like the path to the
 package sources and the desired name of the generated documentation PDF
 file.
 
-`GenPackageDoc` is able to use it\'s own sources to document itself.
+**GenPackageDoc** is able to use it\'s own sources to document itself.
 Therefore the complete [GenPackageDoc
 repository](https://github.com/test-fullautomation/python-genpackagedoc)
 can be used as example about about writing a package documentation.
 
 At the end of all preparations you will get for your own repository a
 PDF document that will look like this:
 [GenPackageDoc.pdf](https://github.com/test-fullautomation/python-genpackagedoc/blob/develop/GenPackageDoc/GenPackageDoc.pdf)
-(that is the detailed documentation of `GenPackageDoc`).
+(that is the detailed documentation of **GenPackageDoc**).
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to [Thomas
 Pollerspöck](mailto:Thomas.Pollerspoeck@de.bosch.com)
```

### Comparing `GenPackageDoc-0.34.1/README.rst` & `GenPackageDoc-0.39.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 .. Copyright 2020-2022 Robert Bosch GmbH
 
-   Licensed under the Apache License, Version 2.0 (the "License");
+.. Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
-   http://www.apache.org/licenses/LICENSE-2.0
+.. http://www.apache.org/licenses/LICENSE-2.0
 
-   Unless required by applicable law or agreed to in writing, software
+.. Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 GenPackageDoc Description
 =========================
 
-The Python package ``GenPackageDoc`` generates the documentation of Python modules. The content of this documentation is taken out of the docstrings of
+The Python package **GenPackageDoc** generates the documentation of Python modules. The content of this documentation is taken out of the docstrings of
 functions, classes and their methods.
 
 It is possible to extend the documentation by the content of additional files either in reStructuredText (RST) format or in LaTeX format.
 
 The documentation is generated in four steps:
 
 1. Files in LaTeX format are taken over immediately.
 2. Files in reStructuredText format are converted to LaTeX files.
 3. All docstrings of all Python modules in the package are converted to LaTeX files.
 4. All LaTeX files together are converted to a single PDF document. This requires a separately installed LaTeX distribution (recommended: TeX Live).
-   A LaTeX distribution is **not** part of ``GenPackageDoc`` and has to be installed separately!
+   A LaTeX distribution is **not** part of **GenPackageDoc** and has to be installed separately!
 
 How to install
 --------------
 
-``GenPackageDoc`` can be installed in two different ways.
+**GenPackageDoc** can be installed in two different ways.
 
 1. Installation via PyPi (recommended for users)
 
    .. code::
 
       pip install GenPackageDoc
 
@@ -47,36 +47,36 @@
 
    .. code::
 
       git clone https://github.com/test-fullautomation/python-genpackagedoc.git
 
    `GenPackageDoc in GitHub <https://github.com/test-fullautomation/python-genpackagedoc>`_
 
-   Use the following command to install ``GenPackageDoc``:
+   Use the following command to install **GenPackageDoc**:
 
    .. code::
 
       setup.py install
 
 How to use
 ----------
 
-``GenPackageDoc`` provides a toolchain to generate documentation out of Python sources that are stored within a repository.
-``GenPackageDoc`` is also designed to be able to consider setup informations of a repository.
+**GenPackageDoc** provides a toolchain to generate documentation out of Python sources that are stored within a repository.
+**GenPackageDoc** is also designed to be able to consider setup informations of a repository.
 
 The impact is: There is a deep relationship between the repository containing the sources to be documented, and the sources and the configuration
-of ``GenPackageDoc`` itself. Therefore ``GenPackageDoc`` needs to be configured to get to know about things like the path to the package sources
+of **GenPackageDoc** itself. Therefore **GenPackageDoc** needs to be configured to get to know about things like the path to the package sources
 and the desired name of the generated documentation PDF file.
 
-``GenPackageDoc`` is able to use it's own sources to document itself. Therefore the complete
+**GenPackageDoc** is able to use it's own sources to document itself. Therefore the complete
 `GenPackageDoc repository <https://github.com/test-fullautomation/python-genpackagedoc>`_ can be used as example about about writing a package documentation.
 
 At the end of all preparations you will get for your own repository a PDF document that will look like this:
 `GenPackageDoc.pdf <https://github.com/test-fullautomation/python-genpackagedoc/blob/develop/GenPackageDoc/GenPackageDoc.pdf>`_
-(that is the detailed documentation of ``GenPackageDoc``).
+(that is the detailed documentation of **GenPackageDoc**).
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to `Thomas Pollerspöck <mailto:Thomas.Pollerspoeck@de.bosch.com>`_ 
 
 In case you want to report a bug or request any interesting feature, please don't hesitate to raise a ticket.
```

### Comparing `GenPackageDoc-0.34.1/setup.py` & `GenPackageDoc-0.39.0/setup.py`

 * *Files identical despite different names*


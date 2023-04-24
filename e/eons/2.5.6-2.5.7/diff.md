# Comparing `tmp/eons-2.5.6.tar.gz` & `tmp/eons-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.6.tar", last modified: Mon Apr 24 07:41:43 2023, max compression
+gzip compressed data, was "eons-2.5.7.tar", last modified: Mon Apr 24 07:47:50 2023, max compression
```

## Comparing `eons-2.5.6.tar` & `eons-2.5.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.593702 eons-2.5.6/
--rw-rw-r--   0 eons      (1000) eons      (1000)    19826 2023-04-24 07:41:43.593702 eons-2.5.6/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)    19582 2023-04-24 07:41:16.000000 eons-2.5.6/README.md
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.485702 eons-2.5.6/pkg/
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.521702 eons-2.5.6/pkg/eons/
--rw-rw-r--   0 eons      (1000) eons      (1000)       20 2023-04-24 07:41:22.000000 eons-2.5.6/pkg/eons/__init__.py
--rw-rw-r--   0 eons      (1000) eons      (1000)    84500 2023-04-24 07:41:22.000000 eons-2.5.6/pkg/eons/eons.py
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.573702 eons-2.5.6/pkg/eons/method/
--rw-rw-r--   0 eons      (1000) eons      (1000)     1311 2023-04-22 03:51:47.000000 eons-2.5.6/pkg/eons/method/External.py
--rw-rw-r--   0 eons      (1000) eons      (1000)        1 2023-04-24 07:41:22.000000 eons-2.5.6/pkg/eons/method/__init__.py
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.589702 eons-2.5.6/pkg/eons/resolve/
--rw-rw-r--   0 eons      (1000) eons      (1000)        1 2023-04-24 07:41:22.000000 eons-2.5.6/pkg/eons/resolve/__init__.py
--rw-rw-r--   0 eons      (1000) eons      (1000)     3398 2023-03-12 22:13:03.000000 eons-2.5.6/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-rw-r--   0 eons      (1000) eons      (1000)      552 2023-03-12 22:44:28.000000 eons-2.5.6/pkg/eons/resolve/resolve_import_module.py
--rw-rw-r--   0 eons      (1000) eons      (1000)      490 2023-04-06 23:51:53.000000 eons-2.5.6/pkg/eons/resolve/resolve_install_from_repo.py
--rw-rw-r--   0 eons      (1000) eons      (1000)      594 2023-04-07 00:10:27.000000 eons-2.5.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-rw-r--   0 eons      (1000) eons      (1000)      390 2023-04-06 23:51:53.000000 eons-2.5.6/pkg/eons/resolve/resolve_install_with_pip.py
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-04-24 07:41:43.565702 eons-2.5.6/pkg/eons.egg-info/
--rw-rw-r--   0 eons      (1000) eons      (1000)    19826 2023-04-24 07:41:43.000000 eons-2.5.6/pkg/eons.egg-info/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)      563 2023-04-24 07:41:43.000000 eons-2.5.6/pkg/eons.egg-info/SOURCES.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)        1 2023-04-24 07:41:43.000000 eons-2.5.6/pkg/eons.egg-info/dependency_links.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)       32 2023-04-24 07:41:43.000000 eons-2.5.6/pkg/eons.egg-info/requires.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)        5 2023-04-24 07:41:43.000000 eons-2.5.6/pkg/eons.egg-info/top_level.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)      104 2023-04-24 07:41:22.000000 eons-2.5.6/pyproject.toml
--rw-rw-r--   0 eons      (1000) eons      (1000)      714 2023-04-24 07:41:43.601702 eons-2.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.671429 eons-2.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 07:47:50.671429 eons-2.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-24 07:47:31.000000 eons-2.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.663429 eons-2.5.7/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.671429 eons-2.5.7/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:40.000000 eons-2.5.7/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 07:47:19.000000 eons-2.5.7/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:47:50.667429 eons-2.5.7/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 07:47:50.000000 eons-2.5.7/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 07:47:40.000000 eons-2.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 07:47:50.671429 eons-2.5.7/setup.cfg
```

### Comparing `eons-2.5.6/PKG-INFO` & `eons-2.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.6
+Version: 2.5.7
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.6/README.md` & `eons-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/pkg/eons/eons.py` & `eons-2.5.7/pkg/eons/eons.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
-import operator
-import traceback
-import jsonpickle
-from copy import deepcopy
 import os
+import shutil
+from copy import deepcopy
+import builtins
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
-import re
+import traceback
+import jsonpickle
 from pathlib import Path
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
-import shutil
-import builtins
 import inspect
+import ctypes
+import operator
+import re
 import argparse
 import requests
 import yaml
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
-import ctypes
 
 ######## START CONTENT ########
 def INVALID_NAME():
 	return "INVALID_NAME"
 
 class ActualType(type):
 	def __repr__(self):
@@ -60,157 +60,14 @@
 class FatalCannotExecute(Fatal, metaclass=ActualType): pass
 
 class PackageError(Exception, metaclass=ActualType): pass
 
 class MethodPendingPopulation(Exception, metaclass=ActualType): pass
 
 
-# util is a namespace for any miscellaneous utilities.
-# You cannot create a util.
-class util:
-	def __init__(this):
-		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
-
-	#dot.notation access to dictionary attributes
-	class DotDict(dict):
-		__getattr__ = dict.get
-		__setattr__ = dict.__setitem__
-		__delattr__ = dict.__delitem__
-
-		def __deepcopy__(this, memo=None):
-			return util.DotDict(deepcopy(dict(this), memo=memo))
-
-	# DotDict doesn't pickle right, since it's a class and not a native dict.
-	class DotDictPickler(jsonpickle.handlers.BaseHandler):
-		def flatten(this, dotdict, data):
-			return dict(dotdict)
-
-	@staticmethod
-	def RecursiveAttrFunc(func, obj, attrList):
-		attr = attrList.pop(0)
-		if (not attrList):
-			return eval(f"{func}attr(obj, attr)")
-		if (not hasattr(obj, attr)):
-			raise AttributeError(f"{obj} has not attribute '{attr}'")
-		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
-
-	@staticmethod
-	def HasAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
-
-	@staticmethod
-	def GetAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
-
-	@staticmethod
-	def SetAttr(obj, attrStr):
-		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
-
-
-	@staticmethod
-	def LogStack():
-		logging.debug(traceback.format_exc())
-
-
-	class console:
-
-		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
-
-		saturationCode = {
-			'dark': 3,
-			'light': 9
-		}
-
-		foregroundCodes = {
-			'black': 0,
-			'red': 1,
-			'green': 2,
-			'yellow': 3,
-			'blue': 4,
-			'magenta': 5,
-			'cyan': 6,
-			'white': 7
-		}
-
-		backgroundCodes = {
-			'none': 0,
-			'black': 40,
-			'red': 41,
-			'green': 42,
-			'yellow': 43,
-			'blue': 44,
-			'magenta': 45,
-			'cyan': 46,
-			'white': 47,
-		}
-
-		styleCodes = {
-			'none': 0,
-			'bold': 1,
-			'faint': 2, # Not widely supported.
-			'italic': 3, # Not widely supported.
-			'underline': 4,
-			'blink_slow': 5,
-			'blink_fast': 6, # Not widely supported.
-			'invert': 7,
-			'conceal': 8, # Not widely supported.
-			'strikethrough': 9, # Not widely supported.
-			'frame': 51,
-			'encircle': 52,
-			'overline': 53
-		}
-
-		@classmethod
-		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
-			if (styles is None):
-				styles = []
-			#\x1b may also work.
-			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
-			if (background != 'none'):
-				compiledCode += f";{cls.backgroundCodes[background]}"
-			if (styles):
-				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in styles])
-			compiledCode += 'm'
-			return compiledCode
-
-		resetStyle = "\033[0m"
-
-
-	# Add a logging level
-	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
-	@staticmethod
-	def AddLoggingLevel(level, value):
-		levelName = level.upper()
-		methodName = level.lower()
-
-		if hasattr(logging, levelName):
-			raise AttributeError('{} already defined in logging module'.format(levelName))
-		if hasattr(logging, methodName):
-			raise AttributeError('{} already defined in logging module'.format(methodName))
-		if hasattr(logging.getLogger(), methodName):
-			raise AttributeError('{} already defined in logger class'.format(methodName))
-
-		# This method was inspired by the answers to Stack Overflow post
-		# http://stackoverflow.com/q/2183233/2988730, especially
-		# http://stackoverflow.com/a/13638084/2988730
-		def logForLevel(this, message, *args, **kwargs):
-			if this.isEnabledFor(value):
-				this._log(value, message, args, **kwargs)
-		def logToRoot(message, *args, **kwargs):
-			logging.log(value, message, *args, **kwargs)
-
-		logging.addLevelName(value, levelName)
-		setattr(logging, levelName, value)
-		setattr(logging.getLogger(), methodName, logForLevel)
-		setattr(logging, methodName, logToRoot)
-
-
-jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
-
-
 #Self registration for use with json loading.
 #Any class that derives from SelfRegistering can be instantiated with:
 #   SelfRegistering("ClassName")
 #Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
 class SelfRegistering(object):
 
 	def __init__(this, *args, **kwargs):
@@ -320,171 +177,155 @@
 
 
 	# Sets valid to false.
 	def Invalidate(this):
 		this.valid = False
 
 
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
+# util is a namespace for any miscellaneous utilities.
+# You cannot create a util.
+class util:
+	def __init__(this):
+		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
 
+	#dot.notation access to dictionary attributes
+	class DotDict(dict):
+		__getattr__ = dict.get
+		__setattr__ = dict.__setitem__
+		__delattr__ = dict.__delitem__
 
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
+		def __deepcopy__(this, memo=None):
+			return util.DotDict(deepcopy(dict(this), memo=memo))
 
+	# DotDict doesn't pickle right, since it's a class and not a native dict.
+	class DotDictPickler(jsonpickle.handlers.BaseHandler):
+		def flatten(this, dotdict, data):
+			return dict(dotdict)
 
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
+	@staticmethod
+	def RecursiveAttrFunc(func, obj, attrList):
+		attr = attrList.pop(0)
+		if (not attrList):
+			return eval(f"{func}attr(obj, attr)")
+		if (not hasattr(obj, attr)):
+			raise AttributeError(f"{obj} has not attribute '{attr}'")
+		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
 
+	@staticmethod
+	def HasAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
 
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
+	@staticmethod
+	def GetAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
 
+	@staticmethod
+	def SetAttr(obj, attrStr):
+		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
 
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
 
+	@staticmethod
+	def LogStack():
+		logging.debug(traceback.format_exc())
 
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
 
+	class console:
 
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
+		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
 
+		saturationCode = {
+			'dark': 3,
+			'light': 9
+		}
 
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
+		foregroundCodes = {
+			'black': 0,
+			'red': 1,
+			'green': 2,
+			'yellow': 3,
+			'blue': 4,
+			'magenta': 5,
+			'cyan': 6,
+			'white': 7
+		}
 
+		backgroundCodes = {
+			'none': 0,
+			'black': 40,
+			'red': 41,
+			'green': 42,
+			'yellow': 43,
+			'blue': 44,
+			'magenta': 45,
+			'cyan': 46,
+			'white': 47,
+		}
 
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
+		styleCodes = {
+			'none': 0,
+			'bold': 1,
+			'faint': 2, # Not widely supported.
+			'italic': 3, # Not widely supported.
+			'underline': 4,
+			'blink_slow': 5,
+			'blink_fast': 6, # Not widely supported.
+			'invert': 7,
+			'conceal': 8, # Not widely supported.
+			'strikethrough': 9, # Not widely supported.
+			'frame': 51,
+			'encircle': 52,
+			'overline': 53
+		}
 
+		@classmethod
+		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
+			if (styles is None):
+				styles = []
+			#\x1b may also work.
+			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
+			if (background != 'none'):
+				compiledCode += f";{cls.backgroundCodes[background]}"
+			if (styles):
+				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in styles])
+			compiledCode += 'm'
+			return compiledCode
 
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
+		resetStyle = "\033[0m"
 
 
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
+	# Add a logging level
+	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
+	@staticmethod
+	def AddLoggingLevel(level, value):
+		levelName = level.upper()
+		methodName = level.lower()
 
+		if hasattr(logging, levelName):
+			raise AttributeError('{} already defined in logging module'.format(levelName))
+		if hasattr(logging, methodName):
+			raise AttributeError('{} already defined in logging module'.format(methodName))
+		if hasattr(logging.getLogger(), methodName):
+			raise AttributeError('{} already defined in logger class'.format(methodName))
 
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
+		# This method was inspired by the answers to Stack Overflow post
+		# http://stackoverflow.com/q/2183233/2988730, especially
+		# http://stackoverflow.com/a/13638084/2988730
+		def logForLevel(this, message, *args, **kwargs):
+			if this.isEnabledFor(value):
+				this._log(value, message, args, **kwargs)
+		def logToRoot(message, *args, **kwargs):
+			logging.log(value, message, *args, **kwargs)
 
+		logging.addLevelName(value, levelName)
+		setattr(logging, levelName, value)
+		setattr(logging.getLogger(), methodName, logForLevel)
+		setattr(logging, methodName, logToRoot)
 
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
 
+jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
@@ -1444,14 +1285,232 @@
 		if (saveout):
 			return process.returncode, output
 		
 		return process.returncode
 	######## END: UTILITIES ########
 
 
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# The data *this contains.
+		this.data = []
+
+
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
+
+
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
+
+
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
+
+
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
+
+
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
+
+
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
+
+
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
+
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
+
+
+
 # Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
 # ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
 # Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
 # NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
 # startPosition is always positive
 # endPosition is always negative
@@ -1676,64 +1735,14 @@
 		return ret
 
 	#  We failed to resolve the error. Die
 	sys.tracebacklimit = 0 # traceback is NOT helpful here.
 	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
 
 
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
-#
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
-		else:
-			return None
-
-		this.executors = [None]
-
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
-
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
-
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
-
-		logging.debug(f"Now tracking Executor: {executor}")
-
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
-
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
-
-
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
 #			super().__init__()
 #	. . .
@@ -2395,16 +2404,7 @@
 		for key, val in this.extraArgs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
-
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
```

### Comparing `eons-2.5.6/pkg/eons/method/External.py` & `eons-2.5.7/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.7/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.7/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.7/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.7/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.6
+Version: 2.5.7
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.6/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.7/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.5.6/setup.cfg` & `eons-2.5.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.5.6
+version = 2.5.7
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	jsonpickle
-	tqdm
 	pyyaml
 	requests
+	jsonpickle
+	tqdm
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


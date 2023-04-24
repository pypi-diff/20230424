# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.2.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.2.tar", last modified: Thu Apr 20 20:33:46 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.3.tar", last modified: Mon Apr 24 15:45:47 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.2.tar` & `com.castsoftware.uc.oneclick-0.2.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:33:46.579041 com.castsoftware.uc.oneclick-0.2.2.2/
--rw-rw-rw-   0        0        0      517 2023-04-20 20:33:46.567851 com.castsoftware.uc.oneclick-0.2.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 20:33:46.316697 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-04-20 20:33:46.000000 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-04-20 20:33:46.000000 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:33:46.000000 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-04-20 20:33:46.000000 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 20:33:46.000000 com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 20:33:46.405889 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:33:46.459137 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3454 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19726 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:33:46.555390 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9049 2023-04-20 20:31:28.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6803 2023-04-20 20:26:23.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11312 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.2/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0      737 2023-04-20 20:33:31.000000 com.castsoftware.uc.oneclick-0.2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 20:33:46.579041 com.castsoftware.uc.oneclick-0.2.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.988118 com.castsoftware.uc.oneclick-0.2.2.3/
+-rw-rw-rw-   0        0        0      517 2023-04-24 15:45:46.978077 com.castsoftware.uc.oneclick-0.2.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.680508 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.769439 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.826132 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3454 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19536 2023-04-24 15:43:03.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.964703 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9049 2023-04-20 20:31:28.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6803 2023-04-20 20:26:23.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11311 2023-04-24 15:11:15.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0      737 2023-04-24 15:45:27.000000 com.castsoftware.uc.oneclick-0.2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:45:46.988118 com.castsoftware.uc.oneclick-0.2.2.3/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,17 @@
             if self.check_default(args.hlURL,self.hl_url,default_args['hlURL']):
                 self.hl_url = f'{args.hlURL}/WS2'
             if args.hlUser is not None: self.hl_user = args.hlUser
             if args.hlPassword is not None: self.hl_password = args.hlPassword
             if args.hlInstance is not None: self.hl_instance = args.hlInstance
             if self.check_default(args.hlCLI,self.hl_cli,default_args['hlCLI']):
                 self.hl_cli = args.hlCLI
-            if self.check_default(args.HLPerlInstallDir,self.perl_install_dir,default_args['HLPerlInstallDir']):
-                self.perl_install_dir = args.HLPerlInstallDir
-            if self.check_default(args.HLAnalyzerDir,self.analyzer_dir,default_args['HLAnalyzerDir']):
-                self.analyzer_dir = args.HLAnalyzerDir
+
+            self.perl_install_dir = abspath(f'{args.hlAgent}/strawberry/perl')
+            self.analyzer_dir = abspath(f'{args.hlAgent}/perl')
 
             #AIPConsole
             if args.consoleURL is not None: self.console_url = args.consoleURL
             if args.consoleKey is not None: self.console_key = args.consoleKey
             if args.consoleCLI is not None: self.console_cli = args.consoleCLI
             if args.enable_security_assessment is not None: self.enable_security_assessment = args.enable_security_assessment
             if args.blueprint is not None: self.blueprint = args.blueprint
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cloc.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,22 +82,22 @@
     highlight.add_argument('--hlUser',  help='Highlight User',metavar='USER')
     highlight.add_argument('--hlPassword',  help='Highlight Password',metavar='PASSWORD')
     highlight.add_argument('--hlInstance',  help='Highlight Instance Id',type=int,metavar='ID')
     highlight.add_argument('--hlCLI',
                             default='c:/Program Files/CAST/Highlight-Automation-Command/HighlightAutomation.jar', 
                             help='Highlight CLI Location',
                             metavar='LOCATION')
-    highlight.add_argument('--HLPerlInstallDir',
+    highlight.add_argument('--hlAgent',
                             default='c:/Program Files/CAST/HighlightAgent',
                             help='Highlight Perl Installation Location (HighlightAgent/strawberry/perl)',
                             metavar='LOCATION')
-    highlight.add_argument('--HLAnalyzerDir', 
-                           default='c:/Program Files/CAST/HighlightAgent/perl',
-                           help='Highlight Perl Installation Location (HighlightAgent/perl)',
-                           metavar='LOCATION')
+    # highlight.add_argument('--HLAnalyzerDir', 
+    #                        default='c:/Program Files/CAST/HighlightAgent/perl',
+    #                        help='Highlight Perl Installation Location (HighlightAgent/perl)',
+    #                        metavar='LOCATION')
 
     console=config_parser.add_argument_group('CAST AIP Console')
     console.add_argument('--consoleURL',  help='AIP Console URL',metavar='URL')
     console.add_argument('--consoleKey',  help='AIP Console Key',metavar='KEY')
     console.add_argument('--consoleCLI',  help='AIP Console CLI Location',metavar='LOCATION')
     console.add_argument('--enable-security-assessment', help='AIP Console security-assessment', default=True)
     console.add_argument('--blueprint', help='AIP Console blueprint design', default=True)
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.2/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.2' #prod version
+version='0.2.2.3' #prod version
 dependencies = [
     'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
     'com.castsoftware.uc.python.common>=0.1.6',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
```


# Comparing `tmp/oxdork-3.0.0.tar.gz` & `tmp/oxdork-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxdork-3.0.0.tar", last modified: Tue Feb  7 11:08:40 2023, max compression
+gzip compressed data, was "oxdork-3.1.0.tar", last modified: Mon Apr 24 21:58:25 2023, max compression
```

## Comparing `oxdork-3.0.0.tar` & `oxdork-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:08:40.134744 oxdork-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-07 11:08:21.000000 oxdork-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-07 11:08:40.134744 oxdork-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-07 11:08:21.000000 oxdork-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:08:40.134744 oxdork-3.0.0/oxdork/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-07 11:08:21.000000 oxdork-3.0.0/oxdork/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-07 11:08:21.000000 oxdork-3.0.0/oxdork/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-07 11:08:21.000000 oxdork-3.0.0/oxdork/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-07 11:08:21.000000 oxdork-3.0.0/oxdork/oxdork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:08:40.134744 oxdork-3.0.0/oxdork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-07 11:08:40.000000 oxdork-3.0.0/oxdork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 11:08:40.134744 oxdork-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-07 11:08:21.000000 oxdork-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 21:58:14.000000 oxdork-3.1.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 21:58:14.000000 oxdork-3.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 21:58:14.000000 oxdork-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:58:14.000000 oxdork-3.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 21:58:14.000000 oxdork-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-24 21:58:25.954233 oxdork-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-24 21:58:14.000000 oxdork-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/dork_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)   148095 2023-04-24 21:58:14.000000 oxdork-3.1.0/dork_queries/dork_queries.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/oxdork/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/oxdork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/oxdork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 21:58:14.000000 oxdork-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:58:25.954233 oxdork-3.1.0/setup.cfg
```

### Comparing `oxdork-3.0.0/LICENSE` & `oxdork-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oxdork-3.0.0/PKG-INFO` & `oxdork-3.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 Metadata-Version: 2.1
 Name: oxdork
-Version: 3.0.0
+Version: 3.1.0
 Summary: Google dorking tool
-Home-page: https://github.com/rly0nheart/oxdork
-Author: Richard Mwewa
-Author-email: rly0nheart@duck.com
+Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
+        
+        Copyright (c) 2022 Richard Mwewa
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/rly0nheart/oxdork
+Project-URL: documentation, https://github.com/rly0nheart/oxdork/wiki/
+Project-URL: repository, https://github.com/rly0nheart/oxdork.git
+Keywords: python,osint,google-dorking,osint,inurl,intext,intitle
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
+Classifier: 
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Screenshot_20210827-111909-removebg-preview](https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-fe9b76c4518c.png)
 
 ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-red?style=for-the-badge&logo=linux)
+![OS](https://img.shields.io/badge/OS-Windows-blue?style=for-the-badge&logo=Windows)
 ![GitHub](https://img.shields.io/github/license/rly0nheart/oxdork?style=for-the-badge&logo=github)
-![CodeFactor](https://www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-badge&logo=codefactor)
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/oxdork?include_prereleases&style=for-the-badge&logo=github)
 ![GitHub repo size](https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-badge&logo=github)
 
 
 
 ![Screenshot_20230207_124512](https://user-images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-09c7dad081e3.png)
```

#### html2text {}

```diff
@@ -1,22 +1,40 @@
-Metadata-Version: 2.1 Name: oxdork Version: 3.0.0 Summary: Google dorking tool
-Home-page: https://github.com/rly0nheart/oxdork Author: Richard Mwewa Author-
-email: rly0nheart@duck.com License: MIT License Classifier: Development Status
-:: 5 - Production/Stable Classifier: Intended Audience :: Information
-Technology Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Description-Content-Type: text/
-markdown License-File: LICENSE ![Screenshot_20210827-111909-removebg-preview]
-(https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-
-4876-8665-fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
-red?style=for-the-badge&logo=linux) ![GitHub](https://img.shields.io/github/
-license/rly0nheart/oxdork?style=for-the-badge&logo=github) ![CodeFactor](https:
-//www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-
-badge&logo=codefactor) ![GitHub release (latest by date including pre-
-releases)](https://img.shields.io/github/v/release/rly0nheart/
+Metadata-Version: 2.1 Name: oxdork Version: 3.1.0 Summary: Google dorking tool
+Author-email: Richard Mwewa
+duck.com> License: MIT License Copyright (c) 2022 Richard Mwewa Permission is
+hereby granted, free of charge, to any person obtaining a copy of this software
+and associated documentation files (the "Software"), to deal in the Software
+without restriction, including without limitation the rights to use, copy,
+modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/rly0nheart/
+oxdork Project-URL: documentation, https://github.com/rly0nheart/oxdork/wiki/
+Project-URL: repository, https://github.com/rly0nheart/oxdork.git Keywords:
+python,osint,google-dorking,osint,inurl,intext,intitle Classifier: Development
+Status :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English Classifier: Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE !
+[Screenshot_20210827-111909-removebg-preview](https://user-
+images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-
+fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
+red?style=for-the-badge&logo=linux) ![OS](https://img.shields.io/badge/OS-
+Windows-blue?style=for-the-badge&logo=Windows) ![GitHub](https://
+img.shields.io/github/license/rly0nheart/oxdork?style=for-the-
+badge&logo=github) ![GitHub release (latest by date including pre-releases)]
+(https://img.shields.io/github/v/release/rly0nheart/
 oxdork?include_prereleases&style=for-the-badge&logo=github) ![GitHub repo size]
 (https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-
 badge&logo=github) ![Screenshot_20230207_124512](https://user-
 images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-
 09c7dad081e3.png) oxDork uses Google dorking techniques and Google dorks to
 find security holes and misconfigurations in web servers. # Wiki Check the
 *Installation guide*, *Usage*, and *a Available options* on the [wiki](https://
```

### Comparing `oxdork-3.0.0/README.md` & `oxdork-3.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![Screenshot_20210827-111909-removebg-preview](https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-fe9b76c4518c.png)
 
 ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-red?style=for-the-badge&logo=linux)
+![OS](https://img.shields.io/badge/OS-Windows-blue?style=for-the-badge&logo=Windows)
 ![GitHub](https://img.shields.io/github/license/rly0nheart/oxdork?style=for-the-badge&logo=github)
-![CodeFactor](https://www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-badge&logo=codefactor)
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/oxdork?include_prereleases&style=for-the-badge&logo=github)
 ![GitHub repo size](https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-badge&logo=github)
 
 
 
 ![Screenshot_20230207_124512](https://user-images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-09c7dad081e3.png)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ![Screenshot_20210827-111909-removebg-preview](https://user-
 images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-
 fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
-red?style=for-the-badge&logo=linux) ![GitHub](https://img.shields.io/github/
-license/rly0nheart/oxdork?style=for-the-badge&logo=github) ![CodeFactor](https:
-//www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-
-badge&logo=codefactor) ![GitHub release (latest by date including pre-
-releases)](https://img.shields.io/github/v/release/rly0nheart/
+red?style=for-the-badge&logo=linux) ![OS](https://img.shields.io/badge/OS-
+Windows-blue?style=for-the-badge&logo=Windows) ![GitHub](https://
+img.shields.io/github/license/rly0nheart/oxdork?style=for-the-
+badge&logo=github) ![GitHub release (latest by date including pre-releases)]
+(https://img.shields.io/github/v/release/rly0nheart/
 oxdork?include_prereleases&style=for-the-badge&logo=github) ![GitHub repo size]
 (https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-
 badge&logo=github) ![Screenshot_20230207_124512](https://user-
 images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-
 09c7dad081e3.png) oxDork uses Google dorking techniques and Google dorks to
 find security holes and misconfigurations in web servers. # Wiki Check the
 *Installation guide*, *Usage*, and *a Available options* on the [wiki](https://
```

### Comparing `oxdork-3.0.0/oxdork/banner.py` & `oxdork-3.1.0/oxdork/banner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-version_tag = "3.0.0"
-
-
 def ascii_banner():
+    version_tag = "3.1.0"
     banner = f"""[red]
       ▐▄• ▄ ·▄▄▄▄        ▄▄▄  ▄ •▄ 
  ▄█▀▄  █▌█▌▪██▪ ██  ▄█▀▄ ▀▄ █·█▌▄▌▪
 ▐█▌.▐▌ ·██· ▐█· ▐█▌▐█▌.▐▌▐▀▀▄ ▐▀▀▄·
 ▐█▌.▐▌▪▐█·█▌██. ██ ▐█▌.▐▌▐█•█▌▐█.█▌
  ▀█▄▀▪•▀▀ ▀▀▀▀▀▀▀•  ▀█▄▀▪.▀  ▀·▀  ▀
                              [/]v{version_tag}"""
-    return banner
+    return banner, version_tag
```

### Comparing `oxdork-3.0.0/oxdork.egg-info/PKG-INFO` & `oxdork-3.1.0/oxdork.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 Metadata-Version: 2.1
 Name: oxdork
-Version: 3.0.0
+Version: 3.1.0
 Summary: Google dorking tool
-Home-page: https://github.com/rly0nheart/oxdork
-Author: Richard Mwewa
-Author-email: rly0nheart@duck.com
+Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
+        
+        Copyright (c) 2022 Richard Mwewa
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/rly0nheart/oxdork
+Project-URL: documentation, https://github.com/rly0nheart/oxdork/wiki/
+Project-URL: repository, https://github.com/rly0nheart/oxdork.git
+Keywords: python,osint,google-dorking,osint,inurl,intext,intitle
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
+Classifier: 
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Screenshot_20210827-111909-removebg-preview](https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-fe9b76c4518c.png)
 
 ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-red?style=for-the-badge&logo=linux)
+![OS](https://img.shields.io/badge/OS-Windows-blue?style=for-the-badge&logo=Windows)
 ![GitHub](https://img.shields.io/github/license/rly0nheart/oxdork?style=for-the-badge&logo=github)
-![CodeFactor](https://www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-badge&logo=codefactor)
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/oxdork?include_prereleases&style=for-the-badge&logo=github)
 ![GitHub repo size](https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-badge&logo=github)
 
 
 
 ![Screenshot_20230207_124512](https://user-images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-09c7dad081e3.png)
```

#### html2text {}

```diff
@@ -1,22 +1,40 @@
-Metadata-Version: 2.1 Name: oxdork Version: 3.0.0 Summary: Google dorking tool
-Home-page: https://github.com/rly0nheart/oxdork Author: Richard Mwewa Author-
-email: rly0nheart@duck.com License: MIT License Classifier: Development Status
-:: 5 - Production/Stable Classifier: Intended Audience :: Information
-Technology Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Description-Content-Type: text/
-markdown License-File: LICENSE ![Screenshot_20210827-111909-removebg-preview]
-(https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-
-4876-8665-fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
-red?style=for-the-badge&logo=linux) ![GitHub](https://img.shields.io/github/
-license/rly0nheart/oxdork?style=for-the-badge&logo=github) ![CodeFactor](https:
-//www.codefactor.io/repository/github/rly0nheart/oxdork/badge?style=for-the-
-badge&logo=codefactor) ![GitHub release (latest by date including pre-
-releases)](https://img.shields.io/github/v/release/rly0nheart/
+Metadata-Version: 2.1 Name: oxdork Version: 3.1.0 Summary: Google dorking tool
+Author-email: Richard Mwewa
+duck.com> License: MIT License Copyright (c) 2022 Richard Mwewa Permission is
+hereby granted, free of charge, to any person obtaining a copy of this software
+and associated documentation files (the "Software"), to deal in the Software
+without restriction, including without limitation the rights to use, copy,
+modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/rly0nheart/
+oxdork Project-URL: documentation, https://github.com/rly0nheart/oxdork/wiki/
+Project-URL: repository, https://github.com/rly0nheart/oxdork.git Keywords:
+python,osint,google-dorking,osint,inurl,intext,intitle Classifier: Development
+Status :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English Classifier: Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE !
+[Screenshot_20210827-111909-removebg-preview](https://user-
+images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-
+fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
+red?style=for-the-badge&logo=linux) ![OS](https://img.shields.io/badge/OS-
+Windows-blue?style=for-the-badge&logo=Windows) ![GitHub](https://
+img.shields.io/github/license/rly0nheart/oxdork?style=for-the-
+badge&logo=github) ![GitHub release (latest by date including pre-releases)]
+(https://img.shields.io/github/v/release/rly0nheart/
 oxdork?include_prereleases&style=for-the-badge&logo=github) ![GitHub repo size]
 (https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-
 badge&logo=github) ![Screenshot_20230207_124512](https://user-
 images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-
 09c7dad081e3.png) oxDork uses Google dorking techniques and Google dorks to
 find security holes and misconfigurations in web servers. # Wiki Check the
 *Installation guide*, *Usage*, and *a Available options* on the [wiki](https://
```


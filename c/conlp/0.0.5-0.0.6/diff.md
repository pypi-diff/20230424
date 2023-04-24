# Comparing `tmp/conlp-0.0.5.tar.gz` & `tmp/conlp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlp-0.0.5.tar", last modified: Thu Apr 20 19:23:23 2023, max compression
+gzip compressed data, was "conlp-0.0.6.tar", last modified: Mon Apr 24 06:58:22 2023, max compression
```

## Comparing `conlp-0.0.5.tar` & `conlp-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.249848 conlp-0.0.5/
--rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      403 2023-04-20 19:23:23.249848 conlp-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.244849 conlp-0.0.5/conlp/
--rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.5/conlp/__init__.py
--rw-rw-rw-   0        0        0    13681 2023-04-20 19:20:32.000000 conlp-0.0.5/conlp/download.py
--rw-rw-rw-   0        0        0     2553 2023-04-20 19:02:41.000000 conlp-0.0.5/conlp/preprocess.py
--rw-rw-rw-   0        0        0    26142 2023-04-20 19:21:04.000000 conlp-0.0.5/conlp/sentiment.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.249848 conlp-0.0.5/conlp.egg-info/
--rw-rw-rw-   0        0        0      403 2023-04-20 19:23:22.000000 conlp-0.0.5/conlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:23:22.000000 conlp-0.0.5/conlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 19:23:23.250848 conlp-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-04-20 19:23:14.000000 conlp-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:58:22.437680 conlp-0.0.6/
+-rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      403 2023-04-24 06:58:22.437680 conlp-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:58:22.430682 conlp-0.0.6/conlp/
+-rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.6/conlp/__init__.py
+-rw-rw-rw-   0        0        0    13681 2023-04-20 19:20:32.000000 conlp-0.0.6/conlp/download.py
+-rw-rw-rw-   0        0        0     3259 2023-04-24 06:55:57.000000 conlp-0.0.6/conlp/keyword.py
+-rw-rw-rw-   0        0        0     2553 2023-04-20 19:02:41.000000 conlp-0.0.6/conlp/preprocess.py
+-rw-rw-rw-   0        0        0    26142 2023-04-20 19:21:04.000000 conlp-0.0.6/conlp/sentiment.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:58:22.436680 conlp-0.0.6/conlp.egg-info/
+-rw-rw-rw-   0        0        0      403 2023-04-24 06:58:22.000000 conlp-0.0.6/conlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-24 06:58:22.000000 conlp-0.0.6/conlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:58:22.000000 conlp-0.0.6/conlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-24 06:58:22.000000 conlp-0.0.6/conlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 06:58:22.000000 conlp-0.0.6/conlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-24 06:58:22.438680 conlp-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-24 06:57:51.000000 conlp-0.0.6/setup.py
```

### Comparing `conlp-0.0.5/LICENSE.txt` & `conlp-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conlp-0.0.5/conlp/download.py` & `conlp-0.0.6/conlp/download.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.5/conlp/preprocess.py` & `conlp-0.0.6/conlp/preprocess.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.5/conlp/sentiment.py` & `conlp-0.0.6/conlp/sentiment.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.5/setup.py` & `conlp-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup 
 
 setup(
   name = 'conlp',
   packages = ['conlp'],
-  version = '0.0.5',
+  version = '0.0.6',
   license='Apache-2.0',
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',
   author_email = 'nick.sh.oh@socialscience.ai',    
   url = 'https://github.com/SOCIALSCIENCEai/coNLP',  
-  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.5.tar.gz',
+  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.6.tar.gz',
   keywords = ['NLP', 'SOCIAL SCIENCE'],   
   install_requires=[           
           'torch',
           'transformers',
           'transformers[sentencepiece]',
           'scipy',
           'numpy',
```


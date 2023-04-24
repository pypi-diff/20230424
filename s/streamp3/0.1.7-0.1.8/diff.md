# Comparing `tmp/streamp3-0.1.7.tar.gz` & `tmp/streamp3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/streamp3-0.1.7.tar", last modified: Tue Sep 15 21:09:49 2020, max compression
+gzip compressed data, was "dist/streamp3-0.1.8.tar", last modified: Mon Apr 24 21:17:33 2023, max compression
```

## Comparing `streamp3-0.1.7.tar` & `streamp3-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2020-09-15 21:09:49.000000 streamp3-0.1.7/
--rw-r--r--   0 brent      (501) staff       (20)       38 2019-07-03 00:24:06.000000 streamp3-0.1.7/MANIFEST.in
--rw-r--r--   0 brent      (501) staff       (20)     4409 2020-09-15 21:09:49.000000 streamp3-0.1.7/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)     3156 2019-07-03 00:24:06.000000 streamp3-0.1.7/README.md
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2020-09-15 21:09:49.000000 streamp3-0.1.7/lame/
--rw-r--r--   0 brent      (501) staff       (20)        0 2019-07-03 00:24:06.000000 streamp3-0.1.7/lame/__init__.py
--rw-r--r--   0 brent      (501) staff       (20)     2429 2019-07-03 00:24:06.000000 streamp3-0.1.7/lame/hip.pyx
--rw-r--r--   0 brent      (501) staff       (20)      487 2019-07-03 00:24:06.000000 streamp3-0.1.7/lame/lame.pxd
--rw-r--r--   0 brent      (501) staff       (20)       38 2020-09-15 21:09:49.000000 streamp3-0.1.7/setup.cfg
--rw-r--r--   0 brent      (501) staff       (20)      888 2020-09-15 21:09:20.000000 streamp3-0.1.7/setup.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2020-09-15 21:09:49.000000 streamp3-0.1.7/streamp3/
--rw-r--r--   0 brent      (501) staff       (20)     7429 2020-09-15 21:08:12.000000 streamp3-0.1.7/streamp3/__init__.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2020-09-15 21:09:49.000000 streamp3-0.1.7/streamp3.egg-info/
--rw-r--r--   0 brent      (501) staff       (20)     4409 2020-09-15 21:09:48.000000 streamp3-0.1.7/streamp3.egg-info/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      264 2020-09-15 21:09:49.000000 streamp3-0.1.7/streamp3.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (501) staff       (20)        1 2020-09-15 21:09:48.000000 streamp3-0.1.7/streamp3.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (501) staff       (20)       15 2020-09-15 21:09:48.000000 streamp3-0.1.7/streamp3.egg-info/requires.txt
--rw-r--r--   0 brent      (501) staff       (20)       14 2020-09-15 21:09:48.000000 streamp3-0.1.7/streamp3.egg-info/top_level.txt
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/
+-rw-r--r--   0 brent      (501) staff       (20)       38 2019-07-03 00:24:06.000000 streamp3-0.1.8/MANIFEST.in
+-rw-r--r--   0 brent      (501) staff       (20)     4559 2023-04-24 21:17:33.000000 streamp3-0.1.8/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)     3242 2020-10-19 14:24:34.000000 streamp3-0.1.8/README.md
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/lame/
+-rw-r--r--   0 brent      (501) staff       (20)        0 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/__init__.py
+-rw-r--r--   0 brent      (501) staff       (20)     2429 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/hip.pyx
+-rw-r--r--   0 brent      (501) staff       (20)      487 2019-07-03 00:24:06.000000 streamp3-0.1.8/lame/lame.pxd
+-rw-r--r--   0 brent      (501) staff       (20)       38 2023-04-24 21:17:33.000000 streamp3-0.1.8/setup.cfg
+-rw-r--r--   0 brent      (501) staff       (20)      888 2023-04-24 21:17:22.000000 streamp3-0.1.8/setup.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3/
+-rw-r--r--   0 brent      (501) staff       (20)     7427 2020-09-16 18:14:48.000000 streamp3-0.1.8/streamp3/__init__.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/
+-rw-r--r--   0 brent      (501) staff       (20)     4559 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      264 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (501) staff       (20)        1 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (501) staff       (20)       15 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/requires.txt
+-rw-r--r--   0 brent      (501) staff       (20)       14 2023-04-24 21:17:33.000000 streamp3-0.1.8/streamp3.egg-info/top_level.txt
```

### Comparing `streamp3-0.1.7/PKG-INFO` & `streamp3-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamp3
-Version: 0.1.7
+Version: 0.1.8
 Summary: streaming mp3 decoder
 Home-page: https://github.com/pylon/streamp3/
 Author: Brent M. Spell
 Author-email: brent@pylon.com
 License: UNKNOWN
 Description: # streamp3
         
@@ -13,15 +13,29 @@
         ## Status
         [![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
         [![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
         [![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
         
         ## Installation
         
-        ### Pip
+        First, make sure you have the LAME libraries and headers installed.
+        
+        #### macOS
+        
+        ```bash
+        brew install lame
+        ```
+        
+        #### Debian/Ubuntu
+        
+        ```bash
+        apt install libmp3lame-dev
+        ```
+        
+        ### Install with pip
         ```bash
         pip install streamp3
         ```
         
         ## Usage
         To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
         stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
@@ -68,20 +82,14 @@
         
         ```bash
         pyenv install 3.6.4
         pyenv virtualenv 3.6.4 streamp3
         pip install -r requirements.txt
         ```
         
-        LAME must also be installed. This can be done on OSX via homebrew.
-        
-        ```bash
-        brew install lame
-        ```
-        
         ### Deployment
         The project uses setup.py for installation and is deployed to
         [PyPI](https://pypi.org). The project can be built for installation with
         the following command:
         
         ```bash
         python setup.py clean --all; rm -r ./dist
```

### Comparing `streamp3-0.1.7/README.md` & `streamp3-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,29 @@
 ## Status
 [![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
 [![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
 [![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
 
 ## Installation
 
-### Pip
+First, make sure you have the LAME libraries and headers installed.
+
+#### macOS
+
+```bash
+brew install lame
+```
+
+#### Debian/Ubuntu
+
+```bash
+apt install libmp3lame-dev
+```
+
+### Install with pip
 ```bash
 pip install streamp3
 ```
 
 ## Usage
 To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
 stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
@@ -60,20 +74,14 @@
 
 ```bash
 pyenv install 3.6.4
 pyenv virtualenv 3.6.4 streamp3
 pip install -r requirements.txt
 ```
 
-LAME must also be installed. This can be done on OSX via homebrew.
-
-```bash
-brew install lame
-```
-
 ### Deployment
 The project uses setup.py for installation and is deployed to
 [PyPI](https://pypi.org). The project can be built for installation with
 the following command:
 
 ```bash
 python setup.py clean --all; rm -r ./dist
```

### Comparing `streamp3-0.1.7/lame/hip.pyx` & `streamp3-0.1.8/lame/hip.pyx`

 * *Files identical despite different names*

### Comparing `streamp3-0.1.7/setup.py` & `streamp3-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 
 import setuptools
 from distutils.core import setup
 from distutils.extension import Extension
 
 setup(name='streamp3',
-      version='0.1.7',
+      version='0.1.8',
       description="streaming mp3 decoder",
       long_description=open('README.md', 'r').read(),
       long_description_content_type='text/markdown',
       url='https://github.com/pylon/streamp3/',
       author="Brent M. Spell",
       author_email='brent@pylon.com',
       packages=setuptools.find_packages(),
-      setup_requires=['Cython>=0.28.5'],
-      install_requires=['Cython>=0.28.5'],
+      setup_requires=['Cython==0.28.5'],
+      install_requires=['Cython==0.28.5'],
       ext_modules=[Extension('lame.hip',
                              ['lame/hip.pyx'],
                              libraries=['mp3lame'])],
       classifiers=("Programming Language :: Python :: 3",
                    "License :: OSI Approved :: Apache Software License",
                    "Operating System :: OS Independent"))
```

### Comparing `streamp3-0.1.7/streamp3/__init__.py` & `streamp3-0.1.8/streamp3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,16 @@
         channels = 1 if channel_code == 0b11 else 2
 
         self._bit_rate = bit_rate
         self._sample_rate = sample_rate
         self._num_channels = channels
 
         # calculate the size of the whole frame
-        output_size = 1152 if version == 1 else 576
-        frame_size = bit_rate // 8 * output_size // sample_rate
+        frame_size = 1152 if version == 1 else 576
+        frame_size = bit_rate // 8 * frame_size // sample_rate
         if is_padded:
             frame_size += 1
 
         # read the remainder of the frame
         while len(self._mp3_buffer) < frame_size:
             if not self._read_buffer():
                 return False
```

### Comparing `streamp3-0.1.7/streamp3.egg-info/PKG-INFO` & `streamp3-0.1.8/streamp3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamp3
-Version: 0.1.7
+Version: 0.1.8
 Summary: streaming mp3 decoder
 Home-page: https://github.com/pylon/streamp3/
 Author: Brent M. Spell
 Author-email: brent@pylon.com
 License: UNKNOWN
 Description: # streamp3
         
@@ -13,15 +13,29 @@
         ## Status
         [![PyPI](https://badge.fury.io/py/streamp3.svg)](https://badge.fury.io/py/streamp3)
         [![CircleCI](https://circleci.com/gh/pylon/streamp3.svg?style=shield)](https://circleci.com/gh/pylon/streamp3)
         [![Coveralls](https://coveralls.io/repos/github/pylon/streamp3/badge.svg?branch=master)](https://coveralls.io/github/pylon/streamp3?branch=master)
         
         ## Installation
         
-        ### Pip
+        First, make sure you have the LAME libraries and headers installed.
+        
+        #### macOS
+        
+        ```bash
+        brew install lame
+        ```
+        
+        #### Debian/Ubuntu
+        
+        ```bash
+        apt install libmp3lame-dev
+        ```
+        
+        ### Install with pip
         ```bash
         pip install streamp3
         ```
         
         ## Usage
         To begin decoding an MP3, construct an MP3Decoder, passing it in a binary
         stream or `bytes` object. You can then access the `bit_rate`, `sample_rate`,
@@ -68,20 +82,14 @@
         
         ```bash
         pyenv install 3.6.4
         pyenv virtualenv 3.6.4 streamp3
         pip install -r requirements.txt
         ```
         
-        LAME must also be installed. This can be done on OSX via homebrew.
-        
-        ```bash
-        brew install lame
-        ```
-        
         ### Deployment
         The project uses setup.py for installation and is deployed to
         [PyPI](https://pypi.org). The project can be built for installation with
         the following command:
         
         ```bash
         python setup.py clean --all; rm -r ./dist
```


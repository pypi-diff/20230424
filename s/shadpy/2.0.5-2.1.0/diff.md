# Comparing `tmp/shadpy-2.0.5.tar.gz` & `tmp/shadpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadpy-2.0.5.tar", last modified: Thu Nov 17 00:40:49 2022, max compression
+gzip compressed data, was "shadpy-2.1.0.tar", last modified: Mon Apr 24 12:25:24 2023, max compression
```

## Comparing `shadpy-2.0.5.tar` & `shadpy-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/
--rw-rw-rw-   0        0        0      975 2022-11-17 00:40:49.627417 shadpy-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-11-17 00:40:49.627417 shadpy-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1271 2022-11-17 00:40:23.000000 shadpy-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.614880 shadpy-2.0.5/shadpy/
--rw-rw-rw-   0        0        0      154 2022-11-17 00:38:01.000000 shadpy-2.0.5/shadpy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/shadpy/connections/
--rw-rw-rw-   0        0        0        4 2022-11-10 21:41:17.000000 shadpy-2.0.5/shadpy/connections/__init__.py
--rw-rw-rw-   0        0        0     6094 2022-11-17 00:38:41.000000 shadpy-2.0.5/shadpy/connections/requests.py
--rw-rw-rw-   0        0        0     1889 2022-11-17 00:38:23.000000 shadpy-2.0.5/shadpy/connections/websocket.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/shadpy/encryption/
--rw-rw-rw-   0        0        0      829 2022-11-16 19:20:03.000000 shadpy-2.0.5/shadpy/encryption/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/shadpy/exceptions/
--rw-rw-rw-   0        0        0      219 2022-11-13 20:20:19.000000 shadpy-2.0.5/shadpy/exceptions/__init__.py
--rw-rw-rw-   0        0        0    30666 2022-11-16 22:01:36.000000 shadpy-2.0.5/shadpy/shad.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/shadpy/tools/
--rw-rw-rw-   0        0        0     2307 2022-11-16 21:17:21.000000 shadpy-2.0.5/shadpy/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 00:40:49.627417 shadpy-2.0.5/shadpy.egg-info/
--rw-rw-rw-   0        0        0      975 2022-11-17 00:40:49.000000 shadpy-2.0.5/shadpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2022-11-17 00:40:49.000000 shadpy-2.0.5/shadpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 00:40:49.000000 shadpy-2.0.5/shadpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-11-17 00:40:49.000000 shadpy-2.0.5/shadpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-17 00:40:49.000000 shadpy-2.0.5/shadpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.371544 shadpy-2.1.0/
+-rw-rw-rw-   0        0        0     3350 2023-04-24 12:25:24.371544 shadpy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2206 2023-04-24 12:24:15.000000 shadpy-2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:25:24.371544 shadpy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1542 2023-04-24 12:25:07.000000 shadpy-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.230565 shadpy-2.1.0/shadpy/
+-rw-rw-rw-   0        0        0      240 2023-04-24 00:07:06.000000 shadpy-2.1.0/shadpy/__init__.py
+-rw-rw-rw-   0        0        0    29264 2023-04-24 00:05:02.000000 shadpy-2.1.0/shadpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.277427 shadpy-2.1.0/shadpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.309063 shadpy-2.1.0/shadpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 shadpy-2.1.0/shadpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25880 2023-04-24 12:22:04.000000 shadpy-2.1.0/shadpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 shadpy-2.1.0/shadpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.324683 shadpy-2.1.0/shadpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 shadpy-2.1.0/shadpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.340304 shadpy-2.1.0/shadpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.371544 shadpy-2.1.0/shadpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 shadpy-2.1.0/shadpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.261807 shadpy-2.1.0/shadpy.egg-info/
+-rw-rw-rw-   0        0        0     3350 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/top_level.txt
```

### Comparing `shadpy-2.0.5/setup.py` & `shadpy-2.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from setuptools import setup, find_packages
-
-
-requirements = ['wheel', 'pycryptodome', 'websockets', 'ujson', 'pybase64', 'urllib3']
-
-
-setup(
-    name = 'shadpy',
-    version = '2.0.5',
-    author='Shayan Heidari',
-    author_email = 'snipe4kill@yahoo.com',
-    description = 'This is an unofficial library and fastest library for deploying robots on shad accounts.',
-    keywords = ['shad', 'shadpy', 'shadio', 'chat', 'asyncio', 'bot', 'robot'],
-    long_description = 'Loading...',
-    python_requires="~=3.8",
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/snipe4kill/shad/',
-    packages = find_packages(),
-    install_requires = requirements,
-    classifiers=[
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: MIT License',
-        'Topic :: Internet',
-        'Topic :: Communications',
-        'Topic :: Communications :: Chat',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Software Development :: Libraries :: Application Frameworks'
-    ],
+from setuptools import setup, find_packages
+
+requirements = ['aiohttp', 'pycryptodome']
+
+with open("README.md", encoding="UTF-8") as f:
+    readme = f.read()
+
+setup(
+    name = 'shadpy',
+    version = '2.1.0',
+    author='Shayan Heidari',
+    author_email = 'contact@shayanheidari.info',
+    description = 'This is an unofficial library and fastest library for deploying robots on Shad accounts.',
+    keywords = ['shad', 'rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
+    long_description = readme,
+    python_requires="~=3.7",
+    long_description_content_type = 'text/markdown',
+    url = 'https://github.com/shayanheidari01/rubika',
+    packages = find_packages(),
+    install_requires = requirements,
+    extras_require={
+        'opencv-python': ['opencv-python']
+    },
+    classifiers=[
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
+        'Topic :: Internet',
+        'Topic :: Communications',
+        'Topic :: Communications :: Chat',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Software Development :: Libraries :: Application Frameworks'
+    ],
 )
```


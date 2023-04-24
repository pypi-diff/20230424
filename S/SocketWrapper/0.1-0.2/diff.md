# Comparing `tmp/SocketWrapper-0.1.tar.gz` & `tmp/SocketWrapper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocketWrapper-0.1.tar", last modified: Mon Apr 24 16:30:23 2023, max compression
+gzip compressed data, was "SocketWrapper-0.2.tar", last modified: Mon Apr 24 16:39:31 2023, max compression
```

## Comparing `SocketWrapper-0.1.tar` & `SocketWrapper-0.2.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:30:23.349576 SocketWrapper-0.1/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.1/LICENSE
--rw-r--r--   0 jarredtd   (501) staff       (20)      603 2023-04-24 16:30:23.349647 SocketWrapper-0.1/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 23:18:46.000000 SocketWrapper-0.1/README.md
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:30:23.348931 SocketWrapper-0.1/SocketWrapper/
--rw-r--r--   0 jarredtd   (501) staff       (20)      266 2023-04-24 16:18:36.000000 SocketWrapper-0.1/SocketWrapper/ClearScreen.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     1119 2023-04-20 22:40:05.000000 SocketWrapper-0.1/SocketWrapper/Client.py
--rw-r--r--   0 jarredtd   (501) staff       (20)      814 2023-04-20 23:18:46.000000 SocketWrapper-0.1/SocketWrapper/ClientInterface.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     1095 2023-04-20 22:42:09.000000 SocketWrapper-0.1/SocketWrapper/Server.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     1108 2023-04-21 03:01:17.000000 SocketWrapper-0.1/SocketWrapper/ServerInterface.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     2278 2023-04-20 23:18:46.000000 SocketWrapper-0.1/SocketWrapper/SocketInterface.py
--rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.1/SocketWrapper/__init__.py
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:30:23.349462 SocketWrapper-0.1/SocketWrapper.egg-info/
--rw-r--r--   0 jarredtd   (501) staff       (20)      603 2023-04-24 16:30:23.000000 SocketWrapper-0.1/SocketWrapper.egg-info/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)      386 2023-04-24 16:30:23.000000 SocketWrapper-0.1/SocketWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-24 16:30:23.000000 SocketWrapper-0.1/SocketWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-24 16:30:23.000000 SocketWrapper-0.1/SocketWrapper.egg-info/top_level.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-24 16:30:23.349953 SocketWrapper-0.1/setup.cfg
--rw-r--r--   0 jarredtd   (501) staff       (20)     1487 2023-04-24 16:30:16.000000 SocketWrapper-0.1/setup.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:39:31.251110 SocketWrapper-0.2/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.2/LICENSE
+-rw-r--r--   0 jarredtd   (501) staff       (20)      603 2023-04-24 16:39:31.251179 SocketWrapper-0.2/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 23:18:46.000000 SocketWrapper-0.2/README.md
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:39:31.250455 SocketWrapper-0.2/SocketWrapper/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1130 2023-04-24 16:38:21.000000 SocketWrapper-0.2/SocketWrapper/Client.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1106 2023-04-24 16:37:22.000000 SocketWrapper-0.2/SocketWrapper/Server.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.2/SocketWrapper/__init__.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-24 16:39:31.250965 SocketWrapper-0.2/SocketWrapper.egg-info/
+-rw-r--r--   0 jarredtd   (501) staff       (20)      603 2023-04-24 16:39:31.000000 SocketWrapper-0.2/SocketWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)      258 2023-04-24 16:39:31.000000 SocketWrapper-0.2/SocketWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-24 16:39:31.000000 SocketWrapper-0.2/SocketWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-24 16:39:31.000000 SocketWrapper-0.2/SocketWrapper.egg-info/top_level.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-24 16:39:31.251403 SocketWrapper-0.2/setup.cfg
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1487 2023-04-24 16:39:29.000000 SocketWrapper-0.2/setup.py
```

### Comparing `SocketWrapper-0.1/LICENSE` & `SocketWrapper-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.1/PKG-INFO` & `SocketWrapper-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.1
+Version: 0.2
 Summary: A wrapper for the socket class to abstract clients and servers
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.1.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SocketWrapper-0.1/SocketWrapper/Client.py` & `SocketWrapper-0.2/SocketWrapper/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Import the ClientInterface that the Client class is a child of
 '''
 
-from ClientInterface import ClientInterface
+from interfaces.ClientInterface import ClientInterface
 
 ##############################
 
 '''
 Client class, child of ClientInterface. Used as a container for the collection of the client information and automatically
 using that information.
 '''
```

### Comparing `SocketWrapper-0.1/SocketWrapper/Server.py` & `SocketWrapper-0.2/SocketWrapper/Server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Import Server interface that the Server class is a child of
 '''
 
-from ServerInterface import ServerInterface
+from interfaces.ServerInterface import ServerInterface
 
 ##############################
 '''
 Server class, child of Server interface. Used as a container for the collection of the server information and automatically
 using that information.
 '''
 class Server(ServerInterface):
```

### Comparing `SocketWrapper-0.1/SocketWrapper.egg-info/PKG-INFO` & `SocketWrapper-0.2/SocketWrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.1
+Version: 0.2
 Summary: A wrapper for the socket class to abstract clients and servers
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.1.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SocketWrapper-0.1/setup.py` & `SocketWrapper-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'SocketWrapper',         # How you named your package folder (MyLib)
   packages = ['SocketWrapper'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A wrapper for the socket class to abstract clients and servers',   # Give a short description about your library
   author = 'Jarred',                   # Type in your name
   author_email = 'jarredtdesrosiers@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/JarredTD/Socket_Wrapper',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.tar.gz',    # I explain this later on
   keywords = [],   # Keywords that define your package best
   install_requires=[],        # I get to this in a second,
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```


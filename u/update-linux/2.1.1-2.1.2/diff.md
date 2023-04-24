# Comparing `tmp/update-linux-2.1.1.tar.gz` & `tmp/update-linux-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-2.1.1.tar", last modified: Sat Apr 15 15:54:04 2023, max compression
+gzip compressed data, was "update-linux-2.1.2.tar", last modified: Mon Apr 24 14:10:06 2023, max compression
```

## Comparing `update-linux-2.1.1.tar` & `update-linux-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:54:04.053706 update-linux-2.1.1/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-15 15:54:04.053706 update-linux-2.1.1/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-15 15:54:03.000000 update-linux-2.1.1/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-15 15:54:04.053706 update-linux-2.1.1/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.1.1/setup_update_linux.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:54:04.052706 update-linux-2.1.1/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    18125 2023-04-15 15:53:46.000000 update-linux-2.1.1/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.1.1/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-15 15:54:04.052706 update-linux-2.1.1/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-15 15:54:03.000000 update-linux-2.1.1/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-15 15:54:04.000000 update-linux-2.1.1/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-15 15:54:03.000000 update-linux-2.1.1/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-15 15:54:03.000000 update-linux-2.1.1/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-15 15:54:03.000000 update-linux-2.1.1/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-15 15:54:03.000000 update-linux-2.1.1/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-24 14:10:06.844797 update-linux-2.1.2/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-24 14:10:06.000000 update-linux-2.1.2/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-24 14:10:06.844797 update-linux-2.1.2/setup.cfg
+-rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.1.2/setup_update_linux.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    18211 2023-04-24 14:09:38.000000 update-linux-2.1.2/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.1.2/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-2.1.1/PKG-INFO` & `update-linux-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.1.1
+Version: 2.1.2
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `update-linux-2.1.1/README.md` & `update-linux-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `update-linux-2.1.1/setup_update_linux.py` & `update-linux-2.1.2/setup_update_linux.py`

 * *Files identical despite different names*

### Comparing `update-linux-2.1.1/update_linux/__init__.py` & `update-linux-2.1.2/update_linux/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import datetime
 import subprocess
 import time
 import socket
 import platform
 import tempfile
 import json
-from config_path import ConfigPath
+from config_path import ConfigPath  # type: ignore
 
-VERSION = '2.1.1'
+VERSION = '2.1.2'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -344,17 +344,19 @@
         release = self.releaseInfo( host )
         self.info( host, 'Running on Fedora release %s' % (release,) )
 
     def releaseInfo( self, host ):
         cmd = ['cat', '/etc/system-release-cpe']
         rc, stdout = self.runAndLog( host, cmd, log=False )
         cpe_parts = stdout[0].strip().split( ':' )
-        if cpe_parts[3] != 'fedora':
-            self.error( host, 'Host is not running Fedora' )
-        return int( cpe_parts[4] )
+        if len(cpe_parts) >= 4 and cpe_parts[3] == 'fedora':
+            return int( cpe_parts[4] )
+
+        self.error( host, 'Host is not running Fedora - %r' % (cpe_parts,) )
+        return 0
 
     def installPackage( self, host, package ):
         rc = ssh_wait( host, wait=False, log_fn=None )
         if rc != 0:
             self.warn( host, 'Is not reachable' )
             return
 
@@ -422,15 +424,15 @@
 
             if stdout[0] == ('Connection to %s closed by remote host.\r\n' % (host,)):
                 # this is success
                 break
 
             self.error( host, 'reboot stdout: %r' % (stdout,) )
 
-            self.info( 'Retry reboot in 10s' )
+            self.info( host, 'Retry reboot in 10s' )
             time.sleep( 10 )
 
         # wait for system to go down
         time.sleep( 30 )
         # wait for it to come back up
         rc = ssh_wait( host, log_fn=None, wait_limit=wait_limit )
         if rc != 0:
@@ -490,17 +492,19 @@
         self.debug( 'runAndLog( %s )' % (' '.join( cmd ),) )
         stdout = []
         p = subprocess.Popen( cmd, stderr=subprocess.STDOUT, stdout=subprocess.PIPE )
         while True:
             line = p.stdout.readline()
             if line == b'':
                 break
+
             line = line.decode( 'utf-8' )
             if log:
                 print( self.ct( '<>proc %s<>: %s' % (host, line.rstrip()) ) )
+
             stdout.append( line )
 
         p.wait( 5 )
         self.debug( 'runAndLog rc=%d' % (p.returncode,) )
         return p.returncode, stdout
 
     def writeLines( self, filename, all_lines ):
```

### Comparing `update-linux-2.1.1/update_linux.egg-info/PKG-INFO` & `update-linux-2.1.2/update_linux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.1.1
+Version: 2.1.2
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
```


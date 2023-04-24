# Comparing `tmp/pyiosbackup-0.2.0.tar.gz` & `tmp/pyiosbackup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiosbackup-0.2.0.tar", last modified: Wed Dec  7 05:50:46 2022, max compression
+gzip compressed data, was "pyiosbackup-0.2.1.tar", last modified: Mon Apr 24 05:41:33 2023, max compression
```

## Comparing `pyiosbackup-0.2.0.tar` & `pyiosbackup-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 05:50:46.439736 pyiosbackup-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2022-12-07 05:50:46.439736 pyiosbackup-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 05:50:46.435736 pyiosbackup-0.2.0/pyiosbackup/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/keybag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 05:50:46.439736 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/manifest_db_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/mbdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/pyiosbackup/manifest_plist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 05:50:46.435736 pyiosbackup-0.2.0/pyiosbackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-07 05:50:46.000000 pyiosbackup-0.2.0/pyiosbackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 05:50:46.439736 pyiosbackup-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2022-12-07 05:50:38.000000 pyiosbackup-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/keybag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/manifest_db_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/mbdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_plist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/setup.py
```

### Comparing `pyiosbackup-0.2.0/LICENSE` & `pyiosbackup-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/PKG-INFO` & `pyiosbackup-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pyiosbackup
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python parser for iOS backups
 Home-page: https://github.com/matan1008/pyiosbackup
 Author: Matan Perelman
 Project-URL: pyiosbackup, https://github.com/matan1008/pyiosbackup
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyiosbackup-0.2.0/README.md` & `pyiosbackup-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/__main__.py` & `pyiosbackup-0.2.1/pyiosbackup/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,25 @@
     """ Decrypt all files in a backup."""
     backup = Backup.from_path(backup_path, password)
     backup.extract_all(target)
 
 
 @cli.command()
 @backup_path_argument
+@password_argument
+@target_option
+@verbosity
+def unback(backup_path, password, target):
+    """ Decrypt all files in a backup to a filesystem layout."""
+    backup = Backup.from_path(backup_path, password)
+    backup.unback(target)
+
+
+@cli.command()
+@backup_path_argument
 @password_option
 @verbosity
 def stats(backup_path, password):
     """ Show statistics about a backup."""
     backup = Backup.from_path(backup_path, password)
     pprint.pprint(backup.stats())
```

### Comparing `pyiosbackup-0.2.0/pyiosbackup/backup.py` & `pyiosbackup-0.2.1/pyiosbackup/backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pathlib import Path
 import logging
 import plistlib
 import shutil
+from pathlib import Path
 
 from packaging.version import Version
 
 from pyiosbackup.entry import Entry
+from pyiosbackup.exceptions import BackupPasswordIsRequired
 from pyiosbackup.keybag import Keybag
 from pyiosbackup.manifest_dbs.factory import from_path as manifest_db_from_path
 from pyiosbackup.manifest_dbs.manifest_db_interface import ManifestDb
 from pyiosbackup.manifest_plist import ManifestPlist
-from pyiosbackup.exceptions import BackupPasswordIsRequired
 
 INFO_PLIST_PATH = 'Info.plist'
 STATUS_PLIST_PATH = 'Status.plist'
 
 logger = logging.getLogger('pyiosbackup')
 logger.addHandler(logging.NullHandler())
 
@@ -53,15 +53,15 @@
 
         if not password and manifest.is_encrypted:
             logger.error('Password is required for encrypted backup')
             raise BackupPasswordIsRequired()
         if password and not manifest.is_encrypted:
             logger.warning('Password supplied for not encrypted backup')
 
-        keybag = Keybag.from_manifest(manifest, password)
+        keybag = Keybag.from_manifest(manifest, password) if manifest.is_encrypted else None
         manifest_db = manifest_db_from_path(backup_path, manifest, keybag)
         info = plistlib.loads((backup_path / INFO_PLIST_PATH).read_bytes())
         status = plistlib.loads((backup_path / STATUS_PLIST_PATH).read_bytes())
         return Backup(backup_path, manifest_db, manifest, status, info, keybag)
 
     @property
     def date(self):
@@ -94,14 +94,28 @@
     def itunes_version(self) -> str:
         return self._info['iTunes Version']
 
     @property
     def is_encrypted(self) -> bool:
         return self._manifest_plist.is_encrypted
 
+    def unback(self, path='.'):
+        """
+        Extract all decrypted files from a backup in a filesystem layout
+        :param path: Path to destination directory.
+        """
+        logger.info(f'Extracting backup to {path}')
+        dest_dir = Path(path)
+        dest_dir.mkdir(exist_ok=True, parents=True)
+        for file in self.iter_files():
+            dest_file = dest_dir / file.domain / file.relative_path
+            logger.debug(f'Extracting file {file.filename} to {dest_file}')
+            dest_file.parent.mkdir(exist_ok=True, parents=True)
+            dest_file.write_bytes(file.read_bytes())
+
     def extract_all(self, path='.'):
         """
         Extract all decrypted files from a backup.
         :param path: Path to destination directory.
         """
         logger.info(f'Extracting backup to {path}')
         dest_dir = Path(path)
```

### Comparing `pyiosbackup-0.2.0/pyiosbackup/entry.py` & `pyiosbackup-0.2.1/pyiosbackup/entry.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/keybag.py` & `pyiosbackup-0.2.1/pyiosbackup/keybag.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/factory.py` & `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/factory.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/manifest_db_interface.py` & `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/manifest_db_interface.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/mbdb.py` & `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/mbdb.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/manifest_dbs/sqlite3.py` & `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup/manifest_plist.py` & `pyiosbackup-0.2.1/pyiosbackup/manifest_plist.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/pyiosbackup.egg-info/PKG-INFO` & `pyiosbackup-0.2.1/pyiosbackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pyiosbackup
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python parser for iOS backups
 Home-page: https://github.com/matan1008/pyiosbackup
 Author: Matan Perelman
 Project-URL: pyiosbackup, https://github.com/matan1008/pyiosbackup
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyiosbackup-0.2.0/pyiosbackup.egg-info/SOURCES.txt` & `pyiosbackup-0.2.1/pyiosbackup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.0/setup.py` & `pyiosbackup-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 BASE_DIR = Path(__file__).parent.resolve(strict=True)
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 PACKAGE_NAME = 'pyiosbackup'
 PACKAGES = [p for p in find_packages() if not p.startswith('tests')]
 
 
 def parse_requirements():
     reqs = []
     with open(BASE_DIR / 'requirements.txt', 'r') as fd:
@@ -34,15 +34,14 @@
         install_requires=parse_requirements(),
         entry_points={
             'console_scripts': [
                 'pyiosbackup=pyiosbackup.__main__:main',
             ],
         },
         classifiers=[
-            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
         ],
         url='https://github.com/matan1008/pyiosbackup',
```


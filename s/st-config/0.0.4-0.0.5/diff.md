# Comparing `tmp/st_config-0.0.4.tar.gz` & `tmp/st_config-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st_config-0.0.4.tar", last modified: Wed Apr 12 09:17:08 2023, max compression
+gzip compressed data, was "dist/st_config-0.0.5.tar", last modified: Mon Apr 24 11:23:46 2023, max compression
```

## Comparing `st_config-0.0.4.tar` & `st_config-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/
--rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-12 09:17:08.000000 st_config-0.0.4/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.4/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/sconf/
--rw-r--r--   0 nezah      (501) staff       (20)     1430 2023-04-12 09:17:08.000000 st_config-0.0.4/sconf/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       71 2023-04-12 09:17:08.000000 st_config-0.0.4/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-12 09:17:08.000000 st_config-0.0.4/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-12 09:17:08.000000 st_config-0.0.4/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:23:46.000000 st_config-0.0.5/
+-rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-24 11:23:46.000000 st_config-0.0.5/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.5/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:23:46.000000 st_config-0.0.5/sconf/
+-rw-r--r--   0 nezah      (501) staff       (20)     1570 2023-04-24 11:23:26.000000 st_config-0.0.5/sconf/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:23:46.000000 st_config-0.0.5/st_config.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-24 11:23:45.000000 st_config-0.0.5/st_config.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 11:23:45.000000 st_config-0.0.5/st_config.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 11:23:45.000000 st_config-0.0.5/st_config.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 11:23:45.000000 st_config-0.0.5/st_config.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       71 2023-04-12 09:17:08.000000 st_config-0.0.5/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-24 11:23:45.000000 st_config-0.0.5/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 11:23:46.000000 st_config-0.0.5/setup.cfg
```

### Comparing `st_config-0.0.4/LICENSE` & `st_config-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st_config-0.0.4/sconf/__init__.py` & `st_config-0.0.5/sconf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,19 @@
         return cls._instance
 
     def __init__(self, filename="config.json"):
         cls = type(self)
         if not hasattr(cls, "_init"):
             env_path = os.getenv("SCONF_PATH")
             if env_path is not None:
+                logger.info(f"USE Config in {env_path}/{filename}")
                 config_file = f"{env_path}/{filename}"
             else:
                 context_root = os.path.dirname(os.path.abspath(sys.modules['__main__'].__file__))
+                logger.info(f"USE Config in {context_root}/{filename}")
                 config_file = f"{context_root}/{filename}"
 
             with open(config_file, encoding="UTF-8") as json_file:
                 self.json_data = json.load(json_file)
                 logger.info(f"Loading config.json for [{self.json_data.get('ENV')}] from {config_file}")
             cls._init = True
```

### Comparing `st_config-0.0.4/setup.py` & `st_config-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_config",
-    version="0.0.4",
+    version="0.0.5",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="Singleton config for python",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/singleton-config",
     packages=setuptools.find_packages(),
```


# Comparing `tmp/layerd-2022.8.11.9.23.tar.gz` & `tmp/layerd-2023.4.24.12.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerd-2022.8.11.9.23.tar", last modified: Thu Aug 11 13:23:54 2022, max compression
+gzip compressed data, was "layerd-2023.4.24.12.34.tar", last modified: Mon Apr 24 16:34:49 2023, max compression
```

## Comparing `layerd-2022.8.11.9.23.tar` & `layerd-2023.4.24.12.34.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2022-08-11 13:23:54.100817 layerd-2022.8.11.9.23/
--rw-r--r--   0 ronnath    (501) staff       (20)     1070 2022-06-21 18:42:26.000000 layerd-2022.8.11.9.23/LICENSE
--rw-r--r--   0 ronnath    (501) staff       (20)     2427 2022-08-11 13:23:54.100433 layerd-2022.8.11.9.23/PKG-INFO
--rw-r--r--   0 ronnath    (501) staff       (20)     1416 2022-08-10 20:30:56.000000 layerd-2022.8.11.9.23/README.md
-drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2022-08-11 13:23:54.096482 layerd-2022.8.11.9.23/layerd/
--rw-r--r--   0 ronnath    (501) staff       (20)       84 2022-08-11 11:23:14.000000 layerd-2022.8.11.9.23/layerd/__init__.py
--rw-r--r--   0 ronnath    (501) staff       (20)     2447 2022-07-11 13:36:12.000000 layerd-2022.8.11.9.23/layerd/__main__.py
--rw-r--r--   0 ronnath    (501) staff       (20)      537 2022-07-09 08:49:50.000000 layerd-2022.8.11.9.23/layerd/package.py
--rw-r--r--   0 ronnath    (501) staff       (20)      988 2022-07-09 08:49:45.000000 layerd-2022.8.11.9.23/layerd/utils.py
-drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2022-08-11 13:23:54.099845 layerd-2022.8.11.9.23/layerd.egg-info/
--rw-r--r--   0 ronnath    (501) staff       (20)     2427 2022-08-11 13:23:53.000000 layerd-2022.8.11.9.23/layerd.egg-info/PKG-INFO
--rw-r--r--   0 ronnath    (501) staff       (20)      295 2022-08-11 13:23:54.000000 layerd-2022.8.11.9.23/layerd.egg-info/SOURCES.txt
--rw-r--r--   0 ronnath    (501) staff       (20)        1 2022-08-11 13:23:53.000000 layerd-2022.8.11.9.23/layerd.egg-info/dependency_links.txt
--rw-r--r--   0 ronnath    (501) staff       (20)       47 2022-08-11 13:23:53.000000 layerd-2022.8.11.9.23/layerd.egg-info/entry_points.txt
--rw-r--r--   0 ronnath    (501) staff       (20)       15 2022-08-11 13:23:53.000000 layerd-2022.8.11.9.23/layerd.egg-info/requires.txt
--rw-r--r--   0 ronnath    (501) staff       (20)        7 2022-08-11 13:23:53.000000 layerd-2022.8.11.9.23/layerd.egg-info/top_level.txt
--rw-r--r--   0 ronnath    (501) staff       (20)       55 2022-07-01 13:20:20.000000 layerd-2022.8.11.9.23/pyproject.toml
--rw-r--r--   0 ronnath    (501) staff       (20)       38 2022-08-11 13:23:54.101004 layerd-2022.8.11.9.23/setup.cfg
--rw-r--r--   0 ronnath    (501) staff       (20)     1969 2022-08-10 20:33:38.000000 layerd-2022.8.11.9.23/setup.py
+drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2023-04-24 16:34:49.783335 layerd-2023.4.24.12.34/
+-rw-r--r--   0 ronnath    (501) staff       (20)     1070 2022-06-21 18:42:26.000000 layerd-2023.4.24.12.34/LICENSE
+-rw-r--r--   0 ronnath    (501) staff       (20)       51 2022-08-11 15:03:23.000000 layerd-2023.4.24.12.34/MANIFEST.in
+-rw-r--r--   0 ronnath    (501) staff       (20)     3951 2023-04-24 16:34:49.782881 layerd-2023.4.24.12.34/PKG-INFO
+-rw-r--r--   0 ronnath    (501) staff       (20)     2939 2023-04-24 16:23:43.000000 layerd-2023.4.24.12.34/README.md
+drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2023-04-24 16:34:49.778526 layerd-2023.4.24.12.34/layerd/
+-rw-r--r--   0 ronnath    (501) staff       (20)       87 2023-04-24 16:25:02.000000 layerd-2023.4.24.12.34/layerd/__init__.py
+-rw-r--r--   0 ronnath    (501) staff       (20)     2453 2023-04-24 16:28:20.000000 layerd-2023.4.24.12.34/layerd/__main__.py
+-rw-r--r--   0 ronnath    (501) staff       (20)      875 2023-04-24 16:32:42.000000 layerd-2023.4.24.12.34/layerd/package.py
+-rw-r--r--   0 ronnath    (501) staff       (20)      988 2022-07-09 08:49:45.000000 layerd-2023.4.24.12.34/layerd/utils.py
+drwxr-xr-x   0 ronnath    (501) staff       (20)        0 2023-04-24 16:34:49.782178 layerd-2023.4.24.12.34/layerd.egg-info/
+-rw-r--r--   0 ronnath    (501) staff       (20)     3951 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/PKG-INFO
+-rw-r--r--   0 ronnath    (501) staff       (20)      307 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/SOURCES.txt
+-rw-r--r--   0 ronnath    (501) staff       (20)        1 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/dependency_links.txt
+-rw-r--r--   0 ronnath    (501) staff       (20)       52 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/entry_points.txt
+-rw-r--r--   0 ronnath    (501) staff       (20)       22 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/requires.txt
+-rw-r--r--   0 ronnath    (501) staff       (20)        7 2023-04-24 16:34:49.000000 layerd-2023.4.24.12.34/layerd.egg-info/top_level.txt
+-rw-r--r--   0 ronnath    (501) staff       (20)       94 2022-08-11 15:04:17.000000 layerd-2023.4.24.12.34/pyproject.toml
+-rw-r--r--   0 ronnath    (501) staff       (20)       38 2023-04-24 16:34:49.783495 layerd-2023.4.24.12.34/setup.cfg
+-rw-r--r--   0 ronnath    (501) staff       (20)     1958 2023-04-24 16:24:42.000000 layerd-2023.4.24.12.34/setup.py
```

### Comparing `layerd-2022.8.11.9.23/LICENSE` & `layerd-2023.4.24.12.34/LICENSE`

 * *Files identical despite different names*

### Comparing `layerd-2022.8.11.9.23/layerd/__main__.py` & `layerd-2023.4.24.12.34/layerd/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,41 +16,40 @@
 from layerd.utils import (
     _flag_add_region,
     _flag_parent_dir,
     _progress_bar,
     _stdout_del_last_row,
 )
 
+
 def parse_cli_args() -> str:
     """
     @returns ARN: str.
     """
     args = [*sys.argv]
     args.pop(0)
     if (not args) or ('help' in args[0].lower()):
-        print(__usage__)
-        exit(1)
+        return
     arn = args[0]
 
     # don't be tempted to return early. leave room for expansion.
     #   - Confucius [Date Unknown]
 
     return arn
 
 
-
-def mount(arn: str = None) -> None:
+def download(arn: str = None) -> None:
     """
     @arg arn: str. ARN of Public (Authorized) Lambda Layer.
     """
-    arn = arn or parse_cli_args()
+    arn = arn or parse_cli_args() or ''
     names = arn.split(':')
     if not (6 <= len(names) <= 8):
         print(__usage__)
-        print('Error: <ARN> not valid. Recieved ' + arn)
+        print('Error: <ARN> not valid. Recieved: ' + (arn or '<NoneType>'))
         exit(1)
     region: str = names[3]
     layer_q: str = names[5]
     layer_name: str = names[6]
     version: int = int(names[-1])
 
     # boto3's LambdaClient.get_layer_version() accepts the arn
@@ -87,9 +86,10 @@
         layer_dir += f'-{region}'
     _progress_bar(8.8, 10, message='Extracting')
     zip.extractall(layer_dir)
     _progress_bar(10, 10, message='Done')
     print()
     print(f'Created: {layer_dir}/')
 
+
 if __name__ == '__main__':
-    mount()
+    download()
```

### Comparing `layerd-2022.8.11.9.23/layerd/utils.py` & `layerd-2023.4.24.12.34/layerd/utils.py`

 * *Files identical despite different names*

### Comparing `layerd-2022.8.11.9.23/setup.py` & `layerd-2023.4.24.12.34/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,29 +18,28 @@
     try_reqs('requirements.txt')
     or
     try_reqs('layerd.egg-info/requires.txt')
     or
     []
 )
 
-print(required)
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="ronnathaniel",
     author_email="rnathaniel7@gmail.com",
     description="Download AWS Lambda Layers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['layerd'],
     package_data={'layerd': ['*.pem']},
     python_requires=">=3.6",
     entry_points={
-        'console_scripts': ['layerd = layerd.__main__:run']
+        'console_scripts': ['layerd = layerd.__main__:download']
     },
     install_requires=required,
     include_package_data=True,
     use_calver='%Y.%m.%d.%H.%M',
     setup_requires=['calver'],
     url="https://github.com/ronnathaniel/layerd",
     project_urls={
```


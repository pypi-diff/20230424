# Comparing `tmp/shortipy-1.3.1.tar.gz` & `tmp/shortipy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortipy-1.3.1.tar", max compression
+gzip compressed data, was "shortipy-1.3.2.tar", max compression
```

## Comparing `shortipy-1.3.1.tar` & `shortipy-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35802 2022-10-12 17:14:51.198988 shortipy-1.3.1/LICENSE
--rw-r--r--   0        0        0     1090 2023-04-19 18:34:24.653773 shortipy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1080 2022-10-17 18:10:54.100415 shortipy-1.3.1/README.md
--rw-r--r--   0        0        0     2277 2023-04-19 18:34:24.682034 shortipy-1.3.1/shortipy/__init__.py
--rw-r--r--   0        0        0       54 2022-10-17 18:41:43.407781 shortipy-1.3.1/shortipy/controllers/__init__.py
--rw-r--r--   0        0        0      566 2022-11-07 19:55:26.410806 shortipy-1.3.1/shortipy/controllers/api/__init__.py
--rw-r--r--   0        0        0     1937 2022-11-07 19:55:26.418842 shortipy-1.3.1/shortipy/controllers/api/auth.py
--rw-r--r--   0        0        0     4286 2022-11-07 19:55:26.426821 shortipy-1.3.1/shortipy/controllers/api/url.py
--rw-r--r--   0        0        0      645 2023-04-14 07:27:31.098766 shortipy-1.3.1/shortipy/controllers/resolution.py
--rw-r--r--   0        0        0       51 2022-10-12 18:35:32.461550 shortipy-1.3.1/shortipy/services/__init__.py
--rw-r--r--   0        0        0     3270 2022-11-07 19:55:26.426821 shortipy-1.3.1/shortipy/services/auth.py
--rw-r--r--   0        0        0      931 2022-11-07 19:55:26.434822 shortipy-1.3.1/shortipy/services/config.py
--rw-r--r--   0        0        0      562 2022-10-30 13:41:28.836036 shortipy-1.3.1/shortipy/services/exceptions.py
--rw-r--r--   0        0        0      812 2022-11-07 19:55:26.442871 shortipy-1.3.1/shortipy/services/hash.py
--rw-r--r--   0        0        0      457 2022-10-13 18:25:48.640051 shortipy-1.3.1/shortipy/services/redis.py
--rw-r--r--   0        0        0      449 2022-10-30 13:41:28.844112 shortipy-1.3.1/shortipy/services/serialization.py
--rw-r--r--   0        0        0     3457 2022-11-07 19:55:26.442871 shortipy-1.3.1/shortipy/services/url.py
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 shortipy-1.3.1/setup.py
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 shortipy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-10-12 17:14:51.198988 shortipy-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1090 2023-04-24 19:02:51.420472 shortipy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1080 2022-10-17 18:10:54.100415 shortipy-1.3.2/README.md
+-rw-r--r--   0        0        0     2271 2023-04-24 19:02:51.394578 shortipy-1.3.2/shortipy/__init__.py
+-rw-r--r--   0        0        0       54 2022-10-17 18:41:43.407781 shortipy-1.3.2/shortipy/controllers/__init__.py
+-rw-r--r--   0        0        0      566 2022-11-07 19:55:26.410806 shortipy-1.3.2/shortipy/controllers/api/__init__.py
+-rw-r--r--   0        0        0     1937 2022-11-07 19:55:26.418842 shortipy-1.3.2/shortipy/controllers/api/auth.py
+-rw-r--r--   0        0        0     4286 2022-11-07 19:55:26.426821 shortipy-1.3.2/shortipy/controllers/api/url.py
+-rw-r--r--   0        0        0      645 2023-04-14 07:27:31.098766 shortipy-1.3.2/shortipy/controllers/resolution.py
+-rw-r--r--   0        0        0       51 2022-10-12 18:35:32.461550 shortipy-1.3.2/shortipy/services/__init__.py
+-rw-r--r--   0        0        0     3270 2022-11-07 19:55:26.426821 shortipy-1.3.2/shortipy/services/auth.py
+-rw-r--r--   0        0        0      931 2022-11-07 19:55:26.434822 shortipy-1.3.2/shortipy/services/config.py
+-rw-r--r--   0        0        0      562 2022-10-30 13:41:28.836036 shortipy-1.3.2/shortipy/services/exceptions.py
+-rw-r--r--   0        0        0      812 2022-11-07 19:55:26.442871 shortipy-1.3.2/shortipy/services/hash.py
+-rw-r--r--   0        0        0      457 2022-10-13 18:25:48.640051 shortipy-1.3.2/shortipy/services/redis.py
+-rw-r--r--   0        0        0      449 2022-10-30 13:41:28.844112 shortipy-1.3.2/shortipy/services/serialization.py
+-rw-r--r--   0        0        0     3457 2022-11-07 19:55:26.442871 shortipy-1.3.2/shortipy/services/url.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 shortipy-1.3.2/setup.py
+-rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 shortipy-1.3.2/PKG-INFO
```

### Comparing `shortipy-1.3.1/LICENSE` & `shortipy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/pyproject.toml` & `shortipy-1.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shortipy"
-version = "1.3.1"
+version = "1.3.2"
 description = "Shortipy is a RESTful Web API, written in Python language and based on the Flask micro-framework, designed to manage shortened links."
 authors = ["Simone Perini <perinisimone98@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 repository = "https://github.com/CoffeePerry/shortipy"
 keywords = ["shortipy", "url", "shortener"]
 classifiers = [
```

### Comparing `shortipy-1.3.1/README.md` & `shortipy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/__init__.py` & `shortipy-1.3.2/shortipy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from shortipy.services.hash import init_app as init_hash
 from shortipy.services.auth import init_app as init_auth
 from shortipy.services.serialization import init_app as init_serialization
 from shortipy.services.url import init_app as init_url
 from shortipy.controllers.resolution import resolution_blueprint
 from shortipy.controllers.api import init_app as init_api
 
-VERSION: Final = '1.3.1'
+VERSION: Final = '1.3.2'
 CONFIG_FILENAME: Final = 'config.py'
 
 
 def create_app(options: dict | None = None) -> Flask | None:
     """Application factory.
 
     :param options: Optional application options (default: None).
@@ -46,15 +46,15 @@
             raise Exception(f'Configuration file not found: {config_file}')
         app.config.from_pyfile(config_file)
 
     if options is not None:
         app.config.from_mapping(options)
 
     if app.config.get('SECRET_KEY') is None:
-        raise Exception(f'Set variable SECRET_KEY with random string in file: {config_file}')
+        raise Exception('Set variable SECRET_KEY with cryptographically strong random')
 
     init_url(init_serialization(init_auth(init_hash(init_redis(app)))))
 
     app.register_blueprint(resolution_blueprint)
     app.register_blueprint(init_api())
 
     @app.cli.command('version', help='Display version.')
```

### Comparing `shortipy-1.3.1/shortipy/controllers/api/__init__.py` & `shortipy-1.3.2/shortipy/controllers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/controllers/api/auth.py` & `shortipy-1.3.2/shortipy/controllers/api/auth.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/controllers/api/url.py` & `shortipy-1.3.2/shortipy/controllers/api/url.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/controllers/resolution.py` & `shortipy-1.3.2/shortipy/controllers/resolution.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/services/auth.py` & `shortipy-1.3.2/shortipy/services/auth.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/services/config.py` & `shortipy-1.3.2/shortipy/services/config.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/services/exceptions.py` & `shortipy-1.3.2/shortipy/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/services/hash.py` & `shortipy-1.3.2/shortipy/services/hash.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/shortipy/services/url.py` & `shortipy-1.3.2/shortipy/services/url.py`

 * *Files identical despite different names*

### Comparing `shortipy-1.3.1/setup.py` & `shortipy-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'flask-marshmallow>=0.14.0,<0.15.0',
  'flask-redis>=0.4.0,<0.5.0',
  'flask>=2.2.2,<3.0.0',
  'webargs>=8.2.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'shortipy',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'Shortipy is a RESTful Web API, written in Python language and based on the Flask micro-framework, designed to manage shortened links.',
     'long_description': '![shortipy logo](https://github.com/CoffeePerry/shortipy/blob/main/art/shortipy.png?raw=true)\n\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/CoffeePerry/shortipy)\n![PyPI](https://img.shields.io/pypi/v/shortipy?logo=PyPI&logoColor=white)\n![PyPI - Status](https://img.shields.io/pypi/status/shortipy)\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/shortipy?logo=Python&logoColor=white)\n![PyPI - Implementation](https://img.shields.io/pypi/implementation/shortipy)\n\n[![Flask](https://img.shields.io/badge/framework-Flask-black?logo=Flask&logoColor=white)](https://github.com/pallets/flask/)\n\n[![GitHub license](https://img.shields.io/github/license/CoffeePerry/shortipy)](https://github.com/CoffeePerry/shortipy/blob/master/LICENSE)\n\n[![GitHub issues](https://img.shields.io/github/issues/CoffeePerry/shortipy)](https://github.com/CoffeePerry/shortipy/issues)\n\n# shortipy\n\n**Shortipy** is a *RESTful Web API*, written in *Python* language and based on the *Flask* micro-framework, designed to manage shortened links. \n',
     'author': 'Simone Perini',
     'author_email': 'perinisimone98@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CoffeePerry/shortipy',
```

### Comparing `shortipy-1.3.1/PKG-INFO` & `shortipy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortipy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Shortipy is a RESTful Web API, written in Python language and based on the Flask micro-framework, designed to manage shortened links.
 Home-page: https://github.com/CoffeePerry/shortipy
 License: GPL-3.0
 Keywords: shortipy,url,shortener
 Author: Simone Perini
 Author-email: perinisimone98@gmail.com
 Requires-Python: >=3.10,<4.0
```


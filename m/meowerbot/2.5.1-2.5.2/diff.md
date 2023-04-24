# Comparing `tmp/meowerbot-2.5.1.tar.gz` & `tmp/meowerbot-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.1.tar", max compression
+gzip compressed data, was "meowerbot-2.5.2.tar", max compression
```

## Comparing `meowerbot-2.5.1.tar` & `meowerbot-2.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.1/LICENSE
--rw-r--r--   0        0        0      154 2023-04-18 21:53:53.656983 meowerbot-2.5.1/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.1/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1384 2023-04-15 02:05:09.867583 meowerbot-2.5.1/MeowerBot/API.py
--rw-r--r--   0        0        0    13593 2023-04-18 21:45:43.038089 meowerbot-2.5.1/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.1/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.1/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.1/MeowerBot/cog.py
--rw-r--r--   0        0        0     2084 2023-04-15 02:19:55.402707 meowerbot-2.5.1/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.1/MeowerBot/context.py
--rw-r--r--   0        0        0      566 2023-04-18 21:53:43.212775 meowerbot-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.1/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.1/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.2/LICENSE
+-rw-r--r--   0        0        0      154 2023-04-24 21:38:04.560934 meowerbot-2.5.2/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.2/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-04-24 21:38:04.548919 meowerbot-2.5.2/MeowerBot/API.py
+-rw-r--r--   0        0        0    13593 2023-04-18 21:45:43.038089 meowerbot-2.5.2/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.2/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.2/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.2/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2084 2023-04-15 02:19:55.402707 meowerbot-2.5.2/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.2/MeowerBot/context.py
+-rw-r--r--   0        0        0      566 2023-04-24 21:38:04.561918 meowerbot-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.2/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.2/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.2/PKG-INFO
```

### Comparing `meowerbot-2.5.1/LICENSE` & `meowerbot-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/MeowerBot/API.py` & `meowerbot-2.5.2/MeowerBot/API.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             urljoin(self.base_uri, "/users/{0}".format(username))
         ).json()
 
     def get_user_posts(self, username, page=1):
         return self.session.get(
             urljoin(
                 self.base_uri,
-                "/users/{0}/posts?autoget&page={page}".format(username, page),
+                "/users/{0}/posts?autoget&page={1}".format(username, page),
             )
         ).json()
 
     def statistics(self):
         return self.session.get(urljoin(self.base_uri, "statistics")).json()
 
     def status(self):
```

### Comparing `meowerbot-2.5.1/MeowerBot/Bot.py` & `meowerbot-2.5.2/MeowerBot/Bot.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.2/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/MeowerBot/cog.py` & `meowerbot-2.5.2/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/MeowerBot/command.py` & `meowerbot-2.5.2/MeowerBot/command.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/MeowerBot/context.py` & `meowerbot-2.5.2/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.1/pyproject.toml` & `meowerbot-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.1"
+version = "2.5.2"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
```

### Comparing `meowerbot-2.5.1/setup.py` & `meowerbot-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.1',
+    'version': '2.5.2',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.5.1/PKG-INFO` & `meowerbot-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.1
+Version: 2.5.2
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


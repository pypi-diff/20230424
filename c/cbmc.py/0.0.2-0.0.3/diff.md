# Comparing `tmp/cbmc.py-0.0.2.tar.gz` & `tmp/cbmc.py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmc.py-0.0.2.tar", last modified: Fri Apr 14 01:13:09 2023, max compression
+gzip compressed data, was "cbmc.py-0.0.3.tar", last modified: Mon Apr 24 20:33:02 2023, max compression
```

## Comparing `cbmc.py-0.0.2.tar` & `cbmc.py-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/cbmc/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/cbmc/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/cbmc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 01:13:09.000000 cbmc.py-0.0.2/cbmc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:13:09.567752 cbmc.py-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 01:12:56.000000 cbmc.py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/cbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/cbmc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/test_post.py
```

### Comparing `cbmc.py-0.0.2/LICENSE` & `cbmc.py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.2/cbmc/api.py` & `cbmc.py-0.0.3/cbmc/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
         :raise TypeError: The post ID is not an integer.
         :raise NotFound: The post was not found.
         :raise HTTPException: The HTTP request failed.
 
         :return: The post object.
         :rtype: Post
         """
+        if not isinstance(post_id, int):
+            raise TypeError("The post ID must be an integer.")
         url = f"{cls.base_url}/post/{post_id}"
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
                 if resp.status == 200:
                     data = await resp.json()
                     if data["status"] == "failed":
                         raise NotFound(data.get("message", "Post not found."))
```

### Comparing `cbmc.py-0.0.2/cbmc/exception.py` & `cbmc.py-0.0.3/cbmc/exception.py`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.2/cbmc/post.py` & `cbmc.py-0.0.3/cbmc/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,114 +44,119 @@
         :type data: dict
         """
         self._post_id = data.get("id", {}).get("post")
         self._platform_id = data.get("id", {}).get("platform")
         self._type = data.get("type")
         self._content = data.get("content")
         self._photo = data.get("photo")
-        self._admin_post = data.get("adminPost", False)
-        self._approve_timestamp = data.get("approve", {}).get("timestamp", 0)
-        self._approve_time = datetime.datetime.utcfromtimestamp(self._approve_timestamp)
+        self._admin_post = data.get("adminPost")
+        self._approve_timestamp = data.get("approve", {}).get("timestamp")
         self._approve_user = data.get("approve", {}).get("user")
         self._fbid = data.get("fbid")
 
+        if self._approve_timestamp is not None:
+            approve_time = datetime.datetime.utcfromtimestamp(self._approve_timestamp)
+            self._approve_time = approve_time.replace(tzinfo=datetime.timezone.utc)
+        else:
+            self._approve_time = None
+
     @property
     def post_id(self) -> int:
         """
-        Get the post ID.
+        The post ID of the post.
 
-        :return: The post ID.
+        :return: The value of the post ID.
         :rtype: int
         """
         return self._post_id
 
     @property
     def platform_id(self) -> int:
         """
-        Get the platform ID.
+        The platform ID of the post.
 
-        :return: The platform ID.
+        :return: The value of the platform ID.
         :rtype: int
         """
         return self._platform_id
 
     @property
     def type(self) -> str:
         """
-        Get the post type.
+        The post type of the post.
 
-        :return: The post type.
+        :return: The value of the post type.
         :rtype: str
         """
         return self._type
 
     @property
     def content(self) -> str:
         """
-        Get the post content.
+        The content of the post.
 
-        :return: The post content.
+        :return: The value of the content.
         :rtype: str
         """
         return self._content
 
     @property
     def photo(self) -> str | None:
         """
-        Get the post photo.
+        The photo url of the post.
 
         :return: The post photo url or None if there is no photo.
         :rtype: str | None
         """
         return self._photo
 
     @property
     def admin_post(self) -> bool:
         """
-        Get whether the post is an admin post.
+        Whether the post is an admin post.
 
         :return: Whether the post is an admin post.
         :rtype: bool
         """
         return self._admin_post
 
     @property
     def approve_time(self) -> datetime.datetime:
         """
-        Get the time the post was approved. (UTC)
+        The time the post was approved in UTC.
 
         :return: The time the post was approved.
         :rtype: datetime.datetime
         """
         return self._approve_time
 
     @property
     def approve_timestamp(self) -> int:
         """
-        Get the timestamp the post was approved. (Unix timestamp UTC)
+        The Unix timestamp the post was approved in UTC.
 
         :return: The timestamp the post was approved.
         :rtype: int
         """
         return self._approve_timestamp
 
     @property
     def approve_user(self) -> str:
         """
-        Get the user who approved the post.
+        The user who approved the post.
 
         :return: The user who approved the post.
         :rtype: str
         """
         return self._approve_user
 
     @property
     def fbid(self) -> str:
         """
-        Get the post fbid.
+        The fbid of the post.
 
         :return: The post fbid.
         :rtype: str
         """
         return self._fbid
 
     def to_dict(self) -> dict:
```

### Comparing `cbmc.py-0.0.2/setup.py` & `cbmc.py-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 setup(
     name="cbmc.py",
     version=VERSION,
     author="ItsRqtl",
     author_email="itsrql@gmail.com",
     description="An unofficial 麥塊匿名發文平台 API wrapper.",
```


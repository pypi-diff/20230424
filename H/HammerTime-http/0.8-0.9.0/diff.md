# Comparing `tmp/HammerTime-http-0.8.tar.gz` & `tmp/HammerTime-http-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HammerTime-http-0.8.tar", last modified: Wed Mar 17 19:22:00 2021, max compression
+gzip compressed data, was "HammerTime-http-0.9.0.tar", last modified: Mon Apr 24 17:16:35 2023, max compression
```

## Comparing `HammerTime-http-0.8.tar` & `HammerTime-http-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      925 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-03-17 19:22:00.000000 HammerTime-http-0.8/HammerTime_http.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2021-03-17 19:22:00.000000 HammerTime-http-0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1753 2021-03-17 19:21:27.000000 HammerTime-http-0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/hammertime/
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2021-03-17 19:21:44.000000 HammerTime-http-0.8/hammertime/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1308 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6054 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/hammertime/engine/
--rw-rw-r--   0 travis    (2000) travis    (2000)      916 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/engine/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7198 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/engine/aiohttp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      897 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/engine/interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2980 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/engine/retry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7051 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/engine/scaling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3201 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/kb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2935 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/requestscheduler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/hammertime/rules/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1630 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3332 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/behavior.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/body.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2191 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/deadhostdetection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3560 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/filterrequestfromurl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6765 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/redirects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4642 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/sampling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2399 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/simhash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13063 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3656 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/timeout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1464 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/rules/waf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2796 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/ruleset.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 19:22:00.000000 HammerTime-http-0.8/hammertime/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2647 2021-03-17 19:21:27.000000 HammerTime-http-0.8/hammertime/utils/har.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2021-03-17 19:22:00.000000 HammerTime-http-0.8/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1142 2021-03-17 19:21:27.000000 HammerTime-http-0.8/setup.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/HammerTime_http.egg-info/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)      936 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/SOURCES.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        1 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/dependency_links.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)      140 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/requires.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       11 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/top_level.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/LICENSE.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1753 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/README.md
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      929 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      778 2023-04-24 17:15:45.000000 HammerTime-http-0.9.0/hammertime/__version__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1308 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/config.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5947 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/core.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/engine/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      916 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     7190 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/engine/aiohttp.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      897 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/interface.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2963 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/engine/retry.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     7051 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/scaling.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3201 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/http.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1214 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/kb.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2935 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/requestscheduler.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/rules/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1630 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3332 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/behavior.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2992 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/body.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2191 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/deadhostdetection.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3560 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/filterrequestfromurl.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      962 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/header.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     6765 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/redirects.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     4642 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/sampling.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2399 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/simhash.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)    13063 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/status.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3656 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/timeout.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1464 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/waf.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2796 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/ruleset.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/utils/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2647 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/utils/har.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)       97 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/setup.cfg
+-rwxrwxr-x   0 lph       (1000) lph       (1000)     1270 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `HammerTime-http-0.8/HammerTime_http.egg-info/SOURCES.txt` & `HammerTime-http-0.9.0/HammerTime_http.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.cfg
 setup.py
 HammerTime_http.egg-info/PKG-INFO
 HammerTime_http.egg-info/SOURCES.txt
 HammerTime_http.egg-info/dependency_links.txt
 HammerTime_http.egg-info/requires.txt
```

### Comparing `HammerTime-http-0.8/README.md` & `HammerTime-http-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/__init__.py` & `HammerTime-http-0.9.0/hammertime/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/__version__.py` & `HammerTime-http-0.9.0/hammertime/__version__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-__version__ = "0.1.x"
-__version__ = '0.8'
+__version__ = "0.9.0"
```

### Comparing `HammerTime-http-0.8/hammertime/config.py` & `HammerTime-http-0.9.0/hammertime/config.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/core.py` & `HammerTime-http-0.9.0/hammertime/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,22 @@
 class HammerTime:
 
     def __init__(self, loop=None, request_engine=None, kb=None, retry_count=0, proxy=None,
                  scale_policy: Policy = None):
         self.loop = loop
         self.stats = Stats()
 
-        self.request_engine = RetryEngine(request_engine, loop=loop, stats=self.stats, retry_count=retry_count,
+        self.request_engine = RetryEngine(request_engine, stats=self.stats, retry_count=retry_count,
                                           scale_policy=scale_policy)
         if proxy is not None:
             self.request_engine.set_proxy(proxy)
         self.heuristics = Heuristics(kb=kb, request_engine=self.request_engine)
 
         self.tasks = deque()
-        self.closed = asyncio.Future(loop=loop)
-        self.loop.add_signal_handler(signal.SIGINT, self._interrupt)
+        self.closed = asyncio.Future()
         self._success_iterator = None
         self._interrupted = False
         self._request_scheduler = RequestScheduler(loop=loop)
 
     @property
     def completed_count(self):
         return self.stats.completed
@@ -62,15 +61,15 @@
     @property
     def is_closed(self):
         return self.closed.done()
 
     def request(self, *args, **kwargs):
         if self.is_closed:
             # Return an exception as if it were a task when attempting to request on a closed engine
-            future = asyncio.Future(loop=self.loop)
+            future = asyncio.Future()
             future.set_exception(asyncio.CancelledError())
             return future
 
         self.stats.requested += 1
         future = self._request_scheduler.request(self._request(*args, **kwargs))
         self.tasks.append(future)
         future.add_done_callback(self._on_completion)
@@ -140,16 +139,16 @@
         if not self._interrupted:
             self._interrupted = True
             asyncio.ensure_future(self.close(), loop=self.loop)
 
 
 class QueueIterator:
 
-    def __init__(self, *, loop, has_pending_cb):
-        self.queue = asyncio.Queue(loop=loop)
+    def __init__(self, *, loop=None, has_pending_cb):
+        self.queue = asyncio.Queue()
         self.has_pending = has_pending_cb
 
     def complete(self, entry):
         if entry or not self.has_pending():
             self.queue.put_nowait(entry)
 
     def __aiter__(self):
```

### Comparing `HammerTime-http-0.8/hammertime/engine/__init__.py` & `HammerTime-http-0.9.0/hammertime/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/engine/aiohttp.py` & `HammerTime-http-0.9.0/hammertime/engine/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 import ssl
 
 from ..ruleset import StopRequest, RejectRequest
 
 
 class AioHttpEngine:
 
-    def __init__(self, *, loop, verify_ssl=True, ca_certificate_file=None, proxy=None, timeout=0.2,
+    def __init__(self, *, loop=None, verify_ssl=True, ca_certificate_file=None, proxy=None, timeout=0.2,
                  disable_cookies=False, client_session=None):
-        self.loop = loop
         self.session = client_session
         if self.session is None:
             if disable_cookies:
-                self.session = ClientSession(loop=loop, cookie_jar=DummyCookieJar(loop=loop))
+                self.session = ClientSession(loop=loop, cookie_jar=DummyCookieJar())
             else:
                 self.session = ClientSession(loop=loop)
+        self.loop = loop
         self.proxy = proxy
         self.timeout = timeout
         self.ssl = None
         self.set_ssl_parameters(verify_ssl=verify_ssl, ca_certificate_file=ca_certificate_file)
 
     def set_ssl_parameters(self, *, verify_ssl=True, ca_certificate_file=None):
         if ca_certificate_file:
@@ -74,15 +74,15 @@
         except (KeyError, RuntimeError, asyncio.CancelledError):
             raise asyncio.CancelledError
 
     async def _perform(self, entry, heuristics):
         req = entry.request
 
         timeout_value = entry.arguments.get("timeout", self.timeout)
-        with timeout(timeout_value + 0.3, loop=self.loop):
+        async with timeout(timeout_value + 0.3):
             extra_args = {}
             if self.proxy:
                 extra_args["proxy"] = self.proxy
             if entry.request.headers:
                 extra_args["headers"] = entry.request.headers
 
             response = await self.session.request(method=req.method, url=req.url, allow_redirects=False,
@@ -90,15 +90,15 @@
 
         # When the request is simply rejected, we want to keep the persistent connection alive
         async with ProtectedSession(response, RejectRequest):
             entry.response = Response(response.status, response.headers)
 
             await heuristics.after_headers(entry)
 
-            with timeout(2.0):
+            async with timeout(2.0):
                 # read_length is set to -1 if unlimited, which is the same as aiohttp
                 max_length = entry.result.read_length
                 entry.response.set_content(await response.content.read(max_length), response.content.at_eof())
 
         await heuristics.after_response(entry)
 
         return entry
```

### Comparing `HammerTime-http-0.8/hammertime/engine/interface.py` & `HammerTime-http-0.9.0/hammertime/engine/interface.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/engine/retry.py` & `HammerTime-http-0.9.0/hammertime/engine/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 from . import Engine
 from .scaling import Policy, StaticPolicy
 from ..ruleset import StopRequest
 
 
 class RetryEngine(Engine):
 
-    def __init__(self, engine, *, loop, stats, retry_count=0, retry_delay=1.0,
+    def __init__(self, engine, *, stats, retry_count=0, retry_delay=1.0,
                  scale_policy: Policy = None):
         self.scale_policy = scale_policy or StaticPolicy(30)
         self.request_engine = engine
         self.retry_count = retry_count
         self.stats = stats
         self.general_limiter = self.scale_policy.get_semaphore()
-        self.priority_limiter = asyncio.Semaphore(3, loop=loop)
+        self.priority_limiter = asyncio.Semaphore(3)
         self.default_heuristics = None
         self.retry_delay = retry_delay
 
     async def perform(self, entry, heuristics):
         if self.default_heuristics is None:
             self.default_heuristics = weakref(heuristics)
```

### Comparing `HammerTime-http-0.8/hammertime/engine/scaling.py` & `HammerTime-http-0.9.0/hammertime/engine/scaling.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/http.py` & `HammerTime-http-0.9.0/hammertime/http.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/kb.py` & `HammerTime-http-0.9.0/hammertime/kb.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/requestscheduler.py` & `HammerTime-http-0.9.0/hammertime/requestscheduler.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/__init__.py` & `HammerTime-http-0.9.0/hammertime/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/behavior.py` & `HammerTime-http-0.9.0/hammertime/rules/behavior.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/body.py` & `HammerTime-http-0.9.0/hammertime/rules/body.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/deadhostdetection.py` & `HammerTime-http-0.9.0/hammertime/rules/deadhostdetection.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/filterrequestfromurl.py` & `HammerTime-http-0.9.0/hammertime/rules/filterrequestfromurl.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/header.py` & `HammerTime-http-0.9.0/hammertime/rules/header.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/redirects.py` & `HammerTime-http-0.9.0/hammertime/rules/redirects.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/sampling.py` & `HammerTime-http-0.9.0/hammertime/rules/sampling.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/simhash.py` & `HammerTime-http-0.9.0/hammertime/rules/simhash.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/status.py` & `HammerTime-http-0.9.0/hammertime/rules/status.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/timeout.py` & `HammerTime-http-0.9.0/hammertime/rules/timeout.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/rules/waf.py` & `HammerTime-http-0.9.0/hammertime/rules/waf.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/ruleset.py` & `HammerTime-http-0.9.0/hammertime/ruleset.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/hammertime/utils/har.py` & `HammerTime-http-0.9.0/hammertime/utils/har.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.8/setup.py` & `HammerTime-http-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 with open(version_file) as f:
     code = compile(f.read(), version_file, 'exec')
     exec(code, globals(), version_data)
 
 setup(name='HammerTime-http',
       version=version_data['__version__'],
       description='HammerTime is an HTTP client library aiming to perform a large number of requests on a server as fast as it can take them, but without distrupting operations significantly.',
-      python_requires='>=3.6.0,<3.9.0',
+      python_requires='>=3.8.0,<3.12.0',
       author='Delve Labs inc.',
       author_email='info@delvelabs.ca',
       url='https://github.com/delvelabs/hammertime',
       packages=['hammertime',
                 'hammertime.engine',
                 'hammertime.rules',
                 'hammertime.utils'],
       install_requires=[
-          'aiohttp>=3.7.3,<4.0.0',
-          'easyinject==0.3',
-          'aiodns>=1.1.1,<3.0.0'
+        'aiodns>=1.1.1,<3.0.0',
+        'aiohttp>=3.7.3,<4.0.0',
+        'coverage==4.2',
+        'easyinject==0.3',
+        'flake8==3.8.4',
+        'marshmallow_autoschema==0.3.3',
+        'marshmallow_har==1.1.0',
       ],
-      extras_require={
-          'simhash':  ['simhash==2.0.0'],
-          'simhash-py': [
-              'forkedsimhash-py==0.4.2',
-              'six'
-          ]
-      },
-      license="GPLv2"
-     )
+      setup_requires=["pytest-runner"],
+      tests_require=[
+        'async_timeout==4.0.0a3',
+        'flake8==3.8.4',
+        'pytest>=6.0,<7.0',
+        'simhash==2.1.2',
+      ],
+      license="GPLv2",
+)
```


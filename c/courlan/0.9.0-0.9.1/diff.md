# Comparing `tmp/courlan-0.9.0.tar.gz` & `tmp/courlan-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "courlan-0.9.0.tar", last modified: Tue Mar  7 12:17:45 2023, max compression
+gzip compressed data, was "courlan-0.9.1.tar", last modified: Mon Apr 24 16:06:18 2023, max compression
```

## Comparing `courlan-0.9.0.tar` & `courlan-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2023-03-07 12:17:45.390548 courlan-0.9.0/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1131 2020-08-31 17:20:52.000000 courlan-0.9.0/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2477 2023-03-07 12:04:02.000000 courlan-0.9.0/HISTORY.md
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    35141 2020-08-31 17:20:52.000000 courlan-0.9.0/LICENSE
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      160 2022-07-18 17:01:18.000000 courlan-0.9.0/MANIFEST.in
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    17283 2023-03-07 12:17:45.390548 courlan-0.9.0/PKG-INFO
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    15627 2023-03-07 12:00:30.000000 courlan-0.9.0/README.rst
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2023-03-07 12:17:45.390548 courlan-0.9.0/courlan/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      629 2023-03-07 12:13:05.000000 courlan-0.9.0/courlan/__init__.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     6234 2023-03-07 12:15:30.000000 courlan-0.9.0/courlan/clean.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3691 2022-07-27 15:47:45.000000 courlan-0.9.0/courlan/cli.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     8447 2023-03-07 11:31:10.000000 courlan-0.9.0/courlan/core.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     7309 2023-03-07 11:39:05.000000 courlan-0.9.0/courlan/filters.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     7223 2023-03-07 12:06:22.000000 courlan-0.9.0/courlan/langinfo.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1220 2023-03-07 11:46:14.000000 courlan-0.9.0/courlan/network.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        0 2022-07-18 15:53:08.000000 courlan-0.9.0/courlan/py.typed
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1786 2022-07-07 18:06:58.000000 courlan-0.9.0/courlan/settings.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    15143 2023-03-03 13:37:11.000000 courlan-0.9.0/courlan/urlstore.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5794 2023-03-03 12:29:51.000000 courlan-0.9.0/courlan/urlutils.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2023-03-07 12:17:45.390548 courlan-0.9.0/courlan.egg-info/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    17283 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      605 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       45 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      111 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        8 2023-03-07 12:17:45.000000 courlan-0.9.0/courlan.egg-info/top_level.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   151953 2020-08-31 17:20:52.000000 courlan-0.9.0/courlan_harns-march.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       40 2021-12-07 18:31:00.000000 courlan-0.9.0/pytest.ini
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       38 2023-03-07 12:17:45.390548 courlan-0.9.0/setup.cfg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3840 2023-03-07 12:11:21.000000 courlan-0.9.0/setup.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2023-03-07 12:17:45.390548 courlan-0.9.0/tests/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        0 2020-08-31 17:20:52.000000 courlan-0.9.0/tests/__init__.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2023-03-07 12:17:45.390548 courlan-0.9.0/tests/data/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      324 2021-12-07 18:52:06.000000 courlan-0.9.0/tests/data/input.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    34473 2023-03-07 11:32:47.000000 courlan-0.9.0/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    11242 2023-02-23 16:32:17.000000 courlan-0.9.0/tests/urlstore_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-0.9.1/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2698 2023-04-24 16:04:57.000000 courlan-0.9.1/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    35141 2020-08-31 17:20:52.000000 courlan-0.9.1/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-0.9.1/MANIFEST.in
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-04-24 16:06:18.728592 courlan-0.9.1/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16025 2023-04-24 16:04:57.000000 courlan-0.9.1/README.rst
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/courlan/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2023-04-24 16:04:57.000000 courlan-0.9.1/courlan/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6234 2023-03-07 12:15:30.000000 courlan-0.9.1/courlan/clean.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3691 2022-07-27 15:47:45.000000 courlan-0.9.1/courlan/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8447 2023-03-07 11:31:10.000000 courlan-0.9.1/courlan/core.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7309 2023-03-07 11:39:05.000000 courlan-0.9.1/courlan/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-0.9.1/courlan/langinfo.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1637 2023-04-21 11:54:56.000000 courlan-0.9.1/courlan/network.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-0.9.1/courlan/py.typed
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1786 2022-07-07 18:06:58.000000 courlan-0.9.1/courlan/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16274 2023-04-24 15:31:49.000000 courlan-0.9.1/courlan/urlstore.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5794 2023-03-03 12:29:51.000000 courlan-0.9.1/courlan/urlutils.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/courlan.egg-info/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      605 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       46 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-03-07 12:17:45.000000 courlan-0.9.1/courlan.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      111 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2023-04-24 16:06:18.000000 courlan-0.9.1/courlan.egg-info/top_level.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-0.9.1/courlan_harns-march.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-0.9.1/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2023-04-24 16:06:18.728592 courlan-0.9.1/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3840 2023-03-07 12:11:21.000000 courlan-0.9.1/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-0.9.1/tests/__init__.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-04-24 16:06:18.728592 courlan-0.9.1/tests/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-0.9.1/tests/data/input.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    34473 2023-03-07 11:32:47.000000 courlan-0.9.1/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13038 2023-04-24 15:31:25.000000 courlan-0.9.1/tests/urlstore_tests.py
```

### Comparing `courlan-0.9.0/CONTRIBUTING.md` & `courlan-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/HISTORY.md` & `courlan-0.9.1/HISTORY.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 ## History / Changelog
 
 
+### 0.9.1
+
+- network tests: larger throughput
+- UrlStore: optional compression of rules (#21), added `reset()` (#22) and `get_all_counts()` methods
+- UrlStore fixes: `signal` in #18, `total_url_number`
+- updated Readme
+
+
 ### 0.9.0
 
 - hardening of filters and URL parses (#14)
 - normalize punicode to unicode
 - methods added to `UrlStore`: `get_crawl_delay()`, `print_unvisited_urls()`
 - `UrlStore` now triggers exit code 1 when interrupted
 - argument added to `extract_links()`: `no_filter`
```

### Comparing `courlan-0.9.0/LICENSE` & `courlan-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/PKG-INFO` & `courlan-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.0
+Version: 0.9.1
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
 Keywords: cleaner,crawler,preprocessing,url-parsing,url-manipulation,urls,validation,webcrawling
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -287,32 +288,40 @@
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
    - ``dump_urls()``: Return a list of all known URLs.
    - ``print_urls()``: Print all URLs in store (URL + TAB + visited or not).
    - ``print_unvisited_urls()``: Print all unvisited URLs in store.
+   - ``get_all_counts()``: Return all download counts for the hosts in store.
    - ``get_known_domains()``: Return all known domains as a list.
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
    - ``download_threshold_reached(threshold)``: Find out if the download limit (in seconds) has been reached for one of the websites in store.
    - ``unvisited_websites_number()``: Return the number of websites for which there are still URLs to visit.
    - ``is_exhausted_domain(domain)``: Tell if all known URLs for the website have been visited.
 
+Optional settings:
+- ``compressed=True``: activate compression of URLs and rules
+- ``language=XX``: focus on a particular target language (two-letter code)
+- ``strict=True``: stricter URL filtering
+- ``verbose=True``: dump URLs if interrupted (requires use of ``signal``)
+
 
 Command-line
 ------------
 
 The main fonctions are also available through a command-line utility.
 
 .. code-block:: bash
@@ -410,7 +419,9 @@
 
 
 References
 ----------
 
 - Cho, J., Garcia-Molina, H., & Page, L. (1998). Efficient crawling through URL ordering. *Computer networks and ISDN systems*, 30(1-7), 161–172.
 - Edwards, J., McCurley, K. S., and Tomlin, J. A. (2001). "An adaptive model for optimizing performance of an incremental web crawler". In *Proceedings of the 10th international conference on World Wide Web - WWW '01*, pp. 106–113.
+
+
```

### Comparing `courlan-0.9.0/README.rst` & `courlan-0.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -251,32 +251,40 @@
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
    - ``dump_urls()``: Return a list of all known URLs.
    - ``print_urls()``: Print all URLs in store (URL + TAB + visited or not).
    - ``print_unvisited_urls()``: Print all unvisited URLs in store.
+   - ``get_all_counts()``: Return all download counts for the hosts in store.
    - ``get_known_domains()``: Return all known domains as a list.
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
    - ``download_threshold_reached(threshold)``: Find out if the download limit (in seconds) has been reached for one of the websites in store.
    - ``unvisited_websites_number()``: Return the number of websites for which there are still URLs to visit.
    - ``is_exhausted_domain(domain)``: Tell if all known URLs for the website have been visited.
 
+Optional settings:
+- ``compressed=True``: activate compression of URLs and rules
+- ``language=XX``: focus on a particular target language (two-letter code)
+- ``strict=True``: stricter URL filtering
+- ``verbose=True``: dump URLs if interrupted (requires use of ``signal``)
+
 
 Command-line
 ------------
 
 The main fonctions are also available through a command-line utility.
 
 .. code-block:: bash
```

### Comparing `courlan-0.9.0/courlan/__init__.py` & `courlan-0.9.1/courlan/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # meta
 __title__ = "courlan"
 __author__ = "Adrien Barbaresi"
 __license__ = "GNU GPL v3+"
 __copyright__ = "Copyright 2020-2023, Adrien Barbaresi"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 # imports
 from .clean import clean_url, normalize_url, scrub_url
 from .core import check_url, extract_links, sample_urls
 from .filters import is_navigation_page, is_not_crawlable, lang_filter, validate_url
 from .urlstore import UrlStore
```

### Comparing `courlan-0.9.0/courlan/clean.py` & `courlan-0.9.1/courlan/clean.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/cli.py` & `courlan-0.9.1/courlan/cli.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/core.py` & `courlan-0.9.1/courlan/core.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/filters.py` & `courlan-0.9.1/courlan/filters.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/langinfo.py` & `courlan-0.9.1/courlan/langinfo.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/network.py` & `courlan-0.9.1/courlan/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,41 @@
 
 import urllib3
 
 
 LOGGER = logging.getLogger(__name__)
 
 RETRY_STRATEGY = urllib3.util.Retry(
-    total=5,
-    redirect=5,
+    total=2,
+    redirect=2,
     raise_on_redirect=False,
+    status_forcelist=[
+        429,
+        499,
+        500,
+        502,
+        503,
+        504,
+        509,
+        520,
+        521,
+        522,
+        523,
+        524,
+        525,
+        526,
+        527,
+        530,
+        598,
+    ],  # unofficial: https://en.wikipedia.org/wiki/List_of_HTTP_status_codes#Unofficial_codes
+    backoff_factor=1,
+)
+HTTP_POOL = urllib3.PoolManager(
+    cert_reqs="CERT_NONE", num_pools=100, retries=RETRY_STRATEGY, timeout=10
 )
-HTTP_POOL = urllib3.PoolManager(retries=RETRY_STRATEGY)
 
 ACCEPTABLE_CODES = {200, 300, 301, 302, 303, 304, 305, 306, 307, 308}
 
 
 # Test redirects
 def redirection_test(url: str) -> str:
     """Test final URL to handle redirects
```

### Comparing `courlan-0.9.0/courlan/settings.py` & `courlan-0.9.1/courlan/settings.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan/urlstore.py` & `courlan-0.9.1/courlan/urlstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Defines a URL store which holds URLs along with relevant information.
 """
 
 import bz2
+import gc
 import logging
 import pickle
 import signal
 import sys
+import zlib
 
 from collections import defaultdict, deque
 from datetime import datetime, timedelta
 from threading import Lock
 from typing import Any, DefaultDict, Deque, Dict, List, Optional, Tuple, Union
 
 from urllib.robotparser import RobotFileParser
@@ -48,14 +50,15 @@
     __slots__ = ("compressed", "done", "language", "strict", "urldict", "_lock")
 
     def __init__(
         self,
         compressed: bool = False,
         language: Optional[str] = None,
         strict: bool = False,
+        verbose: bool = False,
     ) -> None:
         self.compressed: bool = compressed
         self.done: bool = False
         self.language: Optional[str] = language
         self.strict: bool = strict
         self.urldict: DefaultDict[str, DomainEntry] = defaultdict(DomainEntry)
         self._lock: Lock = Lock()
@@ -65,18 +68,25 @@
                 "Processing interrupted, dumping unvisited URLs from %s hosts",
                 len(self.urldict),
             )
             self.print_unvisited_urls()
             sys.exit(1)
 
         # don't use the following on Windows
-        if not sys.platform.startswith("win"):
+        if verbose and not sys.platform.startswith("win"):
             signal.signal(signal.SIGINT, dump_unvisited_urls)
             signal.signal(signal.SIGTERM, dump_unvisited_urls)
 
+    def reset(self) -> None:
+        "Re-initialize the URL store."
+        with self._lock:
+            self.urldict = defaultdict(DomainEntry)
+            num = gc.collect()
+            LOGGER.debug("UrlStore reset, %s objects in GC", num)
+
     def _buffer_urls(
         self, data: List[str], visited: bool = False
     ) -> DefaultDict[str, Deque[UrlPathTuple]]:
         inputdict: DefaultDict[str, Deque[UrlPathTuple]] = defaultdict(deque)
         for url in list(dict.fromkeys(data)):
             # segment URL and add to domain dictionary
             try:
@@ -138,15 +148,15 @@
         if to_left is not None:
             urls.extendleft(t for t in to_left if not is_known_link(t.urlpath, known))
 
         # use lock
         with self._lock:
             # compression
             if self.compressed:
-                self.urldict[domain].tuples = bz2.compress(  # type: ignore
+                self.urldict[domain].tuples = bz2.compress(  # type: ignore[assignment]
                     pickle.dumps(urls, protocol=4)
                 )
             else:
                 self.urldict[domain].tuples = urls
             # adjust all_visited status
             self.urldict[domain].all_visited = all(u.visited for u in urls)
             # timestamp/backoff value
@@ -248,26 +258,28 @@
 
     def unvisited_websites_number(self) -> int:
         "Return the number of websites for which there are still URLs to visit."
         return len([d for d in self.urldict if not self.urldict[d].all_visited])
 
     # DOWNLOADS
 
-    def get_url(self, domain: str) -> Optional[str]:
+    def get_url(self, domain: str, as_visited: bool = True) -> Optional[str]:
         "Retrieve a single URL and consider it to be visited (with corresponding timestamp)."
         # not fully used
         if not self.urldict[domain].all_visited:
             url_tuples = self._load_urls(domain)
             # get first non-seen url
             for url in url_tuples:
                 if not url.visited:
-                    url.visited = True
-                    with self._lock:
-                        self.urldict[domain].count += 1
-                    self._store_urls(domain, url_tuples, timestamp=datetime.now())
+                    # store information
+                    if as_visited is True:
+                        url.visited = True
+                        with self._lock:
+                            self.urldict[domain].count += 1
+                        self._store_urls(domain, url_tuples, timestamp=datetime.now())
                     return domain + url.urlpath
         # nothing to draw from
         with self._lock:
             self.urldict[domain].all_visited = True
         return None
 
     def get_download_urls(self, timelimit: int = 10) -> Optional[List[str]]:
@@ -338,36 +350,53 @@
             # calculate difference and offset last addition
             total_diff = now + timedelta(0, schedule_secs - time_limit)
             # store new info
             self._store_urls(domain, url_tuples, timestamp=total_diff)
         # sort by first tuple element (time in secs)
         return sorted(targets, key=lambda x: x[0])  # type: ignore[arg-type]
 
+    # CRAWLING
+
+    def store_rules(self, website: str, rules: Optional[RobotFileParser]) -> None:
+        "Store crawling rules for a given website."
+        if self.compressed:
+            rules = zlib.compress(  # type: ignore[assignment]
+                pickle.dumps(rules, protocol=4)
+            )
+        self.urldict[website].rules = rules
+
     def get_rules(self, website: str) -> Optional[RobotFileParser]:
         "Return the stored crawling rules for the given website."
         if website in self.urldict:
-            return self.urldict[website].rules
+            if self.compressed:
+                return pickle.loads(zlib.decompress(self.urldict[website].rules))  # type: ignore[arg-type]
+            else:
+                return self.urldict[website].rules
         return None
 
     def get_crawl_delay(self, website: str, default: float = 5) -> float:
         "Return the delay as extracted from robots.txt, or a given default."
         delay = None
         rules = self.get_rules(website)
         try:
             delay = rules.crawl_delay("*")  # type: ignore[union-attr]
         except AttributeError:  # no rules or no crawl delay
             pass
         # backup
-        return delay or default  # type: ignore
+        return delay or default  # type: ignore[return-value]
 
     # GENERAL INFO
 
+    def get_all_counts(self) -> List[int]:
+        "Return all download counts for the hosts in store."
+        return [self.urldict[d].count for d in self.urldict]
+
     def total_url_number(self) -> int:
         "Find number of all URLs in store."
-        return sum(len(self.urldict[d].tuples) for d in self.urldict)
+        return sum(len(self._load_urls(d)) for d in self.urldict)
 
     def download_threshold_reached(self, threshold: float) -> bool:
         "Find out if the download limit (in seconds) has been reached for one of the websites in store."
         return any(self.urldict[d].count >= threshold for d in self.urldict)
 
     def dump_urls(self) -> List[str]:
         "Return a list of all known URLs."
```

### Comparing `courlan-0.9.0/courlan/urlutils.py` & `courlan-0.9.1/courlan/urlutils.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan.egg-info/PKG-INFO` & `courlan-0.9.1/courlan.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.0
+Version: 0.9.1
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
 Keywords: cleaner,crawler,preprocessing,url-parsing,url-manipulation,urls,validation,webcrawling
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -287,32 +288,40 @@
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
    - ``dump_urls()``: Return a list of all known URLs.
    - ``print_urls()``: Print all URLs in store (URL + TAB + visited or not).
    - ``print_unvisited_urls()``: Print all unvisited URLs in store.
+   - ``get_all_counts()``: Return all download counts for the hosts in store.
    - ``get_known_domains()``: Return all known domains as a list.
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
    - ``download_threshold_reached(threshold)``: Find out if the download limit (in seconds) has been reached for one of the websites in store.
    - ``unvisited_websites_number()``: Return the number of websites for which there are still URLs to visit.
    - ``is_exhausted_domain(domain)``: Tell if all known URLs for the website have been visited.
 
+Optional settings:
+- ``compressed=True``: activate compression of URLs and rules
+- ``language=XX``: focus on a particular target language (two-letter code)
+- ``strict=True``: stricter URL filtering
+- ``verbose=True``: dump URLs if interrupted (requires use of ``signal``)
+
 
 Command-line
 ------------
 
 The main fonctions are also available through a command-line utility.
 
 .. code-block:: bash
@@ -410,7 +419,9 @@
 
 
 References
 ----------
 
 - Cho, J., Garcia-Molina, H., & Page, L. (1998). Efficient crawling through URL ordering. *Computer networks and ISDN systems*, 30(1-7), 161–172.
 - Edwards, J., McCurley, K. S., and Tomlin, J. A. (2001). "An adaptive model for optimizing performance of an incremental web crawler". In *Proceedings of the 10th international conference on World Wide Web - WWW '01*, pp. 106–113.
+
+
```

### Comparing `courlan-0.9.0/courlan.egg-info/SOURCES.txt` & `courlan-0.9.1/courlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/courlan_harns-march.jpg` & `courlan-0.9.1/courlan_harns-march.jpg`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/setup.py` & `courlan-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/tests/unit_tests.py` & `courlan-0.9.1/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.0/tests/urlstore_tests.py` & `courlan-0.9.1/tests/urlstore_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Unit tests for the UrlStore class of the courlan package.
 """
 
+import gc
 import os
 import pickle
 import signal
+import sys
 import uuid
 
 from datetime import datetime
 
 import pytest
 
 from courlan import UrlStore
@@ -29,39 +31,56 @@
         "http://example.org/1",
     ]
     my_urls.add_urls(candidates)
     assert len(my_urls.urldict) == 1 and "http://example.org" not in my_urls.urldict
     assert len(my_urls.urldict["https://example.org"].tuples) == 2
     firstelem = my_urls.urldict["https://example.org"].tuples[0]
     assert firstelem.urlpath == "/" and firstelem.visited is False
+    # reset
+    num, _, _ = gc.get_count()
+    my_urls.reset()
+    num2, _, _ = gc.get_count()
+    assert len(my_urls.urldict) == 0
+    assert num2 < num
 
-    my_urls = UrlStore()
     candidates = [
         "http://example.org/",
         "https://example.org/",
         "http://example.org/1",
         "https://example.org/1",
     ]
     my_urls.add_urls(candidates)
     assert len(my_urls.urldict) == 1 and "http://example.org" not in my_urls.urldict
     assert len(my_urls.urldict["https://example.org"].tuples) == 2
 
     # rules
-    my_urls.urldict["https://example.org"].rules = pickle.loads(
+    rules = pickle.loads(
         b"\x80\x03curllib.robotparser\nRobotFileParser\nq\x00)\x81q\x01}q\x02(X\x07\x00\x00\x00entriesq\x03]q\x04X\r\x00\x00\x00default_entryq\x05NX\x0c\x00\x00\x00disallow_allq\x06\x89X\t\x00\x00\x00allow_allq\x07\x89X\x03\x00\x00\x00urlq\x08X\x1f\x00\x00\x00https://sitemaps.org/robots.txtq\tX\x04\x00\x00\x00hostq\nX\x0c\x00\x00\x00sitemaps.orgq\x0bX\x04\x00\x00\x00pathq\x0cX\x0b\x00\x00\x00/robots.txtq\rX\x0c\x00\x00\x00last_checkedq\x0eGA\xd8\x87\xf5\xdc\xab\xd5\x00ub."
     )
+    my_urls.store_rules("https://example.org", rules)
     assert my_urls.get_rules("http://test.org") is None
     assert my_urls.urldict["https://example.org"].rules is not None
     assert (
         my_urls.get_rules("https://example.org")
         == my_urls.urldict["https://example.org"].rules
+        == rules
     )
     assert my_urls.get_crawl_delay("http://test.org", default=2) == 2
     assert my_urls.get_crawl_delay("https://example.org") == 5
 
+    assert my_urls.compressed is False
+    my_urls.urldict["https://example.org"].rules = None
+
+    my_urls.compressed = True
+    my_urls.store_rules("https://example.org", rules)
+    assert my_urls.urldict["https://example.org"].rules is not None
+    # no identity check since different location after compression
+    assert my_urls.get_rules("https://example.org").mtime() == rules.mtime()
+    my_urls.compressed = False
+
     # filters
     my_urls = UrlStore(language="en", strict=True)
     candidates = [
         "https://de.wikipedia.org/",
         "https://www.sitemaps.org/en_GB/protocol.html",
         "http://example.com/de/test.html",
     ]
@@ -78,35 +97,38 @@
     test_urls = [f"https://test.org/{str(uuid.uuid4())[:20]}" for _ in range(10000)]
     urls = example_urls + test_urls
 
     # compression 1
     my_urls = UrlStore(compressed=True)
     url_buffer = UrlStore()._buffer_urls(example_urls)
     my_urls.add_urls(example_urls)
+    assert my_urls.total_url_number() == len(example_urls)
     # necessary to pickle
     my_urls._lock = None
     assert len(pickle.dumps(my_urls)) < len(pickle.dumps(url_buffer))
     assert my_urls.is_known(f"{example_domain}/100") is True
     # compression 2
     my_urls = UrlStore(compressed=True)
     url_buffer = UrlStore()._buffer_urls(test_urls)
     my_urls.add_urls(test_urls)
+    assert my_urls.total_url_number() == len(test_urls)
     # necessary to pickle
     my_urls._lock = None
     assert len(pickle.dumps(my_urls)) < len(pickle.dumps(url_buffer))
 
     # test loading
     url_buffer = UrlStore()._buffer_urls(urls)
     assert sum(len(v) for _, v in url_buffer.items()) == len(urls)
     my_urls = UrlStore()
     my_urls.add_urls(urls)
     assert sum(len(my_urls._load_urls(k)) for k, _ in my_urls.urldict.items()) == len(
         urls
     )
     assert my_urls.total_url_number() == len(urls)
+    assert my_urls.get_all_counts() == [0, 0]
 
     if my_urls.compressed is False:
         assert sum(len(v.tuples) for _, v in my_urls.urldict.items()) == len(urls)
     my_urls.add_urls(["https://visited.com/visited"], visited=True)
     assert my_urls.urldict["https://visited.com"].tuples[0].visited is True
     assert my_urls.urldict["https://visited.com"].all_visited is True
     assert my_urls.is_exhausted_domain("https://visited.com") is True
@@ -139,18 +161,32 @@
         extension_urls
     )
     assert url_tuples[-1].urlpath == "/1/9" and url_tuples[0].urlpath == "/1/10/"
 
     # get_url
     assert my_urls.urldict[example_domain].timestamp is None
     assert my_urls.urldict[example_domain].count == 0
+
     url1 = my_urls.get_url(example_domain)
+    timestamp = my_urls.urldict[example_domain].timestamp
     url2 = my_urls.get_url(example_domain)
     assert url1 != url2 and url1 == "https://www.example.org/1/10/"
     assert my_urls.urldict[example_domain].count == 2
+    assert timestamp != my_urls.urldict[example_domain].timestamp
+    assert url2 not in set(my_urls.find_unvisited_urls(example_domain))
+    assert my_urls.get_all_counts() == [2, 0, 0]
+
+    # as_visited=False
+    timestamp = my_urls.urldict[example_domain].timestamp
+    url3 = my_urls.get_url(example_domain, as_visited=False)
+    assert url3 != url1 and url3 != url2
+    assert my_urls.urldict[example_domain].count == 2
+    assert timestamp == my_urls.urldict[example_domain].timestamp
+    assert url3 in set(my_urls.find_unvisited_urls(example_domain))
+
     url_tuples = my_urls._load_urls(example_domain)
     # positions
     assert url1.endswith(url_tuples[0].urlpath) and url2.endswith(url_tuples[1].urlpath)
     # timestamp
     assert my_urls.urldict[example_domain].timestamp is not None
     # nothing left
     assert my_urls.urldict[example_domain].all_visited is False
@@ -267,15 +303,25 @@
     other_one = UrlStore()
     other_one.add_urls(["http://test.org/this"])
     other_one.print_urls()
     captured = capsys.readouterr()
     assert captured.out.strip() == "http://test.org/this\tFalse"
 
     # dump unvisited, don't test it on Windows
-    interrupted_one = UrlStore()
-    interrupted_one.add_urls(["https://www.test.org/1", "https://www.test.org/2"])
     if os.name != "nt":
+        # standard
+        interrupted_one = UrlStore()
+        interrupted_one.add_urls(["https://www.test.org/1", "https://www.test.org/2"])
+        # sys.exit() since signals are not caught
+        with pytest.raises(SystemExit):
+            sys.exit(1)
+        captured = capsys.readouterr()
+        assert captured.out.strip() == ""
+        # verbose
+        interrupted_one = UrlStore(verbose=True)
+        interrupted_one.add_urls(["https://www.test.org/1", "https://www.test.org/2"])
+        # SIGINT + SIGTERM caught
         pid = os.getpid()
         with pytest.raises(SystemExit):
             os.kill(pid, signal.SIGINT)
         captured = capsys.readouterr()
         assert captured.out.strip().endswith("https://www.test.org/2")
```


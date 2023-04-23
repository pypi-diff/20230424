# Comparing `tmp/snakeviz-2.1.2.tar.gz` & `tmp/snakeviz-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snakeviz-2.1.2.tar", last modified: Sat Apr 15 20:22:14 2023, max compression
+gzip compressed data, was "/Users/jiffyclub/Library/CloudStorage/Dropbox/projects/snakeviz/dist/.tmp-rhc4jzz4/snakeviz-2.2.0.tar", last modified: Sun Apr 23 22:57:12 2023, max compression
```

## Comparing `snakeviz-2.1.2.tar` & `snakeviz-2.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     3693 2023-04-15 20:20:00.000000 snakeviz-2.1.2/CHANGES.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1435 2014-11-30 22:30:22.000000 snakeviz-2.1.2/LICENSE.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)      155 2014-11-30 22:30:22.000000 snakeviz-2.1.2/MANIFEST.in
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2017 2023-04-15 20:22:14.000000 snakeviz-2.1.2/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      901 2021-10-25 00:39:45.000000 snakeviz-2.1.2/README.rst
--rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-15 20:22:14.000000 snakeviz-2.1.2/setup.cfg
--rwxr-xr-x   0 jiffyclub   (501) staff       (20)     2008 2023-04-15 20:21:21.000000 snakeviz-2.1.2/setup.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/
--rw-r--r--   0 jiffyclub   (501) staff       (20)       57 2014-10-14 05:02:54.000000 snakeviz-2.1.2/snakeviz/__init__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)      192 2018-08-04 21:39:42.000000 snakeviz-2.1.2/snakeviz/__main__.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5807 2020-04-26 22:58:54.000000 snakeviz-2.1.2/snakeviz/cli.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5331 2020-04-26 23:59:59.000000 snakeviz-2.1.2/snakeviz/ipymagic.py
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2057 2020-04-26 23:53:30.000000 snakeviz-2.1.2/snakeviz/main.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/
--rw-r--r--   0 jiffyclub   (501) staff       (20)    11369 2023-04-15 20:14:45.000000 snakeviz-2.1.2/snakeviz/static/drawsvg.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1406 2014-10-14 05:02:54.000000 snakeviz-2.1.2/snakeviz/static/favicon.ico
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/images/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1118 2014-10-15 05:48:31.000000 snakeviz-2.1.2/snakeviz/static/images/sort_asc.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1136 2014-10-15 05:48:01.000000 snakeviz-2.1.2/snakeviz/static/images/sort_both.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1127 2014-10-15 05:48:40.000000 snakeviz-2.1.2/snakeviz/static/images/sort_desc.png
--rw-r--r--   0 jiffyclub   (501) staff       (20)     5077 2023-04-15 20:14:45.000000 snakeviz-2.1.2/snakeviz/static/snakeviz.css
--rw-r--r--   0 jiffyclub   (501) staff       (20)     6756 2017-09-24 04:26:04.000000 snakeviz-2.1.2/snakeviz/static/snakeviz.js
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/static/vendor/
--rw-r--r--   0 jiffyclub   (501) staff       (20)   151725 2021-01-24 01:16:36.000000 snakeviz-2.1.2/snakeviz/static/vendor/d3.v3.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    57032 2016-06-22 20:04:09.000000 snakeviz-2.1.2/snakeviz/static/vendor/immutable.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    86659 2017-03-20 19:01:15.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery-3.2.1.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    14112 2017-04-18 08:46:44.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.css
--rw-r--r--   0 jiffyclub   (501) staff       (20)    83268 2017-04-18 08:46:44.000000 snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)    71419 2016-12-31 17:47:51.000000 snakeviz-2.1.2/snakeviz/static/vendor/lodash.min.js
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2175 2017-09-24 04:26:04.000000 snakeviz-2.1.2/snakeviz/stats.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz/templates/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     1757 2017-09-27 04:47:30.000000 snakeviz-2.1.2/snakeviz/templates/dir.html
--rw-r--r--   0 jiffyclub   (501) staff       (20)    11485 2021-10-25 00:39:45.000000 snakeviz-2.1.2/snakeviz/templates/viz.html
--rw-r--r--   0 jiffyclub   (501) staff       (20)       31 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz/version.py
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/snakeviz.egg-info/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2017 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/PKG-INFO
--rw-r--r--   0 jiffyclub   (501) staff       (20)      947 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/SOURCES.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/dependency_links.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       47 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/entry_points.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)       13 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/requires.txt
--rw-r--r--   0 jiffyclub   (501) staff       (20)        9 2023-04-15 20:22:13.000000 snakeviz-2.1.2/snakeviz.egg-info/top_level.txt
-drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-15 20:22:14.000000 snakeviz-2.1.2/tests/
--rw-r--r--   0 jiffyclub   (501) staff       (20)     2031 2021-10-25 01:35:30.000000 snakeviz-2.1.2/tests/test_snakeviz.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3842 2023-04-23 22:55:47.000000 snakeviz-2.2.0/CHANGES.rst
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1435 2014-11-30 22:30:22.000000 snakeviz-2.2.0/LICENSE.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      135 2023-04-20 03:19:33.000000 snakeviz-2.2.0/MANIFEST.in
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3536 2023-04-23 22:57:12.000000 snakeviz-2.2.0/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      901 2021-10-25 00:39:45.000000 snakeviz-2.2.0/README.rst
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1189 2023-04-20 03:19:33.000000 snakeviz-2.2.0/pyproject.toml
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-23 22:57:12.000000 snakeviz-2.2.0/setup.cfg
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       67 2023-04-23 22:56:30.000000 snakeviz-2.2.0/snakeviz/__init__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      192 2018-08-04 21:39:42.000000 snakeviz-2.2.0/snakeviz/__main__.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5806 2023-04-20 03:19:33.000000 snakeviz-2.2.0/snakeviz/cli.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     7008 2023-04-20 02:23:45.000000 snakeviz-2.2.0/snakeviz/ipymagic.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2057 2020-04-26 23:53:30.000000 snakeviz-2.2.0/snakeviz/main.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz/static/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    11369 2023-04-20 02:12:41.000000 snakeviz-2.2.0/snakeviz/static/drawsvg.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1406 2014-10-14 05:02:54.000000 snakeviz-2.2.0/snakeviz/static/favicon.ico
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz/static/images/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1118 2014-10-15 05:48:31.000000 snakeviz-2.2.0/snakeviz/static/images/sort_asc.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1136 2014-10-15 05:48:01.000000 snakeviz-2.2.0/snakeviz/static/images/sort_both.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1127 2014-10-15 05:48:40.000000 snakeviz-2.2.0/snakeviz/static/images/sort_desc.png
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     5077 2023-04-20 02:12:41.000000 snakeviz-2.2.0/snakeviz/static/snakeviz.css
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     6756 2017-09-24 04:26:04.000000 snakeviz-2.2.0/snakeviz/static/snakeviz.js
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz/static/vendor/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)   151725 2021-01-24 01:16:36.000000 snakeviz-2.2.0/snakeviz/static/vendor/d3.v3.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    57032 2016-06-22 20:04:09.000000 snakeviz-2.2.0/snakeviz/static/vendor/immutable.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    86659 2017-03-20 19:01:15.000000 snakeviz-2.2.0/snakeviz/static/vendor/jquery-3.2.1.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    14112 2017-04-18 08:46:44.000000 snakeviz-2.2.0/snakeviz/static/vendor/jquery.dataTables.min.css
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    83268 2017-04-18 08:46:44.000000 snakeviz-2.2.0/snakeviz/static/vendor/jquery.dataTables.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    71419 2016-12-31 17:47:51.000000 snakeviz-2.2.0/snakeviz/static/vendor/lodash.min.js
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2175 2017-09-24 04:26:04.000000 snakeviz-2.2.0/snakeviz/stats.py
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz/templates/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1757 2017-09-27 04:47:30.000000 snakeviz-2.2.0/snakeviz/templates/dir.html
+-rw-r--r--   0 jiffyclub   (501) staff       (20)    11485 2021-10-25 00:39:45.000000 snakeviz-2.2.0/snakeviz/templates/viz.html
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     3536 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/PKG-INFO
+-rw-r--r--   0 jiffyclub   (501) staff       (20)      956 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        1 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       47 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/entry_points.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)       13 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/requires.txt
+-rw-r--r--   0 jiffyclub   (501) staff       (20)        9 2023-04-23 22:57:12.000000 snakeviz-2.2.0/snakeviz.egg-info/top_level.txt
+drwxr-xr-x   0 jiffyclub   (501) staff       (20)        0 2023-04-23 22:57:12.000000 snakeviz-2.2.0/tests/
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     1914 2023-04-20 02:23:45.000000 snakeviz-2.2.0/tests/test_ipymagic.py
+-rw-r--r--   0 jiffyclub   (501) staff       (20)     2015 2023-04-20 03:19:33.000000 snakeviz-2.2.0/tests/test_snakeviz.py
```

### Comparing `snakeviz-2.1.2/CHANGES.rst` & `snakeviz-2.2.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v2.2.0
+===================
+
+* Add configuration options for the %snakeviz magic
+  (thanks @dabacon in #174)
+* Drop explicit support for EOL Pythons
+
 v2.1.2
 ===================
 
 * Add dark theme (thanks @martinbagic in #173)
 * Add python-requires metadata (thanks @matthewfeickert in #188)
 
 v2.1.1
```

### Comparing `snakeviz-2.1.2/LICENSE.txt` & `snakeviz-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/README.rst` & `snakeviz-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/cli.py` & `snakeviz-2.2.0/snakeviz/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pstats import Stats
 
 try:
     from urllib.parse import quote
 except ImportError:
     from urllib import quote
 
-from . import version
+from snakeviz import VERSION
 
 
 # As seen in IPython:
 # https://github.com/ipython/ipython/blob/8be7f9abd97eafb493817371d70101d28640919c/IPython/html/notebookapp.py
 # See the IPython license at:
 # https://github.com/ipython/ipython/blob/master/COPYING.rst.
 def random_ports(port, n):
@@ -46,15 +46,15 @@
 def build_parser():
     parser = SVArgumentParser(
         description='Start SnakeViz to view a Python profile.')
 
     parser.add_argument('filename', help='Python profile to view')
 
     parser.add_argument('-v', '--version', action='version',
-                        version=('%(prog)s ' + version.version))
+                        version=('%(prog)s ' + VERSION))
 
     parser.add_argument('-H', '--hostname', metavar='ADDR', default='127.0.0.1',
                         help='hostname to bind to (default: %(default)s)')
 
     parser.add_argument('-p', '--port', type=int, metavar='PORT', default=8080,
                         help='port to bind to; if this port is already in use a '
                              'free port will be selected automatically '
```

### Comparing `snakeviz-2.1.2/snakeviz/ipymagic.py` & `snakeviz-2.2.0/snakeviz/ipymagic.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,30 +13,36 @@
     from urllib import quote
 
 __all__ = ["load_ipython_extension"]
 
 
 JUPYTER_HTML_TEMPLATE = """
 <iframe id='snakeviz-{uuid}' frameborder=0 seamless width='100%' height='1000'></iframe>
-<script>document.getElementById("snakeviz-{uuid}").setAttribute("src", "http://" + document.location.hostname + ":{port}{path}")</script>
+<script>document.getElementById("snakeviz-{uuid}").setAttribute("src", "http://{host}:{port}{path}")</script>
 """
-
+DEFAULT_HOST = "\" + document.location.hostname + \""
 
 # Users may be using snakeviz in an environment where IPython is not
 # installed, this try/except makes sure that snakeviz is operational
 # in that case.
 try:
-    from IPython.core.magic import Magics, magics_class, line_cell_magic
+    from IPython.core.magic import Magics, magics_class, line_cell_magic, line_magic
     from IPython.display import display, HTML
 except ImportError:
     pass
 else:
 
     @magics_class
     class SnakevizMagic(Magics):
+
+        def __init__(self, shell=None, **kwargs):
+            super().__init__(shell=shell, **kwargs)
+            self._host = None
+            self._port = None
+
         @line_cell_magic
         def snakeviz(self, line, cell=None):
             """
             Profile code and display the profile in Snakeviz.
             Works as a line or cell magic.
 
             Usage, in line mode:
@@ -76,24 +82,51 @@
                 ip.run_cell_magic("prun", line, cell)
             else:
                 ip.run_line_magic("prun", line)
 
             # start up a Snakeviz server
             if _check_ipynb() and not ("t" in opts or "new-tab" in opts):
                 print("Embedding SnakeViz in this document...")
-                sv = open_snakeviz_and_display_in_notebook(filename)
+                sv = open_snakeviz_and_display_in_notebook(filename, self._host, self._port)
             else:
                 print("Opening SnakeViz in a new tab...")
                 sv = subprocess.Popen(
                     [sys.executable, "-m", "snakeviz", filename]
                 )
             # give time for the Snakeviz page to load then shut down the server
             time.sleep(3)
             sv.terminate()
 
+        @line_magic
+        def snakeviz_config(self, line):
+            """
+            Configure the port and host name for snakeviz.
+
+            This line magic takes two options, -h or -p (or alternatively the
+            long forms --host and --post) for configuring the host and port,
+            respectively, of the snakeviz server that is spun up when the
+            snakeviz magic is called.
+
+            The host is the url that will be used by the browser to connect
+            to the server, and the port is the port used by the server and
+            which will be supplied by the browser when it connects to the
+            server.
+            """
+            opts, line = self.parse_options(line, "h:p:", "host=", "port=")
+            for opt in opts:
+                if opt in ("h", "host"):
+                    self._host = opts[opt]
+                elif opt in ("p", "port"):
+                    self._port = opts[opt]
+                else:
+                    raise ValueError("Unsupported option {opt}.".format(opt))
+            host = self._host or DEFAULT_HOST
+            port = self._port or "dynamically chosen"
+            print("Snakeviz configured with host {host} and port {port}".format(host=host,
+                                                                                port=port))
 
 def load_ipython_extension(ipython):
     """Called when user runs %load_ext snakeviz"""
     ipython.register_magics(SnakevizMagic)
 
 
 def _check_ipynb():
@@ -102,15 +135,15 @@
     Jupyter Notebook.
 
     """
     cfg = get_ipython().config
     return "connection_file" in cfg["IPKernelApp"]
 
 
-def open_snakeviz_and_display_in_notebook(filename):
+def open_snakeviz_and_display_in_notebook(filename, override_host=None, override_port=None):
     def _find_free_port():
         import socket
         from contextlib import closing
 
         with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
             # snakeviz frequently gets called many times in a short period.
             # This line tells the kernel it's okay to reuse TIME-WAIT sockets,
@@ -127,15 +160,15 @@
                     if e.errno == errno.EADDRINUSE:
                         pass
                     else:
                         raise
                 else:
                     return s.getsockname()[1]
 
-    port = str(_find_free_port())
+    port = override_port or str(_find_free_port())
 
     def _start_and_wait_when_ready():
         import os
 
         environ = os.environ.copy()
         environ["PYTHONUNBUFFERED"] = "TRUE"
         sv = subprocess.Popen(
@@ -158,15 +191,17 @@
             line = sv.stdout.readline()
             if line.strip().startswith("snakeviz web server started"):
                 break
         return sv
 
     sv = _start_and_wait_when_ready()
     path = "/snakeviz/%s" % quote(filename, safe="")
+    host = override_host or DEFAULT_HOST
+    print(display)
     display(
         HTML(
             JUPYTER_HTML_TEMPLATE.format(
-                port=port, path=path, uuid=uuid.uuid1()
+                port=port, path=path, uuid=uuid.uuid1(), host=host
             )
         )
     )
     return sv
```

### Comparing `snakeviz-2.1.2/snakeviz/main.py` & `snakeviz-2.2.0/snakeviz/main.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/drawsvg.js` & `snakeviz-2.2.0/snakeviz/static/drawsvg.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/favicon.ico` & `snakeviz-2.2.0/snakeviz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/images/sort_asc.png` & `snakeviz-2.2.0/snakeviz/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/images/sort_both.png` & `snakeviz-2.2.0/snakeviz/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/images/sort_desc.png` & `snakeviz-2.2.0/snakeviz/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/snakeviz.css` & `snakeviz-2.2.0/snakeviz/static/snakeviz.css`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/snakeviz.js` & `snakeviz-2.2.0/snakeviz/static/snakeviz.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/d3.v3.min.js` & `snakeviz-2.2.0/snakeviz/static/vendor/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/immutable.min.js` & `snakeviz-2.2.0/snakeviz/static/vendor/immutable.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/jquery-3.2.1.min.js` & `snakeviz-2.2.0/snakeviz/static/vendor/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.css` & `snakeviz-2.2.0/snakeviz/static/vendor/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/jquery.dataTables.min.js` & `snakeviz-2.2.0/snakeviz/static/vendor/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/static/vendor/lodash.min.js` & `snakeviz-2.2.0/snakeviz/static/vendor/lodash.min.js`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/stats.py` & `snakeviz-2.2.0/snakeviz/stats.py`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/templates/dir.html` & `snakeviz-2.2.0/snakeviz/templates/dir.html`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz/templates/viz.html` & `snakeviz-2.2.0/snakeviz/templates/viz.html`

 * *Files identical despite different names*

### Comparing `snakeviz-2.1.2/snakeviz.egg-info/SOURCES.txt` & `snakeviz-2.2.0/snakeviz.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 CHANGES.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
 snakeviz/__init__.py
 snakeviz/__main__.py
 snakeviz/cli.py
 snakeviz/ipymagic.py
 snakeviz/main.py
 snakeviz/stats.py
-snakeviz/version.py
 snakeviz.egg-info/PKG-INFO
 snakeviz.egg-info/SOURCES.txt
 snakeviz.egg-info/dependency_links.txt
 snakeviz.egg-info/entry_points.txt
 snakeviz.egg-info/requires.txt
 snakeviz.egg-info/top_level.txt
 snakeviz/static/drawsvg.js
@@ -28,8 +27,9 @@
 snakeviz/static/vendor/immutable.min.js
 snakeviz/static/vendor/jquery-3.2.1.min.js
 snakeviz/static/vendor/jquery.dataTables.min.css
 snakeviz/static/vendor/jquery.dataTables.min.js
 snakeviz/static/vendor/lodash.min.js
 snakeviz/templates/dir.html
 snakeviz/templates/viz.html
+tests/test_ipymagic.py
 tests/test_snakeviz.py
```

### Comparing `snakeviz-2.1.2/tests/test_snakeviz.py` & `snakeviz-2.2.0/tests/test_snakeviz.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from urllib.parse import quote
 except ImportError:
     from urllib import quote
 
 import pytest
 import requests
 
-from snakeviz import version
+from snakeviz import VERSION
 
 
 @contextmanager
 def snakeviz(fname, port=None):
     if port:
         args = 'snakeviz -s --port {0}'.format(port)
     else:
@@ -83,9 +83,9 @@
 
 
 def test_version():
     vcall = sp.Popen(
         ['snakeviz', '--version'], stdout=sp.PIPE, stderr=sp.PIPE)
     out, err = vcall.communicate()
     # in Python <= 3.3 this comes out on stderr, otherwise on stdout
-    assert version.version in out.decode('utf-8') or \
-        version.version in err.decode('utf-8')
+    assert VERSION in out.decode('utf-8') or \
+        VERSION in err.decode('utf-8')
```


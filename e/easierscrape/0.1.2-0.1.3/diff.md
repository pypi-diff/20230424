# Comparing `tmp/easierscrape-0.1.2.tar.gz` & `tmp/easierscrape-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierscrape-0.1.2.tar", last modified: Wed Apr  5 18:16:25 2023, max compression
+gzip compressed data, was "easierscrape-0.1.3.tar", last modified: Mon Apr 24 14:39:39 2023, max compression
```

## Comparing `easierscrape-0.1.2.tar` & `easierscrape-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.423155 easierscrape-0.1.2/
--rw-rw-rw-   0        0        0      550 2023-04-05 18:09:35.000000 easierscrape-0.1.2/.bumpversion.cfg
--rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.1.2/.readthedocs.yml
--rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.1.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2745 2023-04-05 17:40:22.000000 easierscrape-0.1.2/Makefile
--rw-rw-rw-   0        0        0    18082 2023-04-05 18:16:25.423155 easierscrape-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4050 2023-04-05 17:40:22.000000 easierscrape-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.390636 easierscrape-0.1.2/docs/
--rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0     1098 2023-04-05 18:09:35.000000 easierscrape-0.1.2/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.395496 easierscrape-0.1.2/docs/images/
--rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.1.2/docs/images/cli_recording.gif
--rw-rw-rw-   0        0        0   158783 2023-04-05 17:40:22.000000 easierscrape-0.1.2/docs/images/demo_recording.gif
--rw-rw-rw-   0        0        0     2342 2023-04-05 17:40:22.000000 easierscrape-0.1.2/docs/index.md
--rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0      109 2023-04-05 18:09:35.000000 easierscrape-0.1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.400374 easierscrape-0.1.2/docs/source/
--rw-rw-rw-   0        0        0      195 2023-04-05 17:40:22.000000 easierscrape-0.1.2/docs/source/easierscrape.rst
--rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.1.2/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.407936 easierscrape-0.1.2/easierscrape/
--rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.1.2/easierscrape/__init__.py
--rw-rw-rw-   0        0        0      669 2023-04-05 17:40:22.000000 easierscrape-0.1.2/easierscrape/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-05 18:09:35.000000 easierscrape-0.1.2/easierscrape/_version.py
--rw-rw-rw-   0        0        0     7654 2023-04-05 17:40:22.000000 easierscrape-0.1.2/easierscrape/easierscrape.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.420380 easierscrape-0.1.2/easierscrape/tests/
--rw-rw-rw-   0        0        0     4866 2023-04-05 17:40:22.000000 easierscrape-0.1.2/easierscrape/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:16:25.418428 easierscrape-0.1.2/easierscrape.egg-info/
--rw-rw-rw-   0        0        0    18082 2023-04-05 18:16:25.000000 easierscrape-0.1.2/easierscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-04-05 18:16:25.000000 easierscrape-0.1.2/easierscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 18:16:25.000000 easierscrape-0.1.2/easierscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2023-04-05 18:16:25.000000 easierscrape-0.1.2/easierscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 18:16:25.000000 easierscrape-0.1.2/easierscrape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2434 2023-04-05 18:09:35.000000 easierscrape-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 18:16:25.424212 easierscrape-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:39.000491 easierscrape-0.1.3/
+-rw-rw-rw-   0        0        0      550 2023-04-24 14:34:54.000000 easierscrape-0.1.3/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.1.3/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.1.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.1.3/Makefile
+-rw-rw-rw-   0        0        0    18297 2023-04-24 14:39:38.999419 easierscrape-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4265 2023-04-19 16:51:19.000000 easierscrape-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.948028 easierscrape-0.1.3/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.1.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.911862 easierscrape-0.1.3/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.913993 easierscrape-0.1.3/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.953859 easierscrape-0.1.3/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/_build/html/_images/cli_recording.gif
+-rw-rw-rw-   0        0        0   158783 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/_build/html/_images/demo_recording.gif
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.956942 easierscrape-0.1.3/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     2386 2023-04-23 18:18:13.000000 easierscrape-0.1.3/docs/_build/html/_sources/index.md.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.960484 easierscrape-0.1.3/docs/_build/html/_sources/source/
+-rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.1.3/docs/_build/html/_sources/source/easierscrape.rst.txt
+-rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.1.3/docs/_build/html/_sources/source/modules.rst.txt
+-rw-rw-rw-   0        0        0     1098 2023-04-24 14:34:54.000000 easierscrape-0.1.3/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.966377 easierscrape-0.1.3/docs/images/
+-rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/images/cli_recording.gif
+-rw-rw-rw-   0        0        0   158783 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/images/demo_recording.gif
+-rw-rw-rw-   0        0        0     2386 2023-04-24 13:49:29.000000 easierscrape-0.1.3/docs/index.md
+-rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0      109 2023-04-24 14:34:54.000000 easierscrape-0.1.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.972614 easierscrape-0.1.3/docs/source/
+-rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.1.3/docs/source/easierscrape.rst
+-rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.1.3/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.985129 easierscrape-0.1.3/easierscrape/
+-rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.1.3/easierscrape/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-04-24 13:49:29.000000 easierscrape-0.1.3/easierscrape/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-24 14:34:54.000000 easierscrape-0.1.3/easierscrape/_version.py
+-rw-rw-rw-   0        0        0     8420 2023-04-24 14:03:25.000000 easierscrape-0.1.3/easierscrape/easierscrape.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.998034 easierscrape-0.1.3/easierscrape/tests/
+-rw-rw-rw-   0        0        0    11335 2023-04-24 14:03:25.000000 easierscrape-0.1.3/easierscrape/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.992878 easierscrape-0.1.3/easierscrape.egg-info/
+-rw-rw-rw-   0        0        0    18297 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2434 2023-04-24 14:34:54.000000 easierscrape-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:39:39.000491 easierscrape-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.1.3/setup.py
```

### Comparing `easierscrape-0.1.2/.bumpversion.cfg` & `easierscrape-0.1.3/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.1.3
 commit = True
 tag = True
 
 [bumpversion:file:easierscrape/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `easierscrape-0.1.2/CONTRIBUTING.md` & `easierscrape-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/LICENSE` & `easierscrape-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/MANIFEST.in` & `easierscrape-0.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/Makefile` & `easierscrape-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/PKG-INFO` & `easierscrape-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -258,25 +258,25 @@
 ```
 
 Usage examples:
 ```
 >>> scraper.parse_text("https://quotes.toscrape.com/login")
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
@@ -295,9 +295,17 @@
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
+
+## Contributing
+
+See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+
+## License
+
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
```

### Comparing `easierscrape-0.1.2/README.md` & `easierscrape-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -36,25 +36,25 @@
 ```
 
 Usage examples:
 ```
 >>> scraper.parse_text("https://quotes.toscrape.com/login")
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
@@ -73,9 +73,17 @@
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
+
+## Contributing
+
+See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+
+## License
+
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
```

### Comparing `easierscrape-0.1.2/docs/Makefile` & `easierscrape-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/docs/conf.py` & `easierscrape-0.1.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Path setup --------------------------------------------------------------
 sys.path.insert(0, os.path.abspath('../'))
 
 # -- Project information -----------------------------------------------------
 project = 'easierscrape'
 copyright = '2023, Daniel Greco'
 author = 'Daniel Greco'
-release = '0.1.2'
+release = '0.1.3'
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
 source_suffix = ['.rst', '.md']
```

### Comparing `easierscrape-0.1.2/docs/images/cli_recording.gif` & `easierscrape-0.1.3/docs/_build/html/_images/cli_recording.gif`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/docs/images/demo_recording.gif` & `easierscrape-0.1.3/docs/_build/html/_images/demo_recording.gif`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/docs/index.md` & `easierscrape-0.1.3/docs/_build/html/_sources/index.md.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 ```
 
 Usage examples:
 ```
 >>> scraper.parse_text("https://quotes.toscrape.com/login")
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random"
 ```
 
 ### Downloads
-Using `parse_files`, `parse_images`, or `parse_tables` will result in an "easierscrape_downloads" directory being created in the working directory.
+Using `get_screenshot`, `parse_files`, `parse_images`, or `parse_tables` will result in an "easierscrape_downloads" directory being created in the working directory.
 
 Usage example:
 ```eval_rst
 .. image:: images/demo_recording.gif
 ```
 
 ## Command Line Usage
-When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
+When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
 positional arguments:
   url         the url to scrape
   depth       the depth of the scrape tree
```

### Comparing `easierscrape-0.1.2/docs/make.bat` & `easierscrape-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.2/easierscrape/__main__.py` & `easierscrape-0.1.3/easierscrape/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     parser = ArgumentParser()
     parser.add_argument('url', help='the url to scrape')
     parser.add_argument('depth', type=int, help='the depth of the scrape tree')
     args = parser.parse_args(arg_strings)
 
     scraper = Scraper()
     scraper.print_tree(scraper.tree_gen(args.url, args.depth))
+    screenshot_size = scraper.get_screenshot(args.url)
     image_count = scraper.parse_images(args.url)
     file_counts = scraper.parse_files(args.url, ['txt', 'pdf'])
     table_count = scraper.parse_tables(args.url)
 
-    return image_count, file_counts, table_count
+    return screenshot_size, image_count, file_counts, table_count
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `easierscrape-0.1.2/easierscrape/easierscrape.py` & `easierscrape-0.1.3/easierscrape/easierscrape.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from bs4 import BeautifulSoup
 from os import getcwd, makedirs
 from os.path import basename, exists, join
 from pandas import read_html
 from re import compile
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
 from urllib.parse import urlparse
-from urllib.request import urlcleanup, urlretrieve, url2pathname
+from urllib.request import urlopen, url2pathname
 from uuid import uuid4
 
 
 class Scraper:
     def __init__(self):
         # hide GUI
         options = Options()
@@ -48,24 +49,43 @@
     def _tree_gen_rec(self, url, maxdepth, tree, depth):
         if tree is None:
             url = url.replace("www.", "")
             if url.endswith("/"):
                 url = url[:-1]
             tree = Node(url, url=url)
         if depth < maxdepth:
+            parent_node = tree
             for a in self.parse_anchors(url):
                 try:
                     child_url = self._concat_urls(url, a.attrs["href"].replace("www.", ""))
                     if find(tree.root, lambda node: node.url == child_url) is None:
-                        new_leaf = Node(child_url, url=child_url, parent=tree)
-                        tree = self.tree_gen(child_url, maxdepth, new_leaf, depth + 1)
+                        new_leaf = Node(child_url, url=child_url, parent=parent_node)
+                        tree = self._tree_gen_rec(child_url, maxdepth, new_leaf, depth + 1)
                 except Exception:
                     pass
         return tree.root
 
+    def get_screenshot(self, url):
+        """Downloads screenshot from provided url to an "easierscrape_downloads"
+        folder in the current working directory
+
+        Args:
+            url (str): The url to screenshot
+
+        Returns:
+            bool: True
+
+        """
+        download_file = join(self._get_download_dir("images", url), "easierscrape_screenshot.png")
+
+        self.driver.get(url)
+        self.driver.find_element(By.TAG_NAME, 'body').screenshot(download_file)
+
+        return True  # getsize(download_file)
+
     def parse_anchors(self, url):
         """Parses a list of anchor tags from provided url.
 
         Args:
             url (str): The url to scrape from
 
         Returns:
@@ -93,16 +113,17 @@
             return
         file_download_list = []
         for filetype in filetypes:
             file_download_count = 0
             for file in self._soup_url(url).find_all("a", href=compile(r"(." + filetype + ")")):
                 try:
                     fileUrl = self._concat_urls(url, file.attrs["href"])
-                    urlretrieve(fileUrl, join(self._get_download_dir(filetype, url), basename(fileUrl)))
-                    urlcleanup()
+                    response = urlopen(fileUrl)
+                    with open(join(self._get_download_dir(filetype, url), basename(fileUrl)), "wb") as file:
+                        file.write(response.read())
                     file_download_count += 1
                 except Exception:
                     pass
             file_download_list.append(file_download_count)
         return file_download_list
 
     def parse_images(self, url):
@@ -116,16 +137,17 @@
             int: Number of images downloaded from url
 
         """
         image_download_count = 0
         for image in self._soup_url(url).findAll("img"):
             try:
                 imageUrl = self._concat_urls(url, image.attrs["src"])
-                urlretrieve(imageUrl, join(self._get_download_dir("images", url), basename(imageUrl)))
-                urlcleanup()
+                response = urlopen(imageUrl)
+                with open(join(self._get_download_dir("images", url), basename(imageUrl)), "wb") as file:
+                    file.write(response.read())
                 image_download_count += 1
             except Exception:
                 pass
         return image_download_count
 
     def parse_lists(self, url):
         """Parses a list of lists from provided url.
```

### Comparing `easierscrape-0.1.2/easierscrape.egg-info/PKG-INFO` & `easierscrape-0.1.3/easierscrape.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -258,25 +258,25 @@
 ```
 
 Usage examples:
 ```
 >>> scraper.parse_text("https://quotes.toscrape.com/login")
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
@@ -295,9 +295,17 @@
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
+
+## Contributing
+
+See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+
+## License
+
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
```

### Comparing `easierscrape-0.1.2/easierscrape.egg-info/SOURCES.txt` & `easierscrape-0.1.3/easierscrape.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 pyproject.toml
 setup.py
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/requirements.txt
+docs/_build/html/_images/cli_recording.gif
+docs/_build/html/_images/demo_recording.gif
+docs/_build/html/_sources/index.md.txt
+docs/_build/html/_sources/source/easierscrape.rst.txt
+docs/_build/html/_sources/source/modules.rst.txt
 docs/images/cli_recording.gif
 docs/images/demo_recording.gif
 docs/source/easierscrape.rst
 docs/source/modules.rst
 easierscrape/__init__.py
 easierscrape/__main__.py
 easierscrape/_version.py
```

### Comparing `easierscrape-0.1.2/pyproject.toml` & `easierscrape-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "easierscrape"
 authors = [{name = "Daniel Greco", email = "dag2226@columbia.edu"}]
 description="A library which does some basic web scraping operations"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.7"
 
 dependencies = [
     "anytree",
     "beautifulsoup4",
     "html5lib",
     "lxml",
```


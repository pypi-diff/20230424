# Comparing `tmp/cagen-0.2.0a7.tar.gz` & `tmp/cagen-0.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a7.tar", last modified: Mon Apr 17 08:52:05 2023, max compression
+gzip compressed data, was "cagen-0.2.0a8.tar", last modified: Mon Apr 24 07:43:26 2023, max compression
```

## Comparing `cagen-0.2.0a7.tar` & `cagen-0.2.0a8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a7/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:52:05.616749 cagen-0.2.0a7/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a7/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-17 08:51:52.000000 cagen-0.2.0a7/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-17 08:52:05.616749 cagen-0.2.0a7/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a7/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:18:58.000000 cagen-0.2.0a7/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8236 2023-04-17 08:48:25.000000 cagen-0.2.0a7/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a7/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a7/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a7/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a7/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-17 08:52:05.616749 cagen-0.2.0a7/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-17 08:52:05.000000 cagen-0.2.0a7/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a8/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:43:26.541017 cagen-0.2.0a8/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3465 2023-04-17 09:01:49.000000 cagen-0.2.0a8/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-17 09:02:06.000000 cagen-0.2.0a8/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-24 07:43:26.541017 cagen-0.2.0a8/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.537684 cagen-0.2.0a8/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.537684 cagen-0.2.0a8/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a8/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:18:58.000000 cagen-0.2.0a8/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8539 2023-04-24 07:42:52.000000 cagen-0.2.0a8/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0a8/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a8/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0a8/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a8/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a7/PKG-INFO` & `cagen-0.2.0a8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a7
+Version: 0.2.0a8
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -39,28 +39,28 @@
 
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](src/cagen/libcagen.py)
-- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
+- a [library](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/libcagen.py)
+- a [command line program](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
 ```
 pip install cagen
 ```
 
-If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
 cagen sourcefile.md generatedfile.html template.tmpl
 ```
@@ -83,14 +83,14 @@
 make
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
-- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- You can see the [list of tasks](https://repo.or.cz/cagen.git/tree/HEAD:/tasks) (completed and pending).
 - The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```

### Comparing `cagen-0.2.0a7/README.md` & `cagen-0.2.0a8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](src/cagen/libcagen.py)
-- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
+- a [library](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/libcagen.py)
+- a [command line program](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
 ```
 pip install cagen
 ```
 
-If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
 cagen sourcefile.md generatedfile.html template.tmpl
 ```
@@ -64,14 +64,14 @@
 make
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
-- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- You can see the [list of tasks](https://repo.or.cz/cagen.git/tree/HEAD:/tasks) (completed and pending).
 - The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```

### Comparing `cagen-0.2.0a7/pyproject.toml` & `cagen-0.2.0a8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-7"
+version = "0.2.0.alpha-8"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0a7/src/cagen/cmd.py` & `cagen-0.2.0a8/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a7/src/cagen/libcagen.py` & `cagen-0.2.0a8/src/cagen/libcagen.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,19 @@
     ---
     content
     ```
 
     This class uses extensively the [frontmatter library](https://python-frontmatter.readthedocs.io/en/latest/) for read and write metadata easyly.
     """
 
-    path: str
-    """The path of the entry, i.e. the path of the markdown file we want to process."""
+    path: Optional[str]
+    """
+    The path of the entry, i.e. the path of the markdown file we want to process.
+    If the path is None, then only processing fields are the provided by `additionalsearchlist` in `to` method.
+    """
 
     def __init__(self, path: str):
         """Defines the `Entry` from `path`"""
         self.path = path
 
     @property
     def content(self) -> str:
@@ -86,28 +89,32 @@
     def pandoc_convert(self, destsyntax: str = 'html5', removingheaders: bool = True) -> str:
         """
         Simply uses [pandoc](https://pandoc.org/) to convert `Entry` to `destsyntax` syntax.
         
         - If `removingheaders == True`, we remove all headers except the bibliography information from YAML metadata
         - If `removingheaders == False`, we convert the whole file.
         """
-        post = frontmatter.load(self.path)
-        
-        if removingheaders == True:
-            # Remove all headers in YAML frontend except bibliographic ones
-            keys = sorted(post.keys())
-
-            for k in keys:
-                if k != 'references':
-                    post.__delitem__(k)
-
-        # This is the original markdown file
-        #   - with all keys in metadata removed except references; in case of removingheaders == True
-        #   - with no changes; in case of removingheaders == False
-        markdown = frontmatter.dumps(post)
+
+        if self.path != None:
+            post = frontmatter.load(self.path)
+
+            if removingheaders == True:
+                # Remove all headers in YAML frontend except bibliographic ones
+                keys = sorted(post.keys())
+
+                for k in keys:
+                    if k != 'references':
+                        post.__delitem__(k)
+            
+            # This is the original markdown file
+            #   - with all keys in metadata removed except references; in case of removingheaders == True
+            #   - with no changes; in case of removingheaders == False
+            markdown = frontmatter.dumps(post)
+        else:
+            markdown = ""
 
         # calling pandoc with options
         extra_args = ["--citeproc", "--katex", "--metadata=link-citations:true"]
         return pypandoc.convert_text(markdown, to=destsyntax, format="markdown+smart+ascii_identifiers+citations+strikeout", extra_args=extra_args)
 
     def to(self, mytemplatepath: str,  additionalsearchlist: dict = {}, destsyntax: str = 'html5') -> str:
         """
@@ -148,14 +155,16 @@
 
     def values(self, criterium: types.FunctionType):
         """
         Returns the values of criterium(x) for all x in `self.entries`.
 
         - When criterium(x)=y is not a list, we add y to `values`
         - When criterium(x)=y is a list, we add z to `values` for every z in y.
+
+        It is mainly related to `group_by` method.
         """
 
         # Compute the values
         vals = []
         for v in [criterium(e) for e in self.entries]:
             if isinstance(v, list):
                 for element in v:
```

### Comparing `cagen-0.2.0a7/src/cagen/templates/schema.tmpl` & `cagen-0.2.0a8/src/cagen/templates/schema.tmpl`

 * *Files 10% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 	}}});
   	</script>
 	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.15.1/dist/katex.min.css" />
 	<!-- end: math stuff -->
     </head>
     <body>
 	<header>
-	% if navbar and isinstance(navbar, list):
+	% if navbar is not UNDEFINED and isinstance(navbar, list):
 	<nav id="menu">
 	% for t in navbar:
 	% if isinstance(t, dict):
 	% if 'title' in t.keys () and 'url' in t.keys():
 	<a class="pinned" href="${t['url']}">${t['title']}</a>
 	% endif
 	% endif
 	% endfor
 	</nav>
 	% endif
 	</header>
         ${conversion}
     </body>
     <footer>
-           <p>Generated by <a href="https://sr.ht/~somenxavierb/cagen/">cagen</a>
-           % if sourcefile:
+           <p>Generated by <a href="https://repo.or.cz/cagen.git">cagen</a>
+           % if sourcefile is not UNDEFINED:
            from <a href="${sourcefile}">original markdown file</a>
            <%!
 		import datetime
 	   %>
            % endif
            on <time datetime="${datetime.datetime.now().isoformat()}">${datetime.datetime.now().strftime("%c")}</time>
            .</p>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 % if title:
 % endif
 
 
- % if navbar and isinstance(navbar, list):  % for t in navbar: % if isinstance
-(t, dict): % if 'title' in t.keys () and 'url' in t.keys(): ${t['title']} %
-endif % endif % endfor  % endif  ${conversion}
-Generated by cagen % if sourcefile: from original_markdown_file <%! import
-datetime %> % endif on ${datetime.datetime.now().strftime("%c")} .
+ % if navbar is not UNDEFINED and isinstance(navbar, list):  % for t in navbar:
+% if isinstance(t, dict): % if 'title' in t.keys () and 'url' in t.keys(): ${t
+['title']} % endif % endif % endfor  % endif  ${conversion}
+Generated by cagen % if sourcefile is not UNDEFINED: from original_markdown
+file <%! import datetime %> % endif on ${datetime.datetime.now().strftime
+("%c")} .
```

### Comparing `cagen-0.2.0a7/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a8/src/cagen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a7
+Version: 0.2.0a8
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -39,28 +39,28 @@
 
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
-- a [library](src/cagen/libcagen.py)
-- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
+- a [library](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/libcagen.py)
+- a [command line program](https://repo.or.cz/cagen.git/blob/HEAD:/src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
 ```
 pip install cagen
 ```
 
-If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](extras/PKGBUILD) to make a pacman package.
+If you are running ArchLinux or any Arch derivative distribution, you can use this [PKGBUILD](https://repo.or.cz/cagen.git/blob/HEAD:/extras/PKGBUILD) to make a pacman package.
 
 ## Usage
 
 Basic use is:
 ```
 cagen sourcefile.md generatedfile.html template.tmpl
 ```
@@ -83,14 +83,14 @@
 make
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
-- You can see the [list of tasks](tasks/index.md) (completed and pending).
+- You can see the [list of tasks](https://repo.or.cz/cagen.git/tree/HEAD:/tasks) (completed and pending).
 - The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```


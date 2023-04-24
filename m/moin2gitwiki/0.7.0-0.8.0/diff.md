# Comparing `tmp/moin2gitwiki-0.7.0.tar.gz` & `tmp/moin2gitwiki-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moin2gitwiki-0.7.0.tar", max compression
+gzip compressed data, was "moin2gitwiki-0.8.0.tar", max compression
```

## Comparing `moin2gitwiki-0.7.0.tar` & `moin2gitwiki-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1504 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     3669 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/README.md
--rw-r--r--   0        0        0       17 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/changelog.md
--rw-r--r--   0        0        0      203 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/commands.md
--rw-r--r--   0        0        0      689 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0       14 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/index.md
--rw-r--r--   0        0        0       55 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/cli.md
--rw-r--r--   0        0        0       25 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/context.md
--rw-r--r--   0        0        0       29 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/fetch_cache.md
--rw-r--r--   0        0        0       29 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/gitrevision.md
--rw-r--r--   0        0        0       31 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/moin2markdown.md
--rw-r--r--   0        0        0       23 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/users.md
--rw-r--r--   0        0        0       27 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/docs/internal/wikiindex.md
--rw-r--r--   0        0        0      139 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/__init__.py
--rw-r--r--   0        0        0     9113 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/cli.py
--rw-r--r--   0        0        0     4851 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/context.py
--rw-r--r--   0        0        0     4099 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/fetch_cache.py
--rw-r--r--   0        0        0     5227 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/gitrevision.py
--rw-r--r--   0        0        0     9193 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/moin2markdown.py
--rw-r--r--   0        0        0     4781 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/users.py
--rw-r--r--   0        0        0     9947 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/moin2gitwiki/wikiindex.py
--rw-r--r--   0        0        0     1035 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1203 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/tests/test_command_line.py
--rw-r--r--   0        0        0       93 2022-11-21 17:31:08.646814 moin2gitwiki-0.7.0/tests/test_version.py
--rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 moin2gitwiki-0.7.0/setup.py
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 moin2gitwiki-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1546 2023-04-24 08:22:41.623052 moin2gitwiki-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-04-24 08:00:34.490929 moin2gitwiki-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     3815 2023-04-24 08:22:41.623554 moin2gitwiki-0.8.0/README.md
+-rw-r--r--   0        0        0       17 2020-12-28 17:17:13.469550 moin2gitwiki-0.8.0/docs/changelog.md
+-rw-r--r--   0        0        0      203 2021-01-02 16:25:04.263235 moin2gitwiki-0.8.0/docs/commands.md
+-rw-r--r--   0        0        0      689 2021-01-04 17:59:05.973461 moin2gitwiki-0.8.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0       14 2020-12-28 17:17:13.470739 moin2gitwiki-0.8.0/docs/index.md
+-rw-r--r--   0        0        0       55 2021-01-04 18:04:01.406421 moin2gitwiki-0.8.0/docs/internal/cli.md
+-rw-r--r--   0        0        0       25 2021-01-04 17:55:32.649671 moin2gitwiki-0.8.0/docs/internal/context.md
+-rw-r--r--   0        0        0       29 2021-01-04 17:55:32.652659 moin2gitwiki-0.8.0/docs/internal/fetch_cache.md
+-rw-r--r--   0        0        0       29 2021-01-04 17:55:32.655060 moin2gitwiki-0.8.0/docs/internal/gitrevision.md
+-rw-r--r--   0        0        0       31 2021-01-04 17:55:32.657475 moin2gitwiki-0.8.0/docs/internal/moin2markdown.md
+-rw-r--r--   0        0        0       23 2021-01-04 17:55:32.660204 moin2gitwiki-0.8.0/docs/internal/users.md
+-rw-r--r--   0        0        0       27 2021-01-04 17:55:32.662570 moin2gitwiki-0.8.0/docs/internal/wikiindex.md
+-rw-r--r--   0        0        0      139 2023-04-24 08:22:41.622335 moin2gitwiki-0.8.0/moin2gitwiki/__init__.py
+-rw-r--r--   0        0        0     9113 2022-11-21 17:18:37.889072 moin2gitwiki-0.8.0/moin2gitwiki/cli.py
+-rw-r--r--   0        0        0     4850 2023-04-24 08:13:39.119818 moin2gitwiki-0.8.0/moin2gitwiki/context.py
+-rw-r--r--   0        0        0     4099 2022-11-21 17:18:17.774431 moin2gitwiki-0.8.0/moin2gitwiki/fetch_cache.py
+-rw-r--r--   0        0        0     5227 2021-02-01 16:43:36.779614 moin2gitwiki-0.8.0/moin2gitwiki/gitrevision.py
+-rw-r--r--   0        0        0     9193 2021-09-25 14:54:50.809126 moin2gitwiki-0.8.0/moin2gitwiki/moin2markdown.py
+-rw-r--r--   0        0        0     4781 2021-01-06 20:49:12.122542 moin2gitwiki-0.8.0/moin2gitwiki/users.py
+-rw-r--r--   0        0        0     9947 2021-09-25 14:35:33.412601 moin2gitwiki-0.8.0/moin2gitwiki/wikiindex.py
+-rw-r--r--   0        0        0     1051 2023-04-24 08:22:41.621966 moin2gitwiki-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-12-28 17:30:09.600038 moin2gitwiki-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1203 2020-12-28 17:31:15.008416 moin2gitwiki-0.8.0/tests/test_command_line.py
+-rw-r--r--   0        0        0       93 2023-04-24 08:22:41.622624 moin2gitwiki-0.8.0/tests/test_version.py
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 moin2gitwiki-0.8.0/setup.py
+-rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 moin2gitwiki-0.8.0/PKG-INFO
```

### Comparing `moin2gitwiki-0.7.0/CHANGELOG.md` & `moin2gitwiki-0.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 Unreleased Changes
 ------------------
 
 <!-- insertion marker -->
+[0.8.0] - 2023-04-24
+--------------------
 [0.7.0] - 2022-11-21
 --------------------
 - fix: remove hardwired proxy settings
 - fix: add recursion limit for beautiful soup
 - fix: updated pytest
 - fix: change startup to not require --moin-data for check
```

### Comparing `moin2gitwiki-0.7.0/README.md` & `moin2gitwiki-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 [![pypi version](https://img.shields.io/pypi/v/moin2gitwiki.svg)](https://pypi.python.org/pypi/moin2gitwiki)
 
 App to convert a MoinMoin wiki file tree into a git based wiki as used on
 github, gitlab or gitea.
 
 ## Current Version
 
-Version: `0.7.0`
+Version: `0.8.0`
+
+## Status
+
+This was required for a one-off conversion. I'm not doing any further work on it - if anyone wishes to take this over then please just ask.
 
 ## Translation Method
 
 Originally the intention was to translate purely by converting the MoinMoin
 markup to markdown markup - using the MoinMoin data retrieved from the
 filesystem.
 
 However, although it makes determining the overall page list and revision list
 much easier, it was found that translating the wiki markup at this level was
 too complex and fragile for this to work without a huge amount of special
 casing.
 
 So, after the revision structure is derived from the filesystem, each page
-revision is retrieved by http requests to the running MoinMoin wiki.  This is
+revision is retrieved by http requests to the running MoinMoin wiki. This is
 then reduced to just the page content (by picking out the content div from the
 html), and some light editing applied to simplify the HTML - specifically:-
 
 - Remove the anchor spans that MoinMoin adds - these add no visual or
   readable content, but confuse the translator
 - Remove paragraph entries with CSS classes that start `line` - these
   again appear to be for non-required purposes (likely for showing diffs
@@ -41,28 +45,28 @@
 This simplified HTML is then passed through the pandoc command:-
 
     pandoc -f html -t gfm
 
 And the resulting Github flavoured Markdown is taken as the new form.
 
 This handles the vast majority of normal markup correctly, including lists and
-many types of tables.  Some complicated markup or complex tables end up being
+many types of tables. Some complicated markup or complex tables end up being
 passed through as HTML - which displays correctly but is less easy to parse
 and edit.
 
 Attachments that are available in the wiki are also handled - they are put
 into a `_attachments` directory under a subdirectory named for the original
-page directory name.  Links to attachments should be handled correctly.
+page directory name. Links to attachments should be handled correctly.
 
 ## Issues
 
-The overall process is not particularly fast.  But this should be something
+The overall process is not particularly fast. But this should be something
 you only do once (or a few attempts) so raw speed is not needed.
 
-Attachments are not versioned by MoinMon.  This means any attachment that was
+Attachments are not versioned by MoinMon. This means any attachment that was
 deleted from MoinMoin is no longer available to put into the converted wiki.
 Any attachment that was updated a few times is only available in the last
 version (but will probably be inserted into the history at the point where it
 first appeared but with the latest content).
 
 ## Installation
 
@@ -85,8 +89,8 @@
 
     poetry run moin2gitwiki ...
 
 ## Todo
 
 - Make tests effective
 
-----
+---
```

### Comparing `moin2gitwiki-0.7.0/docs/css/mkdocstrings.css` & `moin2gitwiki-0.8.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/cli.py` & `moin2gitwiki-0.8.0/moin2gitwiki/cli.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/context.py` & `moin2gitwiki-0.8.0/moin2gitwiki/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if "user_map" in kwargs:
             user_map = kwargs["user_map"]
             del kwargs["user_map"]
 
         if moin_data:
             #
             # make the paths absolute
-            kwargs["_moin_data"] = Path(moin_data).resolve(strict=True)
+            kwargs["moin_data"] = Path(moin_data).resolve(strict=True)
             #
             # get the proxies
             proxies: Dict[str, str] = {}
             if "proxies" in kwargs:
                 for proxy_setting in kwargs["proxies"]:
                     key, value = proxy_setting.split("=", maxsplit=1)
                     proxies[key] = value
```

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/fetch_cache.py` & `moin2gitwiki-0.8.0/moin2gitwiki/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/gitrevision.py` & `moin2gitwiki-0.8.0/moin2gitwiki/gitrevision.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/moin2markdown.py` & `moin2gitwiki-0.8.0/moin2gitwiki/moin2markdown.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/users.py` & `moin2gitwiki-0.8.0/moin2gitwiki/users.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/moin2gitwiki/wikiindex.py` & `moin2gitwiki-0.8.0/moin2gitwiki/wikiindex.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/pyproject.toml` & `moin2gitwiki-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "moin2gitwiki"
-version = "0.7.0"
+version = "0.8.0"
 description = "MoinMoin To Git (Markdown) Wiki Converter"
 authors = ["Nigel Metheringham <nigelm@cpan.org>"]
 readme = "README.md"
+license = "MIT"
 homepage = "https://github.com/nigelm/moin2gitwiki"
 repository = "https://github.com/nigelm/moin2gitwiki"
 documentation = "https://nigelm.github.io/moin2gitwiki/"
 include = [
     "CHANGELOG.md",
     "README.md",
     "tests/*",
```

### Comparing `moin2gitwiki-0.7.0/tests/test_command_line.py` & `moin2gitwiki-0.8.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `moin2gitwiki-0.7.0/setup.py` & `moin2gitwiki-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'requests[socks]>=2.25.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['moin2gitwiki = moin2gitwiki.cli:moin2gitwiki']}
 
 setup_kwargs = {
     'name': 'moin2gitwiki',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'MoinMoin To Git (Markdown) Wiki Converter',
-    'long_description': '# MoinMoin To Git (Markdown) Wiki Converter\n\n[![ci](https://img.shields.io/travis/com/nigelm/moin2gitwiki.svg)](https://travis-ci.com/nigelm/moin2gitwiki)\n[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://nigelm.github.io/moin2gitwiki/)\n[![pypi version](https://img.shields.io/pypi/v/moin2gitwiki.svg)](https://pypi.python.org/pypi/moin2gitwiki)\n\nApp to convert a MoinMoin wiki file tree into a git based wiki as used on\ngithub, gitlab or gitea.\n\n## Current Version\n\nVersion: `0.7.0`\n\n## Translation Method\n\nOriginally the intention was to translate purely by converting the MoinMoin\nmarkup to markdown markup - using the MoinMoin data retrieved from the\nfilesystem.\n\nHowever, although it makes determining the overall page list and revision list\nmuch easier, it was found that translating the wiki markup at this level was\ntoo complex and fragile for this to work without a huge amount of special\ncasing.\n\nSo, after the revision structure is derived from the filesystem, each page\nrevision is retrieved by http requests to the running MoinMoin wiki.  This is\nthen reduced to just the page content (by picking out the content div from the\nhtml), and some light editing applied to simplify the HTML - specifically:-\n\n- Remove the anchor spans that MoinMoin adds - these add no visual or\n  readable content, but confuse the translator\n- Remove paragraph entries with CSS classes that start `line` - these\n  again appear to be for non-required purposes (likely for showing diffs\n  between revisions) - and they break the translator\n- Fix links that point within the wiki - if the target does not exist\n  then the text is left but the link removed.\n- Strips CSS classes off links - again these upset the translator\n- Translate any images that appear to be MoinMoin emoji characters (which\n  are rendered as images) into gollum emoji characters\n\nThis simplified HTML is then passed through the pandoc command:-\n\n    pandoc -f html -t gfm\n\nAnd the resulting Github flavoured Markdown is taken as the new form.\n\nThis handles the vast majority of normal markup correctly, including lists and\nmany types of tables.  Some complicated markup or complex tables end up being\npassed through as HTML - which displays correctly but is less easy to parse\nand edit.\n\nAttachments that are available in the wiki are also handled - they are put\ninto a `_attachments` directory under a subdirectory named for the original\npage directory name.  Links to attachments should be handled correctly.\n\n## Issues\n\nThe overall process is not particularly fast.  But this should be something\nyou only do once (or a few attempts) so raw speed is not needed.\n\nAttachments are not versioned by MoinMon.  This means any attachment that was\ndeleted from MoinMoin is no longer available to put into the converted wiki.\nAny attachment that was updated a few times is only available in the last\nversion (but will probably be inserted into the history at the point where it\nfirst appeared but with the latest content).\n\n## Installation\n\nI have now made this available as a pypi package, in which case it can be\ninstalled by running\n\n    pip install moin2gitwiki\n\nHowever to use it you will also need to install the `pandoc` and `git`\npackages as these commands are run during the conversion.\n\nHowever it can be installed from the repo - it uses\n[`poetry`](https://python-poetry.org/) to manage dependancies etc, so the best\nway to make use of this is to install [`poetry`](https://python-poetry.org/)\nfor your python version and then:-\n\n    poetry install\n\nthe command can then be run as\n\n    poetry run moin2gitwiki ...\n\n## Todo\n\n- Make tests effective\n\n----\n',
+    'long_description': "# MoinMoin To Git (Markdown) Wiki Converter\n\n[![ci](https://img.shields.io/travis/com/nigelm/moin2gitwiki.svg)](https://travis-ci.com/nigelm/moin2gitwiki)\n[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://nigelm.github.io/moin2gitwiki/)\n[![pypi version](https://img.shields.io/pypi/v/moin2gitwiki.svg)](https://pypi.python.org/pypi/moin2gitwiki)\n\nApp to convert a MoinMoin wiki file tree into a git based wiki as used on\ngithub, gitlab or gitea.\n\n## Current Version\n\nVersion: `0.8.0`\n\n## Status\n\nThis was required for a one-off conversion. I'm not doing any further work on it - if anyone wishes to take this over then please just ask.\n\n## Translation Method\n\nOriginally the intention was to translate purely by converting the MoinMoin\nmarkup to markdown markup - using the MoinMoin data retrieved from the\nfilesystem.\n\nHowever, although it makes determining the overall page list and revision list\nmuch easier, it was found that translating the wiki markup at this level was\ntoo complex and fragile for this to work without a huge amount of special\ncasing.\n\nSo, after the revision structure is derived from the filesystem, each page\nrevision is retrieved by http requests to the running MoinMoin wiki. This is\nthen reduced to just the page content (by picking out the content div from the\nhtml), and some light editing applied to simplify the HTML - specifically:-\n\n- Remove the anchor spans that MoinMoin adds - these add no visual or\n  readable content, but confuse the translator\n- Remove paragraph entries with CSS classes that start `line` - these\n  again appear to be for non-required purposes (likely for showing diffs\n  between revisions) - and they break the translator\n- Fix links that point within the wiki - if the target does not exist\n  then the text is left but the link removed.\n- Strips CSS classes off links - again these upset the translator\n- Translate any images that appear to be MoinMoin emoji characters (which\n  are rendered as images) into gollum emoji characters\n\nThis simplified HTML is then passed through the pandoc command:-\n\n    pandoc -f html -t gfm\n\nAnd the resulting Github flavoured Markdown is taken as the new form.\n\nThis handles the vast majority of normal markup correctly, including lists and\nmany types of tables. Some complicated markup or complex tables end up being\npassed through as HTML - which displays correctly but is less easy to parse\nand edit.\n\nAttachments that are available in the wiki are also handled - they are put\ninto a `_attachments` directory under a subdirectory named for the original\npage directory name. Links to attachments should be handled correctly.\n\n## Issues\n\nThe overall process is not particularly fast. But this should be something\nyou only do once (or a few attempts) so raw speed is not needed.\n\nAttachments are not versioned by MoinMon. This means any attachment that was\ndeleted from MoinMoin is no longer available to put into the converted wiki.\nAny attachment that was updated a few times is only available in the last\nversion (but will probably be inserted into the history at the point where it\nfirst appeared but with the latest content).\n\n## Installation\n\nI have now made this available as a pypi package, in which case it can be\ninstalled by running\n\n    pip install moin2gitwiki\n\nHowever to use it you will also need to install the `pandoc` and `git`\npackages as these commands are run during the conversion.\n\nHowever it can be installed from the repo - it uses\n[`poetry`](https://python-poetry.org/) to manage dependancies etc, so the best\nway to make use of this is to install [`poetry`](https://python-poetry.org/)\nfor your python version and then:-\n\n    poetry install\n\nthe command can then be run as\n\n    poetry run moin2gitwiki ...\n\n## Todo\n\n- Make tests effective\n\n---\n",
     'author': 'Nigel Metheringham',
     'author_email': 'nigelm@cpan.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nigelm/moin2gitwiki',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `moin2gitwiki-0.7.0/PKG-INFO` & `moin2gitwiki-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: moin2gitwiki
-Version: 0.7.0
+Version: 0.8.0
 Summary: MoinMoin To Git (Markdown) Wiki Converter
 Home-page: https://github.com/nigelm/moin2gitwiki
+License: MIT
 Author: Nigel Metheringham
 Author-email: nigelm@cpan.org
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20.3.0,<21.0.0)
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
@@ -27,29 +29,33 @@
 [![pypi version](https://img.shields.io/pypi/v/moin2gitwiki.svg)](https://pypi.python.org/pypi/moin2gitwiki)
 
 App to convert a MoinMoin wiki file tree into a git based wiki as used on
 github, gitlab or gitea.
 
 ## Current Version
 
-Version: `0.7.0`
+Version: `0.8.0`
+
+## Status
+
+This was required for a one-off conversion. I'm not doing any further work on it - if anyone wishes to take this over then please just ask.
 
 ## Translation Method
 
 Originally the intention was to translate purely by converting the MoinMoin
 markup to markdown markup - using the MoinMoin data retrieved from the
 filesystem.
 
 However, although it makes determining the overall page list and revision list
 much easier, it was found that translating the wiki markup at this level was
 too complex and fragile for this to work without a huge amount of special
 casing.
 
 So, after the revision structure is derived from the filesystem, each page
-revision is retrieved by http requests to the running MoinMoin wiki.  This is
+revision is retrieved by http requests to the running MoinMoin wiki. This is
 then reduced to just the page content (by picking out the content div from the
 html), and some light editing applied to simplify the HTML - specifically:-
 
 - Remove the anchor spans that MoinMoin adds - these add no visual or
   readable content, but confuse the translator
 - Remove paragraph entries with CSS classes that start `line` - these
   again appear to be for non-required purposes (likely for showing diffs
@@ -63,28 +69,28 @@
 This simplified HTML is then passed through the pandoc command:-
 
     pandoc -f html -t gfm
 
 And the resulting Github flavoured Markdown is taken as the new form.
 
 This handles the vast majority of normal markup correctly, including lists and
-many types of tables.  Some complicated markup or complex tables end up being
+many types of tables. Some complicated markup or complex tables end up being
 passed through as HTML - which displays correctly but is less easy to parse
 and edit.
 
 Attachments that are available in the wiki are also handled - they are put
 into a `_attachments` directory under a subdirectory named for the original
-page directory name.  Links to attachments should be handled correctly.
+page directory name. Links to attachments should be handled correctly.
 
 ## Issues
 
-The overall process is not particularly fast.  But this should be something
+The overall process is not particularly fast. But this should be something
 you only do once (or a few attempts) so raw speed is not needed.
 
-Attachments are not versioned by MoinMon.  This means any attachment that was
+Attachments are not versioned by MoinMon. This means any attachment that was
 deleted from MoinMoin is no longer available to put into the converted wiki.
 Any attachment that was updated a few times is only available in the last
 version (but will probably be inserted into the history at the point where it
 first appeared but with the latest content).
 
 ## Installation
 
@@ -107,9 +113,9 @@
 
     poetry run moin2gitwiki ...
 
 ## Todo
 
 - Make tests effective
 
-----
+---
```


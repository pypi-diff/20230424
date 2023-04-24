# Comparing `tmp/griptape_tools-0.7.1.tar.gz` & `tmp/griptape_tools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.7.1.tar", max compression
+gzip compressed data, was "griptape_tools-0.8.0.tar", max compression
```

## Comparing `griptape_tools-0.7.1.tar` & `griptape_tools-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.7.1/LICENSE
--rw-r--r--   0        0        0     1284 2023-04-21 17:41:39.072846 griptape_tools-0.7.1/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.7.1/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.7.1/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.7.1/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-18 22:49:15.710526 griptape_tools-0.7.1/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1447 2023-04-16 19:44:48.773728 griptape_tools-0.7.1/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.7.1/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-18 22:49:15.709272 griptape_tools-0.7.1/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      652 2023-04-16 19:44:48.772145 griptape_tools-0.7.1/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.7.1/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-18 22:49:15.704485 griptape_tools-0.7.1/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     6073 2023-04-21 17:41:59.159404 griptape_tools-0.7.1/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.7.1/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.7.1/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-18 22:49:15.707814 griptape_tools-0.7.1/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1259 2023-04-16 19:44:48.779356 griptape_tools-0.7.1/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.1/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.7.1/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-18 22:49:15.706181 griptape_tools-0.7.1/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4437 2023-04-18 22:36:34.063641 griptape_tools-0.7.1/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.7.1/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.7.1/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-18 22:49:15.701853 griptape_tools-0.7.1/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2272 2023-04-16 19:44:48.776769 griptape_tools-0.7.1/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-21 20:55:35.986257 griptape_tools-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 griptape_tools-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1284 2023-04-21 17:41:39.072846 griptape_tools-0.8.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.8.0/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.8.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.8.0/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       71 2023-04-23 21:38:29.292854 griptape_tools-0.8.0/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1467 2023-04-24 19:00:12.784453 griptape_tools-0.8.0/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.8.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       14 2023-04-23 21:38:29.291686 griptape_tools-0.8.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      676 2023-04-24 19:00:12.782272 griptape_tools-0.8.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.8.0/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       14 2023-04-23 21:38:29.288512 griptape_tools-0.8.0/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     5893 2023-04-24 19:00:12.786990 griptape_tools-0.8.0/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.8.0/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.8.0/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       26 2023-04-23 21:38:29.287003 griptape_tools-0.8.0/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1259 2023-04-24 19:00:12.780590 griptape_tools-0.8.0/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.8.0/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.8.0/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       46 2023-04-23 21:38:29.290644 griptape_tools-0.8.0/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4437 2023-04-24 19:00:12.789352 griptape_tools-0.8.0/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.8.0/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.8.0/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       22 2023-04-23 21:38:29.289637 griptape_tools-0.8.0/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2263 2023-04-24 19:00:12.778362 griptape_tools-0.8.0/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      541 2023-04-24 19:31:33.753195 griptape_tools-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 griptape_tools-0.8.0/PKG-INFO
```

### Comparing `griptape_tools-0.7.1/LICENSE` & `griptape_tools-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.1/README.md` & `griptape_tools-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.1/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.8.0/griptape/tools/aws_cli/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from typing import Optional
 from schema import Schema
-from griptape.core import BaseTool, action, utils
+from griptape.core import action, BaseTool
+from griptape import utils
 from attr import define, field
 
 
 @define
 class AwsCli(BaseTool):
     aws_access_key_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_ACCESS_KEY_ID"})
     aws_secret_access_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_SECRET_ACCESS_KEY"})
```

### Comparing `griptape_tools-0.7.1/griptape/tools/calculator/tool.py` & `griptape_tools-0.8.0/griptape/tools/calculator/tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from griptape.core import BaseTool, action, utils
+from griptape.core import BaseTool, action
+import griptape.utils as utils
 from schema import Schema
 
 
 class Calculator(BaseTool):
     @action(config={
         "name": "calculate",
         "description": "Can be used for making simple calculations in Python",
```

### Comparing `griptape_tools-0.7.1/griptape/tools/email_client/tool.py` & `griptape_tools-0.8.0/griptape/tools/email_client/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class EmailClient(BaseTool):
     # if you set imap|smtp creds explicitly these fields will be overridden
     username: Optional[str] = field(default=None, kw_only=True, metadata={"env": "EMAIL_USERNAME"})
     password: Optional[str] = field(default=None, kw_only=True, metadata={"env": "EMAIL_PASSWORD"})
 
     smtp_host: Optional[str] = field(default=None, kw_only=True, metadata={"env": "SMTP_HOST"})
     smtp_port: Optional[int] = field(default=None, kw_only=True, metadata={"env": "SMTP_PORT"})
-    smtp_from_email: Optional[str] = field(default=None, kw_only=True, metadata={"env": "SMTP_FROM_EMAIL"})
     smtp_use_ssl: bool = field(default=True, kw_only=True, metadata={"env": "SMTP_USE_SSL"})
 
     # if you set the smtp user/password fields they will override
     smtp_user: Optional[str] = field(default=None, kw_only=True, metadata={"env": "SMTP_USER"})
     smtp_password: Optional[str] = field(default=None, kw_only=True, metadata={"env": "SMTP_PASSWORD"})
 
     imap_url: Optional[str] = field(default=None, kw_only=True, metadata={"env": "IMAP_URL"})
@@ -127,32 +126,31 @@
         # email password can be overridden by setting the smtp password explicitly
         smtp_password = self.env_value("SMTP_PASSWORD")
         if smtp_password is None:
             smtp_password = self.env_value("EMAIL_PASSWORD")
 
         smtp_host = self.env_value("SMTP_HOST")
         smtp_port = int(self.env_value("SMTP_PORT"))
-        smtp_from_email = self.env_value("SMTP_FROM_EMAIL")
 
         to_email = params["to"]
         subject = params["subject"]
         msg = MIMEText(params["body"])
 
         try:
             if self.env_value("SMTP_USE_SSL"):
                 server = smtplib.SMTP_SSL(smtp_host, smtp_port)
             else:
                 server = smtplib.SMTP(smtp_host, smtp_port)
 
             msg["Subject"] = subject
-            msg["From"] = smtp_from_email
+            msg["From"] = smtp_user
             msg["To"] = to_email
 
             server.login(smtp_user, smtp_password)
-            server.sendmail(smtp_from_email, [to_email], msg.as_string())
+            server.sendmail(smtp_user, [to_email], msg.as_string())
 
             return "email was successfully sent"
         except Exception as e:
             logging.error(e)
 
             return f"error sending email: {e}"
         finally:
```

### Comparing `griptape_tools-0.7.1/griptape/tools/sql_client/tool.py` & `griptape_tools-0.8.0/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.1/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.8.0/griptape/tools/web_scraper/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.7.1/griptape/tools/web_search/tool.py` & `griptape_tools-0.8.0/griptape/tools/web_search/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 from attr import define, field
-from schema import Schema, Literal
+from schema import Schema
 from griptape.core import BaseTool, action
 
 
 @define
 class WebSearch(BaseTool):
     results_count: int = field(default=5, kw_only=True, metadata={"env": "SEARCH_RESULTS_COUNT"})
     google_api_lang: str = field(default="lang_en", kw_only=True, metadata={"env": "GOOGLE_API_LANG"})
```

### Comparing `griptape_tools-0.7.1/pyproject.toml` & `griptape_tools-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.7.1"
+version = "0.8.0"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = ">=0.9.2"
-
+griptape = ">=0.6"
+llama_index = ">= 0.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `griptape_tools-0.7.1/PKG-INFO` & `griptape_tools-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.7.1
+Version: 0.8.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.9.2)
+Requires-Dist: griptape (>=0.6)
+Requires-Dist: llama_index (>=0.5)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # griptape-tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
```


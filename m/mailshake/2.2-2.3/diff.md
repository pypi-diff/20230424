# Comparing `tmp/mailshake-2.2.tar.gz` & `tmp/mailshake-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailshake-2.2.tar", last modified: Mon Aug 24 03:47:29 2020, max compression
+gzip compressed data, was "mailshake-2.3.tar", last modified: Mon Apr 24 16:47:20 2023, max compression
```

## Comparing `mailshake-2.2.tar` & `mailshake-2.3.tar`

### file list

```diff
@@ -1,35 +1,30 @@
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2020-08-24 03:47:29.048915 mailshake-2.2/
--rw-r--r--   0 jps        (501) staff       (20)     2607 2020-08-23 19:33:05.000000 mailshake-2.2/CONTRIBUTING.md
--rwxr-xr-x   0 jps        (501) staff       (20)    10212 2020-06-28 18:22:30.000000 mailshake-2.2/LICENSE
--rwxr-xr-x   0 jps        (501) staff       (20)      905 2020-08-24 03:42:53.000000 mailshake-2.2/Makefile
--rw-r--r--   0 jps        (501) staff       (20)     2827 2020-08-24 03:47:29.049263 mailshake-2.2/PKG-INFO
--rw-r--r--   0 jps        (501) staff       (20)     1642 2020-08-23 19:34:04.000000 mailshake-2.2/README.md
--rw-r--r--   0 jps        (501) staff       (20)        0 2020-06-28 16:42:15.000000 mailshake-2.2/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2020-08-24 03:47:29.032914 mailshake-2.2/mailshake/
--rwxr-xr-x   0 jps        (501) staff       (20)      458 2020-06-28 18:20:27.000000 mailshake-2.2/mailshake/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2020-08-24 03:47:29.045263 mailshake-2.2/mailshake/mailers/
--rwxr-xr-x   0 jps        (501) staff       (20)        0 2020-06-28 16:42:15.000000 mailshake-2.2/mailshake/mailers/__init__.py
--rwxr-xr-x   0 jps        (501) staff       (20)     2220 2020-08-24 03:05:03.000000 mailshake-2.2/mailshake/mailers/amazon_ses.py
--rwxr-xr-x   0 jps        (501) staff       (20)     1365 2020-08-23 19:08:32.000000 mailshake-2.2/mailshake/mailers/base.py
--rwxr-xr-x   0 jps        (501) staff       (20)     1271 2020-08-24 03:04:57.000000 mailshake-2.2/mailshake/mailers/console.py
--rwxr-xr-x   0 jps        (501) staff       (20)      183 2020-08-24 03:04:53.000000 mailshake-2.2/mailshake/mailers/dummy.py
--rwxr-xr-x   0 jps        (501) staff       (20)     1967 2020-08-24 03:04:49.000000 mailshake-2.2/mailshake/mailers/filebased.py
--rwxr-xr-x   0 jps        (501) staff       (20)      649 2020-08-23 19:14:59.000000 mailshake-2.2/mailshake/mailers/memory.py
--rwxr-xr-x   0 jps        (501) staff       (20)     5036 2020-08-23 19:08:32.000000 mailshake-2.2/mailshake/mailers/smtp.py
--rwxr-xr-x   0 jps        (501) staff       (20)    10010 2020-08-23 19:27:37.000000 mailshake-2.2/mailshake/message.py
--rwxr-xr-x   0 jps        (501) staff       (20)     3934 2020-08-23 19:27:37.000000 mailshake-2.2/mailshake/utils.py
--rw-r--r--   0 jps        (501) staff       (20)      152 2020-08-23 19:34:32.000000 mailshake-2.2/mailshake/version.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2020-08-24 03:47:29.037369 mailshake-2.2/mailshake.egg-info/
--rw-r--r--   0 jps        (501) staff       (20)     2827 2020-08-24 03:47:28.000000 mailshake-2.2/mailshake.egg-info/PKG-INFO
--rw-r--r--   0 jps        (501) staff       (20)      655 2020-08-24 03:47:28.000000 mailshake-2.2/mailshake.egg-info/SOURCES.txt
--rw-r--r--   0 jps        (501) staff       (20)        1 2020-08-24 03:47:28.000000 mailshake-2.2/mailshake.egg-info/dependency_links.txt
--rw-r--r--   0 jps        (501) staff       (20)       79 2020-08-24 03:47:28.000000 mailshake-2.2/mailshake.egg-info/requires.txt
--rw-r--r--   0 jps        (501) staff       (20)       10 2020-08-24 03:47:28.000000 mailshake-2.2/mailshake.egg-info/top_level.txt
--rw-r--r--   0 jps        (501) staff       (20)     1410 2020-08-24 03:47:29.050794 mailshake-2.2/setup.cfg
--rw-r--r--   0 jps        (501) staff       (20)       69 2020-08-23 19:15:16.000000 mailshake-2.2/setup.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2020-08-24 03:47:29.048383 mailshake-2.2/tests/
--rwxr-xr-x   0 jps        (501) staff       (20)        0 2020-06-28 16:42:15.000000 mailshake-2.2/tests/__init__.py
--rw-r--r--   0 jps        (501) staff       (20)        0 2020-06-28 16:42:15.000000 mailshake-2.2/tests/conftest.py
--rwxr-xr-x   0 jps        (501) staff       (20)     4530 2020-08-23 19:08:32.000000 mailshake-2.2/tests/test_mailers.py
--rwxr-xr-x   0 jps        (501) staff       (20)    15459 2020-08-24 03:03:58.000000 mailshake-2.2/tests/test_message.py
--rwxr-xr-x   0 jps        (501) staff       (20)     4521 2020-08-23 19:08:32.000000 mailshake-2.2/tests/test_smtp_mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:20.600051 mailshake-2.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10212 2023-04-24 16:47:01.000000 mailshake-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-24 16:47:20.600051 mailshake-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 16:47:01.000000 mailshake-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:20.600051 mailshake-2.3/mailshake/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:20.600051 mailshake-2.3/mailshake/mailers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2207 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/amazon_ses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/dummy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/filebased.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5018 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/mailers/smtp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10005 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/message.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3924 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 16:47:01.000000 mailshake-2.3/mailshake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:20.600051 mailshake-2.3/mailshake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-24 16:47:20.000000 mailshake-2.3/mailshake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 16:47:20.000000 mailshake-2.3/mailshake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:47:20.000000 mailshake-2.3/mailshake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:47:20.000000 mailshake-2.3/mailshake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 16:47:20.000000 mailshake-2.3/mailshake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-24 16:47:20.600051 mailshake-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 16:47:01.000000 mailshake-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:47:20.600051 mailshake-2.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4525 2023-04-24 16:47:01.000000 mailshake-2.3/tests/test_mailers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-04-24 16:47:01.000000 mailshake-2.3/tests/test_message.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3851 2023-04-24 16:47:01.000000 mailshake-2.3/tests/test_smtp_mailer.py
```

### Comparing `mailshake-2.2/LICENSE` & `mailshake-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailshake-2.2/PKG-INFO` & `mailshake-2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 Metadata-Version: 2.1
 Name: mailshake
-Version: 2.2
+Version: 2.3
 Summary: Dramatically simplify sending email from your python app.
 Home-page: https://github.com/jpsca/mailshake
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 License: Apache License Version 2.0
 Project-URL: Issue tracker, https://github.com/jpsca/mailshake/issues
-Description: ![Mailshake logo](https://raw.github.com/jpsca/mailshake/master/docs/static/images/mailshake@2x.png)
-        
-        # Mailshake
-        
-        [![Build Status](https://travis-ci.org/jpsca/mailshake.svg?branch=master)](https://travis-ci.org/jpsca/mailshake)
-        
-        Although Python makes sending email relatively easy via the smtplib
-        module, this library provides a couple of light wrappers over it.
-        
-        These wrappers make sending email extra quick, easy to test email
-        sending during development, and provides support for platforms that
-        can't use SMTP.
-        
-        Mailers availiable:
-        
-        -   SMTPMailer
-        -   AmazonSESMailer
-        -   ToConsoleMailer (prints the emails in the console)
-        -   ToFileMailer (save the emails in a file)
-        -   ToMemoryMailer (for testing)
-        -   DummyMailer (does nothing)
-        
-        Usage:
-        
-        ```python
-        from mailshake import SMTPMailer
-        
-        mailer = SMTPMailer()
-        mailer.send(
-            subject='Hi',
-            text_content='Hello world!',
-            from_email='from@example.com',
-            to=['mary@example.com', 'bob@example.com']
-        )
-        ```
-        
-        You can also compose several messages and send them at the same time:
-        
-        ```python
-        from mailshake import SMTPMailer, EmailMessage
-        
-        mailer = SMTPMailer()
-        messages = []
-        
-        email_msg = EmailMessage(
-            "Weekend getaway",
-            "Here's a photo of us from our trip.",
-            "from@example.com",
-            "bob@example.com"
-        )
-        email_msg.attach_file("picture.jpg")
-        messages.append(email_msg)
-        
-        #…
-        
-        mailer.send_messages(*messages)
-        ```
-        
-        ## Install for development
-        
-        First, create an activate a virtualenv. eg:
-        
-        ```bash
-        python -m virtualenv .venv
-        source .venv/bin/activate
-        ```
-        
-        Then run `pip install -e .[dev]` or `make install`. This will install the library in editable mode and all its dependencies.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: <4.0,>=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+![Mailshake logo](https://raw.github.com/jpsca/mailshake/master/docs/static/images/mailshake@2x.png)
+
+# Mailshake
+
+[![Build Status](https://travis-ci.org/jpsca/mailshake.svg?branch=master)](https://travis-ci.org/jpsca/mailshake)
+
+Although Python makes sending email relatively easy via the smtplib
+module, this library provides a couple of light wrappers over it.
+
+These wrappers make sending email extra quick, easy to test email
+sending during development, and provides support for platforms that
+can't use SMTP.
+
+Mailers availiable:
+
+-   SMTPMailer
+-   AmazonSESMailer
+-   ToConsoleMailer (prints the emails in the console)
+-   ToFileMailer (save the emails in a file)
+-   ToMemoryMailer (for testing)
+-   DummyMailer (does nothing)
+
+Usage:
+
+```python
+from mailshake import SMTPMailer
+
+mailer = SMTPMailer()
+mailer.send(
+    subject='Hi',
+    text_content='Hello world!',
+    from_email='from@example.com',
+    to=['mary@example.com', 'bob@example.com']
+)
+```
+
+You can also compose several messages and send them at the same time:
+
+```python
+from mailshake import SMTPMailer, EmailMessage
+
+mailer = SMTPMailer()
+messages = []
+
+email_msg = EmailMessage(
+    "Weekend getaway",
+    "Here's a photo of us from our trip.",
+    "from@example.com",
+    "bob@example.com"
+)
+email_msg.attach_file("picture.jpg")
+messages.append(email_msg)
+
+#…
+
+mailer.send_messages(*messages)
+```
+
+## Install for development
+
+First, create an activate a virtualenv. eg:
+
+```bash
+python -m virtualenv .venv
+source .venv/bin/activate
+```
+
+Then run `pip install -e .[dev]` or `make install`. This will install the library in editable mode and all its dependencies.
```

### Comparing `mailshake-2.2/README.md` & `mailshake-2.3/README.md`

 * *Files identical despite different names*

### Comparing `mailshake-2.2/mailshake/mailers/amazon_ses.py` & `mailshake-2.3/mailshake/mailers/amazon_ses.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,54 +16,52 @@
         aws_access_key_id,
         aws_secret_access_key,
         region_name="us-east-1",
         return_path=None,
         *args,
         **kwargs
     ):
-        """
-        """
+        """ """
         import boto3
 
         self.client = boto3.client(
             "ses",
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             region_name=region_name,
         )
         assert self.client
         self.return_path = return_path
         super(AmazonSESMailer, self).__init__(*args, **kwargs)
 
     def send_messages(self, *email_messages):
-        """
-        """
+        """ """
         logger = logging.getLogger("mailshake:AmazonSESMailer")
         if not email_messages:
             logger.debug("No email messages to send")
             return
 
         responses = []
 
         for msg in email_messages:
             destination_data = {"ToAddresses": msg.to}
             if msg.cc:
                 destination_data["CcAddresses"] = msg.cc
             if msg.bcc:
                 destination_data["BccAddresses"] = msg.bcc
 
-            body_data = {"Text": {"Data": msg.text, "Charset": "utf8"}}
+            body_data = {"Text": {"Data": msg.text, "Charset": "UTF-8"}}
             if msg.html:
-                body_data["Html"] = {"Data": msg.html, "Charset": "utf8"}
+                body_data["Html"] = {"Data": msg.html, "Charset": "UTF-8"}
 
             data = {
                 "Source": msg.from_email,
                 "Destination": destination_data,
                 "Message": {
-                    "Subject": {"Data": msg.subject, "Charset": "utf8"},
+                    "Subject": {"Data": msg.subject, "Charset": "UTF-8"},
                     "Body": body_data,
                 },
             }
             if msg.reply_to:
                 data["ReplyToAddresses"] = msg.reply_to
             if msg.tags:
                 data["Tags"] = msg.tags
```

### Comparing `mailshake-2.2/mailshake/mailers/base.py` & `mailshake-2.3/mailshake/mailers/base.py`

 * *Files identical despite different names*

### Comparing `mailshake-2.2/mailshake/mailers/console.py` & `mailshake-2.3/mailshake/mailers/console.py`

 * *Files identical despite different names*

### Comparing `mailshake-2.2/mailshake/mailers/filebased.py` & `mailshake-2.3/mailshake/mailers/filebased.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         # Finally, call super().
         # Since we're using the console-based backend as a base,
         # force the stream to be None, so we don't default to stdout
         kwargs["stream"] = None
         super(ToFileMailer, self).__init__(*args, **kwargs)
 
     def _get_filename(self):
-        """Return a unique file name.
-        """
+        """Return a unique file name."""
         if self._fname is None:
             now = datetime.datetime.now()
             timestamp = now.strftime("%Y%m%d-%H%M%S")
             ms = now.microsecond
             fname = "%s-%s-%s.log" % (timestamp, abs(id(self)), ms)
             self._fname = os.path.join(self.path, fname)
         return self._fname
```

### Comparing `mailshake-2.2/mailshake/mailers/memory.py` & `mailshake-2.3/mailshake/mailers/memory.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,11 +13,10 @@
     """
 
     def __init__(self, *args, **kwargs):
         self.outbox = []
         super(ToMemoryMailer, self).__init__(*args, **kwargs)
 
     def send_messages(self, *email_messages):
-        """Redirect messages to the dummy outbox.
-        """
+        """Redirect messages to the dummy outbox."""
         self.outbox.extend(email_messages)
         return len(email_messages)
```

### Comparing `mailshake-2.2/mailshake/mailers/smtp.py` & `mailshake-2.3/mailshake/mailers/smtp.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,15 @@
         except Exception:
             if not self.fail_silently:
                 raise
 
         return True
 
     def close(self):
-        """Closes the connection to the email server.
-        """
+        """Closes the connection to the email server."""
         if self.connection is None:
             return
         try:
             try:
                 self.connection.quit()
             except (ssl.SSLError, smtplib.SMTPServerDisconnected):
                 # This happens when calling quit() on a TLS connection
@@ -121,16 +120,15 @@
             if sent:
                 num_sent += 1
         if new_conn_created:
             self.close()
         return num_sent
 
     def _send(self, message):
-        """A helper method that does the actual sending.
-        """
+        """A helper method that does the actual sending."""
         recipients = message.get_recipients()
         if not recipients:
             return False
         from_email = message.from_email or self.default_from
         to_set = set(message.to)
         cc_set = set(message.cc)
         bcc_set = set(message.bcc)
```

### Comparing `mailshake-2.2/mailshake/message.py` & `mailshake-2.3/mailshake/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,15 @@
     ):
         self.encoding = encoding
         super().__init__(_subtype, boundary, _subparts, **_params)
 
 
 class EmailMessage:
 
-    """A container for email information.
-    """
+    """A container for email information."""
 
     content_subtype = "plain"
     mixed_subtype = "mixed"
     html_subtype = "html"
     alternative_subtype = "alternative"
 
     def __init__(
```

### Comparing `mailshake-2.2/mailshake/utils.py` & `mailshake-2.3/mailshake/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,22 +110,20 @@
         idstring = "." + idstring
     return "<{}.{}.{:x}.{}{}@{}>".format(
         utcdate, pid, function_id, sequence_id, idstring, host_id
     )
 
 
 def forbid_multi_line_headers(name, val):
-    """Forbids multi-line headers, to prevent header injection.
-    """
+    """Forbids multi-line headers, to prevent header injection."""
     if "\n" in val or "\r" in val:
         raise ValueError(
             "Header values can't contain newlines "
             "(got {val} for header {name})".format(val=val, name=name)
         )
 
 
 def to_str(s, encoding="utf-8", errors="strict"):
-    """Force a string to be the native text_type
-    """
+    """Force a string to be the native text_type"""
     if isinstance(s, str):
         return s
     return str(s, encoding, errors)
```

### Comparing `mailshake-2.2/mailshake.egg-info/PKG-INFO` & `mailshake-2.3/mailshake.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 Metadata-Version: 2.1
 Name: mailshake
-Version: 2.2
+Version: 2.3
 Summary: Dramatically simplify sending email from your python app.
 Home-page: https://github.com/jpsca/mailshake
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 License: Apache License Version 2.0
 Project-URL: Issue tracker, https://github.com/jpsca/mailshake/issues
-Description: ![Mailshake logo](https://raw.github.com/jpsca/mailshake/master/docs/static/images/mailshake@2x.png)
-        
-        # Mailshake
-        
-        [![Build Status](https://travis-ci.org/jpsca/mailshake.svg?branch=master)](https://travis-ci.org/jpsca/mailshake)
-        
-        Although Python makes sending email relatively easy via the smtplib
-        module, this library provides a couple of light wrappers over it.
-        
-        These wrappers make sending email extra quick, easy to test email
-        sending during development, and provides support for platforms that
-        can't use SMTP.
-        
-        Mailers availiable:
-        
-        -   SMTPMailer
-        -   AmazonSESMailer
-        -   ToConsoleMailer (prints the emails in the console)
-        -   ToFileMailer (save the emails in a file)
-        -   ToMemoryMailer (for testing)
-        -   DummyMailer (does nothing)
-        
-        Usage:
-        
-        ```python
-        from mailshake import SMTPMailer
-        
-        mailer = SMTPMailer()
-        mailer.send(
-            subject='Hi',
-            text_content='Hello world!',
-            from_email='from@example.com',
-            to=['mary@example.com', 'bob@example.com']
-        )
-        ```
-        
-        You can also compose several messages and send them at the same time:
-        
-        ```python
-        from mailshake import SMTPMailer, EmailMessage
-        
-        mailer = SMTPMailer()
-        messages = []
-        
-        email_msg = EmailMessage(
-            "Weekend getaway",
-            "Here's a photo of us from our trip.",
-            "from@example.com",
-            "bob@example.com"
-        )
-        email_msg.attach_file("picture.jpg")
-        messages.append(email_msg)
-        
-        #…
-        
-        mailer.send_messages(*messages)
-        ```
-        
-        ## Install for development
-        
-        First, create an activate a virtualenv. eg:
-        
-        ```bash
-        python -m virtualenv .venv
-        source .venv/bin/activate
-        ```
-        
-        Then run `pip install -e .[dev]` or `make install`. This will install the library in editable mode and all its dependencies.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: <4.0,>=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+![Mailshake logo](https://raw.github.com/jpsca/mailshake/master/docs/static/images/mailshake@2x.png)
+
+# Mailshake
+
+[![Build Status](https://travis-ci.org/jpsca/mailshake.svg?branch=master)](https://travis-ci.org/jpsca/mailshake)
+
+Although Python makes sending email relatively easy via the smtplib
+module, this library provides a couple of light wrappers over it.
+
+These wrappers make sending email extra quick, easy to test email
+sending during development, and provides support for platforms that
+can't use SMTP.
+
+Mailers availiable:
+
+-   SMTPMailer
+-   AmazonSESMailer
+-   ToConsoleMailer (prints the emails in the console)
+-   ToFileMailer (save the emails in a file)
+-   ToMemoryMailer (for testing)
+-   DummyMailer (does nothing)
+
+Usage:
+
+```python
+from mailshake import SMTPMailer
+
+mailer = SMTPMailer()
+mailer.send(
+    subject='Hi',
+    text_content='Hello world!',
+    from_email='from@example.com',
+    to=['mary@example.com', 'bob@example.com']
+)
+```
+
+You can also compose several messages and send them at the same time:
+
+```python
+from mailshake import SMTPMailer, EmailMessage
+
+mailer = SMTPMailer()
+messages = []
+
+email_msg = EmailMessage(
+    "Weekend getaway",
+    "Here's a photo of us from our trip.",
+    "from@example.com",
+    "bob@example.com"
+)
+email_msg.attach_file("picture.jpg")
+messages.append(email_msg)
+
+#…
+
+mailer.send_messages(*messages)
+```
+
+## Install for development
+
+First, create an activate a virtualenv. eg:
+
+```bash
+python -m virtualenv .venv
+source .venv/bin/activate
+```
+
+Then run `pip install -e .[dev]` or `make install`. This will install the library in editable mode and all its dependencies.
```

### Comparing `mailshake-2.2/setup.cfg` & `mailshake-2.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mailshake
-version = 2.2
+version = 2.3
 url = https://github.com/jpsca/mailshake
 project_urls = 
 	Issue tracker = https://github.com/jpsca/mailshake/issues
 author = Juan-Pablo Scaletti
 author_email = juanpablo@jpscaletti.com
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -28,38 +28,40 @@
 	tests
 
 [options.extras_require]
 test = 
 	flake8
 	pytest
 	pytest-cov
+	smtpdfix
 dev = 
+	black
 	flake8
 	pytest
 	pytest-cov
 	tox
 
 [flake8]
 select = 
-	B,  # bugbear
-	B9,  # bugbear opinionated
-	C,  # mccabe, comprehensions, commas
-	E,  # pycodestyle errors
-	F,  # pyflakes
-	G,  # logging format
-	I,  # imports
+	B,
+	B9,
+	C,
+	E,
+	F,
+	G,
+	I,
 	P,
-	Q,  # quotes
-	RST,  # rst docstring formatting
-	T0,  # print
-	T4,  # mypy
-	W,  # pycodestyle warnings
+	Q,
+	RST,
+	T0,
+	T4,
+	W,
 ignore = 
-	W503,  # W503 line break before binary operator
-	E203,  # E203 whitespace before ':'
+	W503,
+	E203,
 max-complexity = 10
 max-line-length = 88
 statistics = true
 doctests = True
 accept-encodings = utf-8
 
 [tool:pytest]
```

### Comparing `mailshake-2.2/tests/test_mailers.py` & `mailshake-2.3/tests/test_mailers.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,15 @@
     mailer.fail_silently = True
     mailer.send("Subject", "Content", "from@example.com", "to@example.com")
 
     sys.stdout = __stdout
 
 
 def test_to_console_stream_kwarg():
-    """Test that the console backend can be pointed at an arbitrary stream.
-    """
+    """Test that the console backend can be pointed at an arbitrary stream."""
     s = StringIO()
     mailer = ToConsoleMailer(stream=s)
     mailer.send("Subject", "Content", "from@example.com", "to@example.com")
 
     value = s.getvalue()
     assert value.startswith(
         'Content-Type: text/plain; charset="utf-8"'
```

### Comparing `mailshake-2.2/tests/test_message.py` & `mailshake-2.3/tests/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,16 +212,15 @@
     lines = set(email_as_string.split("\n"))
     for header in headers:
         assert header in lines
     assert email_as_string.endswith("\n\nContent")
 
 
 def test_from_header():
-    """Make sure we can manually set the From header.
-    """
+    """Make sure we can manually set the From header."""
     email = EmailMessage(
         "Subject",
         "Content",
         "bounce@example.com",
         "to@example.com",
         headers={"From": "from@example.com"},
     )
@@ -432,16 +431,15 @@
     )
     str_email = email.as_bytes()
     print(str_email)
     assert b">From the future" not in str_email
 
 
 def test_dont_base64_encode():
-    """Shouldn't use Base64 encoding at all.
-    """
+    """Shouldn't use Base64 encoding at all."""
     email = EmailMessage(
         "Subject",
         "UTF-8 encoded body",
         "bounce@example.com",
         "to@example.com",
         headers={"From": "from@example.com"},
     )
@@ -501,19 +499,26 @@
 
     assert message["Subject"] == "Subject"
     assert message.get_payload() == "Content"
     assert message["From"] == "from@example.com"
     assert message["To"] != dest
 
 
+rx_message_id = re.compile(
+    r"^<[0-9]{14}\.[0-9]+\.[0-9a-f]+\.[0-9]+@[a-z0-9\-]+(\.[a-z0-9\-]+)*>$",
+    re.IGNORECASE,
+)
+
+
 def test_message_id():
-    message_id_re = re.compile(
-        r"^<[0-9]{14}\.[0-9]+\.[0-9a-f]+\.[0-9]+@[a-z\-]+(\.[a-z\-]+)*>$",
-        re.IGNORECASE
-    )
     email1 = EmailMessage("Subject 1", "Content", "from@example.com", "to@example.com")
     msg1 = email1.render()
-    assert message_id_re.match(msg1["Message-ID"])
+    mid1 = msg1["Message-ID"]
+    print("Message-ID 1:", mid1)
+    assert rx_message_id.match(mid1)
+
     email2 = EmailMessage("Subject 2", "Content", "from@example.com", "to@example.com")
     msg2 = email2.render()
-    assert message_id_re.match(msg2["Message-ID"])
-    assert msg2["Message-ID"] != msg1["Message-ID"]
+    mid2 = msg2["Message-ID"]
+    print("Message-ID 2:", mid2)
+    assert rx_message_id.match(mid2)
+    assert mid2 != mid1
```

### Comparing `mailshake-2.2/tests/test_smtp_mailer.py` & `mailshake-2.3/tests/test_smtp_mailer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,164 +1,132 @@
-import asyncore
-from email import message_from_bytes
-import smtpd
-from smtplib import SMTPException
-import threading
-
 import pytest
+from smtplib import SMTP, SMTPException
 
 from ..mailshake import EmailMessage, SMTPMailer
 
 
 def make_emails():
     return [
         EmailMessage(
             "Subject-%s" % num, "Content", "from@example.com", "to@example.com"
         )
         for num in range(1, 5)
     ]
 
 
-smtp_server = None
-SMTP_HOST = "127.0.0.1"
-SMTP_PORT = 8080
-
-
-class FakeSMTPServer(smtpd.SMTPServer):
-    """A Fake smtp server"""
-
-    def __init__(self, host, port):
-        print("Running fake SMTP server")
-        localaddr = (host, port)
-        remoteaddr = None
-        smtpd.SMTPServer.__init__(self, localaddr, remoteaddr)
-        self.flush_sink()
-
-    def flush_sink(self):
-        self.sink = []
-
-    def process_message(self, peer, from_, to, bmessage, **kwargs):
-        self.sink.append(message_from_bytes(bmessage))
-
-    def start(self):
-        # timeout parameter is important, otherwise code will block 30 seconds after
-        # the SMTP channel has been closed
-        self.thread = threading.Thread(target=asyncore.loop, kwargs={"timeout": 0.1})
-        self.thread.daemon = True
-        self.thread.start()
-
-    def stop(self):
-        # close the SMTPserver to ensure no channels connect to asyncore
-        self.close()
-        # now it is save to wait for the thread to finish,
-        # i.e. for asyncore.loop() to exit
-        self.thread.join(timeout=0.5)
-
-
-def setup_module():
-    global smtp_server
-    smtp_server = FakeSMTPServer(SMTP_HOST, SMTP_PORT)
-    smtp_server.start()
-
-
-def teardown_module():
-    global smtp_server
-    if smtp_server is not None:
-        smtp_server.stop()
-
-
-def test_sending():
-    global smtp_server
-    smtp_server.flush_sink()
-
-    mailer = SMTPMailer(host=SMTP_HOST, port=SMTP_PORT, use_tls=False)
+def test_sending(smtpd):
+    mailer = SMTPMailer(host=smtpd.hostname, port=smtpd.port, use_tls=False)
     email1, email2, email3, email4 = make_emails()
 
-    assert mailer.send_messages(email1) == 1
-    assert mailer.send_messages(email2, email3) == 2
-    assert mailer.send_messages(email4) == 1
+    with SMTP(smtpd.hostname, smtpd.port):
+        assert mailer.send_messages(email1) == 1
+        assert mailer.send_messages(email2, email3) == 2
+        assert mailer.send_messages(email4) == 1
 
-    sink = smtp_server.sink
-    assert len(sink) == 4
+    assert len(smtpd.messages) == 4
 
-    message = sink[0]
+    message = smtpd.messages[0]
     print(message)
     assert message.get_content_type() == "text/plain"
     assert message.get("subject") == "Subject-1"
     assert message.get("from") == "from@example.com"
     assert message.get("to") == "to@example.com"
 
 
-def test_sending_unicode():
-    global smtp_server
-    smtp_server.flush_sink()
-
-    mailer = SMTPMailer(host="127.0.0.1", port=SMTP_PORT, use_tls=False)
+def test_sending_unicode(smtpd):
+    mailer = SMTPMailer(host=smtpd.hostname, port=smtpd.port, use_tls=False)
     email = EmailMessage(
-        "Olé", "Contenido en español", "from@example.com", "toБ@example.com"
+        subject="Olé",
+        text="Contenido en español",
+        from_email="from@example.com",
+        to="toБ@example.com",
     )
-    assert mailer.send_messages(email)
-    sink = smtp_server.sink
-    assert len(sink) == 1
+
+    with SMTP(smtpd.hostname, smtpd.port):
+        assert mailer.send_messages(email)
+
+    assert len(smtpd.messages) == 1
+    message = smtpd.messages[0]
+    print(message)
+    assert message.get_content_type() == "text/plain"
+    assert message.get("subject") == "=?utf-8?q?Ol=C3=A9?="
 
 
-def test_notls():
-    mailer = SMTPMailer(host="127.0.0.1", port=SMTP_PORT, use_tls=True)
+def test_notls(smtpd):
+    mailer = SMTPMailer(host=smtpd.hostname, port=smtpd.port, use_tls=True)
     with pytest.raises(SMTPException):
-        mailer.open()
+        with SMTP(smtpd.hostname, smtpd.port):
+            mailer.open()
     mailer.close()
 
 
-def test_wrong_host():
-    mailer = SMTPMailer(host="123", port=SMTP_PORT, use_tls=False, timeout=0.5)
+def test_wrong_host(smtpd):
+    mailer = SMTPMailer(host="123", port=smtpd.port, use_tls=False, timeout=0.5)
     with pytest.raises(Exception):
-        mailer.open()
+        with SMTP(smtpd.hostname, smtpd.port):
+            mailer.open()
     mailer.close()
 
 
-def test_wrong_port():
-    mailer = SMTPMailer(host="127.0.0.1", port=3000, use_tls=False)
+def test_wrong_port(smtpd):
+    mailer = SMTPMailer(host=smtpd.hostname, port=3000, use_tls=False)
     with pytest.raises(Exception):
-        mailer.open()
+        with SMTP(smtpd.hostname, smtpd.port):
+            mailer.open()
     mailer.close()
 
 
-def test_fail_silently():
+def test_fail_silently(smtpd):
     mailer = SMTPMailer(
-        host="127.0.0.1", port=SMTP_PORT, use_tls=True, fail_silently=True
+        host=smtpd.hostname,
+        port=smtpd.port,
+        use_tls=True,
+        fail_silently=True,
     )
-    mailer.open()
+    with SMTP(smtpd.hostname, smtpd.port):
+        mailer.open()
     mailer.close()
 
     mailer = SMTPMailer(
-        host="123", port=SMTP_PORT, use_tls=False, fail_silently=True, timeout=0.5
+        host="123",
+        port=smtpd.port,
+        use_tls=False,
+        fail_silently=True,
+        timeout=0.5,
     )
-    mailer.open()
+    with SMTP(smtpd.hostname, smtpd.port):
+        mailer.open()
     mailer.close()
 
-    mailer = SMTPMailer(host="127.0.0.1", port=3000, use_tls=False, fail_silently=True)
-    mailer.open()
+    mailer = SMTPMailer(
+        host=smtpd.hostname,
+        port=3000,
+        use_tls=False,
+        fail_silently=True,
+    )
+    with SMTP(smtpd.hostname, smtpd.port):
+        mailer.open()
     mailer.close()
 
 
-def test_batch_too_many_recipients():
-    global smtp_server
-    smtp_server.flush_sink()
-
+def test_batch_too_many_recipients(smtpd):
     mailer = SMTPMailer(
-        host="127.0.0.1", port=SMTP_PORT, use_tls=False, max_recipients=200
+        host=smtpd.hostname,
+        port=smtpd.port,
+        use_tls=False,
+        max_recipients=200,
     )
     send_to = ["user{}@example.com".format(i) for i in range(1, 1501)]
     msg = EmailMessage("The Subject", "Content", "from@example.com", send_to)
 
-    assert mailer.send_messages(msg) == 1
-    sink = smtp_server.sink
-    assert len(sink) == 8
-
-    assert len(sink[0].get("to").split(",")) == 200
-    assert len(sink[1].get("to").split(",")) == 200
-    assert len(sink[2].get("to").split(",")) == 200
-    assert len(sink[3].get("to").split(",")) == 200
-    assert len(sink[4].get("to").split(",")) == 200
-    assert len(sink[5].get("to").split(",")) == 200
-    assert len(sink[6].get("to").split(",")) == 200
-    assert len(sink[7].get("to").split(",")) == 100
+    with SMTP(smtpd.hostname, smtpd.port):
+        assert mailer.send_messages(msg) == 1
+
+    assert len(smtpd.messages) == 8
+    assert len(smtpd.messages[0].get("to").split(",")) == 200
+    assert len(smtpd.messages[1].get("to").split(",")) == 200
+    assert len(smtpd.messages[2].get("to").split(",")) == 200
+    assert len(smtpd.messages[3].get("to").split(",")) == 200
+    assert len(smtpd.messages[4].get("to").split(",")) == 200
+    assert len(smtpd.messages[5].get("to").split(",")) == 200
+    assert len(smtpd.messages[6].get("to").split(",")) == 200
+    assert len(smtpd.messages[7].get("to").split(",")) == 100
```


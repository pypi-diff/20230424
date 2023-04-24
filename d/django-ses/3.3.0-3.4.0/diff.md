# Comparing `tmp/django_ses-3.3.0.tar.gz` & `tmp/django_ses-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-3.3.0.tar", max compression
+gzip compressed data, was "django_ses-3.4.0.tar", max compression
```

## Comparing `django_ses-3.3.0.tar` & `django_ses-3.4.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1057 2022-12-16 22:35:13.166651 django_ses-3.3.0/LICENSE
--rw-r--r--   0        0        0    21942 2022-12-16 22:35:13.166651 django_ses-3.3.0/README.rst
--rw-r--r--   0        0        0    13800 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/admin.py
--rw-r--r--   0        0        0      181 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/apps.py
--rw-r--r--   0        0        0       65 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/models.py
--rw-r--r--   0        0        0     2610 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/settings.py
--rw-r--r--   0        0        0      290 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      157 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/urls.py
--rw-r--r--   0        0        0     9218 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/utils.py
--rw-r--r--   0        0        0    20602 2022-12-16 22:35:13.166651 django_ses-3.3.0/django_ses/views.py
--rw-r--r--   0        0        0        0 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/__init__.py
--rw-r--r--   0        0        0       90 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/middleware.py
--rw-r--r--   0        0        0     2173 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/settings.py
--rw-r--r--   0        0        0      295 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/templates/base.html
--rw-r--r--   0        0        0      220 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/templates/index.html
--rw-r--r--   0        0        0      756 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/templates/send-email.html
--rw-r--r--   0        0        0      818 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/urls.py
--rw-r--r--   0        0        0      885 2022-12-16 22:35:13.166651 django_ses-3.3.0/example/views.py
--rw-r--r--   0        0        0     1560 2022-12-16 22:35:13.166651 django_ses-3.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-16 22:35:13.166651 django_ses-3.3.0/tests/__init__.py
--rw-r--r--   0        0        0    14752 2022-12-16 22:35:13.166651 django_ses-3.3.0/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2022-12-16 22:35:13.166651 django_ses-3.3.0/tests/test_commands.py
--rw-r--r--   0        0        0     2609 2022-12-16 22:35:13.166651 django_ses-3.3.0/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2022-12-16 22:35:13.170651 django_ses-3.3.0/tests/test_stats.py
--rw-r--r--   0        0        0      366 2022-12-16 22:35:13.170651 django_ses-3.3.0/tests/test_urls.py
--rw-r--r--   0        0        0    12140 2022-12-16 22:35:13.170651 django_ses-3.3.0/tests/test_verifier.py
--rw-r--r--   0        0        0    13333 2022-12-16 22:35:13.170651 django_ses-3.3.0/tests/test_views.py
--rw-r--r--   0        0        0      115 2022-12-16 22:35:13.170651 django_ses-3.3.0/tests/utils.py
--rw-r--r--   0        0        0    23680 1970-01-01 00:00:00.000000 django_ses-3.3.0/setup.py
--rw-r--r--   0        0        0    23659 1970-01-01 00:00:00.000000 django_ses-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-24 16:20:44.326568 django_ses-3.4.0/LICENSE
+-rw-r--r--   0        0        0    22379 2023-04-24 16:20:44.326568 django_ses-3.4.0/README.rst
+-rw-r--r--   0        0        0    13974 2023-04-24 16:20:44.326568 django_ses-3.4.0/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/models.py
+-rw-r--r--   0        0        0     2677 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      157 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/urls.py
+-rw-r--r--   0        0        0     9218 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/utils.py
+-rw-r--r--   0        0        0    20602 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/views.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/middleware.py
+-rw-r--r--   0        0        0     2173 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/settings.py
+-rw-r--r--   0        0        0      295 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/base.html
+-rw-r--r--   0        0        0      220 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/index.html
+-rw-r--r--   0        0        0      756 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/send-email.html
+-rw-r--r--   0        0        0      818 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/urls.py
+-rw-r--r--   0        0        0      885 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/views.py
+-rw-r--r--   0        0        0     1560 2023-04-24 16:20:44.330568 django_ses-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    15650 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_commands.py
+-rw-r--r--   0        0        0     2609 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_stats.py
+-rw-r--r--   0        0        0      366 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_urls.py
+-rw-r--r--   0        0        0    12140 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_verifier.py
+-rw-r--r--   0        0        0    13333 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_views.py
+-rw-r--r--   0        0        0      115 2023-04-24 16:20:44.334568 django_ses-3.4.0/tests/utils.py
+-rw-r--r--   0        0        0    24096 1970-01-01 00:00:00.000000 django_ses-3.4.0/PKG-INFO
```

### Comparing `django_ses-3.3.0/LICENSE` & `django_ses-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/README.rst` & `django_ses-3.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -475,17 +475,22 @@
 ``AWS_SES_REGION_NAME``, ``AWS_SES_REGION_ENDPOINT``
   Optionally specify what region your SES service is using. Note that this is
   required if your SES service is not using us-east-1, as omitting these settings
   implies this region. Details:
   http://readthedocs.org/docs/boto/en/latest/ref/ses.html#boto.ses.regions
   http://docs.aws.amazon.com/general/latest/gr/rande.html
 
+``AWS_SES_FROM_EMAIL``
+  Optional. The email address to be used as the "From" address for the email. The address that you specify has to be verified.  
+  For more information please refer to https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
 ``AWS_SES_RETURN_PATH``
-  Instruct Amazon SES to forward bounced emails and complaints to this email.
-  For more information please refer to http://aws.amazon.com/ses/faqs/#38
+  Optional. Use `AWS_SES_RETURN_PATH` to receive complaint notifications
+  You must use the v2 client by setting `USE_SES_V2=True` for this setting to work, otherwise it is ignored.
+  https://docs.aws.amazon.com/ses/latest/APIReference-V2/API_SendEmail.html#API_SendEmail_RequestSyntax
+
 
 ``AWS_SES_CONFIGURATION_SET``
   Optional. Use this to mark your e-mails as from being from a particular SES
   Configuration Set. Set this to a string if you want all messages to have the
   same configuration set.  Set this to a callable if you want to set
   configuration set on a per message basis.
```

### Comparing `django_ses-3.3.0/django_ses/__init__.py` & `django_ses-3.4.0/django_ses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 
         new_conn_created = self.open()
         if not self.connection:
             # Failed silently
             return
 
         num_sent = 0
-        source = settings.AWS_SES_RETURN_PATH
+        source = settings.AWS_SES_FROM_EMAIL
+        email_feedback = settings.AWS_SES_RETURN_PATH
         for message in email_messages:
             # SES Configuration sets. If the AWS_SES_CONFIGURATION_SET setting
             # is not None, append the appropriate header to the message so that
             # SES knows which configuration set it belongs to.
             #
             # If settings.AWS_SES_CONFIGURATION_SET is a callable, pass it the
             # message object and dkim settings and expect it to return a string
@@ -155,15 +156,15 @@
             # currently operating. The AWS_SES_AUTO_THROTTLE setting is a
             # factor to apply to the rate limit, with a default of 0.5 to stay
             # well below the actual SES throttle.
             # Set the setting to 0 or None to disable throttling.
             if self._throttle:
                 self._update_throttling()
 
-            kwargs = self._get_send_email_parameters(message, source)
+            kwargs = self._get_send_email_parameters(message, source, email_feedback)
 
             try:
                 response = (self.connection.send_email(**kwargs)
                             if self._use_ses_v2
                             else self.connection.send_raw_email(**kwargs))
                 message.extra_headers['status'] = 200
                 message.extra_headers['message_id'] = response['MessageId']
@@ -234,25 +235,26 @@
                                                    delta.days * 24 * 3600) * 10 ** 6) / 10 ** 6
             delay = window - total_seconds
             if delay > 0:
                 sleep(delay)
         recent_send_times.append(now)
         # end of throttling
 
-    def _get_send_email_parameters(self, message, source):
-        return (self._get_v2_parameters(message, source)
+    def _get_send_email_parameters(self, message, source, email_feedack):
+        return (self._get_v2_parameters(message, source, email_feedack)
                 if self._use_ses_v2
                 else self._get_v1_parameters(message, source))
 
-    def _get_v2_parameters(self, message, source):
+    def _get_v2_parameters(self, message, source, email_feedback):
         """V2-Style raw payload for `send_email`.
 
         https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
         """
         params = dict(
+            FeedbackForwardingEmailAddress=email_feedback,
             FromEmailAddress=source or message.from_email,
             Destination={
                 'ToAddresses': message.recipients()
             },
             Content={
                 'Raw': {
                     'Data': dkim_sign(message.message().as_string(),
```

### Comparing `django_ses-3.3.0/django_ses/management/commands/get_ses_statistics.py` & `django_ses-3.4.0/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/django_ses/management/commands/ses_email_address.py` & `django_ses-3.4.0/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/django_ses/migrations/0001_initial.py` & `django_ses-3.4.0/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/django_ses/settings.py` & `django_ses-3.4.0/django_ses/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                        ('From', 'To', 'Cc', 'Subject'))
 
 AWS_SES_SOURCE_ARN = getattr(settings, 'AWS_SES_SOURCE_ARN', None)
 AWS_SES_FROM_ARN = getattr(settings, 'AWS_SES_FROM_ARN', None)
 AWS_SES_RETURN_PATH_ARN = getattr(settings, 'AWS_SES_RETURN_PATH_ARN', None)
 
 USE_SES_V2 = getattr(settings, 'USE_SES_V2', False)
+AWS_SES_FROM_EMAIL = getattr(settings, 'AWS_SES_FROM_EMAIL', None)
 
 TIME_ZONE = settings.TIME_ZONE
 
 VERIFY_EVENT_SIGNATURES = getattr(settings, 'AWS_SES_VERIFY_EVENT_SIGNATURES',
                                   getattr(settings, 'AWS_SES_VERIFY_BOUNCE_SIGNATURES', True))
 VERIFY_BOUNCE_SIGNATURES = VERIFY_EVENT_SIGNATURES
```

### Comparing `django_ses-3.3.0/django_ses/templates/django_ses/send_stats.html` & `django_ses-3.4.0/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/django_ses/utils.py` & `django_ses-3.4.0/django_ses/utils.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/django_ses/views.py` & `django_ses-3.4.0/django_ses/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/example/settings.py` & `django_ses-3.4.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/example/templates/send-email.html` & `django_ses-3.4.0/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/example/urls.py` & `django_ses-3.4.0/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/example/views.py` & `django_ses-3.4.0/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/pyproject.toml` & `django_ses-3.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ses"
-version = "3.3.0"
+version = "3.4.0"
 description = "A Django email backend for Amazon's Simple Email Service"
 authors = [
     "Harry Marr <harry@hmarr.com>",
     "Wes Winham <winhamwr@gmail.com>",
     "Ross Lawley <ross.lawley@gmail.com>",
     "Paul Craciunoiu <paul@craciunoiu.net>",
 ]
```

### Comparing `django_ses-3.3.0/tests/test_backend.py` & `django_ses-3.4.0/tests/test_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         # ensure we passed in the proper arguments to our callable
         self.assertEqual(config_set_callable.message.subject, 'subject')
         self.assertEqual(config_set_callable.dkim_domain, None)
         self.assertEqual(config_set_callable.dkim_key, None)
         self.assertEqual(config_set_callable.dkim_selector, 'ses')
         self.assertEqual(config_set_callable.dkim_headers, ('From', 'To', 'Cc', 'Subject'))
 
+
 class SESV2BackendTest(TestCase):
     def setUp(self):
         django_settings.EMAIL_BACKEND = 'tests.test_backend.FakeSESBackend'
         settings.USE_SES_V2 = True
         settings.AWS_SES_FROM_ARN = None
         settings.AWS_SES_SOURCE_ARN = None
         django_ses.boto3.client = FakeSESConnection
@@ -255,17 +256,26 @@
         self.assertFalse(dkim.verify(
                             message.replace('from@example.com', 'from@spam.com')))
 
     def test_return_path(self):
         """Ensure that the 'Source' argument sent into send_raw_email uses FromEmailAddress.
         """
         settings.AWS_SES_RETURN_PATH = None
+        settings.AWS_SES_FROM_EMAIL = 'from@example.com'
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         self.assertEqual(self.outbox.pop()['FromEmailAddress'], 'from@example.com')
 
+    def test_feedback_forwarding(self):
+        """
+        Ensure that the notification address argument uses FeedbackForwardingEmailAddress.
+        """
+        settings.AWS_SES_RETURN_PATH = 'reply@example.com'
+        send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
+        self.assertEqual(self.outbox.pop()['FeedbackForwardingEmailAddress'], 'reply@example.com')
+
     def test_source_arn_is_NOT_set(self):
         """
         Ensure that the helpers for Identity Owner for SES Sending Authorization are not present, if nothing has been
         configured.
         """
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         mail = self.outbox.pop()
@@ -320,12 +330,21 @@
         django_settings.EMAIL_BACKEND = 'tests.test_backend.FakeSESBackend'
         django_ses.SESConnection = FakeSESConnection
         self.outbox = FakeSESConnection.outbox
 
     def tearDown(self):
         # Empty outbox everytime test finishes
         FakeSESConnection.outbox = []
-
+    
+    def test_from_email(self):
+        settings.AWS_SES_FROM_EMAIL = "my_default_from@example.com"
+        send_mail('subject', 'body', 'ignored_from@example.com', ['to@example.com'])
+        self.assertEqual(self.outbox.pop()['Source'], 'my_default_from@example.com')
+    
     def test_return_path(self):
+        settings.USE_SES_V2 = True
         settings.AWS_SES_RETURN_PATH = "return@example.com"
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
-        self.assertEqual(self.outbox.pop()['Source'], 'return@example.com')
+        message = self.outbox.pop()
+
+        self.assertEqual(message['FromEmailAddress'], 'my_default_from@example.com')
+        self.assertEqual(message['FeedbackForwardingEmailAddress'], 'return@example.com')
```

### Comparing `django_ses-3.3.0/tests/test_commands.py` & `django_ses-3.4.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/tests/test_settings.py` & `django_ses-3.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/tests/test_stats.py` & `django_ses-3.4.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/tests/test_verifier.py` & `django_ses-3.4.0/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/tests/test_views.py` & `django_ses-3.4.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.3.0/setup.py` & `django_ses-3.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,638 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-ses
+Version: 3.4.0
+Summary: A Django email backend for Amazon's Simple Email Service
+Home-page: https://github.com/django-ses/django-ses
+License: MIT
+Author: Harry Marr
+Author-email: harry@hmarr.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: bounce
+Provides-Extra: events
+Requires-Dist: boto3 (>=1.0.0)
+Requires-Dist: cryptography (>=36.0.2) ; extra == "bounce" or extra == "events"
+Requires-Dist: django (>=2.2)
+Requires-Dist: importlib-metadata (>=1) ; python_version < "3.8"
+Requires-Dist: pytz (>=2016.10)
+Requires-Dist: requests (>=2.27.1) ; extra == "bounce" or extra == "events"
+Project-URL: Repository, https://github.com/django-ses/django-ses
+Description-Content-Type: text/x-rst
 
-packages = \
-['django_ses',
- 'django_ses.management',
- 'django_ses.management.commands',
- 'django_ses.migrations']
-
-package_data = \
-{'': ['*'], 'django_ses': ['templates/django_ses/*']}
-
-install_requires = \
-['boto3>=1.0.0', 'django>=2.2', 'pytz>=2016.10']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=1'],
- 'bounce': ['cryptography>=36.0.2', 'requests>=2.27.1'],
- 'events': ['cryptography>=36.0.2', 'requests>=2.27.1']}
-
-setup_kwargs = {
-    'name': 'django-ses',
-    'version': '3.3.0',
-    'description': "A Django email backend for Amazon's Simple Email Service",
-    'long_description': '==========\nDjango-SES\n==========\n:Info: A Django email backend for Amazon\'s Simple Email Service\n:Author: Harry Marr (http://github.com/hmarr, http://twitter.com/harrymarr)\n:Collaborators: Paul Craciunoiu (http://github.com/pcraciunoiu, http://twitter.com/embrangler)\n\n|pypi| |build| |python| |django|\n\nA bird\'s eye view\n=================\nDjango-SES is a drop-in mail backend for Django_. Instead of sending emails\nthrough a traditional SMTP mail server, Django-SES routes email through\nAmazon Web Services\' excellent Simple Email Service (SES_).\n\n\nPlease Contribute!\n==================\nThis project is maintained, but not actively used by the maintainer. Interested\nin helping maintain this project? Reach out via GitHub Issues if you\'re actively\nusing `django-ses` and would be interested in contributing to it.\n\n\nChangelog\n=========\n\nFor details about each release, see the GitHub releases page: https://github.com/django-ses/django-ses/releases or CHANGES.md.\n\n\nUsing Django directly\n=====================\n\nAmazon SES allows you to also setup usernames and passwords. If you do configure\nthings that way, you do not need this package. The Django default email backend\nis capable of authenticating with Amazon SES and correctly sending email.\n\nUsing django-ses gives you additional features like deliverability reports that\ncan be hard and/or cumbersome to obtain when using the SMTP interface.\n\n\nWhy SES instead of SMTP?\n========================\nConfiguring, maintaining, and dealing with some complicated edge cases can be\ntime-consuming. Sending emails with Django-SES might be attractive to you if:\n\n* You don\'t want to maintain mail servers.\n* You are already deployed on EC2 (In-bound traffic to SES is free from EC2\n  instances).\n* You need to send a high volume of email.\n* You don\'t want to have to worry about PTR records, Reverse DNS, email\n  whitelist/blacklist services.\n* You want to improve delivery rate and inbox cosmetics by DKIM signing\n  your messages using SES\'s Easy DKIM feature.\n* Django-SES is a truely drop-in replacement for the default mail backend.\n  Your code should require no changes.\n\nGetting going\n=============\nAssuming you\'ve got Django_ installed, you\'ll just need to install django-ses::\n\n    pip install django-ses\n\n\nTo receive bounces or webhook events install the events "extra"::\n\n    pip install django-ses[events]\n\nAdd the following to your settings.py::\n\n    EMAIL_BACKEND = \'django_ses.SESBackend\'\n\n    # These are optional -- if they\'re set as environment variables they won\'t\n    # need to be set here as well\n    AWS_ACCESS_KEY_ID = \'YOUR-ACCESS-KEY-ID\'\n    AWS_SECRET_ACCESS_KEY = \'YOUR-SECRET-ACCESS-KEY\'\n\n    # Additionally, if you are not using the default AWS region of us-east-1,\n    # you need to specify a region, like so:\n    AWS_SES_REGION_NAME = \'us-west-2\'\n    AWS_SES_REGION_ENDPOINT = \'email.us-west-2.amazonaws.com\'\n\n    # If you want to use the SESv2 client\n    USE_SES_V2 = True\n\nAlternatively, instead of `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`, you\ncan include the following two settings values. This is useful in situations\nwhere you would like to use a separate access key to send emails via SES than\nyou would to upload files via S3::\n\n    AWS_SES_ACCESS_KEY_ID = \'YOUR-ACCESS-KEY-ID\'\n    AWS_SES_SECRET_ACCESS_KEY = \'YOUR-SECRET-ACCESS-KEY\'\n\nNow, when you use ``django.core.mail.send_mail``, Simple Email Service will\nsend the messages by default.\n\nSince SES imposes a rate limit and will reject emails after the limit has been\nreached, django-ses will attempt to conform to the rate limit by querying the\nAPI for your current limit and then sending no more than that number of\nmessages in a two-second period (which is half of the rate limit, just to\nbe sure to stay clear of the limit). This is controlled by the following setting:\n\n    AWS_SES_AUTO_THROTTLE = 0.5 # (default; safety factor applied to rate limit)\n\nTo turn off automatic throttling, set this to None.\n\nCheck out the ``example`` directory for more information.\n\nMonitoring email status using Amazon Simple Notification Service (Amazon SNS)\n=============================================================================\nTo set this up, install `django-ses` with the `events` extra::\n\n    pip install django-ses[events]\n\nThen add a event url handler in your `urls.py`::\n\n    from django_ses.views import SESEventWebhookView\n    from django.views.decorators.csrf import csrf_exempt\n    urlpatterns = [ ...\n                    url(r\'^ses/event-webhook/$\', SESEventWebhookView.as_view(), name=\'handle-event-webhook\'),\n                    ...\n    ]\n\nSESEventWebhookView handles bounce, complaint, send, delivery, open and click events.\nIt is also capable of auto confirming subscriptions, it handles `SubscriptionConfirmation` notification.\n\nOn AWS\n-------\n1. Add an SNS topic.\n\n2. In SES setup an SNS destination in "Configuration Sets". Use this\nconfiguration set by setting ``AWS_SES_CONFIGURATION_SET``. Set the topic\nto what you created in 1.\n\n3. Add an https subscriber to the topic. (eg. https://www.yourdomain.com/ses/event-webhook/)\nDo not check "Enable raw message delivery".\n\n\nBounces\n-------\nUsing signal \'bounce_received\' for manager bounce email. For example::\n\n    from django_ses.signals import bounce_received\n    from django.dispatch import receiver\n\n\n    @receiver(bounce_received)\n    def bounce_handler(sender, mail_obj, bounce_obj, raw_message, *args, **kwargs):\n        # you can then use the message ID and/or recipient_list(email address) to identify any problematic email messages that you have sent\n        message_id = mail_obj[\'messageId\']\n        recipient_list = mail_obj[\'destination\']\n        ...\n        print("This is bounce email object")\n        print(mail_obj)\n\nComplaint\n---------\nUsing signal \'complaint_received\' for manager complaint email. For example::\n\n    from django_ses.signals import complaint_received\n    from django.dispatch import receiver\n\n\n    @receiver(complaint_received)\n    def complaint_handler(sender, mail_obj, complaint_obj, raw_message,  *args, **kwargs):\n        ...\n\nSend\n----\nUsing signal \'send_received\' for manager send email. For example::\n\n    from django_ses.signals import send_received\n    from django.dispatch import receiver\n\n\n    @receiver(send_received)\n    def send_handler(sender, mail_obj, raw_message,  *args, **kwargs):\n        ...\n\nDelivery\n--------\nUsing signal \'delivery_received\' for manager delivery email. For example::\n\n    from django_ses.signals import delivery_received\n    from django.dispatch import receiver\n\n\n    @receiver(delivery_received)\n    def delivery_handler(sender, mail_obj, delivery_obj, raw_message,  *args, **kwargs):\n        ...\n\nOpen\n----\nUsing signal \'open_received\' for manager open email. For example::\n\n    from django_ses.signals import open_received\n    from django.dispatch import receiver\n\n\n    @receiver(open_received)\n    def open_handler(sender, mail_obj, raw_message, *args, **kwargs):\n        ...\n\nClick\n-----\nUsing signal \'click_received\' for manager send email. For example::\n\n    from django_ses.signals import click_received\n    from django.dispatch import receiver\n\n\n    @receiver(click_received)\n    def click_handler(sender, mail_obj, raw_message, *args, **kwargs):\n        ...\n        \nTesting Signals\n===============\n\nIf you would like to test your signals, you can optionally disable `AWS_SES_VERIFY_EVENT_SIGNATURES` in settings. Examples for the JSON object AWS SNS sends can be found here: https://docs.aws.amazon.com/sns/latest/dg/sns-message-and-json-formats.html#http-subscription-confirmation-json\n\nSES Event Monitoring with Configuration Sets\n============================================\n\nYou can track your SES email sending at a granular level using `SES Event Publishing`_.\nTo do this, you set up an SES Configuration Set and add event\nhandlers to it to send your events on to a destination within AWS (SNS,\nCloudwatch or Kinesis Firehose) for further processing and analysis.\n\nTo ensure that emails you send via `django-ses` will be tagged with your\nSES Configuration Set, set the `AWS_SES_CONFIGURATION_SET` setting in your\nsettings.py to the name of the configuration set::\n\n    AWS_SES_CONFIGURATION_SET = \'my-configuration-set-name\'\n\nThis will add the `X-SES-CONFIGURATION-SET` header to all your outgoing\ne-mails.\n\nIf you want to set the SES Configuration Set on a per message basis, set\n`AWS_SES_CONFIGURATION_SET` to a callable.  The callable should conform to the\nfollowing prototype::\n\n    def ses_configuration_set(message, dkim_domain=None, dkim_key=None,\n                                dkim_selector=None, dkim_headers=()):\n        configuration_set = \'my-default-set\'\n        # use message and dkim_* to modify configuration_set\n        return configuration_set\n\n    AWS_SES_CONFIGURATION_SET = ses_configuration_set\n\nwhere\n\n* `message` is a `django.core.mail.EmailMessage` object (or subclass)\n* `dkim_domain` is a string containing the DKIM domain for this message\n* `dkim_key` is a string containing the DKIM private key for this message\n* `dkim_selector` is a string containing the DKIM selector (see DKIM, below for\n  explanation)\n* `dkim_headers` is a list of strings containing the names of the headers to\n  be DKIM signed (see DKIM, below for explanation)\n\nDKIM\n====\n\nUsing DomainKeys_ is entirely optional, however it is recommended by Amazon for\nauthenticating your email address and improving delivery success rate.  See\nhttp://docs.amazonwebservices.com/ses/latest/DeveloperGuide/DKIM.html.\nBesides authentication, you might also want to consider using DKIM in order to\nremove the `via email-bounces.amazonses.com` message shown to gmail users -\nsee http://support.google.com/mail/bin/answer.py?hl=en&answer=1311182.\n\nCurrently there are two methods to use DKIM with Django-SES: traditional Manual\nSigning and the more recently introduced Amazon Easy DKIM feature.\n\nEasy DKIM\n---------\nEasy DKIM is a feature of Amazon SES that automatically signs every message\nthat you send from a verified email address or domain with a DKIM signature.\n\nYou can enable Easy DKIM in the AWS Management Console for SES. There you can\nalso add the required domain verification and DKIM records to Route 53 (or\ncopy them to your alternate DNS).\n\nOnce enabled and verified Easy DKIM needs no additional dependencies or\nDKIM specific settings to work with Django-SES.\n\nFor more information and a setup guide see:\nhttp://docs.aws.amazon.com/ses/latest/DeveloperGuide/easy-dkim.html\n\nManual DKIM Signing\n-------------------\nTo enable Manual DKIM Signing you should install the pydkim_ package and specify values\nfor the ``DKIM_PRIVATE_KEY`` and ``DKIM_DOMAIN`` settings.  You can generate a\nprivate key with a command such as ``openssl genrsa 512`` and get the public key\nportion with ``openssl rsa -pubout <private.key``.  The public key should be\npublished to ``ses._domainkey.example.com`` if your domain is example.com.  You\ncan use a different name instead of ``ses`` by changing the ``DKIM_SELECTOR``\nsetting.\n\nThe SES relay will modify email headers such as `Date` and `Message-Id` so by\ndefault only the `From`, `To`, `Cc`, `Subject` headers are signed, not the full\nset of headers.  This is sufficient for most DKIM validators but can be overridden\nwith the ``DKIM_HEADERS`` setting.\n\n\nExample settings.py::\n\n   DKIM_DOMAIN = \'example.com\'\n   DKIM_PRIVATE_KEY = \'\'\'\n   -----BEGIN RSA PRIVATE KEY-----\n   xxxxxxxxxxx\n   -----END RSA PRIVATE KEY-----\n   \'\'\'\n\nExample DNS record published to Route53 with boto:\n\n   route53 add_record ZONEID ses._domainkey.example.com. TXT \'"v=DKIM1; p=xxx"\' 86400\n\n\n.. _DomainKeys: http://dkim.org/\n\n\nIdentity Owners\n===============\n\nWith Identity owners, you can use validated SES-domains across multiple accounts:\nhttps://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html\n\nThis is useful if you got multiple environments in different accounts and still want to send mails via the same domain.\n\nYou can configure the following environment variables to use them as described in boto3-docs_::\n\n    AWS_SES_SOURCE_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com\n    AWS_SES_FROM_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com\n    AWS_SES_RETURN_PATH_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com\n\n.. _boto3-docs: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.send_raw_email\n\n\nSES Sending Stats\n=================\n\nDjango SES comes with two ways of viewing sending statistics.\n\nThe first one is a simple read-only report on your 24 hour sending quota,\nverified email addresses and bi-weekly sending statistics.\n\nTo generate and view SES sending statistics reports, include, update\n``INSTALLED_APPS``::\n\n    INSTALLED_APPS = (\n        # ...\n        \'django.contrib.admin\',\n        \'django_ses\',\n        # ...\n    )\n\n... and ``urls.py``::\n\n    urlpatterns += (url(r\'^admin/django-ses/\', include(\'django_ses.urls\')),)\n\n*Optional enhancements to stats:*\n\nOverride the dashboard view\n---------------------------\nYou can override the Dashboard view, for example, to add more context data::\n\n    class CustomSESDashboardView(DashboardView):\n        def get_context_data(self, **kwargs):\n            context = super().get_context_data(**kwargs)\n            context.update(**admin.site.each_context(self.request))\n            return context\n\nThen update your urls::\n\n    urlpatterns += path(\'admin/django-ses/\', CustomSESDashboardView.as_view(), name=\'django_ses_stats\'),\n\n\nLink the dashboard from the admin\n---------------------------------\nYou can use adminplus for this (https://github.com/jsocol/django-adminplus)::\n\n    from django_ses.views import DashboardView\n    admin.site.register_view(\'django-ses\', DashboardView.as_view(), \'Django SES Stats\')\n\n\n\nStore daily stats\n-----------------\nIf you need to keep send statistics around for longer than two weeks,\ndjango-ses also comes with a model that lets you store these. To use this\nfeature you\'ll need to run::\n\n    python manage.py migrate\n\nTo collect the statistics, run the ``get_ses_statistics`` management command\n(refer to next section for details). After running this command the statistics\nwill be viewable via ``/admin/django_ses/``.\n\nDjango SES Management Commands\n==============================\n\nTo use these you must include ``django_ses`` in your INSTALLED_APPS.\n\nManaging Verified Email Addresses\n---------------------------------\n\nManage verified email addresses through the management command.\n\n    python manage.py ses_email_address --list\n\nAdd emails to the verified email list through:\n\n    python manage.py ses_email_address --add john.doe@example.com\n\nRemove emails from the verified email list through:\n\n    python manage.py ses_email_address --delete john.doe@example.com\n\nYou can toggle the console output through setting the verbosity level.\n\n    python manage.py ses_email_address --list --verbosity 0\n\n\nCollecting Sending Statistics\n-----------------------------\n\nTo collect and store SES sending statistics in the database, run:\n\n    python manage.py get_ses_statistics\n\nSending statistics are aggregated daily (UTC time). Stats for the latest day\n(when you run the command) may be inaccurate if run before end of day (UTC).\nIf you want to keep your statistics up to date, setup ``cron`` to run this\ncommand a short time after midnight (UTC) daily.\n\n\nDjango Builtin-in Error Emails\n==============================\n\nIf you\'d like Django\'s `Builtin Email Error Reporting`_ to function properly\n(actually send working emails), you\'ll have to explicitly set the\n``SERVER_EMAIL`` setting to one of your SES-verified addresses. Otherwise, your\nerror emails will all fail and you\'ll be blissfully unaware of a problem.\n\n*Note:* You will need to sign up for SES_ and verify any emails you\'re going\nto use in the `from_email` argument to `django.core.mail.send_email()`. Boto_\nhas a `verify_email_address()` method: https://github.com/boto/boto/blob/master/boto/ses/connection.py\n\n.. _Builtin Email Error Reporting: https://docs.djangoproject.com/en/dev/howto/error-reporting/\n.. _Django: http://djangoproject.com\n.. _Boto: http://boto.cloudhackers.com/\n.. _SES: http://aws.amazon.com/ses/\n.. _SES Event Publishing: https://docs.aws.amazon.com/ses/latest/DeveloperGuide/monitor-using-event-publishing.html\n\n\nRequirements\n============\ndjango-ses requires supported version of Django or Python.\n\n\nFull List of Settings\n=====================\n\n``AWS_ACCESS_KEY_ID``, ``AWS_SECRET_ACCESS_KEY``\n  *Required.* Your API keys for Amazon SES.\n\n``AWS_SES_ACCESS_KEY_ID``, ``AWS_SES_SECRET_ACCESS_KEY``\n  *Required.* Alternative API keys for Amazon SES. This is useful in situations\n  where you would like to use separate access keys for different AWS services.\n\n``AWS_SES_SESSION_TOKEN``, ``AWS_SES_SECRET_ACCESS_KEY``\n  Optional. Use `AWS_SES_SESSION_TOKEN` to provide session token\n  when temporary credentials are used. Details:\n  https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html\n  https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_use-resources.html\n\n``AWS_SES_REGION_NAME``, ``AWS_SES_REGION_ENDPOINT``\n  Optionally specify what region your SES service is using. Note that this is\n  required if your SES service is not using us-east-1, as omitting these settings\n  implies this region. Details:\n  http://readthedocs.org/docs/boto/en/latest/ref/ses.html#boto.ses.regions\n  http://docs.aws.amazon.com/general/latest/gr/rande.html\n\n``AWS_SES_RETURN_PATH``\n  Instruct Amazon SES to forward bounced emails and complaints to this email.\n  For more information please refer to http://aws.amazon.com/ses/faqs/#38\n\n``AWS_SES_CONFIGURATION_SET``\n  Optional. Use this to mark your e-mails as from being from a particular SES\n  Configuration Set. Set this to a string if you want all messages to have the\n  same configuration set.  Set this to a callable if you want to set\n  configuration set on a per message basis.\n\n``TIME_ZONE``\n  Default Django setting, optionally set this. Details:\n  https://docs.djangoproject.com/en/dev/ref/settings/#time-zone\n\n``DKIM_DOMAIN``, ``DKIM_PRIVATE_KEY``\n  Optional. If these settings are defined and the pydkim_ module is installed\n  then email messages will be signed with the specified key.   You will also\n  need to publish your public key on DNS; the selector is set to ``ses`` by\n  default.  See http://dkim.org/ for further detail.\n\n``AWS_SES_SOURCE_ARN``\n  Instruct Amazon SES to use a domain from another account.\n  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html\n\n``AWS_SES_FROM_ARN``\n  Instruct Amazon SES to use a domain from another account.\n  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html\n\n``AWS_SES_RETURN_PATH_ARN``\n  Instruct Amazon SES to use a domain from another account.\n  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html\n\n``AWS_SES_VERIFY_EVENT_SIGNATURES``, ``AWS_SES_VERIFY_BOUNCE_SIGNATURES``\n  Optional. Default is True. Verify the contents of the message by matching the signature\n  you recreated from the message contents with the signature that Amazon SNS sent with the message.\n  See https://docs.aws.amazon.com/sns/latest/dg/sns-verify-signature-of-message.html for further detail.\n\n``EVENT_CERT_DOMAINS``, ``BOUNCE_CERT_DOMAINS``\n  Optional. Default is \'amazonaws.com\' and \'amazon.com\'.\n\n.. _pydkim: http://hewgill.com/pydkim/\n\nProxy\n=====\n\nIf you are using a proxy, please enable it via the env variables.\n\nIf your proxy server does not have a password try the following:\n\n.. code-block:: python\n\n   import os\n   os.environ["HTTP_PROXY"] = "http://proxy.com:port"\n   os.environ["HTTPS_PROXY"] = "https://proxy.com:port"\n\nif your proxy server has a password try the following:\n\n.. code-block:: python\n\n   import os\n   os.environ["HTTP_PROXY"] = "http://user:password@proxy.com:port"\n   os.environ["HTTPS_PROXY"] = "https://user:password@proxy.com:port"\n\nSource: https://stackoverflow.com/a/33501223/1331671\n\nContributing\n============\nIf you\'d like to fix a bug, add a feature, etc\n\n#. Start by opening an issue.\n    Be explicit so that project collaborators can understand and reproduce the\n    issue, or decide whether the feature falls within the project\'s goals.\n    Code examples can be useful, too.\n\n#. File a pull request.\n    You may write a prototype or suggested fix.\n\n#. Check your code for errors, complaints.\n    Use `check.py <https://github.com/jbalogh/check>`_\n\n#. Write and run tests.\n    Write your own test showing the issue has been resolved, or the feature\n    works as intended.\n\nRunning Tests\n=============\nTo run the tests::\n\n    python runtests.py\n\nIf you want to debug the tests, just add this file as a python script to your IDE run configuration.\n\nCreating a Release\n==================\n\nTo create a release:\n\n* Run ``poetry version {patch|minor|major}`` as explained in `the docs <https://python-poetry.org/docs/cli/#version>`_. This will update the version in pyproject.toml.\n* Commit that change and use git to tag that commit with a version that matches the pattern ``v*.*.*``.\n* Push the tag and the commit (note some IDEs don\'t push tags by default).\n\n\n.. |pypi| image:: https://badge.fury.io/py/django-ses.svg\n    :target: http://badge.fury.io/py/django-ses\n.. |build| image:: https://github.com/django-ses/django-ses/actions/workflows/ci.yml/badge.svg\n    :target: https://github.com/django-ses/django-ses/actions/workflows/ci.yml\n.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg\n    :target: https://pypi.org/project/django-ses/\n.. |django| image:: https://img.shields.io/badge/django-2.2%7C%203.2+-blue.svg\n    :target: https://www.djangoproject.com/\n',
-    'author': 'Harry Marr',
-    'author_email': 'harry@hmarr.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/django-ses/django-ses',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+==========
+Django-SES
+==========
+:Info: A Django email backend for Amazon's Simple Email Service
+:Author: Harry Marr (http://github.com/hmarr, http://twitter.com/harrymarr)
+:Collaborators: Paul Craciunoiu (http://github.com/pcraciunoiu, http://twitter.com/embrangler)
 
+|pypi| |build| |python| |django|
+
+A bird's eye view
+=================
+Django-SES is a drop-in mail backend for Django_. Instead of sending emails
+through a traditional SMTP mail server, Django-SES routes email through
+Amazon Web Services' excellent Simple Email Service (SES_).
+
+
+Please Contribute!
+==================
+This project is maintained, but not actively used by the maintainer. Interested
+in helping maintain this project? Reach out via GitHub Issues if you're actively
+using `django-ses` and would be interested in contributing to it.
+
+
+Changelog
+=========
+
+For details about each release, see the GitHub releases page: https://github.com/django-ses/django-ses/releases or CHANGES.md.
+
+
+Using Django directly
+=====================
+
+Amazon SES allows you to also setup usernames and passwords. If you do configure
+things that way, you do not need this package. The Django default email backend
+is capable of authenticating with Amazon SES and correctly sending email.
+
+Using django-ses gives you additional features like deliverability reports that
+can be hard and/or cumbersome to obtain when using the SMTP interface.
+
+
+Why SES instead of SMTP?
+========================
+Configuring, maintaining, and dealing with some complicated edge cases can be
+time-consuming. Sending emails with Django-SES might be attractive to you if:
+
+* You don't want to maintain mail servers.
+* You are already deployed on EC2 (In-bound traffic to SES is free from EC2
+  instances).
+* You need to send a high volume of email.
+* You don't want to have to worry about PTR records, Reverse DNS, email
+  whitelist/blacklist services.
+* You want to improve delivery rate and inbox cosmetics by DKIM signing
+  your messages using SES's Easy DKIM feature.
+* Django-SES is a truely drop-in replacement for the default mail backend.
+  Your code should require no changes.
+
+Getting going
+=============
+Assuming you've got Django_ installed, you'll just need to install django-ses::
+
+    pip install django-ses
+
+
+To receive bounces or webhook events install the events "extra"::
+
+    pip install django-ses[events]
+
+Add the following to your settings.py::
+
+    EMAIL_BACKEND = 'django_ses.SESBackend'
+
+    # These are optional -- if they're set as environment variables they won't
+    # need to be set here as well
+    AWS_ACCESS_KEY_ID = 'YOUR-ACCESS-KEY-ID'
+    AWS_SECRET_ACCESS_KEY = 'YOUR-SECRET-ACCESS-KEY'
+
+    # Additionally, if you are not using the default AWS region of us-east-1,
+    # you need to specify a region, like so:
+    AWS_SES_REGION_NAME = 'us-west-2'
+    AWS_SES_REGION_ENDPOINT = 'email.us-west-2.amazonaws.com'
+
+    # If you want to use the SESv2 client
+    USE_SES_V2 = True
+
+Alternatively, instead of `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`, you
+can include the following two settings values. This is useful in situations
+where you would like to use a separate access key to send emails via SES than
+you would to upload files via S3::
+
+    AWS_SES_ACCESS_KEY_ID = 'YOUR-ACCESS-KEY-ID'
+    AWS_SES_SECRET_ACCESS_KEY = 'YOUR-SECRET-ACCESS-KEY'
+
+Now, when you use ``django.core.mail.send_mail``, Simple Email Service will
+send the messages by default.
+
+Since SES imposes a rate limit and will reject emails after the limit has been
+reached, django-ses will attempt to conform to the rate limit by querying the
+API for your current limit and then sending no more than that number of
+messages in a two-second period (which is half of the rate limit, just to
+be sure to stay clear of the limit). This is controlled by the following setting:
+
+    AWS_SES_AUTO_THROTTLE = 0.5 # (default; safety factor applied to rate limit)
+
+To turn off automatic throttling, set this to None.
+
+Check out the ``example`` directory for more information.
+
+Monitoring email status using Amazon Simple Notification Service (Amazon SNS)
+=============================================================================
+To set this up, install `django-ses` with the `events` extra::
+
+    pip install django-ses[events]
+
+Then add a event url handler in your `urls.py`::
+
+    from django_ses.views import SESEventWebhookView
+    from django.views.decorators.csrf import csrf_exempt
+    urlpatterns = [ ...
+                    url(r'^ses/event-webhook/$', SESEventWebhookView.as_view(), name='handle-event-webhook'),
+                    ...
+    ]
+
+SESEventWebhookView handles bounce, complaint, send, delivery, open and click events.
+It is also capable of auto confirming subscriptions, it handles `SubscriptionConfirmation` notification.
+
+On AWS
+-------
+1. Add an SNS topic.
+
+2. In SES setup an SNS destination in "Configuration Sets". Use this
+configuration set by setting ``AWS_SES_CONFIGURATION_SET``. Set the topic
+to what you created in 1.
+
+3. Add an https subscriber to the topic. (eg. https://www.yourdomain.com/ses/event-webhook/)
+Do not check "Enable raw message delivery".
+
+
+Bounces
+-------
+Using signal 'bounce_received' for manager bounce email. For example::
+
+    from django_ses.signals import bounce_received
+    from django.dispatch import receiver
+
+
+    @receiver(bounce_received)
+    def bounce_handler(sender, mail_obj, bounce_obj, raw_message, *args, **kwargs):
+        # you can then use the message ID and/or recipient_list(email address) to identify any problematic email messages that you have sent
+        message_id = mail_obj['messageId']
+        recipient_list = mail_obj['destination']
+        ...
+        print("This is bounce email object")
+        print(mail_obj)
+
+Complaint
+---------
+Using signal 'complaint_received' for manager complaint email. For example::
+
+    from django_ses.signals import complaint_received
+    from django.dispatch import receiver
+
+
+    @receiver(complaint_received)
+    def complaint_handler(sender, mail_obj, complaint_obj, raw_message,  *args, **kwargs):
+        ...
+
+Send
+----
+Using signal 'send_received' for manager send email. For example::
+
+    from django_ses.signals import send_received
+    from django.dispatch import receiver
+
+
+    @receiver(send_received)
+    def send_handler(sender, mail_obj, raw_message,  *args, **kwargs):
+        ...
+
+Delivery
+--------
+Using signal 'delivery_received' for manager delivery email. For example::
+
+    from django_ses.signals import delivery_received
+    from django.dispatch import receiver
+
+
+    @receiver(delivery_received)
+    def delivery_handler(sender, mail_obj, delivery_obj, raw_message,  *args, **kwargs):
+        ...
+
+Open
+----
+Using signal 'open_received' for manager open email. For example::
+
+    from django_ses.signals import open_received
+    from django.dispatch import receiver
+
+
+    @receiver(open_received)
+    def open_handler(sender, mail_obj, raw_message, *args, **kwargs):
+        ...
+
+Click
+-----
+Using signal 'click_received' for manager send email. For example::
+
+    from django_ses.signals import click_received
+    from django.dispatch import receiver
+
+
+    @receiver(click_received)
+    def click_handler(sender, mail_obj, raw_message, *args, **kwargs):
+        ...
+        
+Testing Signals
+===============
+
+If you would like to test your signals, you can optionally disable `AWS_SES_VERIFY_EVENT_SIGNATURES` in settings. Examples for the JSON object AWS SNS sends can be found here: https://docs.aws.amazon.com/sns/latest/dg/sns-message-and-json-formats.html#http-subscription-confirmation-json
+
+SES Event Monitoring with Configuration Sets
+============================================
+
+You can track your SES email sending at a granular level using `SES Event Publishing`_.
+To do this, you set up an SES Configuration Set and add event
+handlers to it to send your events on to a destination within AWS (SNS,
+Cloudwatch or Kinesis Firehose) for further processing and analysis.
+
+To ensure that emails you send via `django-ses` will be tagged with your
+SES Configuration Set, set the `AWS_SES_CONFIGURATION_SET` setting in your
+settings.py to the name of the configuration set::
+
+    AWS_SES_CONFIGURATION_SET = 'my-configuration-set-name'
+
+This will add the `X-SES-CONFIGURATION-SET` header to all your outgoing
+e-mails.
+
+If you want to set the SES Configuration Set on a per message basis, set
+`AWS_SES_CONFIGURATION_SET` to a callable.  The callable should conform to the
+following prototype::
+
+    def ses_configuration_set(message, dkim_domain=None, dkim_key=None,
+                                dkim_selector=None, dkim_headers=()):
+        configuration_set = 'my-default-set'
+        # use message and dkim_* to modify configuration_set
+        return configuration_set
+
+    AWS_SES_CONFIGURATION_SET = ses_configuration_set
+
+where
+
+* `message` is a `django.core.mail.EmailMessage` object (or subclass)
+* `dkim_domain` is a string containing the DKIM domain for this message
+* `dkim_key` is a string containing the DKIM private key for this message
+* `dkim_selector` is a string containing the DKIM selector (see DKIM, below for
+  explanation)
+* `dkim_headers` is a list of strings containing the names of the headers to
+  be DKIM signed (see DKIM, below for explanation)
+
+DKIM
+====
+
+Using DomainKeys_ is entirely optional, however it is recommended by Amazon for
+authenticating your email address and improving delivery success rate.  See
+http://docs.amazonwebservices.com/ses/latest/DeveloperGuide/DKIM.html.
+Besides authentication, you might also want to consider using DKIM in order to
+remove the `via email-bounces.amazonses.com` message shown to gmail users -
+see http://support.google.com/mail/bin/answer.py?hl=en&answer=1311182.
+
+Currently there are two methods to use DKIM with Django-SES: traditional Manual
+Signing and the more recently introduced Amazon Easy DKIM feature.
+
+Easy DKIM
+---------
+Easy DKIM is a feature of Amazon SES that automatically signs every message
+that you send from a verified email address or domain with a DKIM signature.
+
+You can enable Easy DKIM in the AWS Management Console for SES. There you can
+also add the required domain verification and DKIM records to Route 53 (or
+copy them to your alternate DNS).
+
+Once enabled and verified Easy DKIM needs no additional dependencies or
+DKIM specific settings to work with Django-SES.
+
+For more information and a setup guide see:
+http://docs.aws.amazon.com/ses/latest/DeveloperGuide/easy-dkim.html
+
+Manual DKIM Signing
+-------------------
+To enable Manual DKIM Signing you should install the pydkim_ package and specify values
+for the ``DKIM_PRIVATE_KEY`` and ``DKIM_DOMAIN`` settings.  You can generate a
+private key with a command such as ``openssl genrsa 512`` and get the public key
+portion with ``openssl rsa -pubout <private.key``.  The public key should be
+published to ``ses._domainkey.example.com`` if your domain is example.com.  You
+can use a different name instead of ``ses`` by changing the ``DKIM_SELECTOR``
+setting.
+
+The SES relay will modify email headers such as `Date` and `Message-Id` so by
+default only the `From`, `To`, `Cc`, `Subject` headers are signed, not the full
+set of headers.  This is sufficient for most DKIM validators but can be overridden
+with the ``DKIM_HEADERS`` setting.
+
+
+Example settings.py::
+
+   DKIM_DOMAIN = 'example.com'
+   DKIM_PRIVATE_KEY = '''
+   -----BEGIN RSA PRIVATE KEY-----
+   xxxxxxxxxxx
+   -----END RSA PRIVATE KEY-----
+   '''
+
+Example DNS record published to Route53 with boto:
+
+   route53 add_record ZONEID ses._domainkey.example.com. TXT '"v=DKIM1; p=xxx"' 86400
+
+
+.. _DomainKeys: http://dkim.org/
+
+
+Identity Owners
+===============
+
+With Identity owners, you can use validated SES-domains across multiple accounts:
+https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html
+
+This is useful if you got multiple environments in different accounts and still want to send mails via the same domain.
+
+You can configure the following environment variables to use them as described in boto3-docs_::
+
+    AWS_SES_SOURCE_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com
+    AWS_SES_FROM_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com
+    AWS_SES_RETURN_PATH_ARN=arn:aws:ses:eu-central-1:012345678910:identity/example.com
+
+.. _boto3-docs: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.send_raw_email
+
+
+SES Sending Stats
+=================
+
+Django SES comes with two ways of viewing sending statistics.
+
+The first one is a simple read-only report on your 24 hour sending quota,
+verified email addresses and bi-weekly sending statistics.
+
+To generate and view SES sending statistics reports, include, update
+``INSTALLED_APPS``::
+
+    INSTALLED_APPS = (
+        # ...
+        'django.contrib.admin',
+        'django_ses',
+        # ...
+    )
+
+... and ``urls.py``::
+
+    urlpatterns += (url(r'^admin/django-ses/', include('django_ses.urls')),)
+
+*Optional enhancements to stats:*
+
+Override the dashboard view
+---------------------------
+You can override the Dashboard view, for example, to add more context data::
+
+    class CustomSESDashboardView(DashboardView):
+        def get_context_data(self, **kwargs):
+            context = super().get_context_data(**kwargs)
+            context.update(**admin.site.each_context(self.request))
+            return context
+
+Then update your urls::
+
+    urlpatterns += path('admin/django-ses/', CustomSESDashboardView.as_view(), name='django_ses_stats'),
+
+
+Link the dashboard from the admin
+---------------------------------
+You can use adminplus for this (https://github.com/jsocol/django-adminplus)::
+
+    from django_ses.views import DashboardView
+    admin.site.register_view('django-ses', DashboardView.as_view(), 'Django SES Stats')
+
+
+
+Store daily stats
+-----------------
+If you need to keep send statistics around for longer than two weeks,
+django-ses also comes with a model that lets you store these. To use this
+feature you'll need to run::
+
+    python manage.py migrate
+
+To collect the statistics, run the ``get_ses_statistics`` management command
+(refer to next section for details). After running this command the statistics
+will be viewable via ``/admin/django_ses/``.
+
+Django SES Management Commands
+==============================
+
+To use these you must include ``django_ses`` in your INSTALLED_APPS.
+
+Managing Verified Email Addresses
+---------------------------------
+
+Manage verified email addresses through the management command.
+
+    python manage.py ses_email_address --list
+
+Add emails to the verified email list through:
+
+    python manage.py ses_email_address --add john.doe@example.com
+
+Remove emails from the verified email list through:
+
+    python manage.py ses_email_address --delete john.doe@example.com
+
+You can toggle the console output through setting the verbosity level.
+
+    python manage.py ses_email_address --list --verbosity 0
+
+
+Collecting Sending Statistics
+-----------------------------
+
+To collect and store SES sending statistics in the database, run:
+
+    python manage.py get_ses_statistics
+
+Sending statistics are aggregated daily (UTC time). Stats for the latest day
+(when you run the command) may be inaccurate if run before end of day (UTC).
+If you want to keep your statistics up to date, setup ``cron`` to run this
+command a short time after midnight (UTC) daily.
+
+
+Django Builtin-in Error Emails
+==============================
+
+If you'd like Django's `Builtin Email Error Reporting`_ to function properly
+(actually send working emails), you'll have to explicitly set the
+``SERVER_EMAIL`` setting to one of your SES-verified addresses. Otherwise, your
+error emails will all fail and you'll be blissfully unaware of a problem.
+
+*Note:* You will need to sign up for SES_ and verify any emails you're going
+to use in the `from_email` argument to `django.core.mail.send_email()`. Boto_
+has a `verify_email_address()` method: https://github.com/boto/boto/blob/master/boto/ses/connection.py
+
+.. _Builtin Email Error Reporting: https://docs.djangoproject.com/en/dev/howto/error-reporting/
+.. _Django: http://djangoproject.com
+.. _Boto: http://boto.cloudhackers.com/
+.. _SES: http://aws.amazon.com/ses/
+.. _SES Event Publishing: https://docs.aws.amazon.com/ses/latest/DeveloperGuide/monitor-using-event-publishing.html
+
+
+Requirements
+============
+django-ses requires supported version of Django or Python.
+
+
+Full List of Settings
+=====================
+
+``AWS_ACCESS_KEY_ID``, ``AWS_SECRET_ACCESS_KEY``
+  *Required.* Your API keys for Amazon SES.
+
+``AWS_SES_ACCESS_KEY_ID``, ``AWS_SES_SECRET_ACCESS_KEY``
+  *Required.* Alternative API keys for Amazon SES. This is useful in situations
+  where you would like to use separate access keys for different AWS services.
+
+``AWS_SES_SESSION_TOKEN``, ``AWS_SES_SECRET_ACCESS_KEY``
+  Optional. Use `AWS_SES_SESSION_TOKEN` to provide session token
+  when temporary credentials are used. Details:
+  https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp.html
+  https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_use-resources.html
+
+``AWS_SES_REGION_NAME``, ``AWS_SES_REGION_ENDPOINT``
+  Optionally specify what region your SES service is using. Note that this is
+  required if your SES service is not using us-east-1, as omitting these settings
+  implies this region. Details:
+  http://readthedocs.org/docs/boto/en/latest/ref/ses.html#boto.ses.regions
+  http://docs.aws.amazon.com/general/latest/gr/rande.html
+
+``AWS_SES_FROM_EMAIL``
+  Optional. The email address to be used as the "From" address for the email. The address that you specify has to be verified.  
+  For more information please refer to https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
+``AWS_SES_RETURN_PATH``
+  Optional. Use `AWS_SES_RETURN_PATH` to receive complaint notifications
+  You must use the v2 client by setting `USE_SES_V2=True` for this setting to work, otherwise it is ignored.
+  https://docs.aws.amazon.com/ses/latest/APIReference-V2/API_SendEmail.html#API_SendEmail_RequestSyntax
+
+
+``AWS_SES_CONFIGURATION_SET``
+  Optional. Use this to mark your e-mails as from being from a particular SES
+  Configuration Set. Set this to a string if you want all messages to have the
+  same configuration set.  Set this to a callable if you want to set
+  configuration set on a per message basis.
+
+``TIME_ZONE``
+  Default Django setting, optionally set this. Details:
+  https://docs.djangoproject.com/en/dev/ref/settings/#time-zone
+
+``DKIM_DOMAIN``, ``DKIM_PRIVATE_KEY``
+  Optional. If these settings are defined and the pydkim_ module is installed
+  then email messages will be signed with the specified key.   You will also
+  need to publish your public key on DNS; the selector is set to ``ses`` by
+  default.  See http://dkim.org/ for further detail.
+
+``AWS_SES_SOURCE_ARN``
+  Instruct Amazon SES to use a domain from another account.
+  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html
+
+``AWS_SES_FROM_ARN``
+  Instruct Amazon SES to use a domain from another account.
+  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html
+
+``AWS_SES_RETURN_PATH_ARN``
+  Instruct Amazon SES to use a domain from another account.
+  For more information please refer to https://docs.aws.amazon.com/ses/latest/DeveloperGuide/sending-authorization-delegate-sender-tasks-email.html
+
+``AWS_SES_VERIFY_EVENT_SIGNATURES``, ``AWS_SES_VERIFY_BOUNCE_SIGNATURES``
+  Optional. Default is True. Verify the contents of the message by matching the signature
+  you recreated from the message contents with the signature that Amazon SNS sent with the message.
+  See https://docs.aws.amazon.com/sns/latest/dg/sns-verify-signature-of-message.html for further detail.
+
+``EVENT_CERT_DOMAINS``, ``BOUNCE_CERT_DOMAINS``
+  Optional. Default is 'amazonaws.com' and 'amazon.com'.
+
+.. _pydkim: http://hewgill.com/pydkim/
+
+Proxy
+=====
+
+If you are using a proxy, please enable it via the env variables.
+
+If your proxy server does not have a password try the following:
+
+.. code-block:: python
+
+   import os
+   os.environ["HTTP_PROXY"] = "http://proxy.com:port"
+   os.environ["HTTPS_PROXY"] = "https://proxy.com:port"
+
+if your proxy server has a password try the following:
+
+.. code-block:: python
+
+   import os
+   os.environ["HTTP_PROXY"] = "http://user:password@proxy.com:port"
+   os.environ["HTTPS_PROXY"] = "https://user:password@proxy.com:port"
+
+Source: https://stackoverflow.com/a/33501223/1331671
+
+Contributing
+============
+If you'd like to fix a bug, add a feature, etc
+
+#. Start by opening an issue.
+    Be explicit so that project collaborators can understand and reproduce the
+    issue, or decide whether the feature falls within the project's goals.
+    Code examples can be useful, too.
+
+#. File a pull request.
+    You may write a prototype or suggested fix.
+
+#. Check your code for errors, complaints.
+    Use `check.py <https://github.com/jbalogh/check>`_
+
+#. Write and run tests.
+    Write your own test showing the issue has been resolved, or the feature
+    works as intended.
+
+Running Tests
+=============
+To run the tests::
+
+    python runtests.py
+
+If you want to debug the tests, just add this file as a python script to your IDE run configuration.
+
+Creating a Release
+==================
+
+To create a release:
+
+* Run ``poetry version {patch|minor|major}`` as explained in `the docs <https://python-poetry.org/docs/cli/#version>`_. This will update the version in pyproject.toml.
+* Commit that change and use git to tag that commit with a version that matches the pattern ``v*.*.*``.
+* Push the tag and the commit (note some IDEs don't push tags by default).
+
+
+.. |pypi| image:: https://badge.fury.io/py/django-ses.svg
+    :target: http://badge.fury.io/py/django-ses
+.. |build| image:: https://github.com/django-ses/django-ses/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/django-ses/django-ses/actions/workflows/ci.yml
+.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+    :target: https://pypi.org/project/django-ses/
+.. |django| image:: https://img.shields.io/badge/django-2.2%7C%203.2+-blue.svg
+    :target: https://www.djangoproject.com/
 
-setup(**setup_kwargs)
```


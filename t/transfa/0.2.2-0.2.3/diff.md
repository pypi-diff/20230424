# Comparing `tmp/transfa-0.2.2.tar.gz` & `tmp/transfa-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transfa-0.2.2.tar", last modified: Tue Feb 28 18:01:08 2023, max compression
+gzip compressed data, was "transfa-0.2.3.tar", last modified: Mon Apr 24 14:17:16 2023, max compression
```

## Comparing `transfa-0.2.2.tar` & `transfa-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:01:08.776827 transfa-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-28 18:00:59.000000 transfa-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-28 18:01:08.776827 transfa-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-28 18:00:59.000000 transfa-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-28 18:00:59.000000 transfa-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-28 18:01:08.776827 transfa-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 18:00:59.000000 transfa-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:01:08.772827 transfa-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-28 18:00:59.000000 transfa-0.2.2/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-02-28 18:00:59.000000 transfa-0.2.2/tests/test_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:01:08.772827 transfa-0.2.2/transfa/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:01:08.776827 transfa-0.2.2/transfa/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/api_resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-28 18:00:59.000000 transfa-0.2.2/transfa/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:01:08.776827 transfa-0.2.2/transfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 18:01:08.000000 transfa-0.2.2/transfa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 14:17:00.000000 transfa-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 14:17:16.721100 transfa-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-24 14:17:00.000000 transfa-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:17:00.000000 transfa-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 14:17:16.721100 transfa-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:17:00.000000 transfa-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.717100 transfa-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 14:17:00.000000 transfa-0.2.3/tests/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-24 14:17:00.000000 transfa-0.2.3/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.717100 transfa-0.2.3/transfa/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/transfa/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/transfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/top_level.txt
```

### Comparing `transfa-0.2.2/LICENSE` & `transfa-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/PKG-INFO` & `transfa-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfa
-Version: 0.2.2
+Version: 0.2.3
 Summary: This is the official python SDK for the Transfa API.
 Home-page: https://transfapp.com
 Author: Kolawole Mangabo
 Author-email: kolawole.mangabo@transfapp.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -109,15 +109,15 @@
 response = client.Payment.list()
 print(response.text)
 ```
 
 ### Verify webhook
 We will notify you each time there is be an update about your payments at the condition that your Organization supports the webhook feature (check on your organization's dashboard if you wan't to activate it) and that you provided a webhook url at which we can send the datas when sending the payment request. This will help you to automatically get an update without having to periodically send GET requests to our API.
 
-But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Optimus-Signature`. You'll use that signature to make sure that the request is coming from us.
+But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Transfa-Signature`. You'll use that signature to make sure that the request is coming from us.
 
 We provided you with a class called `Webhook` that will handle the whole verification underneath. All you have to do is creating an instance of the class with the required parameters.
 Here is an example of how you would do it with Django Rest Framework.
 
 ```python
 from rest_framework.decorators import api_view
 from rest_framework import status
```

### Comparing `transfa-0.2.2/README.md` & `transfa-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 response = client.Payment.list()
 print(response.text)
 ```
 
 ### Verify webhook
 We will notify you each time there is be an update about your payments at the condition that your Organization supports the webhook feature (check on your organization's dashboard if you wan't to activate it) and that you provided a webhook url at which we can send the datas when sending the payment request. This will help you to automatically get an update without having to periodically send GET requests to our API.
 
-But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Optimus-Signature`. You'll use that signature to make sure that the request is coming from us.
+But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Transfa-Signature`. You'll use that signature to make sure that the request is coming from us.
 
 We provided you with a class called `Webhook` that will handle the whole verification underneath. All you have to do is creating an instance of the class with the required parameters.
 Here is an example of how you would do it with Django Rest Framework.
 
 ```python
 from rest_framework.decorators import api_view
 from rest_framework import status
```

### Comparing `transfa-0.2.2/setup.cfg` & `transfa-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 commit = True
 tag = True
 
 [bumpversion:file:pyproject.toml]
 search = version = "{current_version}"
 replace = version = "{new_version}"
```

### Comparing `transfa-0.2.2/tests/test_payment.py` & `transfa-0.2.3/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/tests/test_webhook.py` & `transfa-0.2.3/tests/test_webhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,52 +25,52 @@
 
 
 def test_valid_webhook_signature(valid_webhook_payload):
     webhook_data = WebhookData()
     signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
 
     webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Optimus-Signature": signature
+        "X-Webhook-Transfa-Signature": signature
     })
 
     verified = webhook.verify()
 
     assert verified == valid_webhook_payload
 
 
 def test_invalid_webhook_signature(valid_webhook_payload, invalid_webhook_payload):
     webhook_data = WebhookData()
     invalid_signature = webhook_data.generate_signature(invalid_webhook_payload, webhook_data.valid_webhook_token)
 
     webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Optimus-Signature": invalid_signature
+        "X-Webhook-Transfa-Signature": invalid_signature
     })
 
     verified = webhook.verify()
 
     assert not verified
 
 
 def test_valid_webhook_token(valid_webhook_payload):
     webhook_data = WebhookData()
     valid_signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
 
     webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Optimus-Signature": valid_signature
+        "X-Webhook-Transfa-Signature": valid_signature
     })
 
     verified = webhook.verify()
 
     assert verified == valid_webhook_payload
 
 
 def test_invalid_webhook_token(valid_webhook_payload):
     webhook_data = WebhookData()
     valid_signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
 
     webhook = Webhook(webhook_token=webhook_data.invalid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Optimus-Signature": valid_signature
+        "X-Webhook-Transfa-Signature": valid_signature
     })
 
     verified = webhook.verify()
 
     assert not verified
```

### Comparing `transfa-0.2.2/transfa/api_client.py` & `transfa-0.2.3/transfa/api_client.py`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/transfa/api_resources/payments.py` & `transfa-0.2.3/transfa/api_resources/payments.py`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/transfa/enums.py` & `transfa-0.2.3/transfa/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
 class PrivateSecretPrefix(Enum):
     test = "ps_test"
     live = "ps_live"
 
 
 class TransfaHeadersIdentifiers(Enum):
-    webhook_signature = "X-Webhook-Optimus-Signature"
+    webhook_signature = "X-Webhook-Transfa-Signature"
```

### Comparing `transfa-0.2.2/transfa/utils.py` & `transfa-0.2.3/transfa/utils.py`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/transfa/webhook.py` & `transfa-0.2.3/transfa/webhook.py`

 * *Files identical despite different names*

### Comparing `transfa-0.2.2/transfa.egg-info/PKG-INFO` & `transfa-0.2.3/transfa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfa
-Version: 0.2.2
+Version: 0.2.3
 Summary: This is the official python SDK for the Transfa API.
 Home-page: https://transfapp.com
 Author: Kolawole Mangabo
 Author-email: kolawole.mangabo@transfapp.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -109,15 +109,15 @@
 response = client.Payment.list()
 print(response.text)
 ```
 
 ### Verify webhook
 We will notify you each time there is be an update about your payments at the condition that your Organization supports the webhook feature (check on your organization's dashboard if you wan't to activate it) and that you provided a webhook url at which we can send the datas when sending the payment request. This will help you to automatically get an update without having to periodically send GET requests to our API.
 
-But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Optimus-Signature`. You'll use that signature to make sure that the request is coming from us.
+But before you process the payload of a Webhook request, you must first verify that it is coming from Transfa and not from an unknown server acting like Transfa's server. Each webhook request will come with a parameter in the headers named `X-Webhook-Transfa-Signature`. You'll use that signature to make sure that the request is coming from us.
 
 We provided you with a class called `Webhook` that will handle the whole verification underneath. All you have to do is creating an instance of the class with the required parameters.
 Here is an example of how you would do it with Django Rest Framework.
 
 ```python
 from rest_framework.decorators import api_view
 from rest_framework import status
```


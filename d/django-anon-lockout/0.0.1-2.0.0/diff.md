# Comparing `tmp/django_anon_lockout-0.0.1.tar.gz` & `tmp/django_anon_lockout-2.0.0.tar.gz`

## Comparing `django_anon_lockout-0.0.1.tar` & `django_anon_lockout-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/admin.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/apps.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/conf.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/handlers.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/models.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/utils.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/anon_lockout/migrations/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 django_anon_lockout-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/admin.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/apps.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/conf.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/handlers.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/models.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/utils.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/0001_initial.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/0002_accesssession_successes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/PKG-INFO
```

### Comparing `django_anon_lockout-0.0.1/anon_lockout/models.py` & `django_anon_lockout-2.0.0/anon_lockout/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     about attempts and resources accessed. 
     """
 
     ip = models.CharField(max_length=256)
     failed_in_row = models.IntegerField(default=0)
     last_access = models.DateTimeField()
     resource = models.CharField(max_length=100)
+    successes = models.IntegerField(default=0)
 
     def has_active_lockout(self):
         """Returns true if there is an active lockout connected to this session."""
 
         return self.lockouts.filter(active=True).exists()
```

### Comparing `django_anon_lockout-0.0.1/anon_lockout/migrations/0001_initial.py` & `django_anon_lockout-2.0.0/anon_lockout/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-0.0.1/.gitignore` & `django_anon_lockout-2.0.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+# vscode
+.vscode
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
```

### Comparing `django_anon_lockout-0.0.1/LICENSE` & `django_anon_lockout-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-0.0.1/README.md` & `django_anon_lockout-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Django Anonymous Lockout
 
 Django anonymous lockout is a simple django module for keeping track of failed loging attemps to an endpoint that is protected by some password, but does not require authentication with an authentication backend.
 
-## Installation
+It works by fetching the IP of the one making the attempt. If the attempt is successful, it stores this and the resource can be shown. If the attempt fails, the session connected to the attempt get's it's `failed_in_row` field incremented. If this counter exceeds the threshold (default 100), the IP address is locked out for `LOCKOUT_DURATION` time (default 1 day). The only time the counter is reset, is after this lockout has expired.
 
-Note: does not work yet.
+## Installation
 
 Djano anonymous lockout can be installed with pip:
 
 ```bash
 pip install django-anon-lockout
 ```
 
@@ -44,15 +44,15 @@
     if user_ip:
         ip = user_ip.split(",")[0]
     else:
         ip = request.META.get("REMOTE_ADDR")
     return hashlib.sha256(ip.encode("utf-8")).hexdigest()
 ```
 
-This snippet is also included in `utils`.
+This snippet is also included in [`utils.py`](./anon_lockout/utils.py).
 
 ### Example
 
 Assuming you have a simple form with the field "password".
 
 `views.py`:
 
@@ -79,21 +79,19 @@
     return render(request, "anon_login.html", context)
 ```
 
 A working, but very simple example is in [`tests/views.py`](./tests/views.py).
 
 ## Configuration
 
-There are 3 settings that you can override:
+There are 2 settings that you can override:
 
 `LOCKOUT_DURATION`: Decides how long a user is locked out for. Default is 1 day.
 
-`LOCKOUT_THRESHOLD`: Decides how many attempts **in a row** that has to fail for a lockout to occur. Default is 5.
-
-`LOCKOUT_RESET_TIME`: This setting decides how long between two attempts by the same user is needed for the attempt counter to reset. If for instance you set this to 10 minutes, then if a user fails an access to a resource, then assuming the user does not try to access the same resource within 10 minutes, the next time the same user accesses the resource, the counter is reset to 0 failed attempts in a row. Default is 30 minutes.
+`LOCKOUT_THRESHOLD`: Decides how many attempts **in a row** that has to fail for a lockout to occur. Default is 100 attempts.
 
 ## Tests
 
 There are a few tests that makes sure the basic funtionality works. These can be run by:
 
 ```bash
 python manage.py test tests.tests
```

### Comparing `django_anon_lockout-0.0.1/pyproject.toml` & `django_anon_lockout-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/anon_lockout"
 ]
 
 [project]
 name = "django-anon-lockout"
-version = "0.0.1"
+version = "2.0.0"
 authors = [
   { name="Erlend Paulsen Skaaden", email="erlendskaaden@gmail.com" },
 ]
 description = "Django module for anonymous lockout"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_anon_lockout-0.0.1/PKG-INFO` & `django_anon_lockout-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-anon-lockout
-Version: 0.0.1
+Version: 2.0.0
 Summary: Django module for anonymous lockout
 Project-URL: Homepage, https://github.com/erlendps/django-anon-lockout
 Project-URL: Bug Tracker, https://github.com/erlendps/django-anon-lockout/issues
 Author-email: Erlend Paulsen Skaaden <erlendskaaden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,17 +12,17 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Django Anonymous Lockout
 
 Django anonymous lockout is a simple django module for keeping track of failed loging attemps to an endpoint that is protected by some password, but does not require authentication with an authentication backend.
 
-## Installation
+It works by fetching the IP of the one making the attempt. If the attempt is successful, it stores this and the resource can be shown. If the attempt fails, the session connected to the attempt get's it's `failed_in_row` field incremented. If this counter exceeds the threshold (default 100), the IP address is locked out for `LOCKOUT_DURATION` time (default 1 day). The only time the counter is reset, is after this lockout has expired.
 
-Note: does not work yet.
+## Installation
 
 Djano anonymous lockout can be installed with pip:
 
 ```bash
 pip install django-anon-lockout
 ```
 
@@ -58,15 +58,15 @@
     if user_ip:
         ip = user_ip.split(",")[0]
     else:
         ip = request.META.get("REMOTE_ADDR")
     return hashlib.sha256(ip.encode("utf-8")).hexdigest()
 ```
 
-This snippet is also included in `utils`.
+This snippet is also included in [`utils.py`](./anon_lockout/utils.py).
 
 ### Example
 
 Assuming you have a simple form with the field "password".
 
 `views.py`:
 
@@ -93,21 +93,19 @@
     return render(request, "anon_login.html", context)
 ```
 
 A working, but very simple example is in [`tests/views.py`](./tests/views.py).
 
 ## Configuration
 
-There are 3 settings that you can override:
+There are 2 settings that you can override:
 
 `LOCKOUT_DURATION`: Decides how long a user is locked out for. Default is 1 day.
 
-`LOCKOUT_THRESHOLD`: Decides how many attempts **in a row** that has to fail for a lockout to occur. Default is 5.
-
-`LOCKOUT_RESET_TIME`: This setting decides how long between two attempts by the same user is needed for the attempt counter to reset. If for instance you set this to 10 minutes, then if a user fails an access to a resource, then assuming the user does not try to access the same resource within 10 minutes, the next time the same user accesses the resource, the counter is reset to 0 failed attempts in a row. Default is 30 minutes.
+`LOCKOUT_THRESHOLD`: Decides how many attempts **in a row** that has to fail for a lockout to occur. Default is 100 attempts.
 
 ## Tests
 
 There are a few tests that makes sure the basic funtionality works. These can be run by:
 
 ```bash
 python manage.py test tests.tests
```


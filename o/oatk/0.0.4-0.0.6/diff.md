# Comparing `tmp/oatk-0.0.4.tar.gz` & `tmp/oatk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oatk-0.0.4.tar", last modified: Sat Oct 15 17:59:06 2022, max compression
+gzip compressed data, was "oatk-0.0.6.tar", last modified: Mon Apr 24 10:46:18 2023, max compression
```

## Comparing `oatk-0.0.4.tar` & `oatk-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.319868 oatk-0.0.4/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.316322 oatk-0.0.4/.github/
--rw-r--r--   0 xtof       (501) staff       (20)    18458 2022-10-15 15:14:06.000000 oatk-0.0.4/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.4/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      154 2022-10-15 17:50:41.000000 oatk-0.0.4/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)    22127 2022-10-15 17:59:06.319658 oatk-0.0.4/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.316752 oatk-0.0.4/examples/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-13 18:35:36.000000 oatk-0.0.4/examples/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.4/examples/create-and-validate.py
--rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.4/examples/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.317097 oatk-0.0.4/oatk/
--rw-r--r--   0 xtof       (501) staff       (20)     4540 2022-10-15 17:51:58.000000 oatk-0.0.4/oatk/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      751 2022-09-21 15:35:49.000000 oatk-0.0.4/oatk/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.318005 oatk-0.0.4/oatk/fake/
--rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.4/oatk/fake/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.4/oatk/fake/db.py
--rw-r--r--   0 xtof       (501) staff       (20)     7982 2022-10-15 14:22:18.000000 oatk-0.0.4/oatk/fake/routes.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.318174 oatk-0.0.4/oatk/fake/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.4/oatk/fake/static/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.4/oatk/fake/static/oatk.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.319177 oatk-0.0.4/oatk/fake/templates/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.4/oatk/fake/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      202 2022-09-28 06:26:40.000000 oatk-0.0.4/oatk/fake/templates/authorize.html
--rw-r--r--   0 xtof       (501) staff       (20)     1422 2022-10-15 14:31:14.000000 oatk-0.0.4/oatk/fake/templates/create_client.html
--rw-r--r--   0 xtof       (501) staff       (20)      451 2022-10-15 14:34:46.000000 oatk-0.0.4/oatk/fake/templates/home.html
--rw-r--r--   0 xtof       (501) staff       (20)      159 2022-09-23 12:22:36.000000 oatk-0.0.4/oatk/fake/templates/login-before-consent.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2022-10-15 17:59:06.317709 oatk-0.0.4/oatk.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)    22127 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      617 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       44 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       85 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       14 2022-10-15 17:59:06.000000 oatk-0.0.4/oatk.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2022-10-15 17:59:06.319915 oatk-0.0.4/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1572 2022-10-15 17:57:08.000000 oatk-0.0.4/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.757566 oatk-0.0.6/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751095 oatk-0.0.6/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)    21159 2023-04-24 10:45:00.000000 oatk-0.0.6/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.6/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      154 2022-10-15 17:50:41.000000 oatk-0.0.6/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 10:46:18.757431 oatk-0.0.6/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751558 oatk-0.0.6/examples/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-13 18:35:36.000000 oatk-0.0.6/examples/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.6/examples/create-and-validate.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751939 oatk-0.0.6/examples/google/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-03-25 10:56:05.000000 oatk-0.0.6/examples/google/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1538 2023-04-24 10:45:04.000000 oatk-0.0.6/examples/google/app.py
+-rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.6/examples/web.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.752166 oatk-0.0.6/oatk/
+-rw-r--r--   0 xtof       (501) staff       (20)     5538 2023-04-24 10:45:34.000000 oatk-0.0.6/oatk/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      751 2023-04-24 09:58:16.000000 oatk-0.0.6/oatk/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.753901 oatk-0.0.6/oatk/fake/
+-rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.6/oatk/fake/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.6/oatk/fake/db.py
+-rw-r--r--   0 xtof       (501) staff       (20)     7971 2022-10-16 09:03:05.000000 oatk-0.0.6/oatk/fake/routes.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.754736 oatk-0.0.6/oatk/fake/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.6/oatk/fake/static/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.6/oatk/fake/static/oatk.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1341 2022-10-16 14:49:57.000000 oatk-0.0.6/oatk/fake/static/style.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.756660 oatk-0.0.6/oatk/fake/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.6/oatk/fake/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      459 2022-10-16 14:32:06.000000 oatk-0.0.6/oatk/fake/templates/authorize.html
+-rw-r--r--   0 xtof       (501) staff       (20)      206 2022-10-16 14:31:57.000000 oatk-0.0.6/oatk/fake/templates/base.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1514 2022-10-16 14:51:49.000000 oatk-0.0.6/oatk/fake/templates/create_client.html
+-rw-r--r--   0 xtof       (501) staff       (20)      249 2022-10-16 14:31:48.000000 oatk-0.0.6/oatk/fake/templates/dialog.html
+-rw-r--r--   0 xtof       (501) staff       (20)      343 2022-10-16 14:49:16.000000 oatk-0.0.6/oatk/fake/templates/home.html
+-rw-r--r--   0 xtof       (501) staff       (20)      254 2022-10-16 14:30:22.000000 oatk-0.0.6/oatk/fake/templates/login.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.757020 oatk-0.0.6/oatk/js/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2023-04-15 12:40:08.000000 oatk-0.0.6/oatk/js/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.753013 oatk-0.0.6/oatk.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      762 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       44 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       94 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       14 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-24 10:46:18.757605 oatk-0.0.6/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1582 2023-04-15 08:19:14.000000 oatk-0.0.6/setup.py
```

### Comparing `oatk-0.0.4/.github/README.md` & `oatk-0.0.6/.github/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # OAuthToolKit
 
 > A collection of useful functions for dealing with OAuth
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/oatk.svg)](https://pypi.python.org/pypi/oatk/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/oatk.svg)](https://pypi.python.org/pypi/oatk/)
-[![Build Status](https://secure.travis-ci.org/christophevg/oatk.svg?branch=master)](http://travis-ci.org/christophevg/oatk)
-[![Documentation Status](https://readthedocs.org/projects/oatk/badge/?version=latest)](https://oatk.readthedocs.io/en/latest/?badge=latest)
-[![Coverage Status](https://coveralls.io/repos/github/christophevg/oatk/badge.svg?branch=master)](https://coveralls.io/github/christophevg/oatk?branch=master)
 [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
 
 ## Installation
 
 Minimal survival command...
 
 ```
@@ -18,15 +15,15 @@
 ```
 
 ## Rationale and Overview
 
 Federated login using OAuth/OpenIDConnect/... is a de facto standard for authenticating and authorizing users nowadays. You simply don't want to deal with them in your application at all. The underlying principle is simple: have someone you trust tell you that you can trust a user and get your own personal token that proves you're operating for that user when accessing other resources, who can validate this token with the trusted authenticating party.
 
 <p align="center">
-  <img alt="Oauth Flow Conceptually" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-conceptually.png" width="400">
+  <img alt="Oauth Flow Conceptually" src="../media/oauth-flow-conceptually.png" width="400">
 </p>
 
 This OAuthTooKit brings together very basic implementations of several aspects of this flow, aiming to have this up and running quickly in a development context, without the hassle of setting up a full-fletched OAuth server or having to go through many hoops in configuring an existing service to accept your application and users.
 
 In a nutshell, the toolkit contains:
 
 * a Python module to create and validate tokens
@@ -276,15 +273,15 @@
 4. after succesfull authorization, you're redirected to your `redirect_uri` (if it was previously registered as an acceptable one), along with a `code` query parameter, containing your authorization code.
 5. post to the `token_endpoint` with JSON fragment containing `grant_type` ("authorization_code") and a `code` (containing the obtained code)
 6. the response is a JSON fragment containing an `access_token`.
 7. get the `userinfo_endpoint` with the `access_token` as a `Bearer` `Authorization` header
 
 Visually:
 
-![Oauth Flow Visually](https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-visually.png)
+![Oauth Flow Visually](../media/oauth-flow-visually.png)
 
 ### Bringing everything together...
 
 Let's fire up our fake OAuth server, our minimal web API and create a web application to interact with the user.
 
 > The root-level Makefile contains targets that automate the require command line instructions. Make will also output these, so you can inspect what is done for you on the first line of the output.
 
@@ -321,33 +318,33 @@
 1. the fake OAuth server on [http://localhost:5000](http://localhost:5000)
 2. the web application on [http://localhost:5001](http://localhost:5001)
 3. the api application on [http://localhost:5002](http://localhost:5002)
 
 We first visit the fake OAuth server to setup a user and a client registration:
 
 <p align="center">
-  <img alt="Step 1: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step1.png" width="800">
+  <img alt="Step 1: Login/Signup" src="../media/step1.png" width="800">
 </p>
 
 Let's login/signup as `xtof`:
 
 <p align="center">
-  <img alt="Step 2: Logged in" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step2.png" width="800">
+  <img alt="Step 2: Logged in" src="../media/step2.png" width="800">
 </p>
 
 Now, create a client registration...
 
 <p align="center">
-  <img alt="Step 3: Create Client Registration" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step3.png" width="800">
+  <img alt="Step 3: Create Client Registration" src="../media/step3.png" width="800">
 </p>
 
 The defaults are all set for this demo, so just submit them...
 
 <p align="center">
-  <img alt="Step 4: All set" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step4.png" width="800">
+  <img alt="Step 4: All set" src="../media/step4.png" width="800">
 </p>
 
 So we now have an OAuth server, with a user `xtof` and a client registration for an application known by the clientId `test`.
 
 > If you hit the "log out" link now, you get back to the first screenshot. If you actually do this, in a few moments you'll have to log in again, else, since you're still logged in, you will see nothing really happen at first... ;-)
 
 Our web application is very simple: it requires and authenticated user and once it has it, it calls our protected web API to say hello...
@@ -374,26 +371,144 @@
   });
 </script>
 ```
 
 Let's visit it...
 
 <p align="center">
-  <img alt="Step 5: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step5.png" width="800">
+  <img alt="Step 5: Login/Signup" src="../media/step5.png" width="800">
 </p>
 
 Did we go to the wrong server? No, our application redirected us to the (fake) OAuth server, based on its known configuration. It could get the URLs, but didn't have an authorization code, so it redirected to the authorization endpoint. And since we're not logged in, because we logged out earlier, we now have to log in again, as `xtof`.
 
 <p align="center">
-  <img alt="Step 6: Give consent" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step6.png" width="800">
+  <img alt="Step 6: Give consent" src="../media/step6.png" width="800">
 </p>
 
 We explicitly have to give consent for the application to use our information and act on our behalf. After that, we are again redirected to our application that now continues the OAuth flow...
 
 <p align="center">
-  <img alt="Step 7: Hello" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step7.png" width="800">
+  <img alt="Step 7: Hello" src="../media/step7.png" width="800">
 </p>
 
 ... and calls our API that requires authentication and authorization using our OAuth token.
 
 > I've checked the console log preservation flag, to see the entire flow more clearly as it happens behind the scenes. You can see that upon returning to our app we now do have an authorization code, start another call to the server to exchange the code for a token, which results in a full set of URLs, code and token, so we can call our API and display the result.
 
+## Google
+
+The `examples/` folder contains another example, which is targetting Google as an authentication provider. The implicit flow is a little different, providing an access token (called `id_token`) immediately after logon and consent. The `id_token` kan be used as a JWT access token, yet it cannot be refreshed from the javascript client side.
+
+> So for now, I use it to authenticate the user once and set up an application-level session.
+
+The `examples/google/templates/home.html` file shows the minimal client-side HTML/javascript implementation:
+
+```html
+<div id="landing">
+  <a id="login" href="#">login with google</a>
+</div>
+
+<div id="app" style="display:none;">
+  <a style="float:right" id="logout" href="#">logout</a>
+  <h1>My App</h1>
+  <div id="output"></div>  
+</div>
+
+<script src="/static/jquery-3.6.1.min.js"></script>
+<script src="/oatk.js"></script>
+<script>
+  oatk.using_provider("{{ OAUTH_PROVIDER }}");
+  oatk.using_client_id("{{ OAUTH_CLIENT_ID }}");
+  oatk.apply_flow("implicit");
+  
+  function show_landing() {
+    $("#app").hide();
+    $("#landing").show();    
+  }
+  
+  function show_app() {
+    $("#app").show();
+    $("#landing").hide();
+  }
+
+  function login() {
+    oatk.with_authenticated_user(function(user, http, logout) {
+      console.log("👩 user is authenticated...", user);
+      $("#logout").click(function() { logout(show_landing); });
+      show_app();
+      
+      // call our API to say hello
+      http.getJSON("http://localhost:8000/api/hello", function(result) {
+        $("#output").text(JSON.stringify(result));
+      }, function(result) {
+        if(result.status == 403) {
+          console.log(result);
+          $("#output").text("You were authenticated by Google, yet you don't have the correct claims.");
+        }
+      });
+    });
+  }
+
+  $("#login").click(login);
+  
+  if(oatk.have_authenticated_user()) {
+    login();
+  }
+</script>
+```
+
+At the server-side of our application we need to:
+
+- serve oatk.js from the package (e.g. using Flask)
+- protect our endpoints with authorisation logic (e.g. using Flask_restful)
+
+```python
+from flask import Flask, render_template, Response
+from flask_restful import Resource, Api
+
+import oatk.js
+from oatk import OAuthToolkit
+
+server = Flask(__name__)
+
+# route to load web app
+@server.route("/", methods=["GET"])
+def home():
+  return render_template("home.html", **os.environ)
+
+# route for oatk.js from the oatk package
+@server.route("/oatk.js", methods=["GET"])
+def oatk_script():
+  return Response(oatk.js.as_src(), mimetype="application/javascript")
+
+# API set up
+api = Api(server)
+
+# setup oatk
+auth = OAuthToolkit()
+auth.using_provider(os.environ["OAUTH_PROVIDER"]);
+auth.with_client_id(os.environ["OAUTH_CLIENT_ID"])
+
+def validate_name(name):
+  return name == "Christophe VG"
+
+class HelloWorld(Resource):
+  @auth.authenticated_with_claims(name=validate_name)
+  def get(self):
+    return {"hello": "world"}
+
+api.add_resource(HelloWorld, "/api/hello")
+```
+
+If you [register an application with Google](https://console.cloud.google.com/apis/dashboard) and add `localhost:8000` as a authorized Javascript source and redirect URL for the credentials, you can run the example using `gunicorn -k eventlet -w 1 examples.google.app:server`, which triggers the following flow:
+
+<p align="center">
+  <img alt="Step 1: request login" src="../media/google-step1.png" width="800">
+</p>
+
+<p align="center">
+  <img alt="Step 2: authenticate and give consent (implicitly)" src="../media/google-step2.png" width="800">
+</p>
+
+<p align="center">
+  <img alt="Step 3: show protected content" src="../media/google-step3.png" width="800">
+</p>
```

### Comparing `oatk-0.0.4/LICENSE.txt` & `oatk-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/PKG-INFO` & `oatk-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.4
+Version: 0.0.6
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/oatk.svg)](https://pypi.python.org/pypi/oatk/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/oatk.svg)](https://pypi.python.org/pypi/oatk/)
-        [![Build Status](https://secure.travis-ci.org/christophevg/oatk.svg?branch=master)](http://travis-ci.org/christophevg/oatk)
-        [![Documentation Status](https://readthedocs.org/projects/oatk/badge/?version=latest)](https://oatk.readthedocs.io/en/latest/?badge=latest)
-        [![Coverage Status](https://coveralls.io/repos/github/christophevg/oatk/badge.svg?branch=master)](https://coveralls.io/github/christophevg/oatk?branch=master)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         ## Installation
         
         Minimal survival command...
         
         ```
@@ -25,15 +22,15 @@
         ```
         
         ## Rationale and Overview
         
         Federated login using OAuth/OpenIDConnect/... is a de facto standard for authenticating and authorizing users nowadays. You simply don't want to deal with them in your application at all. The underlying principle is simple: have someone you trust tell you that you can trust a user and get your own personal token that proves you're operating for that user when accessing other resources, who can validate this token with the trusted authenticating party.
         
         <p align="center">
-          <img alt="Oauth Flow Conceptually" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-conceptually.png" width="400">
+          <img alt="Oauth Flow Conceptually" src="../media/oauth-flow-conceptually.png" width="400">
         </p>
         
         This OAuthTooKit brings together very basic implementations of several aspects of this flow, aiming to have this up and running quickly in a development context, without the hassle of setting up a full-fletched OAuth server or having to go through many hoops in configuring an existing service to accept your application and users.
         
         In a nutshell, the toolkit contains:
         
         * a Python module to create and validate tokens
@@ -283,15 +280,15 @@
         4. after succesfull authorization, you're redirected to your `redirect_uri` (if it was previously registered as an acceptable one), along with a `code` query parameter, containing your authorization code.
         5. post to the `token_endpoint` with JSON fragment containing `grant_type` ("authorization_code") and a `code` (containing the obtained code)
         6. the response is a JSON fragment containing an `access_token`.
         7. get the `userinfo_endpoint` with the `access_token` as a `Bearer` `Authorization` header
         
         Visually:
         
-        ![Oauth Flow Visually](https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-visually.png)
+        ![Oauth Flow Visually](../media/oauth-flow-visually.png)
         
         ### Bringing everything together...
         
         Let's fire up our fake OAuth server, our minimal web API and create a web application to interact with the user.
         
         > The root-level Makefile contains targets that automate the require command line instructions. Make will also output these, so you can inspect what is done for you on the first line of the output.
         
@@ -328,33 +325,33 @@
         1. the fake OAuth server on [http://localhost:5000](http://localhost:5000)
         2. the web application on [http://localhost:5001](http://localhost:5001)
         3. the api application on [http://localhost:5002](http://localhost:5002)
         
         We first visit the fake OAuth server to setup a user and a client registration:
         
         <p align="center">
-          <img alt="Step 1: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step1.png" width="800">
+          <img alt="Step 1: Login/Signup" src="../media/step1.png" width="800">
         </p>
         
         Let's login/signup as `xtof`:
         
         <p align="center">
-          <img alt="Step 2: Logged in" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step2.png" width="800">
+          <img alt="Step 2: Logged in" src="../media/step2.png" width="800">
         </p>
         
         Now, create a client registration...
         
         <p align="center">
-          <img alt="Step 3: Create Client Registration" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step3.png" width="800">
+          <img alt="Step 3: Create Client Registration" src="../media/step3.png" width="800">
         </p>
         
         The defaults are all set for this demo, so just submit them...
         
         <p align="center">
-          <img alt="Step 4: All set" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step4.png" width="800">
+          <img alt="Step 4: All set" src="../media/step4.png" width="800">
         </p>
         
         So we now have an OAuth server, with a user `xtof` and a client registration for an application known by the clientId `test`.
         
         > If you hit the "log out" link now, you get back to the first screenshot. If you actually do this, in a few moments you'll have to log in again, else, since you're still logged in, you will see nothing really happen at first... ;-)
         
         Our web application is very simple: it requires and authenticated user and once it has it, it calls our protected web API to say hello...
@@ -381,33 +378,151 @@
           });
         </script>
         ```
         
         Let's visit it...
         
         <p align="center">
-          <img alt="Step 5: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step5.png" width="800">
+          <img alt="Step 5: Login/Signup" src="../media/step5.png" width="800">
         </p>
         
         Did we go to the wrong server? No, our application redirected us to the (fake) OAuth server, based on its known configuration. It could get the URLs, but didn't have an authorization code, so it redirected to the authorization endpoint. And since we're not logged in, because we logged out earlier, we now have to log in again, as `xtof`.
         
         <p align="center">
-          <img alt="Step 6: Give consent" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step6.png" width="800">
+          <img alt="Step 6: Give consent" src="../media/step6.png" width="800">
         </p>
         
         We explicitly have to give consent for the application to use our information and act on our behalf. After that, we are again redirected to our application that now continues the OAuth flow...
         
         <p align="center">
-          <img alt="Step 7: Hello" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step7.png" width="800">
+          <img alt="Step 7: Hello" src="../media/step7.png" width="800">
         </p>
         
         ... and calls our API that requires authentication and authorization using our OAuth token.
         
         > I've checked the console log preservation flag, to see the entire flow more clearly as it happens behind the scenes. You can see that upon returning to our app we now do have an authorization code, start another call to the server to exchange the code for a token, which results in a full set of URLs, code and token, so we can call our API and display the result.
         
+        ## Google
+        
+        The `examples/` folder contains another example, which is targetting Google as an authentication provider. The implicit flow is a little different, providing an access token (called `id_token`) immediately after logon and consent. The `id_token` kan be used as a JWT access token, yet it cannot be refreshed from the javascript client side.
+        
+        > So for now, I use it to authenticate the user once and set up an application-level session.
+        
+        The `examples/google/templates/home.html` file shows the minimal client-side HTML/javascript implementation:
+        
+        ```html
+        <div id="landing">
+          <a id="login" href="#">login with google</a>
+        </div>
+        
+        <div id="app" style="display:none;">
+          <a style="float:right" id="logout" href="#">logout</a>
+          <h1>My App</h1>
+          <div id="output"></div>  
+        </div>
+        
+        <script src="/static/jquery-3.6.1.min.js"></script>
+        <script src="/oatk.js"></script>
+        <script>
+          oatk.using_provider("{{ OAUTH_PROVIDER }}");
+          oatk.using_client_id("{{ OAUTH_CLIENT_ID }}");
+          oatk.apply_flow("implicit");
+          
+          function show_landing() {
+            $("#app").hide();
+            $("#landing").show();    
+          }
+          
+          function show_app() {
+            $("#app").show();
+            $("#landing").hide();
+          }
+        
+          function login() {
+            oatk.with_authenticated_user(function(user, http, logout) {
+              console.log("👩 user is authenticated...", user);
+              $("#logout").click(function() { logout(show_landing); });
+              show_app();
+              
+              // call our API to say hello
+              http.getJSON("http://localhost:8000/api/hello", function(result) {
+                $("#output").text(JSON.stringify(result));
+              }, function(result) {
+                if(result.status == 403) {
+                  console.log(result);
+                  $("#output").text("You were authenticated by Google, yet you don't have the correct claims.");
+                }
+              });
+            });
+          }
+        
+          $("#login").click(login);
+          
+          if(oatk.have_authenticated_user()) {
+            login();
+          }
+        </script>
+        ```
+        
+        At the server-side of our application we need to:
+        
+        - serve oatk.js from the package (e.g. using Flask)
+        - protect our endpoints with authorisation logic (e.g. using Flask_restful)
+        
+        ```python
+        from flask import Flask, render_template, Response
+        from flask_restful import Resource, Api
+        
+        import oatk.js
+        from oatk import OAuthToolkit
+        
+        server = Flask(__name__)
+        
+        # route to load web app
+        @server.route("/", methods=["GET"])
+        def home():
+          return render_template("home.html", **os.environ)
+        
+        # route for oatk.js from the oatk package
+        @server.route("/oatk.js", methods=["GET"])
+        def oatk_script():
+          return Response(oatk.js.as_src(), mimetype="application/javascript")
+        
+        # API set up
+        api = Api(server)
+        
+        # setup oatk
+        auth = OAuthToolkit()
+        auth.using_provider(os.environ["OAUTH_PROVIDER"]);
+        auth.with_client_id(os.environ["OAUTH_CLIENT_ID"])
+        
+        def validate_name(name):
+          return name == "Christophe VG"
+        
+        class HelloWorld(Resource):
+          @auth.authenticated_with_claims(name=validate_name)
+          def get(self):
+            return {"hello": "world"}
+        
+        api.add_resource(HelloWorld, "/api/hello")
+        ```
+        
+        If you [register an application with Google](https://console.cloud.google.com/apis/dashboard) and add `localhost:8000` as a authorized Javascript source and redirect URL for the credentials, you can run the example using `gunicorn -k eventlet -w 1 examples.google.app:server`, which triggers the following flow:
+        
+        <p align="center">
+          <img alt="Step 1: request login" src="../media/google-step1.png" width="800">
+        </p>
+        
+        <p align="center">
+          <img alt="Step 2: authenticate and give consent (implicitly)" src="../media/google-step2.png" width="800">
+        </p>
+        
+        <p align="center">
+          <img alt="Step 3: show protected content" src="../media/google-step3.png" width="800">
+        </p>
         
 Keywords: oauth human
 Platform: UNKNOWN
 Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oatk-0.0.4/examples/web.py` & `oatk-0.0.6/examples/web.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/oatk/__init__.py` & `oatk-0.0.6/oatk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 import uuid
 
@@ -11,14 +11,16 @@
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
 from functools import wraps
 from flask import request, Response
 
+import requests
+
 from oatk import fake
 
 try:
   from AppKit import NSPasteboard, NSStringPboardType
   pb = NSPasteboard.generalPasteboard()
 except ModuleNotFoundError:
   logger.debug("No AppKit installed, so no MacOS clipboard support!")
@@ -29,14 +31,15 @@
     self._encoded     = None
     self._certs       = {}
     self._private_key = None
     self._public_key  = None
     self._alg         = "RS256"
     self._kid         = str(uuid.uuid4())
     self._claims      = {}
+    self._client_id   = None
     
     self.server       = fake.server
     self.server.oatk  = self
 
   @property
   def version(self):
     return __version__
@@ -55,14 +58,32 @@
       self._public_key = serialization.load_pem_public_key(
         fp.read(),
         backend=default_backend()
       )
     self._certs = { self._kid : self._public_key }
     return self
 
+  def using_provider(self, provider_url):
+    try:
+      config = json.loads(requests.get(provider_url).content)
+    except:
+      logger.exception("could not retrieve openid configuration")
+      return
+    try:
+      self.with_jwks(requests.get(config["jwks_uri"]).content)
+    except:
+      logger.exception("could not import jwks")
+      return
+    logger.info(f"succesfully configured from {provider_url}")
+    return self
+
+  def with_client_id(self, client_id):
+    self._client_id = client_id
+    return self
+
   @property
   def jwks(self):
     return json.dumps({
       "keys" : [
         jwk.dumps(self._public_key, kty="RSA", alg=self._alg, kid=self._kid)
       ]
     }, indent=2)
@@ -118,15 +139,15 @@
     return None
 
   def validate(self, token=None):
     kid = self.header(token)["kid"]
     alg = self.header(token)["alg"]
     if not token:
       token = self._encoded
-    jwt.decode( token, self._certs[kid], algorithms=[alg] )
+    jwt.decode( token, self._certs[kid], algorithms=[alg], audience=self._client_id )
 
   def decode(self, token=None):
     if not token:
       token = self._encoded
     return jwt.decode( token, options={"verify_signature": False} )
 
   def authenticated(self, f):
@@ -152,17 +173,26 @@
         try:
           token = request.headers["Authorization"][7:]
           self.validate(token)
           claims = self.decode(token)
           for claim, value in required_claims.items():
             if not claim in claims:
               raise ValueError(f"required claim {claim} is missing")
-            if not value in claims[claim]:
-              raise ValueError(f"claim {claim} is missing required value")
+            if callable(value):
+              if not value(claims[claim]):
+                raise ValueError(f"claim {claim} doesn't match required criteria")
+            elif type(value) == list:
+              if not value in claims[claim]:
+                raise ValueError(f"claim {claim} is missing required value")
+            elif value != claims[claim]:
+              raise ValueError(f"claim {claim} doesn't equal required value")
           return f(*args, **kwargs)
         except KeyError as ex:
           msg = "Missing Authorization"
+          return Response(msg, 401)
+        except ValueError as e:
+          msg = str(e)
         except Exception as e:
-          msg = repr(e)
-        return Response(msg, 401)
+          msg = str(e)
+        return Response(msg, 403)
       return wrapper
     return decorator
```

### Comparing `oatk-0.0.4/oatk/__main__.py` & `oatk-0.0.6/oatk/__main__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/oatk/fake/__init__.py` & `oatk-0.0.6/oatk/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/oatk/fake/db.py` & `oatk-0.0.6/oatk/fake/db.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/oatk/fake/routes.py` & `oatk-0.0.6/oatk/fake/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,21 @@
       user = { "username": username, "_id" : str(uuid.uuid4()) }
       db["users"].insert_one(user)
     session["id"] = user["_id"]
     return redirect("/")
 
   # GET
   user = current_user()
-  logger.info(user)
   if user:
     clients = list(db["clients"].find({"user_id" : user["_id"]}))
+    for client in clients:
+      client["_id"] = str(client["_id"]) # turn Mongo ObjectID into string
+    return render_template("home.html", user=user, clients=clients)
   else:
-    clients = []
-  for client in clients:
-    client["_id"] = str(client["_id"]) # turn Mongo ObjectID into string
-  return render_template("home.html", user=user, clients=clients)
-
+    return render_template("login.html")
 
 @server.route("/oauth/create-client", methods=["GET", "POST"])
 def create_client():
   """
   The Create Client page allows a user to create a new client registration.
   Client registration is required for an external application to interact and
   act on behalf of our user.
@@ -112,15 +110,15 @@
       "client_id" : client_id
     })
     assert scope == "openid profile"
     assert request.args["response_type"] == "code"
     nonce = request.args["nonce"]
     logger.info(f"got client: {client}")
   else:
-    return render_template("login-before-consent.html", args=str(request.query_string.decode()))
+    return render_template("login.html", args=str(request.query_string.decode()))
 
   if "confirm" in request.form:
     logger.info("got confirmation: f{request.form['confirm']}")
     if request.form["confirm"]:
       logger.info("get positive confirmation... redirecting with code...")
       redirect_uri = client["metadata"]["redirect_uris"][0]
       code = generate_token()
@@ -141,15 +139,15 @@
     grant = {
       "client"  : { "client_name" : client["metadata"]["client_name"] },
       "request" : { "scope"       : scope }
     }
   except Exception as error:
     logger.exception(error)
     return jsonify({"error" : str(error)})
-  return render_template("authorize.html", user=user, grant=grant)
+  return render_template("authorize.html", grant=grant)
 
 @server.route("/oauth/token", methods=["POST"])
 def issue_token():
   try:
     code = db["codes"].find_one({"code" : request.json["code"] })
     client = db["clients"].find_one({
       "user_id"   : code["user_id"],
@@ -215,15 +213,15 @@
     "userinfo_endpoint"      : f"{me}/oauth/userinfo",
     "end_session_endpoint"   : f"{me}/oauth/logout",
     "registration_endpoint"  : f"{me}/oauth/create-client",
   }, indent=2)
 
 @server.route("/oauth/logout")
 def logout():
-  session.pop("id")
+  session.pop("id", None)
   goto = "/"
   return redirect(goto, 302)
 
 # helper functions
 
 def current_user():
   if "id" in session:
```

### Comparing `oatk-0.0.4/oatk/fake/static/oatk.js` & `oatk-0.0.6/oatk/fake/static/oatk.js`

 * *Files identical despite different names*

### Comparing `oatk-0.0.4/oatk/fake/templates/create_client.html` & `oatk-0.0.6/oatk/fake/templates/create_client.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-<style>
-  label, label > span { display: block; }
-  label { margin: 15px 0; }
-</style>
-
-<a href="/">Home</a>
-
-<form action="" method="post">
-  <label>
-    <span>Client Name</span>
-    <input type="text" name="client_name" value="test">
-  </label>
-  <label>
-    <span>Client ID</span>
-    <input type="text" name="client_id" value="test">
-  </label>
-  <label>
-    <span>Client Secret</span>
-    <input type="text" name="client_secret" value="test">
-  </label>
-  <label>
-    <span>Client URI</span>
-    <input type="url" name="client_uri" value="http://localhost:5001">
-  </label>
-  <label>
-    <span>Allowed Scope</span>
-    <input type="text" name="scope" value="openid profile">
-  </label>
-  <label>
-    <span>Redirect URIs</span>
-    <textarea name="redirect_uri" cols="30" rows="3">http://localhost:5001</textarea>
-  </label>
-  <label>
-    <span>Allowed Origins</span>
-    <textarea name="allowed_origins" cols="30" rows="3">http://localhost:5001</textarea>
-  </label>
-  <label>
-    <span>Allowed Grant Types</span>
-    <textarea name="grant_type" cols="30" rows="3">authorization_code</textarea>
-  </label>
-  <label>
-    <span>Allowed Response Types</span>
-    <textarea name="response_type" cols="30" rows="3">code</textarea>
-  </label>
-  <label>
-    <span>Permission Groups</span>
-    <textarea name="permission_groups" cols="30" rows="3">Group1
+{% extends "base.html" %}
+{% block page %}
+<div class="page">
+  <form action="" method="post">
+    <label>
+      <span>Client Name</span>
+      <input type="text" name="client_name" value="test">
+    </label>
+    <label>
+      <span>Client ID</span>
+      <input type="text" name="client_id" value="test">
+    </label>
+    <label>
+      <span>Client Secret</span>
+      <input type="text" name="client_secret" value="test">
+    </label>
+    <label>
+      <span>Client URI</span>
+      <input type="url" name="client_uri" value="http://localhost:5001">
+    </label>
+    <label>
+      <span>Allowed Scope</span>
+      <input type="text" name="scope" value="openid profile">
+    </label>
+    <label>
+      <span>Redirect URIs</span>
+      <textarea name="redirect_uri" cols="30" rows="3">http://localhost:5001</textarea>
+    </label>
+    <label>
+      <span>Allowed Origins</span>
+      <textarea name="allowed_origins" cols="30" rows="3">http://localhost:5001</textarea>
+    </label>
+    <label>
+      <span>Allowed Grant Types</span>
+      <textarea name="grant_type" cols="30" rows="3">authorization_code</textarea>
+    </label>
+    <label>
+      <span>Allowed Response Types</span>
+      <textarea name="response_type" cols="30" rows="3">code</textarea>
+    </label>
+    <label>
+      <span>Permission Groups</span>
+      <textarea name="permission_groups" cols="30" rows="3">Group1
 Group2
 Group3</textarea>
-  </label>
-  <button>Submit</button>
-</form>
+    </label>
+    <button>Submit</button>
+  </form>
+
+  <hr>
+
+  <a href="/">Home</a>
+</div>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
- Home
+{% extends "base.html" %} {% block page %}
  Client Name [test                ]   Client ID [test                ]   Client
 Secret [test                ]   Client URI [Unknown INPUT type]   Allowed Scope
 [openid profile      ]   Redirect URIs
 http://localhost:5001
    Allowed Origins
 http://localhost:5001
    Allowed Grant Types
 authorization_code
    Allowed Response Types
 code
    Permission Groups
 Group1 Group2 Group3
   Submit
+===============================================================================
+Home
+{% endblock %}
```

### Comparing `oatk-0.0.4/oatk.egg-info/PKG-INFO` & `oatk-0.0.6/oatk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.4
+Version: 0.0.6
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/oatk.svg)](https://pypi.python.org/pypi/oatk/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/oatk.svg)](https://pypi.python.org/pypi/oatk/)
-        [![Build Status](https://secure.travis-ci.org/christophevg/oatk.svg?branch=master)](http://travis-ci.org/christophevg/oatk)
-        [![Documentation Status](https://readthedocs.org/projects/oatk/badge/?version=latest)](https://oatk.readthedocs.io/en/latest/?badge=latest)
-        [![Coverage Status](https://coveralls.io/repos/github/christophevg/oatk/badge.svg?branch=master)](https://coveralls.io/github/christophevg/oatk?branch=master)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         ## Installation
         
         Minimal survival command...
         
         ```
@@ -25,15 +22,15 @@
         ```
         
         ## Rationale and Overview
         
         Federated login using OAuth/OpenIDConnect/... is a de facto standard for authenticating and authorizing users nowadays. You simply don't want to deal with them in your application at all. The underlying principle is simple: have someone you trust tell you that you can trust a user and get your own personal token that proves you're operating for that user when accessing other resources, who can validate this token with the trusted authenticating party.
         
         <p align="center">
-          <img alt="Oauth Flow Conceptually" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-conceptually.png" width="400">
+          <img alt="Oauth Flow Conceptually" src="../media/oauth-flow-conceptually.png" width="400">
         </p>
         
         This OAuthTooKit brings together very basic implementations of several aspects of this flow, aiming to have this up and running quickly in a development context, without the hassle of setting up a full-fletched OAuth server or having to go through many hoops in configuring an existing service to accept your application and users.
         
         In a nutshell, the toolkit contains:
         
         * a Python module to create and validate tokens
@@ -283,15 +280,15 @@
         4. after succesfull authorization, you're redirected to your `redirect_uri` (if it was previously registered as an acceptable one), along with a `code` query parameter, containing your authorization code.
         5. post to the `token_endpoint` with JSON fragment containing `grant_type` ("authorization_code") and a `code` (containing the obtained code)
         6. the response is a JSON fragment containing an `access_token`.
         7. get the `userinfo_endpoint` with the `access_token` as a `Bearer` `Authorization` header
         
         Visually:
         
-        ![Oauth Flow Visually](https://raw.githubusercontent.com/christophevg/oatk/master/media/oauth-flow-visually.png)
+        ![Oauth Flow Visually](../media/oauth-flow-visually.png)
         
         ### Bringing everything together...
         
         Let's fire up our fake OAuth server, our minimal web API and create a web application to interact with the user.
         
         > The root-level Makefile contains targets that automate the require command line instructions. Make will also output these, so you can inspect what is done for you on the first line of the output.
         
@@ -328,33 +325,33 @@
         1. the fake OAuth server on [http://localhost:5000](http://localhost:5000)
         2. the web application on [http://localhost:5001](http://localhost:5001)
         3. the api application on [http://localhost:5002](http://localhost:5002)
         
         We first visit the fake OAuth server to setup a user and a client registration:
         
         <p align="center">
-          <img alt="Step 1: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step1.png" width="800">
+          <img alt="Step 1: Login/Signup" src="../media/step1.png" width="800">
         </p>
         
         Let's login/signup as `xtof`:
         
         <p align="center">
-          <img alt="Step 2: Logged in" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step2.png" width="800">
+          <img alt="Step 2: Logged in" src="../media/step2.png" width="800">
         </p>
         
         Now, create a client registration...
         
         <p align="center">
-          <img alt="Step 3: Create Client Registration" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step3.png" width="800">
+          <img alt="Step 3: Create Client Registration" src="../media/step3.png" width="800">
         </p>
         
         The defaults are all set for this demo, so just submit them...
         
         <p align="center">
-          <img alt="Step 4: All set" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step4.png" width="800">
+          <img alt="Step 4: All set" src="../media/step4.png" width="800">
         </p>
         
         So we now have an OAuth server, with a user `xtof` and a client registration for an application known by the clientId `test`.
         
         > If you hit the "log out" link now, you get back to the first screenshot. If you actually do this, in a few moments you'll have to log in again, else, since you're still logged in, you will see nothing really happen at first... ;-)
         
         Our web application is very simple: it requires and authenticated user and once it has it, it calls our protected web API to say hello...
@@ -381,33 +378,151 @@
           });
         </script>
         ```
         
         Let's visit it...
         
         <p align="center">
-          <img alt="Step 5: Login/Signup" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step5.png" width="800">
+          <img alt="Step 5: Login/Signup" src="../media/step5.png" width="800">
         </p>
         
         Did we go to the wrong server? No, our application redirected us to the (fake) OAuth server, based on its known configuration. It could get the URLs, but didn't have an authorization code, so it redirected to the authorization endpoint. And since we're not logged in, because we logged out earlier, we now have to log in again, as `xtof`.
         
         <p align="center">
-          <img alt="Step 6: Give consent" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step6.png" width="800">
+          <img alt="Step 6: Give consent" src="../media/step6.png" width="800">
         </p>
         
         We explicitly have to give consent for the application to use our information and act on our behalf. After that, we are again redirected to our application that now continues the OAuth flow...
         
         <p align="center">
-          <img alt="Step 7: Hello" src="https://raw.githubusercontent.com/christophevg/oatk/master/media/step7.png" width="800">
+          <img alt="Step 7: Hello" src="../media/step7.png" width="800">
         </p>
         
         ... and calls our API that requires authentication and authorization using our OAuth token.
         
         > I've checked the console log preservation flag, to see the entire flow more clearly as it happens behind the scenes. You can see that upon returning to our app we now do have an authorization code, start another call to the server to exchange the code for a token, which results in a full set of URLs, code and token, so we can call our API and display the result.
         
+        ## Google
+        
+        The `examples/` folder contains another example, which is targetting Google as an authentication provider. The implicit flow is a little different, providing an access token (called `id_token`) immediately after logon and consent. The `id_token` kan be used as a JWT access token, yet it cannot be refreshed from the javascript client side.
+        
+        > So for now, I use it to authenticate the user once and set up an application-level session.
+        
+        The `examples/google/templates/home.html` file shows the minimal client-side HTML/javascript implementation:
+        
+        ```html
+        <div id="landing">
+          <a id="login" href="#">login with google</a>
+        </div>
+        
+        <div id="app" style="display:none;">
+          <a style="float:right" id="logout" href="#">logout</a>
+          <h1>My App</h1>
+          <div id="output"></div>  
+        </div>
+        
+        <script src="/static/jquery-3.6.1.min.js"></script>
+        <script src="/oatk.js"></script>
+        <script>
+          oatk.using_provider("{{ OAUTH_PROVIDER }}");
+          oatk.using_client_id("{{ OAUTH_CLIENT_ID }}");
+          oatk.apply_flow("implicit");
+          
+          function show_landing() {
+            $("#app").hide();
+            $("#landing").show();    
+          }
+          
+          function show_app() {
+            $("#app").show();
+            $("#landing").hide();
+          }
+        
+          function login() {
+            oatk.with_authenticated_user(function(user, http, logout) {
+              console.log("👩 user is authenticated...", user);
+              $("#logout").click(function() { logout(show_landing); });
+              show_app();
+              
+              // call our API to say hello
+              http.getJSON("http://localhost:8000/api/hello", function(result) {
+                $("#output").text(JSON.stringify(result));
+              }, function(result) {
+                if(result.status == 403) {
+                  console.log(result);
+                  $("#output").text("You were authenticated by Google, yet you don't have the correct claims.");
+                }
+              });
+            });
+          }
+        
+          $("#login").click(login);
+          
+          if(oatk.have_authenticated_user()) {
+            login();
+          }
+        </script>
+        ```
+        
+        At the server-side of our application we need to:
+        
+        - serve oatk.js from the package (e.g. using Flask)
+        - protect our endpoints with authorisation logic (e.g. using Flask_restful)
+        
+        ```python
+        from flask import Flask, render_template, Response
+        from flask_restful import Resource, Api
+        
+        import oatk.js
+        from oatk import OAuthToolkit
+        
+        server = Flask(__name__)
+        
+        # route to load web app
+        @server.route("/", methods=["GET"])
+        def home():
+          return render_template("home.html", **os.environ)
+        
+        # route for oatk.js from the oatk package
+        @server.route("/oatk.js", methods=["GET"])
+        def oatk_script():
+          return Response(oatk.js.as_src(), mimetype="application/javascript")
+        
+        # API set up
+        api = Api(server)
+        
+        # setup oatk
+        auth = OAuthToolkit()
+        auth.using_provider(os.environ["OAUTH_PROVIDER"]);
+        auth.with_client_id(os.environ["OAUTH_CLIENT_ID"])
+        
+        def validate_name(name):
+          return name == "Christophe VG"
+        
+        class HelloWorld(Resource):
+          @auth.authenticated_with_claims(name=validate_name)
+          def get(self):
+            return {"hello": "world"}
+        
+        api.add_resource(HelloWorld, "/api/hello")
+        ```
+        
+        If you [register an application with Google](https://console.cloud.google.com/apis/dashboard) and add `localhost:8000` as a authorized Javascript source and redirect URL for the credentials, you can run the example using `gunicorn -k eventlet -w 1 examples.google.app:server`, which triggers the following flow:
+        
+        <p align="center">
+          <img alt="Step 1: request login" src="../media/google-step1.png" width="800">
+        </p>
+        
+        <p align="center">
+          <img alt="Step 2: authenticate and give consent (implicitly)" src="../media/google-step2.png" width="800">
+        </p>
+        
+        <p align="center">
+          <img alt="Step 3: show protected content" src="../media/google-step3.png" width="800">
+        </p>
         
 Keywords: oauth human
 Platform: UNKNOWN
 Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oatk-0.0.4/oatk.egg-info/SOURCES.txt` & `oatk-0.0.6/oatk.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 LICENSE.txt
 MANIFEST.in
 setup.py
 .github/README.md
 examples/__init__.py
 examples/create-and-validate.py
 examples/web.py
+examples/google/__init__.py
+examples/google/app.py
 oatk/__init__.py
 oatk/__main__.py
 oatk.egg-info/PKG-INFO
 oatk.egg-info/SOURCES.txt
 oatk.egg-info/dependency_links.txt
 oatk.egg-info/entry_points.txt
 oatk.egg-info/requires.txt
 oatk.egg-info/top_level.txt
 oatk/fake/__init__.py
 oatk/fake/db.py
 oatk/fake/routes.py
 oatk/fake/static/__init__.py
 oatk/fake/static/oatk.js
+oatk/fake/static/style.css
 oatk/fake/templates/__init__.py
 oatk/fake/templates/authorize.html
+oatk/fake/templates/base.html
 oatk/fake/templates/create_client.html
+oatk/fake/templates/dialog.html
 oatk/fake/templates/home.html
-oatk/fake/templates/login-before-consent.html
+oatk/fake/templates/login.html
+oatk/js/__init__.py
```

### Comparing `oatk-0.0.4/setup.py` & `oatk-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "python-dotenv",
   "fire",
   "authlib",
   "flask",
   "flask_cors",
   "flask_restful",
   "pymongo",
-  
+  "requests"
 ]
 ENTRY_POINTS = {
   "console_scripts" : [
     "oatk=oatk.__main__:cli",
     
   ]
 }
```


# Comparing `tmp/siddhesh-0.1.2.tar.gz` & `tmp/siddhesh-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siddhesh-0.1.2.tar", last modified: Thu Mar 30 13:54:10 2023, max compression
+gzip compressed data, was "siddhesh-0.1.5.tar", last modified: Mon Apr 24 05:52:04 2023, max compression
```

## Comparing `siddhesh-0.1.2.tar` & `siddhesh-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 13:54:10.074283 siddhesh-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      767 2023-03-30 13:54:10.074283 siddhesh-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-30 13:54:10.080892 siddhesh-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-03-30 13:53:58.000000 siddhesh-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:54:10.050624 siddhesh-0.1.2/siddhesh/
--rw-rw-rw-   0        0        0     1153 2023-03-30 13:53:00.000000 siddhesh-0.1.2/siddhesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:54:10.071234 siddhesh-0.1.2/siddhesh.egg-info/
--rw-rw-rw-   0        0        0      767 2023-03-30 13:54:09.000000 siddhesh-0.1.2/siddhesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-03-30 13:54:09.000000 siddhesh-0.1.2/siddhesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 13:54:09.000000 siddhesh-0.1.2/siddhesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-30 13:54:09.000000 siddhesh-0.1.2/siddhesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-30 13:54:09.000000 siddhesh-0.1.2/siddhesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.442646 siddhesh-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-04-24 05:52:04.442646 siddhesh-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 05:52:04.442646 siddhesh-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-24 05:51:58.000000 siddhesh-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.418631 siddhesh-0.1.5/siddhesh/
+-rw-rw-rw-   0        0        0     1335 2023-04-24 05:46:53.000000 siddhesh-0.1.5/siddhesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:52:04.434635 siddhesh-0.1.5/siddhesh.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 05:52:04.000000 siddhesh-0.1.5/siddhesh.egg-info/top_level.txt
```

### Comparing `siddhesh-0.1.2/LICENSE` & `siddhesh-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.2/PKG-INFO` & `siddhesh-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.2
+Version: 0.1.5
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `siddhesh-0.1.2/README.md` & `siddhesh-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.2/setup.py` & `siddhesh-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.5'
 DESCRIPTION = 'Check out Siddhesh Kulthe\'s profile, or send him a direct message!'
 LONG_DESCRIPTION = 'A package that downloads Siddhesh Kulthe\'s Resume on your computer. All you need to do is to import siddhesh and use .Start() method to start the app!'
 
 # Setting up
 setup(
     name="siddhesh",
     version=VERSION,
```

### Comparing `siddhesh-0.1.2/siddhesh/__init__.py` & `siddhesh-0.1.5/siddhesh/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 URL = "https://linkedin.com/in/siddheshkulthe"
 recipient_email = "siddheshkulthe43@gmail.com"
 
 social_list = []
 
 def send_message():
     message = str(input("Enter your message: "))
+    print("...")
+    time.sleep(1)
+    print("Just so that Siddhesh can get back to you,")
+    time.sleep(1)
+    email = str(input("Please enter your email:"))
     vercel_url = "http://34.207.83.162:5000"
-    data = {"message": message}
+    data = {"message": message, "email" : email}
 
     # Make the HTTP POST request to your Vercel app's endpoint
     response = requests.post(vercel_url, json=data)
 
     if response.status_code == 200:
         print("Message sent successfully!")
     else:
```

### Comparing `siddhesh-0.1.2/siddhesh.egg-info/PKG-INFO` & `siddhesh-0.1.5/siddhesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.2
+Version: 0.1.5
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```


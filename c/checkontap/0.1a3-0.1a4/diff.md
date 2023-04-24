# Comparing `tmp/checkontap-0.1a3.tar.gz` & `tmp/checkontap-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a3.tar", last modified: Fri Apr 21 14:52:04 2023, max compression
+gzip compressed data, was "checkontap-0.1a4.tar", last modified: Mon Apr 24 14:10:37 2023, max compression
```

## Comparing `checkontap-0.1a3.tar` & `checkontap-0.1a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a3/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a3/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a3/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a3/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a3/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a3/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     2894 2023-04-21 14:49:01.363591 checkontap-0.1a3/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a3/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a3/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3836 2023-04-21 14:49:37.766604 checkontap-0.1a3/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a3/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a3/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     8126 2023-04-21 14:48:07.213286 checkontap-0.1a3/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a3/checkontap/tools/__init__.py
--rw-r--r--   0        0        0     9543 2023-04-21 14:46:55.901090 checkontap-0.1a3/checkontap/tools/cli.py
--rw-r--r--   0        0        0     2986 2023-03-23 10:28:55.299455 checkontap-0.1a3/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-04-21 14:51:14.599000 checkontap-0.1a3/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a4/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a4/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a4/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a4/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a4/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a4/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     2894 2023-04-21 14:49:01.363591 checkontap-0.1a4/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a4/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a4/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3875 2023-04-24 12:40:05.504428 checkontap-0.1a4/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a4/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a4/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     8126 2023-04-21 14:48:07.213286 checkontap-0.1a4/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a4/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0     9543 2023-04-21 14:46:55.901090 checkontap-0.1a4/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     3108 2023-04-24 12:07:20.737893 checkontap-0.1a4/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-04-24 14:04:36.718273 checkontap-0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a4/PKG-INFO
```

### Comparing `checkontap-0.1a3/checkontap/__init__.py` & `checkontap-0.1a4/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/cli.py` & `checkontap-0.1a4/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a4/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/about.py` & `checkontap-0.1a4/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a4/checkontap/ontapcmd/aggregateusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.1a4/checkontap/ontapcmd/clusterhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a4/checkontap/ontapcmd/diskhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a4/checkontap/ontapcmd/hardwarehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a4/checkontap/ontapcmd/interfacehealth.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,14 @@
             check.add_message(Status.CRITICAL, f"int {Int.name} is {Int.state}")
         if not Int.location.is_home:
             check.add_message(Status.CRITICAL, f"Int {Int.name} is on {Int.location.node.name} but should be on {Int.location.home_node.name}")
 
     check.add_message(Status.OK, f"{count} of {len(IpInts)} Interfaces are up")
     
     for Int in IpInts:
-        check.add_message(Status.OK, f"Int {Int.name}\t{Int.state}\t is homed {Int.location.is_home}")
+        check.add_message(Status.OK, f"Int {Int.name:40}{Int.state:5}{Int.ip.address:16}/{Int.ip.netmask:3} is homed {Int.location.is_home}")
         
     (code, message) = check.check_messages(separator='\n  ')
     check.exit(code=code,message=message)
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/lunusage.py` & `checkontap-0.1a4/checkontap/ontapcmd/lunusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a4/checkontap/ontapcmd/volumehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/ontapcmd/volumeusage.py` & `checkontap-0.1a4/checkontap/ontapcmd/volumeusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/tools/__init__.py` & `checkontap-0.1a4/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/tools/cli.py` & `checkontap-0.1a4/checkontap/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a3/checkontap/tools/helper.py` & `checkontap-0.1a4/checkontap/tools/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,25 @@
         if re.search(args.include,item):
             return(False)
         else:
             return(True)
 
 # Percent returned with 2 decimals
 def to_percent(max,value) -> None:
-    pct = (float(value) / int(max) ) * 100
+    try:
+        pct = (float(value) / int(max) ) * 100
+    except Exception as err:
+        return err
     return(round(pct,2))
 
 def percent_to(max, pct) -> None:
-    value = (int(max) / 100) * int(pct)
+    try:
+        value = (int(max) / 100) * int(pct)
+    except Exception as err:
+        return err
     return(int(value))
 
 # Convert bytes to Mb, Gb, Tb ....
 def bytes_to(bytes, to, bsize=1024) -> None: 
     a = {'kB' : 1, 'MB': 2, 'GB' : 3, 'TB' : 4, 'PB' : 5, 'EB' : 6 }
     #r = float(bytes)
     try:
```

### Comparing `checkontap-0.1a3/pyproject.toml` & `checkontap-0.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a3"
+version = "0.1a4"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
     "monplugin >= 0.5",
```

### Comparing `checkontap-0.1a3/PKG-INFO` & `checkontap-0.1a4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a3
+Version: 0.1a4
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```


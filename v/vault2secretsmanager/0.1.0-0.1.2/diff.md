# Comparing `tmp/vault2secretsmanager-0.1.0-py3-none-any.whl.zip` & `tmp/vault2secretsmanager-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4000 bytes, number of entries: 6
--rw-r--r--  2.0 unx     6081 b- defN 23-Apr-24 11:27 vault2secretsmanager/__init__.py
--rw-r--r--  2.0 unx      959 b- defN 23-Apr-24 11:37 vault2secretsmanager-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 11:37 vault2secretsmanager-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-Apr-24 11:37 vault2secretsmanager-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-24 11:37 vault2secretsmanager-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      546 b- defN 23-Apr-24 11:37 vault2secretsmanager-0.1.0.dist-info/RECORD
-6 files, 7767 bytes uncompressed, 2992 bytes compressed:  61.5%
+Zip file size: 4072 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     6452 b- defN 23-Apr-24 12:36 vault2secretsmanager/__init__.py
+-rw-rw-r--  2.0 unx      972 b- defN 23-Apr-24 12:39 vault2secretsmanager-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 12:39 vault2secretsmanager-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-Apr-24 12:39 vault2secretsmanager-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       21 b- defN 23-Apr-24 12:39 vault2secretsmanager-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      546 b- defN 23-Apr-24 12:39 vault2secretsmanager-0.1.2.dist-info/RECORD
+6 files, 8151 bytes uncompressed, 3064 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vault2secretsmanager/__init__.py
 Comment: 
 
-Filename: vault2secretsmanager-0.1.0.dist-info/METADATA
+Filename: vault2secretsmanager-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: vault2secretsmanager-0.1.0.dist-info/WHEEL
+Filename: vault2secretsmanager-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: vault2secretsmanager-0.1.0.dist-info/entry_points.txt
+Filename: vault2secretsmanager-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: vault2secretsmanager-0.1.0.dist-info/top_level.txt
+Filename: vault2secretsmanager-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vault2secretsmanager-0.1.0.dist-info/RECORD
+Filename: vault2secretsmanager-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vault2secretsmanager/__init__.py

```diff
@@ -133,41 +133,49 @@
 
 
 def tail() -> str:
     """
         generator function that yields in the audit file
     """
     while True:
-        with open(LOG_FILE, 'r', encoding='utf8') as handler:
-            file_index = os.stat(LOG_FILE).st_ino
-            counter = 0
-            while True:
-                line = handler.readline()
-                if not line:
-                    time.sleep(0.1)
-                    counter += 1
-                    if counter > 600:  # 1 minute
-                        if file_index != os.stat(LOG_FILE).st_ino:  # file was rotated
-                            break
-                        counter = 0
-                    continue
-                yield line
-
+        try:
+            with open(LOG_FILE, 'r', encoding='utf8') as handler:
+                file_index = os.stat(LOG_FILE).st_ino
+                counter = 0
+                while True:
+                    line = handler.readline()
+                    if not line:
+                        time.sleep(0.1)
+                        counter += 1
+                        if counter > 600:  # 1 minute
+                            if file_index != os.stat(LOG_FILE).st_ino:  # file was rotated
+                                break
+                            counter = 0
+                        continue
+                    yield line
+
+        # bad try except todo add error handling
+        except:  # pylint: disable=bare-except
+            pass
 
 def replicate():
     """
         I monitor for secret changes.
     """
     for line in tail():
-        if line.contains(MATCH):
-            audit_line = json.loads(line)
-            if audit_line['Operation'] in ['create', 'update']:
-                replicate_secret(audit_line['Path'])
-            if audit_line['Operation'] in ['delete']:
-                delete_secret(audit_line['Path'])
+        try:
+            if line.contains(MATCH):
+                audit_line = json.loads(line)
+                if audit_line['Operation'] in ['create', 'update']:
+                    replicate_secret(audit_line['Path'])
+                if audit_line['Operation'] in ['delete']:
+                    delete_secret(audit_line['Path'])
+        # bad try except todo add error handling
+        except:  # pylint: disable=bare-except
+            pass
 
 
 def setup():
     """
         I configure vault/secrets manager replicator.
     """
     user = input('What system user should the replication use: ')
@@ -200,17 +208,17 @@
 
 Type=simple
 ExecStart={sys.executable} {__file__} replicate
 
 [Install]
 WantedBy=multi-user.target
     """)
-    subprocess.run(['systemctl', 'daemon-reload'])
-    subprocess.run(['systemctl', 'start', 'vaultsync.service'])
-    subprocess.run(['systemctl', 'enable', 'vaultsync.service'])
+    subprocess.run(['systemctl', 'daemon-reload'], check=False)
+    subprocess.run(['systemctl', 'start', 'vaultsync.service'], check=False)
+    subprocess.run(['systemctl', 'enable', 'vaultsync.service'], check=False)
 
 
 def main():
     """
         The entrypoint to the app
     """
     args = _options()
```

## Comparing `vault2secretsmanager-0.1.0.dist-info/METADATA` & `vault2secretsmanager-0.1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vault2secretsmanager
-Version: 0.1.0
+Version: 0.1.2
 Summary: A systemd service that syncs vault secrets to secrets manager
-Home-page: https://github.com/tmb28054/bf2pico
+Home-page: https://github.com/tmb28054/vault2secretsmanager
 Author: Topaz M. Bott
 Author-email: topaz@topazhome.net
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```


# Comparing `tmp/micropython-umqtt.robust2-2.1.1.tar.gz` & `tmp/micropython-umqtt.robust2-2.1.2.tar.gz`

## Comparing `micropython-umqtt.robust2-2.1.1.tar` & `micropython-umqtt.robust2-2.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)        0 2021-08-31 09:11:30.000000 micropython-umqtt.robust2-2.1.1/umqtt/__init__.py
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)     4585 2021-08-31 09:11:30.000000 micropython-umqtt.robust2-2.1.1/umqtt/robust2.py
--rw-rw-r--   0 wojciech  (1000) wojciech  (1000)    10286 2021-08-31 09:11:30.000000 micropython-umqtt.robust2-2.1.1/micropython_umqtt.robust2.egg-info/PKG-INFO
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)    10286 2023-04-24 08:25:03.000000 micropython-umqtt.robust2-2.1.2/micropython_umqtt.robust2.egg-info/PKG-INFO
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)     4562 2023-04-24 08:25:03.000000 micropython-umqtt.robust2-2.1.2/umqtt/robust2.py
+-rw-rw-r--   0 wojciech  (1000) wojciech  (1000)        0 2023-04-24 08:25:03.000000 micropython-umqtt.robust2-2.1.2/umqtt/__init__.py
```

### Comparing `micropython-umqtt.robust2-2.1.1/umqtt/robust2.py` & `micropython-umqtt.robust2-2.1.2/umqtt/robust2.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
 	def log(A):
 		if A.DEBUG:
 			if type(A.conn_issue)is tuple:B,C=A.conn_issue
 			else:B=A.conn_issue;C=0
 			D='?','connect','publish','subscribe','reconnect','sendqueue','disconnect','ping','wait_msg','keepalive','check_msg';print('MQTT (%s): %r'%(D[C],B))
 	def reconnect(A):
 		try:B=super().connect(False);A.conn_issue=None;return B
-		except (OSError,simple2.MQTTException)as C:
-			A.conn_issue=C,4
-			if A.sock:A.sock.close();A.sock=None
+		except (OSError,simple2.MQTTException)as C:A.conn_issue=C,4;super().disconnect()
 	def resubscribe(A):
 		for (B,C) in A.subs:A.subscribe(B,C,False)
 	def add_msg_to_send(A,data):
 		C=len(A.msg_to_send);C+=sum(map(len,A.msg_to_confirm.values()))
 		while C>=A.MSG_QUEUE_MAX:
 			E=min(map(lambda x:x[0]if x else 65535,A.msg_to_confirm.values()),default=0)
 			if 0<E<65535:
```

### Comparing `micropython-umqtt.robust2-2.1.1/micropython_umqtt.robust2.egg-info/PKG-INFO` & `micropython-umqtt.robust2-2.1.2/micropython_umqtt.robust2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: micropython-umqtt.robust2
-Version: 2.1.1
+Version: 2.1.2
 Summary: MQTT client for MicroPython ("robust" version).
 Home-page: https://github.com/fizista/micropython-umqtt.robust2
 Author: Wojciech Banaś
 Author-email: fizista+umqtt.robust2@gmail.com
 License: MIT
 Description: .. role:: bash(code)
            :language: bash
```


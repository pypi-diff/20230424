# Comparing `tmp/kisaBobPkgs-1.0.0.8-py3-none-any.whl.zip` & `tmp/kisaBobPkgs-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9050 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     9049 b- defN 22-Aug-22 03:31 kisa.py
+Zip file size: 9074 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     9124 b- defN 22-Aug-22 03:41 kisa.py
 -rw-rw-r--  2.0 unx       23 b- defN 22-Aug-22 03:24 kisaBobPkgs.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Aug-21 12:21 test_bob8gook.py
 -rw-rw-r--  2.0 unx       30 b- defN 22-Aug-22 02:13 testbob8gook.py
 -rw-rw-r--  2.0 unx    13074 b- defN 22-Aug-21 14:44 whois.py
--rw-rw-r--  2.0 unx      201 b- defN 22-Aug-22 03:32 kisaBobPkgs-1.0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-22 03:32 kisaBobPkgs-1.0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 22-Aug-22 03:32 kisaBobPkgs-1.0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      661 b- defN 22-Aug-22 03:32 kisaBobPkgs-1.0.0.8.dist-info/RECORD
-9 files, 23193 bytes uncompressed, 7920 bytes compressed:  65.9%
+-rw-rw-r--  2.0 unx      201 b- defN 22-Aug-22 03:42 kisaBobPkgs-1.0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Aug-22 03:42 kisaBobPkgs-1.0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 22-Aug-22 03:42 kisaBobPkgs-1.0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      661 b- defN 22-Aug-22 03:42 kisaBobPkgs-1.0.0.9.dist-info/RECORD
+9 files, 23268 bytes uncompressed, 7944 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: testbob8gook.py
 Comment: 
 
 Filename: whois.py
 Comment: 
 
-Filename: kisaBobPkgs-1.0.0.8.dist-info/METADATA
+Filename: kisaBobPkgs-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: kisaBobPkgs-1.0.0.8.dist-info/WHEEL
+Filename: kisaBobPkgs-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: kisaBobPkgs-1.0.0.8.dist-info/top_level.txt
+Filename: kisaBobPkgs-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: kisaBobPkgs-1.0.0.8.dist-info/RECORD
+Filename: kisaBobPkgs-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kisa.py

```diff
@@ -21,15 +21,15 @@
         
 botEmail = "bob8gook_kisa@webex.bot"
 accessToken = "YzE4Y2ZhYjAtMDk5Yy00NTZlLWIwYjAtODYwNzQwNDExOWRmMDFjZmI1ODYtM2Rm_PF84_22cb7792-d880-4ec5-b6a6-649d9411bb5e"
 headers = {"Authorization": "Bearer %s" % accessToken, "Content-Type": "application/json", 'Accept' : 'application/json'}
 roomId_kisa_private = 'Y2lzY29zcGFyazovL3VzL1JPT00vNDkwNzIwMjAtMTBhNy0xMWVkLTk4ZDktNzU3YWU5MmY2MDFh' #kisa 개인방
 roomId_soc = 'Y2lzY29zcGFyazovL3VzL1JPT00vZmIwY2M1YTAtMDYzZS0xMWVjLWExNzgtZDEzYjhjMjEwNzVk'
 roomId_availability = 'Y2lzY29zcGFyazovL3VzL1JPT00vZTVmMmJiYTAtMTE2Ni0xMWVkLThmMjctZmQ4YjY5ODZmODc3'
-roomId_use = roomId_kisa_private
+roomId_use = roomId_soc
 
 now = datetime.datetime.now()
 now = now + datetime.timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=9, weeks=0)
 
 try:
     with open('num_last.txt', 'r') as f:
         num_last = int(f.read())
@@ -139,23 +139,25 @@
                     print('@@@ num : ' + str(num_last))
     return list_files
 
                 
 app = Flask(__name__)
 @app.route('/', methods=['POST'])
 def receive():
+    global roomId_kisa_private
     data = request.json.get('data')
     email, messageId = data['personEmail'], data['id']
     print('message : ' + str(data))
     if email == botEmail:
         return ("")
     response = json.loads(requests.request("GET", "https://api.ciscospark.com/v1/messages/{}".format(messageId), headers=headers).text)
     #print(str(response))
     #msgs = response['text'].strip().split('\n')
-    SendMessage(payload, "test")
+    payload = {"roomId": roomId_kisa_private}
+    SendMessage(payload, "Echo : Hi!!")
     return {'status' : 'success', 'num_last': num_last}
 
 @app.route('/', methods=['GET'])
 def BotComu():
     global roomId_use, num_last
     temp = num_last
     print('num_last : ' + str(num_last) )
```


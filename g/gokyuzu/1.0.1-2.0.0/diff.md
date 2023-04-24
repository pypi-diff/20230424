# Comparing `tmp/gokyuzu-1.0.1.tar.gz` & `tmp/gokyuzu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-1.0.1.tar", last modified: Sat Apr 22 19:49:05 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.0.tar", last modified: Mon Apr 24 17:51:15 2023, max compression
```

## Comparing `gokyuzu-1.0.1.tar` & `gokyuzu-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681692 gokyuzu-1.0.1/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-1.0.1/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 19:49:05.681589 gokyuzu-1.0.1/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     1761 2023-04-22 18:24:18.000000 gokyuzu-1.0.1/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.680322 gokyuzu-1.0.1/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     6402 2023-04-22 19:28:38.000000 gokyuzu-1.0.1/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-1.0.1/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)     3075 2023-04-22 19:21:58.000000 gokyuzu-1.0.1/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)     8830 2023-04-22 19:48:01.000000 gokyuzu-1.0.1/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681067 gokyuzu-1.0.1/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     2537 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      331 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-22 19:49:05.000000 gokyuzu-1.0.1/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-22 19:48:23.000000 gokyuzu-1.0.1/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-22 19:49:05.681727 gokyuzu-1.0.1/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-22 19:48:19.000000 gokyuzu-1.0.1/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-22 19:49:05.681289 gokyuzu-1.0.1/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-1.0.1/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-1.0.1/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 17:51:15.263859 gokyuzu-2.0.0/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.0/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6275 2023-04-24 17:51:15.263752 gokyuzu-2.0.0/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5499 2023-04-24 17:49:40.000000 gokyuzu-2.0.0/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 17:51:15.262187 gokyuzu-2.0.0/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8584 2023-04-24 17:04:21.000000 gokyuzu-2.0.0/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-2.0.0/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      224 2023-04-24 17:33:31.000000 gokyuzu-2.0.0/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4015 2023-04-24 17:31:55.000000 gokyuzu-2.0.0/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    29875 2023-04-24 17:38:16.000000 gokyuzu-2.0.0/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 17:51:15.263214 gokyuzu-2.0.0/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6275 2023-04-24 17:51:15.000000 gokyuzu-2.0.0/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-04-24 17:51:15.000000 gokyuzu-2.0.0/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-24 17:51:15.000000 gokyuzu-2.0.0/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-24 17:51:15.000000 gokyuzu-2.0.0/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-24 17:51:15.000000 gokyuzu-2.0.0/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-24 17:50:41.000000 gokyuzu-2.0.0/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-24 17:51:15.263893 gokyuzu-2.0.0/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-24 17:50:35.000000 gokyuzu-2.0.0/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 17:51:15.263444 gokyuzu-2.0.0/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.0/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-2.0.0/tests/test_main.py
```

### Comparing `gokyuzu-1.0.1/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.0/gokyuzu/BlueskyEndpoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,279 @@
 class BlueskyEndpoints():
+
     def __init__(self, BSKY_SERVER):
         self.BSKY_SERVER = BSKY_SERVER
         if not self.BSKY_SERVER:
             self.BSKY_SERVER = "https://bsky.social"
 
     def get_url(self, path):
         return self.BSKY_SERVER + path
     
-    # com.atproto.server
+    #region com.atproto.admin
+    def disableInviteCodes(self):
+        return self.get_url("/xrpc/com.atproto.admin.disableInviteCodes")
+        
+    def getInviteCodes(self):
+        return self.get_url("/xrpc/com.atproto.admin.getInviteCodes")
+
+    def getModerationAction(self):
+        return self.get_url("/xrpc/com.atproto.admin.getModerationAction")
+    
+    def getModerationActions(self):
+        return self.get_url("/xrpc/com.atproto.admin.getModerationActions")
+        
+    def getModerationReport(self):
+        return self.get_url("/xrpc/com.atproto.admin.getModerationReport")
+
+    def getModerationReports(self):
+        return self.get_url("/xrpc/com.atproto.admin.getModerationReports")
+        
+    def getRecord(self):
+        return self.get_url("/xrpc/com.atproto.admin.getRecord")
+        
+    def getRepo(self):
+        return self.get_url("/xrpc/com.atproto.admin.getRepo")
+
+    def resolveModerationReports(self):
+        return self.get_url("/xrpc/com.atproto.admin.resolveModerationReports")
+        
+    def reverseModerationAction(self):
+        return self.get_url("/xrpc/com.atproto.admin.reverseModerationAction")
+        
+    def searchRepos(self):
+        return self.get_url("/xrpc/com.atproto.admin.searchRepos")
+        
+    def takeModerationAction(self):
+        return self.get_url("/xrpc/com.atproto.admin.takeModerationAction")
+        
+    def updateAccountEmail(self):
+        return self.get_url("/xrpc/com.atproto.admin.updateAccountEmail")
+
+    def updateAccountHandle(self):
+        return self.get_url("/xrpc/com.atproto.admin.updateAccountHandle")
+
+    #endregion
+
+    #region com.atproto.identity
+    def resolveHandle(self):
+        return self.get_url("/xrpc/com.atproto.identity.resolveHandle")
+
+    def updateHandle(self):
+        return self.get_url("/xrpc/com.atproto.identity.updateHandle")
+
+    #endregion
+
+    #region com.atproto.label
+    def queryLabels(self):
+        return self.get_url("/com.atproto.label.queryLabels")
+    
+    def subscribeLabels(self):
+        return self.get_url("/com.atproto.label.subscribeLabels")
+    #endregion
+
+    #region com.atproto.repo
+    def applyWrites(self):
+        return self.get_url("/xrpc/com.atproto.repo.applyWrites")
+
+    def createRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.createRecord")
+
+    def deleteRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.deleteRecord")
+
+    def describeRepo(self):
+        return self.get_url("/xrpc/com.atproto.repo.describeRepo")
+
+    def getRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.getRecord")
+
+    def listRecords(self):
+        return self.get_url("/xrpc/com.atproto.repo.listRecords")
+
+    def putRecord(self):
+        return self.get_url("/xrpc/com.atproto.repo.putRecord")
+
+    def uploadBlob(self):
+        return self.get_url("/xrpc/com.atproto.repo.uploadBlob")
+
+    #endregion
+
+    #region com.atproto.server
     def createAccount(self):
         return self.get_url("/xrpc/com.atproto.server.createAccount")
-    
-    def getAccountInviteCodes(self):
-        return self.get_url("/xrpc/com.atproto.server.getAccountInviteCodes")
-    
+
+    def createAppPassword(self):
+        return self.get_url("/xrpc/com.atproto.server.createAppPassword")
+
     def createInviteCode(self):
         return self.get_url("/xrpc/com.atproto.server.createInviteCode")
-    
+
     def createInviteCodes(self):
         return self.get_url("/xrpc/com.atproto.server.createInviteCodes")
-    
-    def describeServer(self):
-        return self.get_url("/xrpc/com.atproto.server.describeServer")
-    
+
+    def createSession(self):
+        return self.get_url("/xrpc/com.atproto.server.createSession")
+
     def deleteAccount(self):
         return self.get_url("/xrpc/com.atproto.server.deleteAccount")
-    
+
+    def deleteSession(self):
+        return self.get_url("/xrpc/com.atproto.server.deleteSession")
+
+    def describeServer(self):
+        return self.get_url("/xrpc/com.atproto.server.describeServer")
+
+    def getAccountInviteCodes(self):
+        return self.get_url("/xrpc/com.atproto.server.getAccountInviteCodes")
+
+    def getSession(self):
+        return self.get_url("/xrpc/com.atproto.server.getSession")
+
+    def listAppPassword(self):
+        return self.get_url("/xrpc/com.atproto.server.listAppPassword")
+
     def resetPassword(self):
         return self.get_url("/xrpc/com.atproto.server.resetPassword")
-    
+
+    def refreshSession(self):
+        return self.get_url("/xrpc/com.atproto.server.refreshSession")
+
+    def requestAccountDelete(self):
+        return self.get_url("/xrpc/com.atproto.server.requestAccountDelete")
+
     def requestPasswordReset(self):
         return self.get_url("/xrpc/com.atproto.server.requestPasswordReset")
+
+    def revokeAppPassword(self):
+        return self.get_url("/xrpc/com.atproto.server.revokeAppPassword")
+
+    #endregion
+
+    #region com.atproto.sync
+    def getBlob(self):
+        return self.get_url("/xrpc/com.atproto.sync.getBlob")
     
-    def createSession(self):
-        return self.get_url("/xrpc/com.atproto.server.createSession")
+    def getBlocks(self):
+        return self.get_url("/xrpc/com.atproto.sync.getBlocks")
     
-    def deleteSession(self):
-        return self.get_url("/xrpc/com.atproto.server.deleteSession")
+    def getCheckout(self):
+        return self.get_url("/xrpc/com.atproto.sync.getCheckout")
     
-    def getSession(self):
-        return self.get_url("/xrpc/com.atproto.server.getSession")
+    def getCommitPath(self):
+        return self.get_url("/xrpc/com.atproto.sync.getCommitPath")
     
-    def refreshSession(self):
-        return self.get_url("/xrpc/com.atproto.server.refreshSession")
+    def getHead(self):
+        return self.get_url("/xrpc/com.atproto.sync.getHead")
     
-    def createAppPassword(self):
-        return self.get_url("/xrpc/com.atproto.server.createAppPassword")
+    def getRecord(self):
+        return self.get_url("/xrpc/com.atproto.sync.getRecord")
     
-    def listAppPassword(self):
-        return self.get_url("/xrpc/com.atproto.server.listAppPassword")
+    def getRepo(self):
+        return self.get_url("/xrpc/com.atproto.sync.getRepo")
     
-    def revokeAppPassword(self):
-        return self.get_url("/xrpc/com.atproto.server.revokeAppPassword")
+    def listBlobs(self):
+        return self.get_url("/xrpc/com.atproto.sync.listBlobs")
+    
+    def notifyOfUpdate(self):
+        return self.get_url("/xrpc/com.atproto.sync.notifyOfUpdate")
+    
+    def requestCrawl(self):
+        return self.get_url("/xrpc/com.atproto.sync.requestCrawl")
+    
+    def subscribeRepos(self):
+        return self.get_url("/xrpc/com.atproto.sync.subscribeRepos")
+
+    #endregion
 
-    # app.bsky.actor
+    #region app.bsky.actor
     def getProfile(self):
         return self.get_url("/xrpc/app.bsky.actor.getProfile")
-    
+
     def getProfiles(self):
         return self.get_url("/xrpc/app.bsky.actor.getProfiles")
     
-    # app.bsky.unspecced
-    def getPopular(self):
-        return self.get_url("/xrpc/app.bsky.unspecced.getPopular")
+    def getSuggestions(self):
+        return self.get_url("/xrpc/app.bsky.actor.getSuggestions")
     
-    # app.bsky.feed
-    def getTimeline(self):
-        return self.get_url("/xrpc/app.bsky.feed.getTimeline")
+    def searchActors(self):
+        return self.get_url("/xrpc/app.bsky.actor.searchActors")
     
+    def searchActorsTypeahead(self):
+        return self.get_url("/xrpc/app.bsky.actor.searchActorsTypeahead")
+    #endregion
+
+    #region app.bsky.feed
     def getAuthorFeed(self):
         return self.get_url("/xrpc/app.bsky.feed.getAuthorFeed")
     
-    def getPostThread(self):
-        return self.get_url("/xrpc/app.bsky.feed.getPostThread")
-    
     def getLikes(self):
         return self.get_url("/xrpc/app.bsky.feed.getLikes")
-    
+
+    def getPostThread(self):
+        return self.get_url("/xrpc/app.bsky.feed.getPostThread")
+
     def getRepostedBy(self):
         return self.get_url("/xrpc/app.bsky.feed.getRepostedBy")
 
-    # app.bsky.graph    
+    def getTimeline(self):
+        return self.get_url("/xrpc/app.bsky.feed.getTimeline")
+
+    def like(self):
+        return self.get_url("/xrpc/app.bsky.feed.like")
+    
+    def post(self):
+        return self.get_url("/xrpc/app.bsky.feed.post")
+    
+    def repost(self):
+        return self.get_url("/xrpc/app.bsky.feed.repost")
+    #endregion
+
+    #region app.bsky.graph
+    def follow(self):
+        return self.get_url("/xrpc/app.bsky.graph.follow")
+
     def getFollowers(self):
         return self.get_url("/xrpc/app.bsky.graph.getFollowers")
-    
+
     def getFollows(self):
         return self.get_url("/xrpc/app.bsky.graph.getFollows")
-    
+
     def getMutes(self):
         return self.get_url("/xrpc/app.bsky.graph.getMutes")
-    
+
     def muteActor(self):
         return self.get_url("/xrpc/app.bsky.graph.muteActor")
-    
+
     def unmuteActor(self):
         return self.get_url("/xrpc/app.bsky.graph.unmuteActor")
-    
-    # app.bsky.notification
+
+    #endregion
+
+    #region app.bsky.notification
+    def getUnreadCount(self):
+        return self.get_url("/xrpc/app.bsky.notification.getUnreadCount")
+
     def listNotifications(self):
         return self.get_url("/xrpc/app.bsky.notification.listNotifications")
-    
+
     def updateSeen(self):
         return self.get_url("/xrpc/app.bsky.notification.updateSeen")
-    
-    def getUnreadCount(self):
-        return self.get_url("/xrpc/app.bsky.notification.getUnreadCount")
-    
-    # com.atproto.repo
-    def applyWrites(self):
-        return self.get_url("/xrpc/com.atproto.repo.applyWrites")
 
-    def createRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.createRecord")
-    
-    def deleteRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.deleteRecord")
-    
-    def describeRepo(self):
-        return self.get_url("/xrpc/com.atproto.repo.describeRepo")
-    
-    def getRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.getRecord")
-    
-    def listRecords(self):
-        return self.get_url("/xrpc/com.atproto.repo.listRecords")
-    
-    def putRecord(self):
-        return self.get_url("/xrpc/com.atproto.repo.putRecord")
-    
-    def uploadBlob(self):
-        return self.get_url("/xrpc/com.atproto.repo.uploadBlob")
-    
-    # com.atproto.identity
-    def resolveHandle(self):
-        return self.get_url("/xrpc/com.atproto.identity.resolveHandle")
-    
-    def updateHandle(self):
-        return self.get_url("/xrpc/com.atproto.identity.updateHandle")
-    
-    # health
-    def health(self):
-        return self.get_url("/xrpc/health")
+    #endregion
 
-    # options
-    def getAllEndpoints(self):
-        all = []
-
-        all.append(self.createAccount())
-        all.append(self.createSession())
-        all.append(self.getSession())
-        all.append(self.getAccountInviteCodes())
-        all.append(self.getProfile())
-        all.append(self.getProfiles())
-        all.append(self.getPopular())
-        all.append(self.getTimeline())
-        all.append(self.getAuthorFeed())
-        all.append(self.getPostThread())
-        all.append(self.getFollowers())
-        all.append(self.getFollows())
-        all.append(self.listNotifications())
-        all.append(self.updateSeen())
-        all.append(self.createRecord())
-        all.append(self.deleteRecord())
-        all.append(self.resolveHandle())
-        all.append(self.updateHandle())
-        all.append(self.getRecord())
-        all.append(self.listRecords())
-        all.append(self.putRecord())
-        all.append(self.uploadBlob())
-        all.append(self.applyWrites())
-        all.append(self.describeRepo())
-        all.append(self.getUnreadCount())
-        all.append(self.getFollowers())
-        all.append(self.getFollows())
-        all.append(self.getMutes())
-        all.append(self.muteActor())
-        all.append(self.unmuteActor())
-        all.append(self.describeServer())
-        all.append(self.deleteAccount())
-        all.append(self.resetPassword())
-        all.append(self.requestPasswordReset())
-        all.append(self.deleteSession())
-        all.append(self.refreshSession())
-        all.append(self.createAppPassword())
-        all.append(self.listAppPassword())
-        all.append(self.revokeAppPassword())
-        all.append(self.health())
+    #region app.bsky.richtext
+    def facet(self):
+        return self.get_url("/xrpc/app.bsky.richtext.facet")
+    #endregion
 
-        return all
+    #region app.bsky.unspecced
+    def getPopular(self):
+        return self.get_url("/xrpc/app.bsky.unspecced.getPopular")
 
-    
+    #endregion
+
+    #region health
+    def health(self):
+        return self.get_url("/xrpc/health")
 
+    #endregion
```

### Comparing `gokyuzu-1.0.1/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.0/gokyuzu/BlueskySession.py`

 * *Files 17% similar despite different names*

```diff
@@ -72,11 +72,31 @@
         return response
     
     def postJson(self, url, json, **kwargs):
         headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
         response = requests.post(url, headers=headers, json=json, **kwargs)
         return response
     
+    def postJpeg(self, url, jpeg, **kwargs):
+        headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'image/jpeg' }
+        response = requests.post(url, headers=headers, data=jpeg, **kwargs)
+        return response
+    
     def options(self, url, **kwargs):
         headers = {'Authorization': f'Bearer {self.getAccessToken()}'}
         response = requests.options(url, headers=headers, **kwargs)
         return response
+    
+    def createRecord(self, request_data, **kwargs):
+        request_url = self.ENDPOINTS.createRecord()
+        headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
+        response = requests.post(request_url, headers=headers, json=request_data, **kwargs)
+        return response
+    
+    def deleteRecord(self, request_data, **kwargs):
+        request_url = self.ENDPOINTS.deleteRecord()
+        headers = { 'Authorization': f'Bearer {self.getAccessToken()}', 'Content-Type': 'application/json' }
+        response = requests.post(request_url, headers=headers, json=request_data, **kwargs)
+        return response
+                
+
+
```

### Comparing `gokyuzu-1.0.1/setup.py` & `gokyuzu-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='1.0.1',
+    version='2.0.0',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-1.0.1/tests/test_main.py` & `gokyuzu-2.0.0/tests/test_main.py`

 * *Files identical despite different names*


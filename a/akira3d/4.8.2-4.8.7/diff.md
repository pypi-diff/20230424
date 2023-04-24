# Comparing `tmp/akira3d-4.8.2.tar.gz` & `tmp/akira3d-4.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akira3d-4.8.2.tar", last modified: Thu Apr 13 13:35:38 2023, max compression
+gzip compressed data, was "akira3d-4.8.7.tar", last modified: Mon Apr 24 17:21:32 2023, max compression
```

## Comparing `akira3d-4.8.2.tar` & `akira3d-4.8.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.493916 akira3d-4.8.2/
--rw-rw-rw-   0        0        0      144 2023-04-13 13:35:38.493916 akira3d-4.8.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.488915 akira3d-4.8.2/akira3d/
--rw-rw-rw-   0        0        0      518 2023-04-12 17:31:21.000000 akira3d-4.8.2/akira3d/__init__.py
--rw-rw-rw-   0        0        0     2045 2023-04-12 17:20:27.000000 akira3d-4.8.2/akira3d/camera.py
--rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/colliders.py
--rw-rw-rw-   0        0        0      170 2023-04-12 17:46:39.000000 akira3d-4.8.2/akira3d/createNewGame.py
--rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/gameEngine.py
--rw-rw-rw-   0        0        0      522 2023-04-12 17:17:16.000000 akira3d-4.8.2/akira3d/light.py
--rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/mesh.py
--rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/mobs.py
--rw-rw-rw-   0        0        0     7810 2023-04-11 08:26:43.000000 akira3d-4.8.2/akira3d/model.py
--rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/phisics.py
--rw-rw-rw-   0        0        0     6942 2023-04-11 08:32:00.000000 akira3d-4.8.2/akira3d/render.py
--rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/shader_program.py
--rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/texture.py
--rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.8.2/akira3d/vao.py
--rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.8.2/akira3d/vbo.py
--rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.8.2/akira3d/vidSys.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:35:38.493916 akira3d-4.8.2/akira3d.egg-info/
--rw-rw-rw-   0        0        0      144 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       84 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 13:35:38.000000 akira3d-4.8.2/akira3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 13:35:38.494917 akira3d-4.8.2/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-04-13 13:35:17.000000 akira3d-4.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:21:32.074711 akira3d-4.8.7/
+-rw-rw-rw-   0        0        0      144 2023-04-24 17:21:32.074711 akira3d-4.8.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 17:21:32.070709 akira3d-4.8.7/akira3d/
+-rw-rw-rw-   0        0        0      518 2023-04-12 17:31:21.000000 akira3d-4.8.7/akira3d/__init__.py
+-rw-rw-rw-   0        0        0     2045 2023-04-12 17:20:27.000000 akira3d-4.8.7/akira3d/camera.py
+-rw-rw-rw-   0        0        0     4758 2023-04-24 08:24:20.000000 akira3d-4.8.7/akira3d/colliders.py
+-rw-rw-rw-   0        0        0      170 2023-04-12 17:46:39.000000 akira3d-4.8.7/akira3d/createNewGame.py
+-rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.8.7/akira3d/gameEngine.py
+-rw-rw-rw-   0        0        0      522 2023-04-12 17:17:16.000000 akira3d-4.8.7/akira3d/light.py
+-rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.8.7/akira3d/mesh.py
+-rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.8.7/akira3d/mobs.py
+-rw-rw-rw-   0        0        0     7810 2023-04-11 08:26:43.000000 akira3d-4.8.7/akira3d/model.py
+-rw-rw-rw-   0        0        0     1249 2023-04-23 08:33:39.000000 akira3d-4.8.7/akira3d/phisics.py
+-rw-rw-rw-   0        0        0     5725 2023-04-23 08:49:47.000000 akira3d-4.8.7/akira3d/render.py
+-rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.8.7/akira3d/shader_program.py
+-rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.8.7/akira3d/texture.py
+-rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.8.7/akira3d/vao.py
+-rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.8.7/akira3d/vbo.py
+-rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.8.7/akira3d/vidSys.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:21:32.073711 akira3d-4.8.7/akira3d.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       84 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 17:21:31.000000 akira3d-4.8.7/akira3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:21:32.075712 akira3d-4.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-04-24 17:21:24.000000 akira3d-4.8.7/setup.py
```

### Comparing `akira3d-4.8.2/akira3d/__init__.py` & `akira3d-4.8.7/akira3d/__init__.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/camera.py` & `akira3d-4.8.7/akira3d/camera.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/light.py` & `akira3d-4.8.7/akira3d/light.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/mobs.py` & `akira3d-4.8.7/akira3d/mobs.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/model.py` & `akira3d-4.8.7/akira3d/model.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/phisics.py` & `akira3d-4.8.7/akira3d/phisics.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         if self.f != [0, 0, 0]:
             m = vecLen(self.f)
             v = normVec(self.f)
             return F(v, m)
         else:
             return F([0, 0, 0], 0)
 
+
 def mul(f1, f2):
     f = [f1.f[i]*f2.f[i] for i in range(3)]
     if f !=[0, 0, 0]:
         m = vecLen(f1)
         v = normVec(f1)
         return F(v, m)
     else:
```

### Comparing `akira3d-4.8.2/akira3d/render.py` & `akira3d-4.8.7/akira3d/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,38 +98,14 @@
 
                 self.app.ctx.screen.use()
                 [self.scs[self.name]['objects'][_].render() for _ in self.scs[self.name]['render']]
 
 
         def destroy(self): self.depth_fbo.release()
 
-    class Pointer():
-        def __init__(self, cam, pos):
-            self.cam = cam
-            self.pos = pos
-            self.fov = cam.FOV
-            self.nfov = self.fov//cam.aspect_ratio
-            self.angle = [0, 0]
-            self.fa = 0
-
-        def behind(self):
-            toOther = self.pos - self.cam.position
-            return glm.dot(self.cam.forward, toOther) < 0
-
-        def update(self):
-            pos = self.cam.position
-            self.fa = math.degrees(math.atan2(self.pos.y - pos.y, self.pos.x - pos.x))
-            self.fa += self.cam.yaw
-            self.fb = math.degrees(math.atan2(self.pos.y - pos.y, self.pos.z - pos.z))
-            self.fb += self.cam.pitch
-            posn = [li(((cos(-self.fov), sin(-self.fov)), (cos(0), sin(0))), ((0, 0), (cos(-self.fa), sin(-self.fa)))), li(((cos(-self.nfov), sin(-self.nfov)), (cos(0), sin(0))), ((0, 0), (cos(-self.fb), sin(-self.fb))))]
-            m = l((cos(-self.fov), sin(-self.fov)), posn[0]) / l((cos(-self.fov), sin(-self.fov)), (cos(0), sin(0)))
-            m1 = l((cos(-self.nfov), sin(-self.nfov)), posn[1]) / l((cos(-self.nfov), sin(-self.nfov)), (cos(0), sin(0)))
-            self.angle = [m, m1]
-
     def quit(self):
         self.mesh.destroy()
         self.scene.destroy()
         pg.quit()
         exit()
 
     def init(self):
```

### Comparing `akira3d-4.8.2/akira3d/shader_program.py` & `akira3d-4.8.7/akira3d/shader_program.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/texture.py` & `akira3d-4.8.7/akira3d/texture.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/vao.py` & `akira3d-4.8.7/akira3d/vao.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/vbo.py` & `akira3d-4.8.7/akira3d/vbo.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.8.2/akira3d/vidSys.py` & `akira3d-4.8.7/akira3d/vidSys.py`

 * *Files identical despite different names*


# Comparing `tmp/aitviewer-1.8.0.tar.gz` & `tmp/aitviewer-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aitviewer-1.8.0.tar", last modified: Tue Mar 28 14:50:05 2023, max compression
+gzip compressed data, was "dist\aitviewer-1.8.1.tar", last modified: Mon Apr 24 13:16:01 2023, max compression
```

## Comparing `aitviewer-1.8.0.tar` & `aitviewer-1.8.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/
--rw-rw-rw-   0        0        0    35823 2023-01-30 08:41:59.000000 aitviewer-1.8.0/LICENSE
--rw-rw-rw-   0        0        0      115 2023-01-30 08:41:59.000000 aitviewer-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4486 2023-03-28 14:50:05.000000 aitviewer-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     4021 2023-03-28 14:45:25.000000 aitviewer-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/
--rw-rw-rw-   0        0        0       23 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/__init__.py
--rw-rw-rw-   0        0        0      749 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/aitvconfig.yaml
--rw-rw-rw-   0        0        0     3626 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/configuration.py
--rw-rw-rw-   0        0        0     6939 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/headless.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/models/
--rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/models/__init__.py
--rw-rw-rw-   0        0        0    11260 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/models/smpl.py
--rw-rw-rw-   0        0        0     6148 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/models/star.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/remote/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/__init__.py
--rw-rw-rw-   0        0        0      918 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/message.py
--rw-rw-rw-   0        0        0     1940 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/node.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/remote/renderables/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/__init__.py
--rw-rw-rw-   0        0        0     1854 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/arrows.py
--rw-rw-rw-   0        0        0     1386 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/lines.py
--rw-rw-rw-   0        0        0     1454 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/meshes.py
--rw-rw-rw-   0        0        0     1738 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/rigid_bodies.py
--rw-rw-rw-   0        0        0     2737 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/smpl.py
--rw-rw-rw-   0        0        0     1475 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/renderables/spheres.py
--rw-rw-rw-   0        0        0     8487 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/remote/viewer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/renderables/
--rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/renderables/__init__.py
--rw-rw-rw-   0        0        0     5482 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/arrows.py
--rw-rw-rw-   0        0        0    10872 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/billboard.py
--rw-rw-rw-   0        0        0     4247 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/bounding_boxes.py
--rw-rw-rw-   0        0        0     1272 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/coordinate_system.py
--rw-rw-rw-   0        0        0    16984 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/lines.py
--rw-rw-rw-   0        0        0    45433 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/meshes.py
--rw-rw-rw-   0        0        0    13660 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/multi_view_system.py
--rw-rw-rw-   0        0        0    12907 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/plane.py
--rw-rw-rw-   0        0        0     8013 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/point_clouds.py
--rw-rw-rw-   0        0        0     6755 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/rigid_bodies.py
--rw-rw-rw-   0        0        0     9946 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/sdf.py
--rw-rw-rw-   0        0        0     4675 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/skeletons.py
--rw-rw-rw-   0        0        0    31990 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/smpl.py
--rw-rw-rw-   0        0        0    10070 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/spheres.py
--rw-rw-rw-   0        0        0     6112 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/renderables/star.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/resources/
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/resources/fonts/
--rw-rw-rw-   0        0        0   162888 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/resources/fonts/Custom.sfd
--rw-rw-rw-   0        0        0    17132 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/resources/fonts/Custom.ttf
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/scene/
--rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/scene/__init__.py
--rw-rw-rw-   0        0        0    39356 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/camera.py
--rw-rw-rw-   0        0        0     2720 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/camera_utils.py
--rw-rw-rw-   0        0        0     9321 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/light.py
--rw-rw-rw-   0        0        0     1538 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/material.py
--rw-rw-rw-   0        0        0    26596 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/node.py
--rw-rw-rw-   0        0        0    17344 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/scene/scene.py
--rw-rw-rw-   0        0        0     8658 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/server.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/shaders/
--rw-rw-rw-   0        0        0     2073 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/chessboard.glsl
--rw-rw-rw-   0        0        0      898 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/clipping.glsl
--rw-rw-rw-   0        0        0     4442 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/cylinder.glsl
--rw-rw-rw-   0        0        0     2440 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/directional_lights.glsl
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/shaders/fragment_picking/
--rw-rw-rw-   0        0        0      427 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/fragment_picking/frag_map.fs.glsl
--rw-rw-rw-   0        0        0     1021 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/fragment_picking/frag_pick.glsl
--rw-rw-rw-   0        0        0     2190 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/lines_instanced.vs.glsl
--rw-rw-rw-   0        0        0     1480 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/lines_instanced_positions.vs.glsl
--rw-rw-rw-   0        0        0     5571 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/lit_with_edges.glsl
--rw-rw-rw-   0        0        0      734 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/mesh_positions.vs.glsl
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/shaders/outline/
--rw-rw-rw-   0        0        0     1398 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/outline/outline_draw.glsl
--rw-rw-rw-   0        0        0      480 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/outline/outline_prepare.fs.glsl
--rw-rw-rw-   0        0        0      522 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/screen_texture.glsl
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/shaders/shadow_mapping/
--rw-rw-rw-   0        0        0      287 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/shadow_mapping/depth_only.fs.glsl
--rw-rw-rw-   0        0        0      497 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/shadow_mapping/raw_depth.glsl
--rw-rw-rw-   0        0        0      481 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/simple_unlit.glsl
--rw-rw-rw-   0        0        0     1015 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/sphere_instanced.vs.glsl
--rw-rw-rw-   0        0        0      641 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders/sphere_instanced_positions.vs.glsl
--rw-rw-rw-   0        0        0     1170 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/shaders/visualize.glsl
--rw-rw-rw-   0        0        0     4413 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/shaders.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/streamables/
--rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.0/aitviewer/streamables/__init__.py
--rw-rw-rw-   0        0        0     1345 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/streamables/streamable.py
--rw-rw-rw-   0        0        0     3951 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/streamables/webcam.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer/utils/
--rw-rw-rw-   0        0        0       49 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/__init__.py
--rw-rw-rw-   0        0        0     1948 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/decorators.py
--rw-rw-rw-   0        0        0     1574 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/exceptions.py
--rw-rw-rw-   0        0        0     4427 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/imgui_integration.py
--rw-rw-rw-   0        0        0     3493 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/path.py
--rw-rw-rw-   0        0        0     3770 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/perf_timer.py
--rw-rw-rw-   0        0        0     4589 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/pyqt5_window.py
--rw-rw-rw-   0        0        0     6798 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/so3.py
--rw-rw-rw-   0        0        0    14475 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/utils/utils.py
--rw-rw-rw-   0        0        0    77877 2023-03-28 14:45:25.000000 aitviewer-1.8.0/aitviewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/
--rw-rw-rw-   0        0        0     4486 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2886 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      285 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-28 14:50:05.000000 aitviewer-1.8.0/aitviewer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2023-03-28 14:45:25.000000 aitviewer-1.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      273 2023-03-28 14:50:05.000000 aitviewer-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-03-28 14:45:25.000000 aitviewer-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 14:50:05.000000 aitviewer-1.8.0/tests/
--rw-rw-rw-   0        0        0     9177 2023-03-28 14:45:25.000000 aitviewer-1.8.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     5739 2023-03-28 14:45:25.000000 aitviewer-1.8.0/tests/test_renderables.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-30 08:41:59.000000 aitviewer-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0      115 2023-01-30 08:41:59.000000 aitviewer-1.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4611 2023-04-24 13:16:01.000000 aitviewer-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4146 2023-04-24 13:02:18.000000 aitviewer-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/
+-rw-rw-rw-   0        0        0       23 2023-04-24 13:14:34.000000 aitviewer-1.8.1/aitviewer/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/aitvconfig.yaml
+-rw-rw-rw-   0        0        0     3626 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/configuration.py
+-rw-rw-rw-   0        0        0     6939 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/headless.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/models/
+-rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/models/__init__.py
+-rw-rw-rw-   0        0        0    11260 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/models/smpl.py
+-rw-rw-rw-   0        0        0     6148 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/models/star.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/remote/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/message.py
+-rw-rw-rw-   0        0        0     1940 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/node.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/remote/renderables/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/__init__.py
+-rw-rw-rw-   0        0        0     1854 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/arrows.py
+-rw-rw-rw-   0        0        0     1386 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/lines.py
+-rw-rw-rw-   0        0        0     1454 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/meshes.py
+-rw-rw-rw-   0        0        0     1738 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/rigid_bodies.py
+-rw-rw-rw-   0        0        0     2737 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/smpl.py
+-rw-rw-rw-   0        0        0     1475 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/renderables/spheres.py
+-rw-rw-rw-   0        0        0     8487 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/remote/viewer.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/renderables/
+-rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/renderables/__init__.py
+-rw-rw-rw-   0        0        0     5482 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/arrows.py
+-rw-rw-rw-   0        0        0    10872 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/billboard.py
+-rw-rw-rw-   0        0        0     4247 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/bounding_boxes.py
+-rw-rw-rw-   0        0        0     1272 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/coordinate_system.py
+-rw-rw-rw-   0        0        0    16984 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/lines.py
+-rw-rw-rw-   0        0        0    45433 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/meshes.py
+-rw-rw-rw-   0        0        0    13660 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/multi_view_system.py
+-rw-rw-rw-   0        0        0    12907 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/plane.py
+-rw-rw-rw-   0        0        0     8013 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/point_clouds.py
+-rw-rw-rw-   0        0        0     6755 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/rigid_bodies.py
+-rw-rw-rw-   0        0        0     9946 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/sdf.py
+-rw-rw-rw-   0        0        0     4675 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/skeletons.py
+-rw-rw-rw-   0        0        0    31990 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/smpl.py
+-rw-rw-rw-   0        0        0    10070 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/spheres.py
+-rw-rw-rw-   0        0        0     6112 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/renderables/star.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/resources/
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/resources/fonts/
+-rw-rw-rw-   0        0        0   162888 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/resources/fonts/Custom.sfd
+-rw-rw-rw-   0        0        0    17132 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/resources/fonts/Custom.ttf
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/scene/
+-rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/scene/__init__.py
+-rw-rw-rw-   0        0        0    39356 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/camera.py
+-rw-rw-rw-   0        0        0     2720 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/camera_utils.py
+-rw-rw-rw-   0        0        0     9321 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/light.py
+-rw-rw-rw-   0        0        0     1538 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/material.py
+-rw-rw-rw-   0        0        0    26596 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/node.py
+-rw-rw-rw-   0        0        0    17344 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/scene/scene.py
+-rw-rw-rw-   0        0        0     8658 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/shaders/
+-rw-rw-rw-   0        0        0     2073 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/chessboard.glsl
+-rw-rw-rw-   0        0        0      898 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/clipping.glsl
+-rw-rw-rw-   0        0        0     4442 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/cylinder.glsl
+-rw-rw-rw-   0        0        0     2440 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/directional_lights.glsl
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/shaders/fragment_picking/
+-rw-rw-rw-   0        0        0      427 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/fragment_picking/frag_map.fs.glsl
+-rw-rw-rw-   0        0        0     1021 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/fragment_picking/frag_pick.glsl
+-rw-rw-rw-   0        0        0     2190 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/lines_instanced.vs.glsl
+-rw-rw-rw-   0        0        0     1480 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/lines_instanced_positions.vs.glsl
+-rw-rw-rw-   0        0        0     5571 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/lit_with_edges.glsl
+-rw-rw-rw-   0        0        0      734 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/mesh_positions.vs.glsl
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/shaders/outline/
+-rw-rw-rw-   0        0        0     1398 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/outline/outline_draw.glsl
+-rw-rw-rw-   0        0        0      480 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/outline/outline_prepare.fs.glsl
+-rw-rw-rw-   0        0        0      522 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/screen_texture.glsl
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/shaders/shadow_mapping/
+-rw-rw-rw-   0        0        0      287 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/shadow_mapping/depth_only.fs.glsl
+-rw-rw-rw-   0        0        0      497 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/shadow_mapping/raw_depth.glsl
+-rw-rw-rw-   0        0        0      481 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/simple_unlit.glsl
+-rw-rw-rw-   0        0        0     1015 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/sphere_instanced.vs.glsl
+-rw-rw-rw-   0        0        0      641 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders/sphere_instanced_positions.vs.glsl
+-rw-rw-rw-   0        0        0     1170 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/shaders/visualize.glsl
+-rw-rw-rw-   0        0        0     4413 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/shaders.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/streamables/
+-rw-rw-rw-   0        0        0        0 2023-01-30 08:41:59.000000 aitviewer-1.8.1/aitviewer/streamables/__init__.py
+-rw-rw-rw-   0        0        0     1345 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/streamables/streamable.py
+-rw-rw-rw-   0        0        0     3951 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/streamables/webcam.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer/utils/
+-rw-rw-rw-   0        0        0       49 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/__init__.py
+-rw-rw-rw-   0        0        0     1948 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/decorators.py
+-rw-rw-rw-   0        0        0     1574 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/exceptions.py
+-rw-rw-rw-   0        0        0     4427 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/imgui_integration.py
+-rw-rw-rw-   0        0        0     3493 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/path.py
+-rw-rw-rw-   0        0        0     3770 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/perf_timer.py
+-rw-rw-rw-   0        0        0     4589 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/pyqt5_window.py
+-rw-rw-rw-   0        0        0     6798 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/so3.py
+-rw-rw-rw-   0        0        0    14475 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/utils/utils.py
+-rw-rw-rw-   0        0        0    77877 2023-03-28 14:45:25.000000 aitviewer-1.8.1/aitviewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/
+-rw-rw-rw-   0        0        0     4611 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2886 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 13:16:01.000000 aitviewer-1.8.1/aitviewer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       93 2023-03-28 14:45:25.000000 aitviewer-1.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0      273 2023-04-24 13:16:01.000000 aitviewer-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-04-24 13:01:21.000000 aitviewer-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:16:01.000000 aitviewer-1.8.1/tests/
+-rw-rw-rw-   0        0        0     9177 2023-03-28 14:45:25.000000 aitviewer-1.8.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5739 2023-03-28 14:45:25.000000 aitviewer-1.8.1/tests/test_renderables.py
```

### Comparing `aitviewer-1.8.0/LICENSE` & `aitviewer-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/PKG-INFO` & `aitviewer-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitviewer
-Version: 1.8.0
+Version: 1.8.1
 Summary: Viewing and rendering of sequences of 3D data.
 Home-page: https://github.com/eth-ait/aitviewer
 Author: Manuel Kaufmann, Velko Vechev, Dario Mylonopoulos
 License: UNKNOWN
 Keywords: viewer,moderngl,machine learning,sequences,smpl,computer graphics,computer vision,3D,meshes,visualization
 Platform: any
 Requires-Python: >=3.7
@@ -61,14 +61,15 @@
     v.scene.add(SMPLSequence.t_pose())
     v.run()
 ```
 
 
 ## Projects using the aitviewer
 A sampling of projects using the aitviewer. Let us know if you want to add you!
+- Fan et al., [ARCTIC: A Dataset for Dexterous Bimanual Hand-Object Manipulation](https://arctic.is.tue.mpg.de/), CVPR 2023
 - Dong et al., [Shape-aware Multi-Person Pose Estimation from Multi-view Images](https://ait.ethz.ch/projects/2021/multi-human-pose/), ICCV 2021
 - Kaufmann et al., [EM-POSE: 3D Human Pose Estimation from Sparse Electromagnetic Trackers](https://ait.ethz.ch/projects/2021/em-pose/), ICCV 2021
 - Vechev et al., [Computational Design of Kinesthetic Garments](https://ait.ethz.ch/projects/2022/cdkg/), Eurographics 2021
 - Guo et al., [Human Performance Capture from Monocular Video in the Wild](https://ait.ethz.ch/projects/2021/human-performance-capture/index.php), 3DV 2021
 - Dong and Guo et al., [PINA: Learning a Personalized Implicit Neural Avatar from a Single RGB-D Video Sequence](https://zj-dong.github.io/pina/), CVPR 2022
 
 ## Citation
```

### Comparing `aitviewer-1.8.0/README.md` & `aitviewer-1.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     v.scene.add(SMPLSequence.t_pose())
     v.run()
 ```
 
 
 ## Projects using the aitviewer
 A sampling of projects using the aitviewer. Let us know if you want to add you!
+- Fan et al., [ARCTIC: A Dataset for Dexterous Bimanual Hand-Object Manipulation](https://arctic.is.tue.mpg.de/), CVPR 2023
 - Dong et al., [Shape-aware Multi-Person Pose Estimation from Multi-view Images](https://ait.ethz.ch/projects/2021/multi-human-pose/), ICCV 2021
 - Kaufmann et al., [EM-POSE: 3D Human Pose Estimation from Sparse Electromagnetic Trackers](https://ait.ethz.ch/projects/2021/em-pose/), ICCV 2021
 - Vechev et al., [Computational Design of Kinesthetic Garments](https://ait.ethz.ch/projects/2022/cdkg/), Eurographics 2021
 - Guo et al., [Human Performance Capture from Monocular Video in the Wild](https://ait.ethz.ch/projects/2021/human-performance-capture/index.php), 3DV 2021
 - Dong and Guo et al., [PINA: Learning a Personalized Implicit Neural Avatar from a Single RGB-D Video Sequence](https://zj-dong.github.io/pina/), CVPR 2022
 
 ## Citation
```

### Comparing `aitviewer-1.8.0/aitviewer/aitvconfig.yaml` & `aitviewer-1.8.1/aitviewer/aitvconfig.yaml`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/configuration.py` & `aitviewer-1.8.1/aitviewer/configuration.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/headless.py` & `aitviewer-1.8.1/aitviewer/headless.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/models/smpl.py` & `aitviewer-1.8.1/aitviewer/models/smpl.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/models/star.py` & `aitviewer-1.8.1/aitviewer/models/star.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/message.py` & `aitviewer-1.8.1/aitviewer/remote/message.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/node.py` & `aitviewer-1.8.1/aitviewer/remote/node.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/arrows.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/arrows.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/lines.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/lines.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/meshes.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/meshes.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/rigid_bodies.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/rigid_bodies.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/smpl.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/smpl.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/renderables/spheres.py` & `aitviewer-1.8.1/aitviewer/remote/renderables/spheres.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/remote/viewer.py` & `aitviewer-1.8.1/aitviewer/remote/viewer.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/arrows.py` & `aitviewer-1.8.1/aitviewer/renderables/arrows.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/billboard.py` & `aitviewer-1.8.1/aitviewer/renderables/billboard.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/bounding_boxes.py` & `aitviewer-1.8.1/aitviewer/renderables/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/coordinate_system.py` & `aitviewer-1.8.1/aitviewer/renderables/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/lines.py` & `aitviewer-1.8.1/aitviewer/renderables/lines.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/meshes.py` & `aitviewer-1.8.1/aitviewer/renderables/meshes.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/multi_view_system.py` & `aitviewer-1.8.1/aitviewer/renderables/multi_view_system.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/plane.py` & `aitviewer-1.8.1/aitviewer/renderables/plane.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/point_clouds.py` & `aitviewer-1.8.1/aitviewer/renderables/point_clouds.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/rigid_bodies.py` & `aitviewer-1.8.1/aitviewer/renderables/rigid_bodies.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/sdf.py` & `aitviewer-1.8.1/aitviewer/renderables/sdf.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/skeletons.py` & `aitviewer-1.8.1/aitviewer/renderables/skeletons.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/smpl.py` & `aitviewer-1.8.1/aitviewer/renderables/smpl.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/spheres.py` & `aitviewer-1.8.1/aitviewer/renderables/spheres.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/renderables/star.py` & `aitviewer-1.8.1/aitviewer/renderables/star.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/resources/fonts/Custom.sfd` & `aitviewer-1.8.1/aitviewer/resources/fonts/Custom.sfd`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/resources/fonts/Custom.ttf` & `aitviewer-1.8.1/aitviewer/resources/fonts/Custom.ttf`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/camera.py` & `aitviewer-1.8.1/aitviewer/scene/camera.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/camera_utils.py` & `aitviewer-1.8.1/aitviewer/scene/camera_utils.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/light.py` & `aitviewer-1.8.1/aitviewer/scene/light.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/material.py` & `aitviewer-1.8.1/aitviewer/scene/material.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/node.py` & `aitviewer-1.8.1/aitviewer/scene/node.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/scene/scene.py` & `aitviewer-1.8.1/aitviewer/scene/scene.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/server.py` & `aitviewer-1.8.1/aitviewer/server.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/chessboard.glsl` & `aitviewer-1.8.1/aitviewer/shaders/chessboard.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/clipping.glsl` & `aitviewer-1.8.1/aitviewer/shaders/clipping.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/cylinder.glsl` & `aitviewer-1.8.1/aitviewer/shaders/cylinder.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/directional_lights.glsl` & `aitviewer-1.8.1/aitviewer/shaders/directional_lights.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/fragment_picking/frag_pick.glsl` & `aitviewer-1.8.1/aitviewer/shaders/fragment_picking/frag_pick.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/lines_instanced.vs.glsl` & `aitviewer-1.8.1/aitviewer/shaders/lines_instanced.vs.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/lines_instanced_positions.vs.glsl` & `aitviewer-1.8.1/aitviewer/shaders/lines_instanced_positions.vs.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/lit_with_edges.glsl` & `aitviewer-1.8.1/aitviewer/shaders/lit_with_edges.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/mesh_positions.vs.glsl` & `aitviewer-1.8.1/aitviewer/shaders/mesh_positions.vs.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/outline/outline_draw.glsl` & `aitviewer-1.8.1/aitviewer/shaders/outline/outline_draw.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/screen_texture.glsl` & `aitviewer-1.8.1/aitviewer/shaders/screen_texture.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/sphere_instanced.vs.glsl` & `aitviewer-1.8.1/aitviewer/shaders/sphere_instanced.vs.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/sphere_instanced_positions.vs.glsl` & `aitviewer-1.8.1/aitviewer/shaders/sphere_instanced_positions.vs.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders/visualize.glsl` & `aitviewer-1.8.1/aitviewer/shaders/visualize.glsl`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/shaders.py` & `aitviewer-1.8.1/aitviewer/shaders.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/streamables/streamable.py` & `aitviewer-1.8.1/aitviewer/streamables/streamable.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/streamables/webcam.py` & `aitviewer-1.8.1/aitviewer/streamables/webcam.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/decorators.py` & `aitviewer-1.8.1/aitviewer/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/exceptions.py` & `aitviewer-1.8.1/aitviewer/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/imgui_integration.py` & `aitviewer-1.8.1/aitviewer/utils/imgui_integration.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/path.py` & `aitviewer-1.8.1/aitviewer/utils/path.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/perf_timer.py` & `aitviewer-1.8.1/aitviewer/utils/perf_timer.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/pyqt5_window.py` & `aitviewer-1.8.1/aitviewer/utils/pyqt5_window.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/so3.py` & `aitviewer-1.8.1/aitviewer/utils/so3.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/utils/utils.py` & `aitviewer-1.8.1/aitviewer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer/viewer.py` & `aitviewer-1.8.1/aitviewer/viewer.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/aitviewer.egg-info/PKG-INFO` & `aitviewer-1.8.1/aitviewer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitviewer
-Version: 1.8.0
+Version: 1.8.1
 Summary: Viewing and rendering of sequences of 3D data.
 Home-page: https://github.com/eth-ait/aitviewer
 Author: Manuel Kaufmann, Velko Vechev, Dario Mylonopoulos
 License: UNKNOWN
 Keywords: viewer,moderngl,machine learning,sequences,smpl,computer graphics,computer vision,3D,meshes,visualization
 Platform: any
 Requires-Python: >=3.7
@@ -61,14 +61,15 @@
     v.scene.add(SMPLSequence.t_pose())
     v.run()
 ```
 
 
 ## Projects using the aitviewer
 A sampling of projects using the aitviewer. Let us know if you want to add you!
+- Fan et al., [ARCTIC: A Dataset for Dexterous Bimanual Hand-Object Manipulation](https://arctic.is.tue.mpg.de/), CVPR 2023
 - Dong et al., [Shape-aware Multi-Person Pose Estimation from Multi-view Images](https://ait.ethz.ch/projects/2021/multi-human-pose/), ICCV 2021
 - Kaufmann et al., [EM-POSE: 3D Human Pose Estimation from Sparse Electromagnetic Trackers](https://ait.ethz.ch/projects/2021/em-pose/), ICCV 2021
 - Vechev et al., [Computational Design of Kinesthetic Garments](https://ait.ethz.ch/projects/2022/cdkg/), Eurographics 2021
 - Guo et al., [Human Performance Capture from Monocular Video in the Wild](https://ait.ethz.ch/projects/2021/human-performance-capture/index.php), 3DV 2021
 - Dong and Guo et al., [PINA: Learning a Personalized Implicit Neural Avatar from a Single RGB-D Video Sequence](https://zj-dong.github.io/pina/), CVPR 2022
 
 ## Citation
```

### Comparing `aitviewer-1.8.0/aitviewer.egg-info/SOURCES.txt` & `aitviewer-1.8.1/aitviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/setup.py` & `aitviewer-1.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "torch>=1.6.0",
         "numpy>=1.18,<2",
         "opencv-contrib-python-headless>=4.5.1.48",
         "smplx",
         "moderngl-window>=2.4.0",
         "moderngl>=5.6.4,<5.7.1",
         "PyQt5>=5.15.4",
-        "imgui>=1.3.0",
+        "imgui==1.4.1",
         "tqdm>=4.60.0",
         "trimesh>=3.9.15,<4",
         "scipy>=1.5.2,<1.8",
         "omegaconf>=2.1.1",
         "roma>=1.2.3",
         "joblib",
         "scikit-image>=0.9.0",
```

### Comparing `aitviewer-1.8.0/tests/test_misc.py` & `aitviewer-1.8.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `aitviewer-1.8.0/tests/test_renderables.py` & `aitviewer-1.8.1/tests/test_renderables.py`

 * *Files identical despite different names*


# Comparing `tmp/sphere_base-0.1.7.tar.gz` & `tmp/sphere_base-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.7.tar", last modified: Sun Apr 23 12:31:41 2023, max compression
+gzip compressed data, was "sphere_base-0.1.8.tar", last modified: Mon Apr 24 09:53:00 2023, max compression
```

## Comparing `sphere_base-0.1.7.tar` & `sphere_base-0.1.8.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.667827 sphere_base-0.1.7/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.7/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      358 2023-04-22 14:48:51.000000 sphere_base-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1987 2023-04-23 12:31:41.667827 sphere_base-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:40.980788 sphere_base-0.1.7/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.7/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:40.963787 sphere_base-0.1.7/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:40.964787 sphere_base-0.1.7/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:40.983788 sphere_base-0.1.7/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.7/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.7/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.7/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:40.986788 sphere_base-0.1.7/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.7/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.7/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.067793 sphere_base-0.1.7/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      154 2023-04-22 14:15:57.000000 sphere_base-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 12:31:41.668827 sphere_base-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-04-23 12:31:31.000000 sphere_base-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.075793 sphere_base-0.1.7/sphere_base/
--rw-rw-rw-   0        0        0      106 2023-04-21 12:08:43.000000 sphere_base-0.1.7/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.7/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.7/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5510 2023-04-23 12:04:09.000000 sphere_base-0.1.7/sphere_base/config.py
--rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.7/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.096794 sphere_base-0.1.7/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.7/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.7/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.7/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.7/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.7/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14126 2023-04-22 13:09:36.000000 sphere_base-0.1.7/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.7/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.101795 sphere_base-0.1.7/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.7/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4199 2023-04-23 11:59:31.000000 sphere_base-0.1.7/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6415 2023-04-22 13:52:18.000000 sphere_base-0.1.7/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3379 2023-04-22 13:55:17.000000 sphere_base-0.1.7/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23303 2023-04-23 11:45:50.000000 sphere_base-0.1.7/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.102795 sphere_base-0.1.7/sphere_base/model/resources/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/model/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.103795 sphere_base-0.1.7/sphere_base/model/resources/icons/
--rw-rw-rw-   0        0        0        0 2023-04-23 10:04:38.000000 sphere_base-0.1.7/sphere_base/model/resources/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.129796 sphere_base-0.1.7/sphere_base/model/resources/meshes/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/__init__.py
--rw-rw-rw-   0        0        0       60 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/crosshair.mtl
--rw-rw-rw-   0        0        0     1720 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/crosshair.obj
--rw-rw-rw-   0        0        0      339 2023-04-19 15:51:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/cubesphere.mtl
--rw-rw-rw-   0        0        0  3258439 2023-04-20 06:45:02.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/cubesphere.obj
--rw-rw-rw-   0        0        0      144 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/line_1x1.mtl
--rw-rw-rw-   0        0        0      377 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/line_1x1.obj
--rw-rw-rw-   0        0        0      319 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/node_disc1.mtl
--rw-rw-rw-   0        0        0     4438 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/node_disc1.obj
--rw-rw-rw-   0        0        0      241 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/skybox.mtl
--rw-rw-rw-   0        0        0     1184 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/skybox.obj
--rw-rw-rw-   0        0        0      327 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere1.mtl
--rw-rw-rw-   0        0        0   334766 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere1.obj
--rw-rw-rw-   0        0        0      148 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere_small.mtl
--rw-rw-rw-   0        0        0    61720 2023-03-06 12:34:58.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere_small.obj
--rw-rw-rw-   0        0        0      134 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/square1x1.mtl
--rw-rw-rw-   0        0        0      362 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/square1x1.obj
--rw-rw-rw-   0        0        0       49 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/vertex1.mtl
--rw-rw-rw-   0        0        0      127 2023-03-13 10:54:30.000000 sphere_base-0.1.7/sphere_base/model/resources/meshes/vertex1.obj
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.185799 sphere_base-0.1.7/sphere_base/model/resources/shaders/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/__init__.py
--rw-rw-rw-   0        0        0       99 2021-02-20 15:08:02.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_2d.glsl
--rw-rw-rw-   0        0        0      103 2021-03-09 15:04:34.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_circle.glsl
--rw-rw-rw-   0        0        0     3157 2021-02-20 08:36:12.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_default.glsl
--rw-rw-rw-   0        0        0     2128 2021-08-09 11:38:22.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_holo.glsl
--rw-rw-rw-   0        0        0      531 2021-08-10 08:30:00.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_holo_sphere.glsl
--rw-rw-rw-   0        0        0      533 2021-08-18 14:31:52.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_node.glsl
--rw-rw-rw-   0        0        0      147 2023-03-11 11:21:38.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_skybox.glsl
--rw-rw-rw-   0        0        0      541 2021-08-17 08:34:24.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_socket.glsl
--rw-rw-rw-   0        0        0     3162 2021-08-18 15:12:02.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_sphere.glsl
--rw-rw-rw-   0        0        0       99 2023-04-14 14:44:46.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_sphere_edge.glsl
--rw-rw-rw-   0        0        0      412 2021-08-20 07:35:34.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_sphere_small.glsl
--rw-rw-rw-   0        0        0      243 2021-03-01 09:41:30.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_square.glsl
--rw-rw-rw-   0        0        0      693 2023-04-14 14:40:36.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_circle.glsl
--rw-rw-rw-   0        0        0     2451 2023-04-05 15:16:56.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_cross.glsl
--rw-rw-rw-   0        0        0     2961 2023-04-14 12:24:33.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_edge.glsl
--rw-rw-rw-   0        0        0      693 2023-04-14 14:39:33.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_edge2.glsl
--rw-rw-rw-   0        0        0      972 2021-03-08 11:27:56.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_square.glsl
--rw-rw-rw-   0        0        0      254 2021-03-01 09:26:34.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_2d.glsl
--rw-rw-rw-   0        0        0      194 2021-03-09 14:50:48.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_circle.glsl
--rw-rw-rw-   0        0        0     2776 2021-02-20 08:36:12.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_default.glsl
--rw-rw-rw-   0        0        0     1384 2021-08-09 11:54:12.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_holo.glsl
--rw-rw-rw-   0        0        0      524 2021-08-10 08:30:00.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_holo_sphere.glsl
--rw-rw-rw-   0        0        0      528 2021-02-24 20:35:30.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_node.glsl
--rw-rw-rw-   0        0        0      246 2023-03-11 11:21:44.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_skybox.glsl
--rw-rw-rw-   0        0        0      524 2021-02-27 18:53:28.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_socket.glsl
--rw-rw-rw-   0        0        0     2692 2021-08-09 14:04:40.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere.glsl
--rw-rw-rw-   0        0        0      524 2021-04-01 08:39:08.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere_edge.glsl
--rw-rw-rw-   0        0        0      522 2021-08-20 07:11:26.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere_small.glsl
--rw-rw-rw-   0        0        0      338 2021-03-01 10:55:38.000000 sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_square.glsl
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.201800 sphere_base-0.1.7/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.7/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8434 2023-04-23 09:16:06.000000 sphere_base-0.1.7/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-22 19:07:09.000000 sphere_base-0.1.7/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.7/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13468 2023-04-23 09:50:46.000000 sphere_base-0.1.7/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8804 2023-04-22 13:09:36.000000 sphere_base-0.1.7/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.7/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.221801 sphere_base-0.1.7/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.7/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0     9344 2023-04-23 11:52:26.000000 sphere_base-0.1.7/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     2129 2023-04-23 09:45:33.000000 sphere_base-0.1.7/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.7/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.7/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.7/sphere_base/shader/drag_edge_shader.py
--rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.7/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.7/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.7/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.7/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.7/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.7/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.7/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.7/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.7/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.7/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.224802 sphere_base-0.1.7/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.7/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28884 2023-04-22 08:44:12.000000 sphere_base-0.1.7/sphere_base/sphere/sphere.py
--rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.7/sphere_base/sphere/sphere_lines.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.228802 sphere_base-0.1.7/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.230802 sphere_base-0.1.7/sphere_base/sphere_overlay/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.232802 sphere_base-0.1.7/sphere_base/sphere_overlay/qss/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/qss/__init__.py
--rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1613 2023-04-23 09:50:46.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.238802 sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1121 2023-04-23 09:53:20.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1038 2023-04-23 09:25:54.000000 sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.664827 sphere_base-0.1.7/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5378 2023-04-22 11:55:42.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14150 2023-04-22 12:54:26.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1493 2023-04-21 11:08:11.000000 sphere_base-0.1.7/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.089794 sphere_base-0.1.7/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     1987 2023-04-23 12:31:40.000000 sphere_base-0.1.7/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8854 2023-04-23 12:31:40.000000 sphere_base-0.1.7/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:31:40.000000 sphere_base-0.1.7/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.7/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      145 2023-04-23 12:31:40.000000 sphere_base-0.1.7/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 12:31:40.000000 sphere_base-0.1.7/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 12:31:41.666827 sphere_base-0.1.7/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.7/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:53:00.068533 sphere_base-0.1.8/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-23 15:03:17.000000 sphere_base-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-04-23 15:03:17.000000 sphere_base-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1987 2023-04-24 09:53:00.066533 sphere_base-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-23 15:03:17.000000 sphere_base-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.508444 sphere_base-0.1.8/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.8/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.479442 sphere_base-0.1.8/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.480442 sphere_base-0.1.8/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.513444 sphere_base-0.1.8/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.8/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.8/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.8/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.8/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.544446 sphere_base-0.1.8/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.8/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.8/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:58.932468 sphere_base-0.1.8/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      154 2023-04-23 15:03:18.000000 sphere_base-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:53:00.068533 sphere_base-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-04-24 09:52:31.000000 sphere_base-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.037474 sphere_base-0.1.8/sphere_base/
+-rw-rw-rw-   0        0        0      106 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.8/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5510 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/config.py
+-rw-rw-rw-   0        0        0     4839 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.155481 sphere_base-0.1.8/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.8/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     6675 2023-04-23 16:40:14.000000 sphere_base-0.1.8/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4592 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      809 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.8/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14126 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.8/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.231485 sphere_base-0.1.8/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.8/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4199 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6415 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3375 2023-04-23 16:38:31.000000 sphere_base-0.1.8/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23303 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.236486 sphere_base-0.1.8/sphere_base/model/resources/
+-rw-rw-rw-   0        0        0       25 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.237486 sphere_base-0.1.8/sphere_base/model/resources/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/resources/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.342492 sphere_base-0.1.8/sphere_base/model/resources/meshes/
+-rw-rw-rw-   0        0        0       25 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/crosshair.mtl
+-rw-rw-rw-   0        0        0     1720 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/crosshair.obj
+-rw-rw-rw-   0        0        0      339 2023-04-19 15:51:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/cubesphere.mtl
+-rw-rw-rw-   0        0        0  3258439 2023-04-20 06:45:02.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/cubesphere.obj
+-rw-rw-rw-   0        0        0      144 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/line_1x1.mtl
+-rw-rw-rw-   0        0        0      377 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/line_1x1.obj
+-rw-rw-rw-   0        0        0      319 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/node_disc1.mtl
+-rw-rw-rw-   0        0        0     4438 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/node_disc1.obj
+-rw-rw-rw-   0        0        0      241 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/skybox.mtl
+-rw-rw-rw-   0        0        0     1184 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/skybox.obj
+-rw-rw-rw-   0        0        0      327 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere1.mtl
+-rw-rw-rw-   0        0        0   334766 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere1.obj
+-rw-rw-rw-   0        0        0      148 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere_small.mtl
+-rw-rw-rw-   0        0        0    61720 2023-03-06 12:34:58.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere_small.obj
+-rw-rw-rw-   0        0        0      134 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/square1x1.mtl
+-rw-rw-rw-   0        0        0      362 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/square1x1.obj
+-rw-rw-rw-   0        0        0       49 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/vertex1.mtl
+-rw-rw-rw-   0        0        0      127 2023-03-13 10:54:30.000000 sphere_base-0.1.8/sphere_base/model/resources/meshes/vertex1.obj
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.528502 sphere_base-0.1.8/sphere_base/model/resources/shaders/
+-rw-rw-rw-   0        0        0       25 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/__init__.py
+-rw-rw-rw-   0        0        0       99 2021-02-20 15:08:02.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_2d.glsl
+-rw-rw-rw-   0        0        0      103 2021-03-09 15:04:34.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_circle.glsl
+-rw-rw-rw-   0        0        0     3157 2021-02-20 08:36:12.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_default.glsl
+-rw-rw-rw-   0        0        0     2128 2021-08-09 11:38:22.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_holo.glsl
+-rw-rw-rw-   0        0        0      531 2021-08-10 08:30:00.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_holo_sphere.glsl
+-rw-rw-rw-   0        0        0      533 2021-08-18 14:31:52.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_node.glsl
+-rw-rw-rw-   0        0        0      147 2023-03-11 11:21:38.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_skybox.glsl
+-rw-rw-rw-   0        0        0      541 2021-08-17 08:34:24.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_socket.glsl
+-rw-rw-rw-   0        0        0     3162 2021-08-18 15:12:02.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_sphere.glsl
+-rw-rw-rw-   0        0        0       99 2023-04-14 14:44:46.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_sphere_edge.glsl
+-rw-rw-rw-   0        0        0      412 2021-08-20 07:35:34.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_sphere_small.glsl
+-rw-rw-rw-   0        0        0      243 2021-03-01 09:41:30.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_square.glsl
+-rw-rw-rw-   0        0        0      693 2023-04-14 14:40:36.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_circle.glsl
+-rw-rw-rw-   0        0        0     2451 2023-04-05 15:16:56.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_cross.glsl
+-rw-rw-rw-   0        0        0     2961 2023-04-14 12:24:33.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_edge.glsl
+-rw-rw-rw-   0        0        0      693 2023-04-14 14:39:33.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_edge2.glsl
+-rw-rw-rw-   0        0        0      972 2021-03-08 11:27:56.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_square.glsl
+-rw-rw-rw-   0        0        0      254 2021-03-01 09:26:34.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_2d.glsl
+-rw-rw-rw-   0        0        0      194 2021-03-09 14:50:48.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_circle.glsl
+-rw-rw-rw-   0        0        0     2776 2021-02-20 08:36:12.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_default.glsl
+-rw-rw-rw-   0        0        0     1384 2021-08-09 11:54:12.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_holo.glsl
+-rw-rw-rw-   0        0        0      524 2021-08-10 08:30:00.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_holo_sphere.glsl
+-rw-rw-rw-   0        0        0      528 2021-02-24 20:35:30.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_node.glsl
+-rw-rw-rw-   0        0        0      246 2023-03-11 11:21:44.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_skybox.glsl
+-rw-rw-rw-   0        0        0      524 2021-02-27 18:53:28.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_socket.glsl
+-rw-rw-rw-   0        0        0     2692 2021-08-09 14:04:40.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere.glsl
+-rw-rw-rw-   0        0        0      524 2021-04-01 08:39:08.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere_edge.glsl
+-rw-rw-rw-   0        0        0      522 2021-08-20 07:11:26.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere_small.glsl
+-rw-rw-rw-   0        0        0      338 2021-03-01 10:55:38.000000 sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_square.glsl
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.594506 sphere_base-0.1.8/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.8/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8434 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.8/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13466 2023-04-24 07:53:36.000000 sphere_base-0.1.8/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8804 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1739 2023-04-23 19:15:20.000000 sphere_base-0.1.8/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.797518 sphere_base-0.1.8/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.8/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0     9344 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     2129 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1969 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.8/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     2243 2023-04-23 15:32:13.000000 sphere_base-0.1.8/sphere_base/shader/drag_edge_shader.py
+-rw-rw-rw-   0        0        0     1164 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      909 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1467 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1166 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1261 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3117 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1668 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1254 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1845 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.816519 sphere_base-0.1.8/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.8/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    29146 2023-04-24 09:30:44.000000 sphere_base-0.1.8/sphere_base/sphere/sphere.py
+-rw-rw-rw-   0        0        0     6068 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere/sphere_lines.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.862521 sphere_base-0.1.8/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.865522 sphere_base-0.1.8/sphere_base/sphere_overlay/icons/
+-rw-rw-rw-   0        0        0       25 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.882522 sphere_base-0.1.8/sphere_base/sphere_overlay/qss/
+-rw-rw-rw-   0        0        0       25 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/qss/__init__.py
+-rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2161 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1613 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.958527 sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1121 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1038 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:53:00.059533 sphere_base-0.1.8/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     8637 2023-04-24 09:04:46.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/camera.py
+-rw-rw-rw-   0        0        0     5440 2023-04-24 09:43:12.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/skybox.py
+-rw-rw-rw-   0        0        0     3432 2023-04-23 19:15:19.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0    14582 2023-04-24 09:48:14.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17863 2023-04-24 09:30:44.000000 sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1493 2023-04-23 15:03:18.000000 sphere_base-0.1.8/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:52:59.065476 sphere_base-0.1.8/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-04-24 09:52:57.000000 sphere_base-0.1.8/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8849 2023-04-24 09:52:58.000000 sphere_base-0.1.8/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:52:57.000000 sphere_base-0.1.8/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.8/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      145 2023-04-24 09:52:57.000000 sphere_base-0.1.8/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 09:52:57.000000 sphere_base-0.1.8/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 09:53:00.065533 sphere_base-0.1.8/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.8/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.7/HISTORY.rst` & `sphere_base-0.1.8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/LICENSE` & `sphere_base-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/PKG-INFO` & `sphere_base-0.1.8/sphere_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sphere_base
-Version: 0.1.7
+Name: sphere-base
+Version: 0.1.8
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.7/README.rst` & `sphere_base-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/Makefile` & `sphere_base-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/make.bat` & `sphere_base-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/source/conf.py` & `sphere_base-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.8/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.8/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/setup.py` & `sphere_base-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.7',
+    version='0.1.8',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.7/sphere_base/calc.py` & `sphere_base-0.1.8/sphere_base/calc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/clipboard.py` & `sphere_base-0.1.8/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/config.py` & `sphere_base-0.1.8/sphere_base/config.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/constants.py` & `sphere_base-0.1.8/sphere_base/constants.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.8/sphere_base/edge/edge_drag.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,42 +63,17 @@
         self.pos_orientation_offset = None
         self._dragging = False
 
         self.unit_length = 0.04
         self.pos_array = []
 
         self.gr_edge = self.__class__.GraphicsEdge_class(self)
-        self.model = self.set_up_model('drag_edge')
+        self.model = self.uv.models.get_model('drag_edge')
         self.calc = Calc()
 
-    def set_up_model(self, model_name):
-        shader, vertex_shader, fragment_shader, geometry_shader = None, None, None, None
-
-        # get the shaders for the edge
-        for _name in MODELS.keys():
-            if _name == model_name:
-                shader = MODELS[_name]["shader"]
-                vertex_shader = MODELS[_name]["vertex_shader"]
-                fragment_shader = MODELS[_name]["fragment_shader"]
-                geometry_shader = MODELS[_name]["geometry_shader"]
-                geometry_shader = None if geometry_shader == "none" else geometry_shader
-
-        # create a model for the edge
-        model = Model(
-                      models=self.uv.models,
-                      model_id=0,
-                      model_name=model_name,
-                      obj_file="",
-                      shader=shader,
-                      vertex_shader=vertex_shader,
-                      fragment_shader=fragment_shader,
-                      geometry_shader=geometry_shader)
-
-        return model
-
     def _init_start_dragging(self, start_socket: 'Socket'):
         # dragging start point is the start socket
         self.start_socket = start_socket
         self.xyz = start_socket.xyz  # position of the mouse at start
         self.pos_orientation_offset = self.start_socket.node.pos_orientation_offset
 
     def _stop_dragging(self):
```

### Comparing `sphere_base-0.1.7/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.8/sphere_base/edge/graphic_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/edge/graphic_line.py` & `sphere_base-0.1.8/sphere_base/edge/graphic_line.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.8/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.8/sphere_base/edge/surface_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/history.py` & `sphere_base-0.1.8/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/mesh.py` & `sphere_base-0.1.8/sphere_base/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/model.py` & `sphere_base-0.1.8/sphere_base/model/model.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/models.py` & `sphere_base-0.1.8/sphere_base/model/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             # model_file = MESH_DIR + MODELS[_name]["model_file_name"]
             model_file = MODELS[_name]["model_file_name"]
             shader = MODELS[_name]["shader"]
             vertex_shader = MODELS[_name]["vertex_shader"]
             fragment_shader = MODELS[_name]["fragment_shader"]
             geometry_shader = None if MODELS[_name]["geometry_shader"] == "none" else MODELS[_name]["geometry_shader"]
 
-            if 'edge' not in model_name:
+            if model_name != 'edge':
                 # Create a new model
                 model = self.Model(self, model_id, model_name, model_file, shader, vertex_shader, fragment_shader,
                                    geometry_shader)
 
                 # add model to internal list
                 self._models.append(model)
```

### Comparing `sphere_base-0.1.7/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.8/sphere_base/model/obj_file_loader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/crosshair.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/crosshair.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/cubesphere.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/cubesphere.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/node_disc1.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/node_disc1.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/skybox.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/skybox.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere1.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere1.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/meshes/sphere_small.obj` & `sphere_base-0.1.8/sphere_base/model/resources/meshes/sphere_small.obj`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_default.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_default.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_holo.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_holo.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_holo_sphere.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_holo_sphere.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_node.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_node.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_socket.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_socket.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/frag_sphere.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/frag_sphere.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_circle.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_circle.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_cross.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_cross.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_edge.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_edge.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_edge2.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_edge2.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/geom_square.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/geom_square.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_default.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_default.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_holo.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_holo.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_holo_sphere.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_holo_sphere.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_node.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_node.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_socket.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_socket.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere_edge.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere_edge.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/model/resources/shaders/vert_sphere_small.glsl` & `sphere_base-0.1.8/sphere_base/model/resources/shaders/vert_sphere_small.glsl`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.8/sphere_base/node/graphic_disc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/node/graphic_node.py` & `sphere_base-0.1.8/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.8/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/node/node.py` & `sphere_base-0.1.8/sphere_base/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,14 @@
             ('node_type_name', self.node_type_name),
             # ('img_id', self.img_id),
             ('img_name', self.img_name),
             ('orientation_offset', self.pos_orientation_offset.tolist()),
             ('scene', self.serialized_detail_scene),
             ('socket_id', self.socket.id),
             ('socket', socket)
-
         ])
 
     def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
         """
         copy, cut paste also uses this. When pasting restore_id is false and new ids are created.
         """
```

### Comparing `sphere_base-0.1.7/sphere_base/node/socket.py` & `sphere_base-0.1.8/sphere_base/node/socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/serializable.py` & `sphere_base-0.1.8/sphere_base/serializable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-A module containing Serializable "Interface". We pretend its an abstract class
+A module containing Serializable "Interface". We pretend it is an abstract class
 
 """
 
 from collections import OrderedDict
 
 
 class Serializable:
```

### Comparing `sphere_base-0.1.7/sphere_base/shader/base_shader.py` & `sphere_base-0.1.8/sphere_base/shader/base_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.8/sphere_base/shader/circle_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.8/sphere_base/shader/cross_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/default_shader.py` & `sphere_base-0.1.8/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/drag_edge_shader.py` & `sphere_base-0.1.8/sphere_base/shader/drag_edge_shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
             This method is using obsolete direct OpenGL instead of modern OpenGL.
             This needs to be updated in a future iteration, however this will not impact performance, as there
             is only one edge being dragged at any one moment.
 
         """
         # drawing lines
-        glUseProgram(self.shader_id)  # using the standard shader
+
+        glUseProgram(self.shader_id)  # using the standard shader ?????
         glUniform1i(self.switcher_loc, 3)  # switch to use fragment and vertex shader for lines
         glLineWidth(width)
 
         if color:
             # enable blending
             glUniform4f(self.a_color, *color)
             glEnable(GL_LINE_SMOOTH)
```

### Comparing `sphere_base-0.1.7/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.8/sphere_base/shader/edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.8/sphere_base/shader/flat_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.8/sphere_base/shader/holo_sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/node_shader.py` & `sphere_base-0.1.8/sphere_base/shader/node_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.8/sphere_base/shader/skybox_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.8/sphere_base/shader/socket_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.8/sphere_base/shader/sphere_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.8/sphere_base/shader/sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.8/sphere_base/shader/sphere_small_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/shader/square_shader.py` & `sphere_base-0.1.8/sphere_base/shader/square_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere/sphere.py` & `sphere_base-0.1.8/sphere_base/sphere/sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,14 +408,22 @@
 
         # update orientation of all nodes on sphere_base
         for item in self.items:
             if item.type in ('node', 'sphere_lines'):
                 # updating the node trickles down to updating sockets and edges"
                 item.update_position()
 
+    def update_item_collision_objects(self):
+        """
+        Update the collision objects of all items on the sphere_base.
+        """
+        for item in self.items:
+            if item.type in ('sphere', 'edge', 'node', 'socket'):
+                item.update_collision_object()
+
     def rotate_sphere(self, offset_degrees: int):
         """
         Rotating the sphere_base over the y-axis as per the offset_degrees.
 
         :param offset_degrees: degrees that the sphere_base rotates over its y-axis
         :type offset_degrees: ``int``
         """
@@ -669,32 +677,29 @@
             ('id', self.id),
             ('type', self.type),
             ('pos', self.xyz),
             ('radius', self.radius),
             ('orientation', self.orientation.tolist()),
             ('texture_id', self.texture_id),
             ('color', self.color),
-            # ('color_id', self.color_id),
-            # ('color_id_per_lens', self.get_color_id_per_lens()),
             ('nodes', nodes),
             ('edges', edges),
         ])
 
     def deserialize(self, data: dict, hashmap: dict = {}, restore_id: bool = True) -> bool:
         if restore_id:
             self.id = data['id']
         hashmap[data['id']] = self
 
         self.xyz = data['pos']
-        self.orientation = np.array(data['orientation'])
+        orientation = np.array(data['orientation'])
+
         self.texture_id = data['texture_id']
-        if 'color' in data:
-            self.color = data['color']
-        if 'radius' in data:
-            self.set_radius(data['radius'])
+        self.color = data['color']
+        self.set_radius(data['radius'])
         self.uv.mouse_ray.reset_position_collision_object(self)
 
         # -- deserialize nodes on sphere_base
 
         # Instead of recreating all the nodes, reuse existing ones...
         all_items = self.items.copy()
 
@@ -735,12 +740,17 @@
 
             if not found:
                 self.Edge(self).deserialize(edge_data, hashmap, restore_id)
             else:
                 found.deserialize(edge_data, hashmap, restore_id)
                 all_items.remove(found)
 
-            # remove items which are left in the scene and were NOT in the serialized data!
+        # rotate the sphere
+        self.orientation = orientation
+        self.update_item_positions()
+        self.update_item_collision_objects()
+
+        # remove items which are left in the scene and were NOT in the serialized data!
         while all_items:
             item = all_items.pop()
             item.remove()
         return True
```

### Comparing `sphere_base-0.1.7/sphere_base/sphere/sphere_lines.py` & `sphere_base-0.1.8/sphere_base/sphere/sphere_lines.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.8/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/camera.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 current implementation there is only need for a single camera object.
 
 """
 
 from pyrr import Vector3, Vector4, vector, matrix44
 from sphere_base.sphere_universe_base.suv_cam_movement import CameraMovement
 from sphere_base.utils import dump_exception
+from sphere_base.serializable import Serializable
+from collections import OrderedDict
+import json
 
 MOUSE_SENSITIVITY = .1
 DEFAULT_TARGET = Vector3([0.0, 0.0, 0.0])
 DEFAULT_POS = Vector3([0.0, 0.0, 3.0])
 
 
-class Camera:
+class Camera(Serializable):
     CameraMovement_class = CameraMovement
     """
     Class representing the camera. 
 
     """
 
     def __init__(self, parent):
@@ -46,14 +49,16 @@
           through the center of the camera.
         - **camera_up** - ``Vector3`` with the ``up`` position of the camera.
         - **xyz** - position of the camera (``Vector3``).
         - **mouse_sensitivity** - ``float`` modifier to adjust the sensitivity of the mouse when moving the camera.
 
         """
 
+        super().__init__("camera")
+
         # camera target pointing at origin
         self.target = DEFAULT_TARGET
         self.xyz = DEFAULT_POS
         self.distance_to_target = None
         self.camera_direction = None
         self.camera_up = None
 
@@ -202,7 +207,29 @@
             p1 = (self.xyz[0], self.xyz[1], self.xyz[2])
             angle = self.uv.target_sphere.calc.find_angle(p1, self.uv.target_sphere.orientation)
             # angle, print yaw degrees, pitch degrees
             print(angle)
         except Exception as e:
             dump_exception(e)
 
+    def serialize(self):
+        p = self.xyz
+
+        return OrderedDict([
+            ('id', self.id),
+            ('cam_pos', json.dumps([p[0], p[1], p[2]])),
+            ('cam_yaw', self.cm.yaw),
+        ])
+
+    def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
+
+        if restore_id:
+            self.id = data['id']
+
+        if 'cam_pos' in data:
+            p = json.loads(data['cam_pos'])
+            self.xyz = (round(p[0], 1), round(p[1], 1), round(p[2], 1))
+            self.cm.yaw = data['cam_yaw']
+            self.cm.radius = self.get_distance_to_target()
+
+        return True
+
```

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
             pos = Vector4([x, y, z, 1])
             new_xyzw = matrix44.apply_to_vector(m, pos)
 
         return new_xyzw
 
     def move_to_new_target(self, target_sphere):
         """
-
         Moves the camera to a new ``Target Sphere``
 
         :param target_sphere: The current ``Target Sphere``
         :type target_sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
         return NotImplemented
```

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/skybox.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,74 +61,74 @@
 
         super().__init__(self, 'skybox')
 
         self.uv = universe
         self.model = self.uv.models.get_model('skybox')
         self.xyz = self.uv.cam.xyz
         self.cf = self.uv.config
+        self.skybox_id = None
 
         # We get the shader from the model
         self.shader = self.model.shader
 
         self.scale = None
         self.index = 0
         self.faces = []
         self.orientation = [0, 0, 0]
         self.paint_skybox = True
 
     def get_skybox_set(self, skybox_name=None, skybox_id=None, random=False):
 
         if skybox_id == 0:  # Do not use a skybox
-            self.skb_id = skybox_id
+            self.skybox_id = skybox_id
         elif not skybox_name and not skybox_id and not random:
             random = True  # select a random skybox
         elif skybox_name:
             lst = ['None' if not txt else os.path.basename(txt) for txt in self.uv.config.skybox_sets]
-            self.skb_id = lst.index(skybox_name)  # choose a skybox by its name
+            self.skybox_id = lst.index(skybox_name)  # choose a skybox by its name
         elif skybox_id:
-            self.skb_id = skybox_id  # choose a skybox by its index
+            self.skybox_id = skybox_id  # choose a skybox by its index
 
         if random:
-            self.skb_id = randint(1, len(self.cf.skybox_sets) - 1)  # select a random skybox
+            self.skybox_id = randint(1, len(self.cf.skybox_sets) - 1)  # select a random skybox
 
         self.create_skybox_faces()
 
     def get_next_set(self):
         """
         Activate next Skybox set in the id sequence.
 
         """
-        _id = self.skb_id
-        _id = 0 if self.skb_id + 1 == len(self.cf.skybox_sets) else _id + 1
-        self.skb_id = _id
+        _id = self.skybox_id
+        _id = 0 if self.skybox_id + 1 == len(self.cf.skybox_sets) else _id + 1
+        self.skybox_id = _id
         self.create_skybox_faces()
 
     def get_former_set(self):
         """
         Activate the former set in the id sequence.
 
         """
         # get the one before current sky box image set
-        if self.skb_id - 1 < 0:
-            self.skb_id = len(self.cf.skybox_sets) - 1
+        if self.skybox_id - 1 < 0:
+            self.skybox_id = len(self.cf.skybox_sets) - 1
         else:
-            self.skb_id -= 1
+            self.skybox_id -= 1
         self.create_skybox_faces()
 
     def get_skybox_path(self) -> str:
         """
         Returns the image path of the current active Skybox id
 
         """
 
-        path = self.cf.skybox_sets[self.skb_id]
+        path = self.cf.skybox_sets[self.skybox_id]
         self.paint_skybox = True if path else False
         return path + "/" if path else path
 
-
     def create_skybox_faces(self):
         """
         Gets the six faces of the Skybox from the image path and adds them to the faces array.
 
         """
 
         path = self.get_skybox_path()
```

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 """
 Module universe. The universe contains all the spheres.
 
 """
 
-from pyrr import quaternion, Quaternion
 from collections import OrderedDict
 from sphere_base.serializable import Serializable
 from sphere_base.sphere.sphere import Sphere
 from sphere_base.model.models import Models
 from sphere_base.sphere_universe_base.suv_mouse_ray import MouseRay
-from sphere_base.sphere_universe_base.suv_cam import Camera
-from sphere_base.sphere_universe_base.suv_skybox import Skybox
+from sphere_base.sphere_universe_base.camera import Camera
+from sphere_base.sphere_universe_base.skybox import Skybox
 from sphere_base.sphere_universe_base.suv_rubber_band import RubberBand
 from sphere_base.clipboard import Clipboard
 from sphere_base.config import UvConfig
 from sphere_base.shader.default_shader import DefaultShader
 from sphere_base.calc import *
+import json
 import os.path
 
 DEBUG = False
 TEST_SPHERE_NUMBER = 1
 
 
 class Universe(Serializable):
@@ -67,15 +67,15 @@
             - **mouse_last_y** - last stored y-position (``float``) of the mouse pointer.
             - **mouse_x** - current x-position (``float``) of the mouse pointer.
             - **mouse_y** - current y-position (``float``) of the mouse pointer.
             - **mouse_offset** - ``float`` used when dragging the sphere_base over its axis.
 
         """
 
-        super().__init__("sphere_iot")
+        super().__init__("universe")
 
         self.view = parent
 
         self._spheres = []
         self._edges = []
         self._lens_index = 1  # variable to decide how to texture a sphere_base
 
@@ -163,81 +163,81 @@
 
         self.target_sphere = self.Sphere(self, position=[0.0, 0.0, 0.0], texture_id=0)
 
         for i in range(number - 1):
             sphere = self.Sphere(self)
             sphere.index = i
 
-    def add_sphere(self, sphere: 'sphere_base'):
+    def add_sphere(self, sphere):
         """
         Add a new sphere_base to the internal list. Adds listeners.
 
         :param sphere: The ``sphere_base`` that will be added to the ``Universe``
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
 
         self._spheres.append(sphere)
         sphere.add_selection_changed_listener(self.on_selection_changed)
         sphere.add_has_been_modified_listener(self.on_modified)
 
-    def remove_sphere(self, sphere: 'sphere_base'):
+    def remove_sphere(self, sphere):
         """
         Removing a sphere_base from the internal list.
 
         :param sphere: The ``sphere_base`` that will be removed from the internal list``
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
 
         """
 
         if sphere in self._spheres:
             self._spheres.remove(sphere)
 
-    def add_edge(self, edge: 'Edge'):
+    def add_edge(self, edge):
         """
         Add a new edge to the internal list.
 
         :param edge: The ``edge`` that will be added to the ``Universe``
         :type edge: :class:`~sphere_iot.uv_sphere_edge.SphereEdge`
 
         """
 
         self._edges.append(edge)
 
-    def remove_edge(self, edge: 'edge'):
+    def remove_edge(self, edge):
         """
         Removing a sphere_base from the internal list.
 
         :param edge: The ``edge`` that will be removed from the internal list``
         :type edge: :class:`~sphere_iot.uv_sphere_edge.SphereEdge`
 
         """
 
         if edge in self._edges:
             self._edges.remove(edge)
 
-    def add_selection_changed_listener(self, callback: 'function'):
+    def add_selection_changed_listener(self, callback):
         """
         Register callback for 'selection changed' event.
 
         :param callback: callback function
 
         """
         self._selection_changed_listeners.append(callback)
 
-    def add_modified_listener(self, callback: 'function'):
+    def add_modified_listener(self, callback):
         """
         Register callback for 'modified' event.
 
         :param callback: callback function
 
         """
         self._has_been_modified_listeners.append(callback)
 
-    def on_selection_changed(self, sphere: 'sphere_base', sphere_items: list):
+    def on_selection_changed(self, sphere, sphere_items: list):
         """
         Handles 'selection changed' and triggers event 'selection changed'.
 
         :param sphere: The target sphere_base that is _selected
         :type sphere: :class:`~sphere_iot.uv_sphere.Sphere`
         :param sphere_items: ``list`` of items on the sphere_base
         :type sphere_items: list with items of type :class:`~sphere_iot.uv_node.Node` or
@@ -305,18 +305,19 @@
                 self.cam.move_to_new_target_sphere(sphere)
                 is_sphere = True
                 self.on_selection_changed(self.target_sphere, None)
         return is_sphere
 
     def rotate_target_sphere_with_mouse(self, offset: float = 0, collision_point=None):
         """
-        Rotating the target sphere_base with the mouse y axis.
+        Rotating the target sphere_base with the mouse y-axis.
         Set the mouse offset here which will be picked up and used from the main loop and will be translated to rotation
 
         :param offset: mouse current x-position offset and last stored position.
+        :param collision_point: mouse ray collision point with sphere.
         :type offset: ``float``
 
         .. note::
 
             This method only sets the mouse offset value which is then picked up from the main loop
 
         """
@@ -382,33 +383,44 @@
             edge.draw()
 
     def serialize(self):
         spheres = []
         for sphere in self._spheres:
             spheres.append(sphere.serialize())
 
-        return OrderedDict([
-            ('id', self.id),
-            ('type', self.type),
-            ('view_width', self.view.view_width),
-            ('view_height', self.view.view_height),
-            ('spheres', spheres),
-            ('target_sphere_id', self.target_sphere.id)
-        ])
+        try:
+            return OrderedDict([
+                ('id', self.id),
+                ('type', self.type),
+                ('view_width', self.view.view_width),
+                ('view_height', self.view.view_height),
+                ('skybox_id', self.skybox.skybox_id),
+                ('camera', [self.cam.serialize()]),
+                ('spheres', spheres),
+                ('target_sphere_id', self.target_sphere.id)
+            ])
+        except Exception as e:
+            dump_exception(e)
 
     def deserialize(self, data: dict, hashmap: dict = None, restore_id: bool = True) -> bool:
         self.clear()
         hashmap = hashmap if hashmap else {}
         self.id = data['id']
         self.mouse_ray.reset()
+        if 'skybox_id' in data:
+            if self.skybox.skybox_id != data['skybox_id']:
+                self.skybox.skybox_id = data['skybox_id']
+                self.skybox.create_skybox_faces()
 
         # deserialize spheres
         for sphere_data in data['spheres']:
             self.Sphere(self, [0.0, 0.0, 0.0], 0).deserialize(sphere_data, hashmap)
 
         for sphere in self._spheres:
             if data['target_sphere_id'] == sphere.id:
                 self.target_sphere = sphere
 
-        self.cam.reset_to_default_view(self.target_sphere)
+        # deserialize camera
+        for camera in data['camera']:
+            self.cam.deserialize(camera, hashmap)
 
         return True
```

### Comparing `sphere_base-0.1.7/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.8/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sphere_base.sphere_universe_base.suv_universe import Universe
 from sphere_base.constants import *
 from sphere_base.utils import dump_exception
 
 
 class UVWidget(QGLWidget):
     """
-    This class represents the ``Universe Widget class`` its a pyqt5 wrapper around the OpenGL widget.
+    This class represents the ``Universe Widget class`` it is a pyqt5 wrapper around the OpenGL widget.
 
     """
 
     Universe_class = Universe
     keyPressed = pyqtSignal(int)
 
     def __init__(self, parent):
@@ -106,15 +106,15 @@
         glViewport(0, 0, width, height)
 
         self.uv.shader.set_window_size()
         self.uv.config.on_win_size_changed()
         self.uv.view_width = width
         self.uv.view_height = height
 
-    def contextMenuEvent(self, event: 'event') -> 'event':
+    def contextMenuEvent(self, event):
         """
 
         :param event: xy-mouse position
         :type event: 'event'
         :return:
 
         """
@@ -131,15 +131,15 @@
         point coordinates.
 
         """
         self._clicked_on_item, self.mouse_ray_collision_point = self.uv.mouse_ray.check_mouse_ray(self.mouse_x,
                                                                                                   self.mouse_y)
         return self._clicked_on_item, self.mouse_ray_collision_point, self.mouse_x, self.mouse_y
 
-    def mousePressEvent(self, event: 'event'):
+    def mousePressEvent(self, event):
         """
         Handles mouse press event
 
         :param event: contains the x and y mouse position
         :type event: 'event'
 
         """
@@ -232,21 +232,20 @@
                     elif item and item.type == "node":
                         # if edge does not already exist, create it
                         self.uv.target_sphere.create_edge(item.socket)
             except Exception as e:
                 dump_exception(e)
 
         if self._middle_mouse_button_down:
-            for item in self.uv.target_sphere.items:
-                if item.type in ('sphere', 'edge', 'node', 'socket'):
-                    item.update_collision_object()
+            # update all the collision objects on the sphere
+            self.uv.target_sphere.update_item_collision_objects()
 
         self._reset_mouse()
 
-    def mouseMoveEvent(self, event: 'event'):
+    def mouseMoveEvent(self, event):
         """
         Handles mouse release event
 
         :param event: contains the x and y mouse position
         :type event: 'event'
 
         """
@@ -291,18 +290,18 @@
         elif self._middle_mouse_button_down:
 
             x_offset, y_offset = self.get_mouse_position_offset(x, y)
 
             if self._clicked_on_item and self._clicked_on_item == self.uv.target_sphere.id:
                 self.setCursor(QCursor(Qt.ClosedHandCursor))
 
-                # only rotate the sphere_base over the y axis
+                # only rotate the sphere_base over the y-axis
                 self.uv.rotate_target_sphere_with_mouse(x_offset, self.mouse_ray_collision_point)
 
-                # rotation over the x axis are done through moving the camera
+                # rotation over the x-axis are done through moving the camera
                 self.uv.cam.process_mouse_movement(self.uv.target_sphere, 0, -y_offset)
 
     def wheelEvent(self, event):
         """
         Handles mouse wheel event.
 
         :param event: contains mouse wheel rotation
@@ -412,36 +411,36 @@
 
         # store the new mouse position as the last mouse position
         self.mouse_last_x = x_pos
         self.mouse_last_y = y_pos
 
         return x_offset, y_offset
 
-    def handle_context_menu(self, event: 'event'):
+    def handle_context_menu(self, event):
         """
         Handles context menu
 
         :param event: Handles context menu
         :type event: 'event
 
         """
 
-        menuStyle = (
+        menu_style = (
             "QMenu::item{"
             "background-color: lightGrey;"
             "color: black;"
             "}"
             "QMenu::item:selected{"
             "background-color: darkGrey;"
             "color: rgb(255, 255, 255, 255);"
             "}"
         )
 
         context_menu = QMenu(self)
-        context_menu.setStyleSheet(menuStyle)
+        context_menu.setStyleSheet(menu_style)
         context_menu.setGraphicsEffect(QGraphicsOpacityEffect(opacity=.8))
         create_person_node = context_menu.addAction("Person node")  # 1
         create_item_node = context_menu.addAction("Item node")  # 2
 
         # create_entity_node = context_menu.addAction("Entity node")  # 3
         action = context_menu.exec_(self.mapToGlobal(event.pos()))
```

### Comparing `sphere_base-0.1.7/sphere_base/utils.py` & `sphere_base-0.1.8/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.7/sphere_base.egg-info/PKG-INFO` & `sphere_base-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sphere-base
-Version: 0.1.7
+Name: sphere_base
+Version: 0.1.8
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.7/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.8/sphere_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -176,16 +176,16 @@
 sphere_base/sphere_overlay/qss/__init__.py
 sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
 sphere_base/sphere_overlay/sphere_nodes/__init__.py
 sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
 sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
 sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
 sphere_base/sphere_universe_base/__init__.py
-sphere_base/sphere_universe_base/suv_cam.py
+sphere_base/sphere_universe_base/camera.py
+sphere_base/sphere_universe_base/skybox.py
 sphere_base/sphere_universe_base/suv_cam_movement.py
 sphere_base/sphere_universe_base/suv_graphic_item.py
 sphere_base/sphere_universe_base/suv_mouse_ray.py
 sphere_base/sphere_universe_base/suv_rubber_band.py
-sphere_base/sphere_universe_base/suv_skybox.py
 sphere_base/sphere_universe_base/suv_universe.py
 sphere_base/sphere_universe_base/suv_widget.py
 tests/test_000_import.py
```

### Comparing `sphere_base-0.1.7/tests/test_000_import.py` & `sphere_base-0.1.8/tests/test_000_import.py`

 * *Files identical despite different names*


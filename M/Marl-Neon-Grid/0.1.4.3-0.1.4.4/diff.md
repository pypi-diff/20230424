# Comparing `tmp/Marl-Neon-Grid-0.1.4.3.tar.gz` & `tmp/Marl-Neon-Grid-0.1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Neon-Grid-0.1.4.3.tar", last modified: Thu Mar 23 14:09:55 2023, max compression
+gzip compressed data, was "Marl-Neon-Grid-0.1.4.4.tar", last modified: Mon Apr 24 12:06:26 2023, max compression
```

## Comparing `Marl-Neon-Grid-0.1.4.3.tar` & `Marl-Neon-Grid-0.1.4.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.336127 Marl-Neon-Grid-0.1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-23 14:09:55.000000 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-23 14:09:55.000000 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:09:55.000000 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 14:09:55.000000 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 14:09:55.000000 Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-23 14:09:55.336127 Marl-Neon-Grid-0.1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/examples.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/eat_food_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/movement_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/open_door_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/door.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/floor.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/food.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/wall.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/closed_rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/game_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.328127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/levels/10x10_left.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/levels/10x10_right.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/doors_n_agents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/levels/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/levels/10x10_2A.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/levels/10x10_2A_hard.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/food_n_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/game_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/levels/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/levels/10x10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/gridworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/ray_caster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/adversary.png
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent.png
--rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_collision.png
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_invalid.png
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_valid.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.332127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/doors/door_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/doors/door_open.png
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/drop_off.png
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/food.png
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/item.png
--rw-r--r--   0 runner    (1001) docker     (123)    52843 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:09:55.336127 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/
--rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall.png
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_lower_left_corner.png
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_lower_right_corner.png
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_upper_left_corner.png
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_upper_right_corner.png
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/zone.png
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/render_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:09:55.336127 Marl-Neon-Grid-0.1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-23 14:09:39.000000 Marl-Neon-Grid-0.1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.475342 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-24 12:06:26.000000 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-24 12:06:26.000000 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:06:26.000000 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 12:06:26.000000 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 12:06:26.000000 Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/examples.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.475342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.475342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/eat_food_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/movement_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/open_door_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/food.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/wall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/closed_rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/game_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/levels/10x10_left.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/levels/10x10_right.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/doors_n_agents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/levels/10x10_2A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/levels/10x10_2A_hard.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/food_n_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/game_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/levels/10x10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/gridworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/ray_caster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/adversary.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_collision.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_invalid.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_valid.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/doors/door_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/doors/door_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/drop_off.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/food.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/item.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52843 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/
+-rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_lower_left_corner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_lower_right_corner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_upper_left_corner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_upper_right_corner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/zone.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/render_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:06:26.479342 Marl-Neon-Grid-0.1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-24 12:06:13.000000 Marl-Neon-Grid-0.1.4.4/setup.py
```

### Comparing `Marl-Neon-Grid-0.1.4.3/LICENSE` & `Marl-Neon-Grid-0.1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/PKG-INFO` & `Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Neon-Grid
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: A collection of MARL gridworlds to study coordination and cooperation.
 Home-page: https://github.com/romue404/marl-neon-grid
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Neon-Grid-0.1.4.3/Marl_Neon_Grid.egg-info/SOURCES.txt` & `Marl-Neon-Grid-0.1.4.4/Marl_Neon_Grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/PKG-INFO` & `Marl-Neon-Grid-0.1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Neon-Grid
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: A collection of MARL gridworlds to study coordination and cooperation.
 Home-page: https://github.com/romue404/marl-neon-grid
 Author: Robert Müller
 Author-email: robert.mueller1990@googlemail.com
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Neon-Grid-0.1.4.3/README.md` & `Marl-Neon-Grid-0.1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/examples.png` & `Marl-Neon-Grid-0.1.4.4/examples.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/command.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/command.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/eat_food_command.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/eat_food_command.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/movement_commands.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/movement_commands.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/commands/open_door_command.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/commands/open_door_command.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/agent.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/door.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/door.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/entity.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/entity.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/food.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/food.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/entitites/states.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/entitites/states.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/closed_rooms.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/closed_rooms.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.lvl_entities = entities.copy()
 
         self.game_state = ClosedRoomsGameState(
             entities=Entities(self.lvl_entities),
             n_agents=self.n_agents,
             max_steps=self.max_steps,
         )
+        self.zone_pos = [e.pos for e in self.game_state.entities.symbol_dict[Zone.SYMBOL]]
 
     def step(self, actions):
         self.game_state.tick()
         commands = []
         agents = self.game_state.agents
         reward = [0]*len(agents)
 
@@ -42,20 +43,14 @@
 
             else:
                 raise NotImplementedError('Use actions from 0-9.')
 
         for c in commands:
             c.run()
 
-        reward = [int(agent.pos in [e.pos for e in self.game_state.entities[agent.pos] if isinstance(e, Zone)])
-                  for agent in agents]
-        success = False#sum(reward) == self.n_agents
-        reward =  [0.25*r -0.01 for r in reward]
-
-        #reward = [2.0]*len(agents) if success else [0.05*r - 0.01 for r in reward]
-
+        ag_pos = [a.pos for a in self.game_state.agents]
+        reward = [int(a in self.zone_pos) for a in ag_pos]
+        reward = [r if r >= 1 else -1e-2 for r in reward]
         obs = self.local_obs()
         obs[1][self.ENTITY_POS[Zone]] = 0.0  # goal is invisible to second agent
-        done = self.game_state.is_game_over() or success
-
         info = {}
-        return obs, reward, [done]*len(agents), info
+        return obs, reward, [self.game_state.is_game_over()]*len(agents), info
```

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/closed_rooms/game_state.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/closed_rooms/game_state.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/doors_n_agents/doors_n_agents.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/doors_n_agents/doors_n_agents.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/food_n_agents.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/food_n_agents.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/food_n_agents/game_state.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/food_n_agents/game_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
         for food in self.get_food():
             self.entities.append(food)
 
     def get_food(self):
         floor_tiles = self.entities[Floor.SYMBOL]
         random.shuffle(floor_tiles)
-        food = [Food(pos=ft.pos, capacity=2 if not self.agents_must_coordinate else 1)
+        food = [Food(pos=ft.pos, capacity=len(self.agents) if self.agents_must_coordinate else 1)
                 for ft in floor_tiles[:self.n_food]]
         return food
 
     def is_game_over(self):
         no_more_food = len(self.entities.symbol_dict[Food.SYMBOL]) == 0
         return super().is_game_over() or no_more_food
```

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/environments/gridworld.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/environments/gridworld.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/ray_caster.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/ray_caster.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/adversary.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_collision.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_invalid.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/agents/agent_valid.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/agents/agent_valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/doors/door_closed.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/doors/door_open.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/drop_off.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/drop_off.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/food.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/food.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/item.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/item.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/logo.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/logo.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_horizontal.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_horizontal.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_lower_left_corner.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_lower_left_corner.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_lower_right_corner.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_lower_right_corner.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_upper_left_corner.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_upper_left_corner.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_upper_right_corner.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_upper_right_corner.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/wall/wall_vertical.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/wall/wall_vertical.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/assets/zone.png` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/assets/zone.png`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/base_renderer.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/base_renderer.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/render_groups.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/render_groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/marl_neon_grid/rendering/renderer.py` & `Marl-Neon-Grid-0.1.4.4/marl_neon_grid/rendering/renderer.py`

 * *Files identical despite different names*

### Comparing `Marl-Neon-Grid-0.1.4.3/setup.py` & `Marl-Neon-Grid-0.1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Neon-Grid',
-      version='0.1.4.3',
+      version='0.1.4.4',
       description='A collection of MARL gridworlds to study coordination and cooperation.',
       author='Robert Müller',
       author_email='robert.mueller1990@googlemail.com',
       url='https://github.com/romue404/marl-neon-grid',
       license='MIT',
       keywords=[
             'artificial intelligence',
```


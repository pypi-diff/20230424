# Comparing `tmp/dj_beatcloud-2.4.1b5.tar.gz` & `tmp/dj_beatcloud-2.4.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b5.tar", last modified: Sun Apr 23 15:10:39 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b6.tar", last modified: Mon Apr 24 19:51:17 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b5.tar` & `dj_beatcloud-2.4.1b6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607978 dj_beatcloud-2.4.1b5/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-23 15:10:39.608108 dj_beatcloud-2.4.1b5/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-23 15:10:39.608472 dj_beatcloud-2.4.1b5/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-23 15:10:29.000000 dj_beatcloud-2.4.1b5/setup.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.591810 dj_beatcloud-2.4.1b5/src/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.595153 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-23 15:10:39.000000 dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.596075 dj_beatcloud-2.4.1b5/src/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/__init__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.598811 dj_beatcloud-2.4.1b5/src/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/.DS_Store
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4641 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/configs/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/dj_tools.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.598976 dj_beatcloud-2.4.1b5/src/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b5/src/djtools/logs/empty.txt
--rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b5/src/djtools/main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.602038 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3013 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.603408 dj_beatcloud-2.4.1b5/src/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.605593 dj_beatcloud-2.4.1b5/src/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8185 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4713 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607334 dj_beatcloud-2.4.1b5/src/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7970 2023-04-23 15:09:12.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/djtools/utils/url_download.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-23 15:10:39.607786 dj_beatcloud-2.4.1b5/src/test_data/
--rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/test_data/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-18 16:15:41.000000 dj_beatcloud-2.4.1b5/src/test_data/conftest.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.293552 dj_beatcloud-2.4.1b6/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-24 19:51:17.293658 dj_beatcloud-2.4.1b6/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-24 19:51:17.294093 dj_beatcloud-2.4.1b6/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.278750 dj_beatcloud-2.4.1b6/src/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.281256 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-24 19:51:17.000000 dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.281916 dj_beatcloud-2.4.1b6/src/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/__init__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.285277 dj_beatcloud-2.4.1b6/src/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/.DS_Store
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4641 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/configs/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/dj_tools.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.285451 dj_beatcloud-2.4.1b6/src/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b6/src/djtools/logs/empty.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b6/src/djtools/main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.287374 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3013 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.288826 dj_beatcloud-2.4.1b6/src/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.290748 dj_beatcloud-2.4.1b6/src/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8185 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4713 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.292988 dj_beatcloud-2.4.1b6/src/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7970 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-24 19:50:59.000000 dj_beatcloud-2.4.1b6/src/djtools/utils/url_download.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-24 19:51:17.293394 dj_beatcloud-2.4.1b6/src/test_data/
+-rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/test_data/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-24 19:50:56.000000 dj_beatcloud-2.4.1b6/src/test_data/conftest.py
```

### Comparing `dj_beatcloud-2.4.1b5/LICENSE` & `dj_beatcloud-2.4.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/PKG-INFO` & `dj_beatcloud-2.4.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b5
+Version: 2.4.1b6
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b5/README.md` & `dj_beatcloud-2.4.1b6/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/setup.py` & `dj_beatcloud-2.4.1b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b5',
+    version='2.4.1-b6',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

### Comparing `dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b5
+Version: 2.4.1b6
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b5/src/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.4.1b6/src/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/__init__.py` & `dj_beatcloud-2.4.1b6/src/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/.DS_Store` & `dj_beatcloud-2.4.1b6/src/djtools/configs/.DS_Store`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/README.md` & `dj_beatcloud-2.4.1b6/src/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/config.py` & `dj_beatcloud-2.4.1b6/src/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b6/src/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.4.1b6/src/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b6/src/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/dj_tools.py` & `dj_beatcloud-2.4.1b6/src/djtools/dj_tools.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/main.py` & `dj_beatcloud-2.4.1b6/src/djtools/main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
 
     Args:
         track: TRACK node from XML.
         destination: Directory to copy tracks to.
         loc_prefix: Location field prefix.
     """
     loc = Path(unquote(track["Location"]).split(loc_prefix)[-1])
-    new_loc = destination / loc.name
-    shutil.copyfile(loc, new_loc)		
-    track["Location"] = f"{loc_prefix}{quote(new_loc.as_posix())}"
+    new_loc = Path(destination / loc.name).as_posix()
+    shutil.copyfile(loc.as_posix(), new_loc)
+    track["Location"] = f"{loc_prefix}{new_loc}"
 
 
 def get_playlist_track_locations(
     soup: BeautifulSoup, _playlist: str, seen_tracks: Set[str]
 ) -> List[str]:
     """Finds playlist in "XML_PATH" that matches "_playlist" and returns a list
         of the track nodes in that playlist that aren't in "seen_tracks".
```

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b6/src/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b6/src/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/config.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b6/src/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/test_main.py` & `dj_beatcloud-2.4.1b6/src/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/__init__.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/config.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b5/src/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b6/src/djtools/utils/url_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ydl_opts = {
         "format": "bestaudio/best",
         "postprocessors": [{
             "key": "FFmpegExtractAudio",
             "preferredcodec": "mp3",
             "preferredquality": "320",
         }],
-        "outtmpl": dl_loc / "%(title)s.%(ext)s"
+        "outtmpl": (dl_loc / "%(title)s.%(ext)s").as_posix()
     }
 
     with ytdl.YoutubeDL(ydl_opts) as ydl:
         logger.info(f"Downloading {config.URL_DOWNLOAD} to {dl_loc}")
         ydl.download([config.URL_DOWNLOAD])
 
     for _file in dl_loc.iterdir():
```

### Comparing `dj_beatcloud-2.4.1b5/src/test_data/conftest.py` & `dj_beatcloud-2.4.1b6/src/test_data/conftest.py`

 * *Files identical despite different names*


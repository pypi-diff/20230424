# Comparing `tmp/thorpy-2.0.1.tar.gz` & `tmp/thorpy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorpy-2.0.1.tar", last modified: Fri Apr 21 16:52:12 2023, max compression
+gzip compressed data, was "thorpy-2.0.3.tar", last modified: Mon Apr 24 16:21:54 2023, max compression
```

## Comparing `thorpy-2.0.1.tar` & `thorpy-2.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 16:52:12.648766 thorpy-2.0.1/
--rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      378 2023-04-21 16:52:12.648766 thorpy-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2231 2023-04-21 16:48:12.000000 thorpy-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 16:52:12.648766 thorpy-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      531 2023-04-21 16:52:04.000000 thorpy-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:52:12.597719 thorpy-2.0.1/thorpy/
--rw-rw-rw-   0        0        0     3494 2023-04-21 13:29:09.000000 thorpy-2.0.1/thorpy/__init__.py
--rw-rw-rw-   0        0        0    53373 2023-04-21 14:37:29.000000 thorpy-2.0.1/thorpy/canonical.py
--rw-rw-rw-   0        0        0   124119 2023-04-21 16:26:17.000000 thorpy-2.0.1/thorpy/elements.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:52:12.647765 thorpy-2.0.1/thorpy/examples/
--rw-rw-rw-   0        0        0        0 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/examples/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-04-21 15:19:35.000000 thorpy-2.0.1/thorpy/examples/_example_alert.py
--rw-rw-rw-   0        0        0     1243 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/examples/_example_anim_move.py
--rw-rw-rw-   0        0        0     1703 2023-04-21 15:37:12.000000 thorpy-2.0.1/thorpy/examples/_example_animatedgif.py
--rw-rw-rw-   0        0        0      992 2023-04-21 15:28:00.000000 thorpy-2.0.1/thorpy/examples/_example_box.py
--rw-rw-rw-   0        0        0      861 2023-04-21 11:02:12.000000 thorpy-2.0.1/thorpy/examples/_example_button_helloworld.py
--rw-rw-rw-   0        0        0      868 2023-04-21 16:26:20.000000 thorpy-2.0.1/thorpy/examples/_example_color_gradient.py
--rw-rw-rw-   0        0        0     1208 2023-04-21 14:42:25.000000 thorpy-2.0.1/thorpy/examples/_example_colorpicker.py
--rw-rw-rw-   0        0        0     2400 2023-04-21 14:42:35.000000 thorpy-2.0.1/thorpy/examples/_example_colorpicker2.py
--rw-rw-rw-   0        0        0     2402 2023-04-21 15:34:14.000000 thorpy-2.0.1/thorpy/examples/_example_colorpicker_fine_tuning.py
--rw-rw-rw-   0        0        0     3284 2023-04-21 15:34:08.000000 thorpy-2.0.1/thorpy/examples/_example_create_style.py
--rw-rw-rw-   0        0        0     3425 2023-04-21 15:34:12.000000 thorpy-2.0.1/thorpy/examples/_example_create_style2.py
--rw-rw-rw-   0        0        0     2249 2023-04-21 16:24:36.000000 thorpy-2.0.1/thorpy/examples/_example_custom_theme.py
--rw-rw-rw-   0        0        0     2063 2023-04-21 15:32:59.000000 thorpy-2.0.1/thorpy/examples/_example_dropdownlist.py
--rw-rw-rw-   0        0        0     1790 2023-04-21 15:21:30.000000 thorpy-2.0.1/thorpy/examples/_example_events.py
--rw-rw-rw-   0        0        0     1177 2023-04-21 15:21:31.000000 thorpy-2.0.1/thorpy/examples/_example_filebrowser.py
--rw-rw-rw-   0        0        0     2245 2023-04-21 15:35:55.000000 thorpy-2.0.1/thorpy/examples/_example_fx_light_emitting_image.py
--rw-rw-rw-   0        0        0     3235 2023-04-21 15:35:59.000000 thorpy-2.0.1/thorpy/examples/_example_fx_lights.py
--rw-rw-rw-   0        0        0     1984 2023-04-21 16:25:31.000000 thorpy-2.0.1/thorpy/examples/_example_get_value_from_elements.py
--rw-rw-rw-   0        0        0     1376 2023-04-21 15:26:49.000000 thorpy-2.0.1/thorpy/examples/_example_grouping.py
--rw-rw-rw-   0        0        0     1112 2023-04-21 15:26:45.000000 thorpy-2.0.1/thorpy/examples/_example_grouping_without_sorting.py
--rw-rw-rw-   0        0        0     2575 2023-04-21 15:27:00.000000 thorpy-2.0.1/thorpy/examples/_example_groups_of_groups.py
--rw-rw-rw-   0        0        0     3731 2023-04-21 16:25:23.000000 thorpy-2.0.1/thorpy/examples/_example_guess_the_number.py
--rw-rw-rw-   0        0        0     1573 2023-04-21 15:21:24.000000 thorpy-2.0.1/thorpy/examples/_example_helper.py
--rw-rw-rw-   0        0        0      982 2023-04-21 15:36:56.000000 thorpy-2.0.1/thorpy/examples/_example_heterogeneous_texts.py
--rw-rw-rw-   0        0        0      685 2023-04-18 17:56:40.000000 thorpy-2.0.1/thorpy/examples/_example_image_with_text.py
--rw-rw-rw-   0        0        0     1322 2023-04-19 11:09:08.000000 thorpy-2.0.1/thorpy/examples/_example_imagebutton.py
--rw-rw-rw-   0        0        0     1532 2023-04-21 15:21:20.000000 thorpy-2.0.1/thorpy/examples/_example_integration_in_existing_code.py
--rw-rw-rw-   0        0        0     1316 2023-04-21 16:25:16.000000 thorpy-2.0.1/thorpy/examples/_example_labels.py
--rw-rw-rw-   0        0        0     3028 2023-04-21 15:21:13.000000 thorpy-2.0.1/thorpy/examples/_example_launch.py
--rw-rw-rw-   0        0        0     1287 2023-04-21 15:21:12.000000 thorpy-2.0.1/thorpy/examples/_example_lifebar.py
--rw-rw-rw-   0        0        0     1305 2023-04-21 15:34:40.000000 thorpy-2.0.1/thorpy/examples/_example_look_tune.py
--rw-rw-rw-   0        0        0     2297 2023-04-21 15:36:39.000000 thorpy-2.0.1/thorpy/examples/_example_rich_text.py
--rw-rw-rw-   0        0        0     1307 2023-04-21 15:34:50.000000 thorpy-2.0.1/thorpy/examples/_example_set_default_font.py
--rw-rw-rw-   0        0        0     2128 2023-04-21 15:36:03.000000 thorpy-2.0.1/thorpy/examples/_example_shadows.py
--rw-rw-rw-   0        0        0     3051 2023-04-21 16:25:09.000000 thorpy-2.0.1/thorpy/examples/_example_showcase_themes.py
--rw-rw-rw-   0        0        0     3184 2023-04-21 16:24:42.000000 thorpy-2.0.1/thorpy/examples/_example_showcase_themes2.py
--rw-rw-rw-   0        0        0     2119 2023-04-21 15:27:41.000000 thorpy-2.0.1/thorpy/examples/_example_showcase_themes_buttons.py
--rw-rw-rw-   0        0        0     1500 2023-04-21 16:23:06.000000 thorpy-2.0.1/thorpy/examples/_example_showfps.py
--rw-rw-rw-   0        0        0     1660 2023-04-21 16:22:42.000000 thorpy-2.0.1/thorpy/examples/_example_slider.py
--rw-rw-rw-   0        0        0     2460 2023-04-21 15:26:13.000000 thorpy-2.0.1/thorpy/examples/_example_text_input.py
--rw-rw-rw-   0        0        0     2765 2023-04-21 15:34:59.000000 thorpy-2.0.1/thorpy/examples/_example_text_width.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 15:27:53.000000 thorpy-2.0.1/thorpy/examples/_example_togglables_pool.py
--rw-rw-rw-   0        0        0     1105 2023-04-21 15:22:04.000000 thorpy-2.0.1/thorpy/examples/_example_user_choices.py
--rw-rw-rw-   0        0        0     1431 2023-04-21 15:22:07.000000 thorpy-2.0.1/thorpy/examples/_example_user_choices2.py
--rw-rw-rw-   0        0        0     2051 2023-04-21 16:22:21.000000 thorpy-2.0.1/thorpy/examples/_example_user_chooses_font.py
--rw-rw-rw-   0        0        0     2219 2023-04-19 17:51:07.000000 thorpy-2.0.1/thorpy/examples/_example_waiting_bar.py
--rw-rw-rw-   0        0        0     4520 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/gametools.py
--rw-rw-rw-   0        0        0    28799 2023-04-19 18:38:31.000000 thorpy-2.0.1/thorpy/graphics.py
--rw-rw-rw-   0        0        0     6018 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/loops.py
--rw-rw-rw-   0        0        0     1563 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/monitoring.py
--rw-rw-rw-   0        0        0      467 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/parameters.py
--rw-rw-rw-   0        0        0      625 2023-04-18 18:04:04.000000 thorpy-2.0.1/thorpy/setup.py
--rw-rw-rw-   0        0        0     3727 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/shadows.py
--rw-rw-rw-   0        0        0     2540 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/sorting.py
--rw-rw-rw-   0        0        0     2307 2023-04-18 17:53:15.000000 thorpy-2.0.1/thorpy/sound.py
--rw-rw-rw-   0        0        0    35577 2023-04-21 15:02:05.000000 thorpy-2.0.1/thorpy/styles.py
--rw-rw-rw-   0        0        0    32875 2023-04-21 15:06:09.000000 thorpy-2.0.1/thorpy/themes.py
-drwxrwxrwx   0        0        0        0 2023-04-21 16:52:12.609721 thorpy-2.0.1/thorpy.egg-info/
--rw-rw-rw-   0        0        0      378 2023-04-21 16:52:12.000000 thorpy-2.0.1/thorpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-04-21 16:52:12.000000 thorpy-2.0.1/thorpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 16:52:12.000000 thorpy-2.0.1/thorpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 16:52:12.000000 thorpy-2.0.1/thorpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.900268 thorpy-2.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-04-18 20:35:49.000000 thorpy-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-04-24 16:21:54.900268 thorpy-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-04-24 16:16:09.000000 thorpy-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:21:54.901269 thorpy-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-04-24 16:21:18.000000 thorpy-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.859259 thorpy-2.0.3/thorpy/
+-rw-rw-rw-   0        0        0     3605 2023-04-24 16:20:06.000000 thorpy-2.0.3/thorpy/__init__.py
+-rw-rw-rw-   0        0        0    53375 2023-04-24 16:05:08.000000 thorpy-2.0.3/thorpy/canonical.py
+-rw-rw-rw-   0        0        0   124135 2023-04-24 16:05:18.000000 thorpy-2.0.3/thorpy/elements.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.899268 thorpy-2.0.3/thorpy/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_alert.py
+-rw-rw-rw-   0        0        0     1243 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_anim_move.py
+-rw-rw-rw-   0        0        0     1703 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_animatedgif.py
+-rw-rw-rw-   0        0        0      992 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_box.py
+-rw-rw-rw-   0        0        0      861 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_button_helloworld.py
+-rw-rw-rw-   0        0        0      868 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_color_gradient.py
+-rw-rw-rw-   0        0        0     1183 2023-04-24 16:05:29.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker.py
+-rw-rw-rw-   0        0        0     2400 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker2.py
+-rw-rw-rw-   0        0        0     2402 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_colorpicker_fine_tuning.py
+-rw-rw-rw-   0        0        0     3284 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_create_style.py
+-rw-rw-rw-   0        0        0     3425 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_create_style2.py
+-rw-rw-rw-   0        0        0     2249 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_custom_theme.py
+-rw-rw-rw-   0        0        0     2063 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_dropdownlist.py
+-rw-rw-rw-   0        0        0     1790 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_events.py
+-rw-rw-rw-   0        0        0     1177 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_filebrowser.py
+-rw-rw-rw-   0        0        0     2245 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_fx_light_emitting_image.py
+-rw-rw-rw-   0        0        0     3235 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_fx_lights.py
+-rw-rw-rw-   0        0        0     1984 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_get_value_from_elements.py
+-rw-rw-rw-   0        0        0     1376 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_grouping.py
+-rw-rw-rw-   0        0        0     1112 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_grouping_without_sorting.py
+-rw-rw-rw-   0        0        0     2575 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_groups_of_groups.py
+-rw-rw-rw-   0        0        0     3731 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_guess_the_number.py
+-rw-rw-rw-   0        0        0     1573 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_helper.py
+-rw-rw-rw-   0        0        0      982 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_heterogeneous_texts.py
+-rw-rw-rw-   0        0        0      685 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_image_with_text.py
+-rw-rw-rw-   0        0        0     1322 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_imagebutton.py
+-rw-rw-rw-   0        0        0     1532 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_integration_in_existing_code.py
+-rw-rw-rw-   0        0        0     1316 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_labels.py
+-rw-rw-rw-   0        0        0     3028 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_launch.py
+-rw-rw-rw-   0        0        0     1287 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_lifebar.py
+-rw-rw-rw-   0        0        0     1305 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_look_tune.py
+-rw-rw-rw-   0        0        0     2297 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_rich_text.py
+-rw-rw-rw-   0        0        0     1307 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_set_default_font.py
+-rw-rw-rw-   0        0        0     2128 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_shadows.py
+-rw-rw-rw-   0        0        0     3051 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes.py
+-rw-rw-rw-   0        0        0     3184 2023-04-24 16:00:12.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes2.py
+-rw-rw-rw-   0        0        0     2119 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showcase_themes_buttons.py
+-rw-rw-rw-   0        0        0     1500 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_showfps.py
+-rw-rw-rw-   0        0        0     1660 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_slider.py
+-rw-rw-rw-   0        0        0     2460 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_text_input.py
+-rw-rw-rw-   0        0        0     2765 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_text_width.py
+-rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_togglables_pool.py
+-rw-rw-rw-   0        0        0     1105 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_user_choices.py
+-rw-rw-rw-   0        0        0     1431 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_user_choices2.py
+-rw-rw-rw-   0        0        0     2051 2023-04-24 16:01:46.000000 thorpy-2.0.3/thorpy/examples/_example_user_chooses_font.py
+-rw-rw-rw-   0        0        0     2219 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/examples/_example_waiting_bar.py
+-rw-rw-rw-   0        0        0     4520 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/gametools.py
+-rw-rw-rw-   0        0        0    28781 2023-04-22 19:22:36.000000 thorpy-2.0.3/thorpy/graphics.py
+-rw-rw-rw-   0        0        0     6068 2023-04-24 15:17:59.000000 thorpy-2.0.3/thorpy/loops.py
+-rw-rw-rw-   0        0        0     2639 2023-04-22 15:23:24.000000 thorpy-2.0.3/thorpy/monitoring.py
+-rw-rw-rw-   0        0        0      467 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/parameters.py
+-rw-rw-rw-   0        0        0      625 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/setup.py
+-rw-rw-rw-   0        0        0     3727 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/shadows.py
+-rw-rw-rw-   0        0        0     2540 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/sorting.py
+-rw-rw-rw-   0        0        0     2307 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/sound.py
+-rw-rw-rw-   0        0        0    35577 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/styles.py
+-rw-rw-rw-   0        0        0    32875 2023-04-21 16:56:57.000000 thorpy-2.0.3/thorpy/themes.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:21:54.863260 thorpy-2.0.3/thorpy.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 16:21:54.000000 thorpy-2.0.3/thorpy.egg-info/top_level.txt
```

### Comparing `thorpy-2.0.1/LICENSE` & `thorpy-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/README.md` & `thorpy-2.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 * Set the root for Thorpy in generate_website.py
 * Run generate_website.py
 
 How to update elements :
 * Nothing special to do for the doc description, it is automatic as long as you indicate things in docstrings
 * For the image, put an image with the same name as the class (but lowercase) in the doc folder
 
+Files to upload to server:
+* All things inside to_upload/
+
 Upload on PyPi :
-1. pip install twine setuptools wheel
-2. python setup.py sdist bdist_wheel
-3. twine upload dist/*
+1. Copy paste the actual thorpy folder to ./thorpy/
+2. Change version number in both setup.py AND thorpy/__init__.py
+3. pip install twine setuptools wheel
+4. python setup.py sdist bdist_wheel
+5. twine upload dist/*
 Account : Thorpy
 Pwd : Don't worry
 
 
 ***TODO***
 
 pygame mailing list
 
-lien vers thorpy1 website et github archivés, et dernier message thorpy
-
 
 # versions + tard: ####################################################################
 #TODOs
 #script de tutos auto basé sur les commentaires
 # detecter quels examples figurent pas dans les automatiquement proposes et faire un systeme de tags bijectifs
 #lifebar vertical
 # site : quand on hover un element de code d'example, un encart qui explique ce qu'est l'élément apparait
```

### Comparing `thorpy-2.0.1/thorpy/__init__.py` & `thorpy-2.0.3/thorpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .loops import Loop
 from . import parameters
 from . import graphics
 from . import sound
 from . import shadows
 from .shadows import Shadow
 from . import gametools
+from .monitoring import Monitor
 
 from .canonical import arrow_cursor, hand_cursor
 
 #Import elements classes
 from .elements import Alert, AlertWithChoices, ArrowButton, Box, Button, DropDownList, Image, Line
 from .elements import Slider, SliderWithText, Text, TextInput, TitleBox, ToggleButton, Helper
 from .elements import Checkbox, Radio, SwitchButton, SwitchButtonWithText, DropDownListButton
@@ -23,15 +24,16 @@
 #Import styling functions
 from .themes import theme_classic, theme_human, theme_round, theme_simple, theme_text, theme_game2
 from .themes import theme_round_gradient, theme_round2
 from .themes import theme_text_dark, theme_game1, set_style_attr, refresh_all_elements_style, get_theme_bck_color, get_theme_main_bck_color
 from .styles import get_default_font, set_default_font, get_text_size, get_text_height
 
 
-__version__ = 2.0
+__version__ = "2.0.3"
+
 
 def set_screen(screen):
     """Set the default surface display for all elements that will be created after this call."""
     parameters.screen = screen
 
 def get_screen():
     """Get the default surface display for elements that will be created after this call."""
@@ -67,15 +69,18 @@
     else:
         parameters.waiting_bar = text_or_bar
 
 def refresh_waiting_bar():
     """Function to call each time the waiting bar has to be updated and drawn to the screen."""
     parameters.refresh_waiting_bar()
 
-pause = loops.pause
+def pause():
+    """Pauses the application until user press a key."""
+    loops.pause()
+
 get_current_loop = loops.get_current_loop
 quit_current_loop = loops.quit_current_loop
 quit_all_loops = loops.quit_all_loops
 exit_app = loops.exit_app
 
 module_path = os.path.abspath(__file__)
 module_directory = os.path.dirname(module_path)
```

### Comparing `thorpy-2.0.1/thorpy/canonical.py` & `thorpy-2.0.3/thorpy/canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 it is your responsibility not to modify the rect directly.<br><br>
 
 <b>All the methods presented below can be called on any Thorpy element.</b> They are primarily defined
 in the file canonical.py for the Element class, and maybe redefined for the specialized class
 of your element in elements.py. <br><br>
 
 """
+
 import pygame
 from . import sorting
 from . import shadows
 from . import parameters as p
 from . import loops
 from . import graphics
 import warnings
```

### Comparing `thorpy-2.0.1/thorpy/elements.py` & `thorpy-2.0.3/thorpy/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
                        "hover":self.__class__.style_hover.copy(),
                         "pressed":self.__class__.style_pressed.copy(),
                         "locked":self.__class__.style_locked.copy()}
         if generate_surfaces:
             self.generate_surfaces()
         if sort_immediately:
             self.sort_children()
-            self.center_on(p.screen)
+            # self.center_on(p.screen)
 
     def set_resizable(self, x, y, clip_children=True):
         """Set the box resizable by the user by dragging the corner and/or the borders.
         ***Mandatory arguments***
         <x> : (bool) set resizable along x-axis.
         <y> : (bool) set resizable along y-axis.
         ***Optional arguments***
@@ -420,15 +420,15 @@
             self.scrollbar_x_factor = int(max_to_move / space_allowed) + 1
         else:
             self.scrollbar_y = s
             s.set_topleft(self.rect.right-s.rect.w-sbox_margins[0],
                             self.rect.top+s.dragger.rect.h + sbox_margins[1])
             space_allowed = s.rect.h
             self.scrollbar_y_factor = int(max_to_move / space_allowed) + 1
-        sbox = Box([s],False)
+        sbox = Box([s],sort_immediately=False)
         sbox.add_scrollbar_if_needed = False
 ##        sbox.englobe_children(margins=(3,3), adapt_parent=False)
         sbox.rect.center = s.rect.center
         # rect = s.rect.unionall([b1,b2])
         rect = s.rect
         sbox.set_size(rect.inflate(*sbox_margins).size, adapt_parent=False)
         sbox.ignore_for_sorting = True
@@ -764,15 +764,15 @@
         if self.cursor_pos > len(self.value):
             self.cursor_pos = len(self.value)
         dragged = Button.update(self, mouse_delta)
         if self.it % self.cursor_blinking_mod == 0:
             self.showing_cursor = not(self.showing_cursor)
         return dragged
 
-    def can_add(self): #TODO: utiliser size !
+    def can_add(self): #TODO: use size !
         style = self.get_current_style()
         if self.placeholder and not(self.value):
             if self.placeholder_color is None:
                 self.placeholder_color = TextInput.style_locked.font_color
             text = style.font.render(self.placeholder, True, self.placeholder_color)
         else:
             text = style.font.render(self.value, True, style.font_color)
@@ -1121,19 +1121,19 @@
             if self.slider.dragger.text != text:
                 self.slider.dragger.set_text(text)
                 # self.slider.dragger.adapt_to_text() #need this if size != "auto"
         if self.value_text:
             if self.edit:
                 if text != self.value_text.get_value():
                     self.value_text.value = text
-                    self.sort_children(self.mode, gap=10)
+                    # self.sort_children(self.mode, gap=10)
             else:
                 if text != self.value_text.text:
                     self.value_text.set_text(text)
-                    self.sort_children(self.mode, gap=10)
+                    # self.sort_children(self.mode, gap=10)
         return dragged
     
 
 class Helper(Element):
     """Text that pops when user is hovering another element. Typically used to display hints to the user.
     ***Mandatory arguments***
     <text> argument is the text shown to the user.
@@ -2063,16 +2063,16 @@
         for key in self.styles.keys():
             self.surfaces[key] = s
         self.has_surfaces_generated = True
         self.refresh_surfaces_shadow()
 
 
 class AnimatedGif(Image):
-    """Animated gif that can be used as a GUI element taking all standard element states
-    (normal, hover, pressed, locked) and actions.
+    """Animation that can be used as a GUI element taking all standard element states
+    (normal, hover, pressed, locked) and actions. 
     ***Mandatory arguments***
     <filename> : filename of a gif file. The frames will automatically be extracted to form pygames surfaces.
     You can also directly provide a sequence of pygame surfaces that are all of the same size.
     ***Optional arguments***
     <frame_mod> : number of logics updates between each frame update. Can be seen as the slowness of the animation. Must be at least 1.
     <size_factor> : 2-tuple of positive real values corresponding to the size multiplicator of the original images to produce the actual images.
     <loops> : number of times the animation must be played. Can be any integer or float('inf').
```

### Comparing `thorpy-2.0.1/thorpy/examples/_example_alert.py` & `thorpy-2.0.3/thorpy/examples/_example_alert.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_anim_move.py` & `thorpy-2.0.3/thorpy/examples/_example_anim_move.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_animatedgif.py` & `thorpy-2.0.3/thorpy/examples/_example_animatedgif.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_box.py` & `thorpy-2.0.3/thorpy/examples/_example_box.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_button_helloworld.py` & `thorpy-2.0.3/thorpy/examples/_example_button_helloworld.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_color_gradient.py` & `thorpy-2.0.3/thorpy/examples/_example_color_gradient.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_colorpicker.py` & `thorpy-2.0.3/thorpy/examples/_example_colorpicker.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pygame, thorpy as tp
 
 pygame.init()
 
 screen = pygame.display.set_mode((1200, 700))
 tp.init(screen, tp.theme_simple) #bind screen to gui elements and set theme
 
-#TODO invalid for game1
 e1 = tp.LabelledColorPicker("Google-like", tp.ColorPicker())
 e2 = tp.LabelledColorPicker("RGB style", tp.ColorPickerRGB())
 e3 = tp.LabelledColorPicker("Discrete set", tp.ColorPickerPredefined(auto_cols_steps=4))
 my_colors = [(255,0,0), (255,100,100), (255,200,200), (0,0,255), (0,255,0)]
 e4 = tp.LabelledColorPicker("Predefined", tp.ColorPickerPredefined(my_colors, mode="h")) 
 
 group = tp.Group([e1,e2,e3,e4])
```

### Comparing `thorpy-2.0.1/thorpy/examples/_example_colorpicker2.py` & `thorpy-2.0.3/thorpy/examples/_example_colorpicker2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_colorpicker_fine_tuning.py` & `thorpy-2.0.3/thorpy/examples/_example_colorpicker_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_create_style.py` & `thorpy-2.0.3/thorpy/examples/_example_create_style.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_create_style2.py` & `thorpy-2.0.3/thorpy/examples/_example_create_style2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_custom_theme.py` & `thorpy-2.0.3/thorpy/examples/_example_custom_theme.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_dropdownlist.py` & `thorpy-2.0.3/thorpy/examples/_example_dropdownlist.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_events.py` & `thorpy-2.0.3/thorpy/examples/_example_events.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_filebrowser.py` & `thorpy-2.0.3/thorpy/examples/_example_filebrowser.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_fx_light_emitting_image.py` & `thorpy-2.0.3/thorpy/examples/_example_fx_light_emitting_image.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_fx_lights.py` & `thorpy-2.0.3/thorpy/examples/_example_fx_lights.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_get_value_from_elements.py` & `thorpy-2.0.3/thorpy/examples/_example_get_value_from_elements.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_grouping.py` & `thorpy-2.0.3/thorpy/examples/_example_grouping.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_grouping_without_sorting.py` & `thorpy-2.0.3/thorpy/examples/_example_grouping_without_sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_groups_of_groups.py` & `thorpy-2.0.3/thorpy/examples/_example_groups_of_groups.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_guess_the_number.py` & `thorpy-2.0.3/thorpy/examples/_example_guess_the_number.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_helper.py` & `thorpy-2.0.3/thorpy/examples/_example_helper.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_heterogeneous_texts.py` & `thorpy-2.0.3/thorpy/examples/_example_heterogeneous_texts.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_image_with_text.py` & `thorpy-2.0.3/thorpy/examples/_example_image_with_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_imagebutton.py` & `thorpy-2.0.3/thorpy/examples/_example_imagebutton.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_integration_in_existing_code.py` & `thorpy-2.0.3/thorpy/examples/_example_integration_in_existing_code.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_labels.py` & `thorpy-2.0.3/thorpy/examples/_example_labels.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_launch.py` & `thorpy-2.0.3/thorpy/examples/_example_launch.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_lifebar.py` & `thorpy-2.0.3/thorpy/examples/_example_lifebar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_look_tune.py` & `thorpy-2.0.3/thorpy/examples/_example_look_tune.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_rich_text.py` & `thorpy-2.0.3/thorpy/examples/_example_rich_text.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_set_default_font.py` & `thorpy-2.0.3/thorpy/examples/_example_set_default_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_shadows.py` & `thorpy-2.0.3/thorpy/examples/_example_shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_showcase_themes.py` & `thorpy-2.0.3/thorpy/examples/_example_showcase_themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_showcase_themes2.py` & `thorpy-2.0.3/thorpy/examples/_example_showcase_themes2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_showcase_themes_buttons.py` & `thorpy-2.0.3/thorpy/examples/_example_showcase_themes_buttons.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_showfps.py` & `thorpy-2.0.3/thorpy/examples/_example_showfps.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_slider.py` & `thorpy-2.0.3/thorpy/examples/_example_slider.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_text_input.py` & `thorpy-2.0.3/thorpy/examples/_example_text_input.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_text_width.py` & `thorpy-2.0.3/thorpy/examples/_example_text_width.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_togglables_pool.py` & `thorpy-2.0.3/thorpy/examples/_example_togglables_pool.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_user_choices.py` & `thorpy-2.0.3/thorpy/examples/_example_user_choices.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_user_choices2.py` & `thorpy-2.0.3/thorpy/examples/_example_user_choices2.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_user_chooses_font.py` & `thorpy-2.0.3/thorpy/examples/_example_user_chooses_font.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/examples/_example_waiting_bar.py` & `thorpy-2.0.3/thorpy/examples/_example_waiting_bar.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/gametools.py` & `thorpy-2.0.3/thorpy/gametools.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/graphics.py` & `thorpy-2.0.3/thorpy/graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,17 +490,16 @@
         nframes += 1
         try:
             frame.seek( nframes )
         except EOFError:
             break
     return imgs
 
-def draw_arrow(screen, start_coord, end_coord):
+def draw_arrow(screen, start_coord, end_coord, arrow_color):
     """Draws an arrow on the screen from start_coord to end_coord, pointing towards end_coord."""
-    arrow_color = (255,255,0)
     angle = math.atan2(end_coord[1] - start_coord[1], end_coord[0] - start_coord[0])
     # Draw the arrow line
     pygame.draw.aaline(screen, arrow_color, start_coord, end_coord)
     # Draw the arrowhead
     arrowhead_length = 13
     arrowhead_angle = math.pi / 6  # 30 degrees in radians
     arrowhead_points = [
```

### Comparing `thorpy-2.0.1/thorpy/loops.py` & `thorpy-2.0.3/thorpy/loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pygame
 
 from . import parameters as p
 
-def pause(debug_msg="Pause thorpy"):
+def pause(debug_msg="Thorpy pause - press a key to continue"):
     print(debug_msg)
     clock = pygame.time.Clock()
     while True:
+        clock.tick(60)
         for e in pygame.event.get():
             if e.type == pygame.KEYDOWN or e.type == pygame.MOUSEBUTTONDOWN:
                 return
             elif e.type == pygame.QUIT:
                 quit_all_loops()
                 pygame.event.post(pygame.event.Event(pygame.QUIT))
                 return
```

### Comparing `thorpy-2.0.1/thorpy/monitoring.py` & `thorpy-2.0.3/thorpy/monitoring.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,27 +11,55 @@
             getattr(self,name).append(time.perf_counter())
 
     def reset(self):
         for letter in "abcdefghijklmnopqrstuvwxyz":
                 if hasattr(self,letter):
                     setattr(self, letter, [])
 
+    def autocomplete(self):
+        lengths = []
+        lengths_dict = {}
+        all_letters = self.list_letters()
+        for letter in all_letters:
+            n = len(getattr(self,letter))
+            lengths.append(n)
+            lengths_dict[letter] = n
+        L = max(lengths)
+        for i in range(1,len(all_letters)):
+            letter = all_letters[i]
+            letter_prev = all_letters[i-1]
+            n = lengths_dict[letter]
+            if n < L:
+                for i in range(n, L):
+                    time_prev_letter = getattr(self, letter_prev)[i]
+                    getattr(self,letter).append(time_prev_letter)
+
+    def list_letters(self):
+        letters = []
+        for letter in "abcdefghijklmnopqrstuvwxyz":
+            if hasattr(self,letter):
+                letters.append(letter)
+        return letters
+
     def show(self, letters=None, rnd=None):
         if not letters:
-            letters = []
-            for letter in "abcdefghijklmnopqrstuvwxyz":
-                if hasattr(self,letter):
-                    letters.append(letter)
+            letters = self.list_letters()
         n_lett = len(letters)
         tot = [0.]*n_lett
         L = len(getattr(self,letters[0]))
         print("Stats over", L, "iterations:")
         for i in range(1,n_lett):
             for k in range(L): #k is the iteration
-                diff = getattr(self,letters[i])[k] - getattr(self,letters[i-1])[k]
+                letter_i = getattr(self,letters[i])
+                letter_j = getattr(self,letters[i-1])
+                if len(letter_i) <= k:
+                    raise Exception("Letter "+str(letters[i])+" not called each frame")
+                if len(letter_j) <= k:
+                    raise Exception("Letter "+str(letters[i-1])+" not called each frame")
+                diff = letter_i[k] - letter_j[k]
                 tot[i] += diff
         for k in range(1,L): #z->a_previous_iteration
             diff = getattr(self,letters[0])[k] - getattr(self,letters[n_lett-1])[k-1]
             tot[0] += diff
         for i in list(range(1,len(tot)))+[0]: #we want z->a displayed at the end
             if rnd is None:
                 n = tot[i]
```

### Comparing `thorpy-2.0.1/thorpy/setup.py` & `thorpy-2.0.3/thorpy/setup.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/shadows.py` & `thorpy-2.0.3/thorpy/shadows.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/sorting.py` & `thorpy-2.0.3/thorpy/sorting.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/sound.py` & `thorpy-2.0.3/thorpy/sound.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/styles.py` & `thorpy-2.0.3/thorpy/styles.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy/themes.py` & `thorpy-2.0.3/thorpy/themes.py`

 * *Files identical despite different names*

### Comparing `thorpy-2.0.1/thorpy.egg-info/SOURCES.txt` & `thorpy-2.0.3/thorpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


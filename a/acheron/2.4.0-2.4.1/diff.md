# Comparing `tmp/acheron-2.4.0.tar.gz` & `tmp/acheron-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acheron-2.4.0.tar", last modified: Thu Mar 30 20:14:16 2023, max compression
+gzip compressed data, was "dist/acheron-2.4.1.tar", last modified: Mon Apr 24 18:58:38 2023, max compression
```

## Comparing `acheron-2.4.0.tar` & `acheron-2.4.1.tar`

### file list

```diff
@@ -1,387 +1,387 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-03-30 20:14:01.000000 acheron-2.4.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/install_extras/
--rw-rw-rw-   0 root         (0) root         (0)    12238 2023-03-30 20:14:01.000000 acheron-2.4.0/install_extras/acheron.bmp
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-03-30 20:14:01.000000 acheron-2.4.0/install_extras/acheron_64bit.iss
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron.code-workspace
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-03-30 20:14:01.000000 acheron-2.4.0/extra_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-03-30 20:14:01.000000 acheron-2.4.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-03-30 20:14:16.000000 acheron-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-03-30 20:14:01.000000 acheron-2.4.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-30 20:14:01.000000 acheron-2.4.0/cx_shim_run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-03-30 20:14:01.000000 acheron-2.4.0/.vscode/launch.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14289 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-30 20:14:01.000000 acheron-2.4.0/cx_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-03-30 20:14:01.000000 acheron-2.4.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2349 2023-03-30 20:14:01.000000 acheron-2.4.0/update_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2023-03-30 20:14:01.000000 acheron-2.4.0/cx_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-03-30 20:14:01.000000 acheron-2.4.0/update_qrc.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2023-03-30 20:14:01.000000 acheron-2.4.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/
--rw-rw-rw-   0 root         (0) root         (0)     5072 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/edit_alert_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     4681 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_edit_alert_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rf_test_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1884 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_ctrl_var_panel.py
--rw-rw-rw-   0 root         (0) root         (0)    12575 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_rf_test_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    93247 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/device_tab.py
--rw-rw-rw-   0 root         (0) root         (0)     7225 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/bulk_update_firmware.ui
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/32x32/
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/application.png
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/about.png
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/tag.png
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/branch.png
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/install.png
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)     2685 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)     1844 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)     1730 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/exit.png
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)     1719 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/gear.png
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/redo.png
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)     2450 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)     1901 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/copy.png
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)     1553 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/information.png
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)     1608 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/32x32/bomb.png
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/index.theme
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/48x48/
--rw-rw-rw-   0 root         (0) root         (0)     3649 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)     3525 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/application.png
--rw-rw-rw-   0 root         (0) root         (0)     4092 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/about.png
--rw-rw-rw-   0 root         (0) root         (0)     3968 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/tag.png
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/branch.png
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/install.png
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)     2142 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)     1433 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)     3120 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)     2383 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)     3369 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)     3164 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)     3180 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/exit.png
--rw-rw-rw-   0 root         (0) root         (0)     3242 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)     4230 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)     4297 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)     2806 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/gear.png
--rw-rw-rw-   0 root         (0) root         (0)     3180 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/redo.png
--rw-rw-rw-   0 root         (0) root         (0)     3389 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)     3138 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     2828 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/copy.png
--rw-rw-rw-   0 root         (0) root         (0)     4118 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)     2494 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)     3726 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)     3161 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/information.png
--rw-rw-rw-   0 root         (0) root         (0)     4338 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)     3961 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)     2641 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/48x48/bomb.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/256x256/
--rw-rw-rw-   0 root         (0) root         (0)    34948 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)    34065 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/application.png
--rw-rw-rw-   0 root         (0) root         (0)    39902 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/about.png
--rw-rw-rw-   0 root         (0) root         (0)    38571 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/tag.png
--rw-rw-rw-   0 root         (0) root         (0)    16709 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/branch.png
--rw-rw-rw-   0 root         (0) root         (0)    59410 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/install.png
--rw-rw-rw-   0 root         (0) root         (0)    26485 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)    31049 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)    22246 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)    27340 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)    12013 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)    32160 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)    67911 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)     8904 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)    31839 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)    18879 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)    35568 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)    38710 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)    22970 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)    32524 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)    40777 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)    30156 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/exit.png
--rw-rw-rw-   0 root         (0) root         (0)    34949 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)    46617 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)    63471 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)    45702 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)    30681 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)    30127 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)    65286 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/gear.png
--rw-rw-rw-   0 root         (0) root         (0)    30075 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/redo.png
--rw-rw-rw-   0 root         (0) root         (0)    37435 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)    37760 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)    24176 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/delete.png
--rw-rw-rw-   0 root         (0) root         (0)    36259 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)    37969 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/copy.png
--rw-rw-rw-   0 root         (0) root         (0)    39078 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)    22392 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)    38228 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)    32406 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)    49748 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/information.png
--rw-rw-rw-   0 root         (0) root         (0)    46304 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)    26939 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)    42896 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)    25109 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/256x256/bomb.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/16x16/
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/application.png
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/about.png
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/tag.png
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/branch.png
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/install.png
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)      739 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/exit.png
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/gear.png
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/redo.png
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)      796 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/delete.png
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/copy.png
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)      733 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/information.png
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/16x16/bomb.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/64x64/
--rw-rw-rw-   0 root         (0) root         (0)     5293 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)     5288 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/application.png
--rw-rw-rw-   0 root         (0) root         (0)     6011 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/about.png
--rw-rw-rw-   0 root         (0) root         (0)     5918 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/tag.png
--rw-rw-rw-   0 root         (0) root         (0)     1864 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/branch.png
--rw-rw-rw-   0 root         (0) root         (0)     8225 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/install.png
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)     4808 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)     4311 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)     8111 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)     4610 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)     3970 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)     4483 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)     5162 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)     4865 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)     4648 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/exit.png
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)     6283 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)     6852 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)     7666 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/gear.png
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/redo.png
--rw-rw-rw-   0 root         (0) root         (0)     5430 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)     6364 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)     4797 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/copy.png
--rw-rw-rw-   0 root         (0) root         (0)     5946 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)     3730 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)     5574 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)     4698 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)     6789 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/information.png
--rw-rw-rw-   0 root         (0) root         (0)     6913 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)     6079 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)     3726 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/64x64/bomb.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/icons/suprock/24x24/
--rw-rw-rw-   0 root         (0) root         (0)     1397 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/folder_up.png
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/application.png
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/about.png
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/tag.png
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/branch.png
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/install.png
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/flash_yellow.png
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/sign_warning.png
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/shaker.png
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/antenna_stop.png
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/text_list_numbers.png
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/branch_view.png
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/cpu_flash.png
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/document_plain.png
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/media_pause.png
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/branch_element_new.png
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/wrench.png
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/plug_usb.png
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/media_play_green.png
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/stethoscope.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/exit.png
--rw-rw-rw-   0 root         (0) root         (0)     1186 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/document_gear.png
--rw-rw-rw-   0 root         (0) root         (0)     1382 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/client_network.png
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/earth_network.png
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/caliper.png
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/signal_flag_white.png
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/signal_flag_red.png
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/gear.png
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/redo.png
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/antenna_play.png
--rw-rw-rw-   0 root         (0) root         (0)     1610 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/replace2.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/document_up.png
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/copy.png
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/symbol_hash.png
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/antenna.png
--rw-rw-rw-   0 root         (0) root         (0)     1497 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/preferences_edit.png
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/plug_lan.png
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/information.png
--rw-rw-rw-   0 root         (0) root         (0)     1440 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/chart_column.png
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/rf_test.png
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/cloud_computing_download.png
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/icons/suprock/24x24/bomb.png
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_about.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/calibration_panel.ui
--rw-rw-rw-   0 root         (0) root         (0)    12689 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/preferences.py
--rw-rw-rw-   0 root         (0) root         (0)    53912 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/radio_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     7103 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/bootloader.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/connect_tcp_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/tcp_scan_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)    12205 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_calibration_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_rf_power_panel.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ctrl_var_widget.ui
--rw-rw-rw-   0 root         (0) root         (0)     6259 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_download_firmware_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/about.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_led_control_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     9225 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/calibration_channel.ui
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/change_stream_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5982 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    33748 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/device_tab.ui
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/detail_scan_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     3266 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/bulk_update_firmware.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/connect_tcp_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rf_power_panel.ui
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 20:14:16.000000 acheron-2.4.0/acheron/html/
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/html/asphodel_channels.html
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/remote_panel.ui
--rw-rw-rw-   0 root         (0) root         (0)     2300 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_hardware_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/led_control_widget.ui
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/setting_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3099 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ctrl_var_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rf_power_panel.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/remote_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     2124 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_setting_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7901 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_bulk_update_firmware.py
--rw-rw-rw-   0 root         (0) root         (0)    10013 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/hardware_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/about.ui
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/edit_alert_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/radio_panel.ui
--rw-rw-rw-   0 root         (0) root         (0)    33823 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_device_tab.py
--rw-rw-rw-   0 root         (0) root         (0)    21471 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/acheron.qrc
--rw-rw-rw-   0 root         (0) root         (0)    15898 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rf_test_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)    27989 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_preferences.py
--rw-rw-rw-   0 root         (0) root         (0)    51300 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/plotmain.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/led_control_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-03-30 20:14:15.000000 acheron-2.4.0/acheron/version.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11047 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/connectivity_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_info_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)   108424 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/acheron.ico
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_change_stream_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5871 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/download_firmware_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2935 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/download_firmware_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    10673 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rgb_control_widget.ui
--rw-rw-rw-   0 root         (0) root         (0)    11824 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/detail_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/info_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/update_func_limiter.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_calibration_panel.py
--rw-rw-rw-   0 root         (0) root         (0)    21509 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/info_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     9425 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_rgb_control_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/rgb_control_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/setting_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     3866 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_connect_tcp_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    11748 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/plotmain.ui
--rw-rw-rw-   0 root         (0) root         (0)     6172 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_radio_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/hardware_tests.ui
--rw-rw-rw-   0 root         (0) root         (0)     6093 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_detail_scan_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)  6701217 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/acheron_rc.py
--rw-rw-rw-   0 root         (0) root         (0)    43429 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/change_stream_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)     5639 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_tcp_scan_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5463 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/connectivity_dialog.ui
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ctrl_var_panel.ui
--rw-rw-rw-   0 root         (0) root         (0)     2006 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_remote_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_connectivity_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    33567 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/preferences.ui
--rw-rw-rw-   0 root         (0) root         (0)    15592 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_plotmain.py
--rw-rw-rw-   0 root         (0) root         (0)     8273 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/tcp_scan_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ctrl_var_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-30 20:14:01.000000 acheron-2.4.0/acheron/ui_ctrl_var_widget.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-30 20:14:16.000000 acheron-2.4.0/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-24 18:58:25.000000 acheron-2.4.1/cx_shim_run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ctrl_var_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/tcp_scan_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)     5639 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_tcp_scan_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3866 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_connect_tcp_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rf_test_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    12205 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_calibration_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)    21509 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/info_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    33748 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/device_tab.ui
+-rw-rw-rw-   0 root         (0) root         (0)     9225 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/calibration_channel.ui
+-rw-rw-rw-   0 root         (0) root         (0)    51300 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/plotmain.py
+-rw-rw-rw-   0 root         (0) root         (0)    10673 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rgb_control_widget.ui
+-rw-rw-rw-   0 root         (0) root         (0)     8273 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/tcp_scan_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/edit_alert_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/hardware_tests.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/led_control_widget.ui
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_setting_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    33567 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/preferences.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/info_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)    43429 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/update_func_limiter.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ctrl_var_panel.ui
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_connectivity_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_remote_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6093 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_detail_scan_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/about.ui
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_about.py
+-rw-rw-rw-   0 root         (0) root         (0)    12689 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ctrl_var_widget.ui
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/download_firmware_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/connect_tcp_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7901 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_bulk_update_firmware.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_change_stream_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    11824 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/detail_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/detail_scan_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)     6259 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_download_firmware_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ctrl_var_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_rf_power_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)    27989 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     1884 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_ctrl_var_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)    12575 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_rf_test_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9425 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_rgb_control_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rgb_control_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5982 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/remote_panel.ui
+-rw-rw-rw-   0 root         (0) root         (0)     7225 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/bulk_update_firmware.ui
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/setting_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)   108424 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/acheron.ico
+-rw-rw-rw-   0 root         (0) root         (0)    33823 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_device_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_info_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/remote_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7103 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/bootloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/connect_tcp_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_calibration_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/setting_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/change_stream_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)    15592 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_plotmain.py
+-rw-rw-rw-   0 root         (0) root         (0)    93247 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/device_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/change_stream_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/connectivity_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)    10013 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/hardware_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/bulk_update_firmware.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11047 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/connectivity_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/led_control_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/radio_panel.ui
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_radio_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     5072 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/edit_alert_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/calibration_panel.ui
+-rw-rw-rw-   0 root         (0) root         (0)     4681 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_edit_alert_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/about.py
+-rw-rw-rw-   0 root         (0) root         (0)    21471 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/acheron.qrc
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/html/
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/html/asphodel_channels.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/48x48/
+-rw-rw-rw-   0 root         (0) root         (0)     1433 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)     4297 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/install.png
+-rw-rw-rw-   0 root         (0) root         (0)     2828 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3389 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     3649 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)     3968 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)     3525 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/application.png
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/information.png
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)     3161 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/about.png
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     2641 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)     4338 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/48x48/media_pause.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/64x64/
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)     6852 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     8225 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/install.png
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     5430 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     5293 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     7666 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     5946 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)     5918 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)     5288 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/application.png
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     6364 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)     4797 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)     4311 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)     5162 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     5574 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)     4865 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)     4610 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)     6789 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/information.png
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)     4483 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)     6011 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/about.png
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)     6913 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/64x64/media_pause.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/32x32/
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)     1553 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/install.png
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/application.png
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/information.png
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/about.png
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/32x32/media_pause.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/24x24/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/install.png
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)     1397 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/application.png
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/information.png
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/about.png
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/24x24/media_pause.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/256x256/
+-rw-rw-rw-   0 root         (0) root         (0)     8904 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)    22392 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)    26485 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)    63471 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)    59410 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/install.png
+-rw-rw-rw-   0 root         (0) root         (0)    36259 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)    37435 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)    12013 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)    46617 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)    34948 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)    65286 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)    39078 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)    31049 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)    16709 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)    26939 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)    38571 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)    34065 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/application.png
+-rw-rw-rw-   0 root         (0) root         (0)    22246 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)    30075 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)    24176 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)    37760 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)    37969 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)    34949 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)    35568 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)    27340 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)    42896 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)    32524 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)    38228 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)    22970 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)    40777 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)    30156 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)    31839 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)    49748 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/information.png
+-rw-rw-rw-   0 root         (0) root         (0)    67911 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)    38710 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)    30681 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)    32406 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)    39902 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/about.png
+-rw-rw-rw-   0 root         (0) root         (0)    32160 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    30127 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)    25109 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)    45702 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)    46304 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)    18879 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/256x256/media_pause.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron/icons/suprock/16x16/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/document_plain.png
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/antenna.png
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/flash_yellow.png
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/earth_network.png
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/install.png
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/document_up.png
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/antenna_play.png
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/text_list_numbers.png
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/client_network.png
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/folder_up.png
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/gear.png
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/symbol_hash.png
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/sign_warning.png
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/rf_test.png
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/tag.png
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/application.png
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/shaker.png
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/redo.png
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/replace2.png
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/document_gear.png
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/branch_element_new.png
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/antenna_stop.png
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/cloud_computing_download.png
+-rw-rw-rw-   0 root         (0) root         (0)      739 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/media_play_green.png
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/preferences_edit.png
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/plug_usb.png
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/stethoscope.png
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/exit.png
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/information.png
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/cpu_flash.png
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/wrench.png
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/signal_flag_white.png
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/plug_lan.png
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/about.png
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/branch_view.png
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/signal_flag_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/bomb.png
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/caliper.png
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/chart_column.png
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/16x16/media_pause.png
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/icons/suprock/index.theme
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_hardware_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)  6701217 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/acheron_rc.py
+-rw-rw-rw-   0 root         (0) root         (0)    11748 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/plotmain.ui
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_ctrl_var_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5871 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/download_firmware_dialog.ui
+-rw-rw-rw-   0 root         (0) root         (0)    53912 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/radio_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rf_power_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/ui_led_control_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rf_power_panel.ui
+-rw-rw-rw-   0 root         (0) root         (0)    15898 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron/rf_test_dialog.ui
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)    14289 2023-04-24 18:58:38.000000 acheron-2.4.1/acheron.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-04-24 18:58:37.000000 acheron-2.4.1/acheron.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-24 18:58:25.000000 acheron-2.4.1/extra_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-24 18:58:25.000000 acheron-2.4.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-24 18:58:38.000000 acheron-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-24 18:58:25.000000 acheron-2.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-24 18:58:25.000000 acheron-2.4.1/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/install_extras/
+-rw-rw-rw-   0 root         (0) root         (0)    12238 2023-04-24 18:58:25.000000 acheron-2.4.1/install_extras/acheron.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2023-04-24 18:58:25.000000 acheron-2.4.1/install_extras/acheron_64bit.iss
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-24 18:58:25.000000 acheron-2.4.1/cx_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-04-24 18:58:25.000000 acheron-2.4.1/acheron.code-workspace
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-04-24 18:58:25.000000 acheron-2.4.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2023-04-24 18:58:25.000000 acheron-2.4.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-04-24 18:58:25.000000 acheron-2.4.1/update_ui.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:58:38.000000 acheron-2.4.1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-04-24 18:58:25.000000 acheron-2.4.1/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-04-24 18:58:38.000000 acheron-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-24 18:58:25.000000 acheron-2.4.1/update_qrc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2023-04-24 18:58:25.000000 acheron-2.4.1/cx_setup.py
```

### Comparing `acheron-2.4.0/install_extras/acheron.bmp` & `acheron-2.4.1/install_extras/acheron.bmp`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/install_extras/acheron_64bit.iss` & `acheron-2.4.1/install_extras/acheron_64bit.iss`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 [InstallDelete]
 ; Remove library files from the last installation; this is the easiest way to allow deletions
 Type: filesandordirs; Name: "{app}\botodata"
 Type: filesandordirs; Name: "{app}\imageformats"
 Type: filesandordirs; Name: "{app}\lib"
 Type: filesandordirs; Name: "{app}\platforms"
 Type: filesandordirs; Name: "{app}\styles"
+Type: files; Name: "{app}\qt.conf"
 
 ; Remove the old style start menu group in favor of the new top level shortcut
 Type: filesandordirs; Name: "{group}"
 
 [Files]
 Source: "*"; DestDir: "{app}"; Excludes: "\*.iss,\*.ico,\*.bmp,\Output,lib\hyperborea\7zip_*,lib\asphodel\lib*"; Flags: recursesubdirs ignoreversion
 Source: "acheron.exe"; DestDir: "{app}"; DestName: "acheron-device.exe"; Flags: ignoreversion
@@ -62,14 +63,14 @@
   begin
     if ExpandConstant('{param:DeleteInstaller|No}') = 'Yes' then
     begin
       strContent := ':try_delete' + #13 + #10 +
             'del "' + ExpandConstant('{srcexe}') + '"' + #13 + #10 +
             'if exist "' + ExpandConstant('{srcexe}') + '" goto try_delete' + #13 + #10 +
             'del %0';
-  
+
       strSelf_Delete_BAT := ExtractFilePath(ExpandConstant('{tmp}')) + 'SelfDelete.bat';
       SaveStringToFile(strSelf_Delete_BAT, strContent, False);
       Exec(strSelf_Delete_BAT, '', '', SW_HIDE, ewNoWait, intErrorCode);
     end;
   end;
 end;
```

### Comparing `acheron-2.4.0/PKG-INFO` & `acheron-2.4.1/acheron.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acheron
-Version: 2.4.0
+Version: 2.4.1
 Summary: Plotting and recording program for Asphodel devices
 Home-page: https://bitbucket.org/suprocktech/acheron
 Author: Suprock Technologies, LLC
 Author-email: inquiries@suprocktech.com
 License: UNKNOWN
 Keywords: asphodel suprock apd
 Platform: UNKNOWN
```

### Comparing `acheron-2.4.0/LICENSE.txt` & `acheron-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron.egg-info/PKG-INFO` & `acheron-2.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acheron
-Version: 2.4.0
+Version: 2.4.1
 Summary: Plotting and recording program for Asphodel devices
 Home-page: https://bitbucket.org/suprocktech/acheron
 Author: Suprock Technologies, LLC
 Author-email: inquiries@suprocktech.com
 License: UNKNOWN
 Keywords: asphodel suprock apd
 Platform: UNKNOWN
```

### Comparing `acheron-2.4.0/acheron.egg-info/SOURCES.txt` & `acheron-2.4.1/acheron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/update_ui.py` & `acheron-2.4.1/update_ui.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/cx_setup.py` & `acheron-2.4.1/cx_setup.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/update_qrc.py` & `acheron-2.4.1/update_qrc.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/setup.py` & `acheron-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/edit_alert_dialog.ui` & `acheron-2.4.1/acheron/edit_alert_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_edit_alert_dialog.py` & `acheron-2.4.1/acheron/ui_edit_alert_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rf_test_dialog.py` & `acheron-2.4.1/acheron/rf_test_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_ctrl_var_panel.py` & `acheron-2.4.1/acheron/ui_ctrl_var_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_rf_test_dialog.py` & `acheron-2.4.1/acheron/ui_rf_test_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/device_tab.py` & `acheron-2.4.1/acheron/device_tab.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/bulk_update_firmware.ui` & `acheron-2.4.1/acheron/bulk_update_firmware.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/application.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/about.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/tag.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/branch.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/branch.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/install.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/document_plain.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/document_plain.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/media_pause.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/media_pause.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/exit.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/client_network.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/client_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/gear.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/redo.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/delete.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/copy.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/information.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/32x32/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/32x32/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/application.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/about.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/tag.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/branch.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/branch.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/install.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/document_plain.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/document_plain.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/media_pause.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/media_pause.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/exit.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/client_network.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/client_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/gear.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/redo.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/delete.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/copy.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/information.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/48x48/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/48x48/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/application.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/about.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/tag.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/branch.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/branch.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/install.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/document_plain.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/document_plain.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/media_pause.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/media_pause.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/exit.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/client_network.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/client_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/gear.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/redo.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/delete.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/copy.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/information.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/256x256/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/256x256/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/application.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/about.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/tag.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/install.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/exit.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/gear.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/redo.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/delete.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/copy.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/information.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/16x16/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/16x16/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/application.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/about.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/tag.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/branch.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/branch.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/install.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/document_plain.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/document_plain.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/media_pause.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/media_pause.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/exit.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/client_network.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/client_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/gear.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/redo.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/delete.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/copy.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/information.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/64x64/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/64x64/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/folder_up.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/folder_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/application.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/application.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/about.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/about.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/tag.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/tag.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/branch.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/branch.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/install.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/install.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/flash_yellow.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/flash_yellow.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/sign_warning.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/sign_warning.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/shaker.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/shaker.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/antenna_stop.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/antenna_stop.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/text_list_numbers.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/text_list_numbers.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/branch_view.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/branch_view.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/cpu_flash.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/cpu_flash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/document_plain.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/document_plain.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/preferences.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/preferences.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/media_pause.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/media_pause.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/branch_element_new.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/branch_element_new.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/wrench.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/wrench.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/plug_usb.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/plug_usb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/media_play_green.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/media_play_green.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/stethoscope.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/stethoscope.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/exit.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/exit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/document_gear.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/document_gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/client_network.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/client_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/earth_network.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/earth_network.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/caliper.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/caliper.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/signal_flag_white.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/signal_flag_white.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/signal_flag_red.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/signal_flag_red.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/gear.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/gear.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/redo.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/redo.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/antenna_play.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/antenna_play.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/replace2.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/replace2.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/delete.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/delete.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/document_up.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/document_up.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/copy.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/copy.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/symbol_hash.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/symbol_hash.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/antenna.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/antenna.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/preferences_edit.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/preferences_edit.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/plug_lan.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/plug_lan.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/information.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/information.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/chart_column.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/chart_column.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/rf_test.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/rf_test.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/cloud_computing_download.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/cloud_computing_download.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/icons/suprock/24x24/bomb.png` & `acheron-2.4.1/acheron/icons/suprock/24x24/bomb.png`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_about.py` & `acheron-2.4.1/acheron/ui_about.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/calibration_panel.ui` & `acheron-2.4.1/acheron/calibration_panel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/preferences.py` & `acheron-2.4.1/acheron/preferences.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/radio_panel.py` & `acheron-2.4.1/acheron/radio_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/bootloader.py` & `acheron-2.4.1/acheron/bootloader.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/connect_tcp_dialog.ui` & `acheron-2.4.1/acheron/connect_tcp_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/tcp_scan_dialog.ui` & `acheron-2.4.1/acheron/tcp_scan_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_calibration_channel.py` & `acheron-2.4.1/acheron/ui_calibration_channel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_rf_power_panel.py` & `acheron-2.4.1/acheron/ui_rf_power_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ctrl_var_widget.ui` & `acheron-2.4.1/acheron/ctrl_var_widget.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_download_firmware_dialog.py` & `acheron-2.4.1/acheron/ui_download_firmware_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/about.py` & `acheron-2.4.1/acheron/about.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_led_control_widget.py` & `acheron-2.4.1/acheron/ui_led_control_widget.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/calibration_channel.ui` & `acheron-2.4.1/acheron/calibration_channel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/change_stream_dialog.py` & `acheron-2.4.1/acheron/change_stream_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/__main__.py` & `acheron-2.4.1/acheron/__main__.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/device_tab.ui` & `acheron-2.4.1/acheron/device_tab.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/detail_scan_dialog.ui` & `acheron-2.4.1/acheron/detail_scan_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/bulk_update_firmware.py` & `acheron-2.4.1/acheron/bulk_update_firmware.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/connect_tcp_dialog.py` & `acheron-2.4.1/acheron/connect_tcp_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rf_power_panel.ui` & `acheron-2.4.1/acheron/rf_power_panel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/html/asphodel_channels.html` & `acheron-2.4.1/acheron/html/asphodel_channels.html`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/remote_panel.ui` & `acheron-2.4.1/acheron/remote_panel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_hardware_tests.py` & `acheron-2.4.1/acheron/ui_hardware_tests.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/led_control_widget.ui` & `acheron-2.4.1/acheron/led_control_widget.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/setting_dialog.py` & `acheron-2.4.1/acheron/setting_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ctrl_var_widget.py` & `acheron-2.4.1/acheron/ctrl_var_widget.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rf_power_panel.py` & `acheron-2.4.1/acheron/rf_power_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/remote_panel.py` & `acheron-2.4.1/acheron/remote_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_setting_dialog.py` & `acheron-2.4.1/acheron/ui_setting_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_bulk_update_firmware.py` & `acheron-2.4.1/acheron/ui_bulk_update_firmware.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/hardware_tests.py` & `acheron-2.4.1/acheron/hardware_tests.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/about.ui` & `acheron-2.4.1/acheron/about.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/edit_alert_dialog.py` & `acheron-2.4.1/acheron/edit_alert_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/radio_panel.ui` & `acheron-2.4.1/acheron/radio_panel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_device_tab.py` & `acheron-2.4.1/acheron/ui_device_tab.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/acheron.qrc` & `acheron-2.4.1/acheron/acheron.qrc`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rf_test_dialog.ui` & `acheron-2.4.1/acheron/rf_test_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_preferences.py` & `acheron-2.4.1/acheron/ui_preferences.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/plotmain.py` & `acheron-2.4.1/acheron/plotmain.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/led_control_widget.py` & `acheron-2.4.1/acheron/led_control_widget.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/connectivity_dialog.py` & `acheron-2.4.1/acheron/connectivity_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_info_dialog.py` & `acheron-2.4.1/acheron/ui_info_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/acheron.ico` & `acheron-2.4.1/acheron/acheron.ico`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_change_stream_dialog.py` & `acheron-2.4.1/acheron/ui_change_stream_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/download_firmware_dialog.ui` & `acheron-2.4.1/acheron/download_firmware_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/calibration.py` & `acheron-2.4.1/acheron/calibration.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/download_firmware_dialog.py` & `acheron-2.4.1/acheron/download_firmware_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rgb_control_widget.ui` & `acheron-2.4.1/acheron/rgb_control_widget.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/detail_scan.py` & `acheron-2.4.1/acheron/detail_scan.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/info_dialog.ui` & `acheron-2.4.1/acheron/info_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/update_func_limiter.py` & `acheron-2.4.1/acheron/update_func_limiter.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_calibration_panel.py` & `acheron-2.4.1/acheron/ui_calibration_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/info_dialog.py` & `acheron-2.4.1/acheron/info_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_rgb_control_widget.py` & `acheron-2.4.1/acheron/ui_rgb_control_widget.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/rgb_control_widget.py` & `acheron-2.4.1/acheron/rgb_control_widget.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/setting_dialog.ui` & `acheron-2.4.1/acheron/setting_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_connect_tcp_dialog.py` & `acheron-2.4.1/acheron/ui_connect_tcp_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/plotmain.ui` & `acheron-2.4.1/acheron/plotmain.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_radio_panel.py` & `acheron-2.4.1/acheron/ui_radio_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/hardware_tests.ui` & `acheron-2.4.1/acheron/hardware_tests.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_detail_scan_dialog.py` & `acheron-2.4.1/acheron/ui_detail_scan_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/acheron_rc.py` & `acheron-2.4.1/acheron/acheron_rc.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/logo.svg` & `acheron-2.4.1/acheron/logo.svg`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/change_stream_dialog.ui` & `acheron-2.4.1/acheron/change_stream_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_tcp_scan_dialog.py` & `acheron-2.4.1/acheron/ui_tcp_scan_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/connectivity_dialog.ui` & `acheron-2.4.1/acheron/connectivity_dialog.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ctrl_var_panel.ui` & `acheron-2.4.1/acheron/ctrl_var_panel.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_remote_panel.py` & `acheron-2.4.1/acheron/ui_remote_panel.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_connectivity_dialog.py` & `acheron-2.4.1/acheron/ui_connectivity_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/preferences.ui` & `acheron-2.4.1/acheron/preferences.ui`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_plotmain.py` & `acheron-2.4.1/acheron/ui_plotmain.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/tcp_scan_dialog.py` & `acheron-2.4.1/acheron/tcp_scan_dialog.py`

 * *Files identical despite different names*

### Comparing `acheron-2.4.0/acheron/ui_ctrl_var_widget.py` & `acheron-2.4.1/acheron/ui_ctrl_var_widget.py`

 * *Files identical despite different names*


# Comparing `tmp/skyeye-3.4.7.tar.gz` & `tmp/skyeye-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyeye-3.4.7.tar", last modified: Thu Mar 23 03:33:29 2023, max compression
+gzip compressed data, was "skyeye-3.4.8.tar", last modified: Mon Apr 24 06:40:26 2023, max compression
```

## Comparing `skyeye-3.4.7.tar` & `skyeye-3.4.8.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.153096 skyeye-3.4.7/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       36 2023-03-16 09:25:15.000000 skyeye-3.4.7/MANIFEST.in
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-03-23 03:33:29.153317 skyeye-3.4.7/PKG-INFO
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1883 2023-03-16 09:25:15.000000 skyeye-3.4.7/README.md
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      147 2023-03-23 03:33:29.154801 skyeye-3.4.7/setup.cfg
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      920 2022-08-15 03:18:06.000000 skyeye-3.4.7/setup.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:28.880549 skyeye-3.4.7/skyeye/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      209 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3779 2023-03-21 11:13:50.000000 skyeye-3.4.7/skyeye/apk_decompiling.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3546 2023-03-23 02:47:33.000000 skyeye-3.4.7/skyeye/apk_scanner.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2224 2023-03-23 03:33:17.000000 skyeye-3.4.7/skyeye/cli.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:28.909249 skyeye-3.4.7/skyeye/config/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     6148 2023-03-16 09:01:10.000000 skyeye-3.4.7/skyeye/config/.DS_Store
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      110 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/config/__init__.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:28.928324 skyeye-3.4.7/skyeye/config/__pycache__/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      271 2023-01-05 02:48:44.000000 skyeye-3.4.7/skyeye/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      182 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye/config/__pycache__/cli_config.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1288 2023-01-05 02:48:44.000000 skyeye-3.4.7/skyeye/config/__pycache__/config_center.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1278692 2022-08-05 05:33:23.000000 skyeye-3.4.7/skyeye/config/baksmali-2.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       39 2023-03-23 03:33:24.000000 skyeye-3.4.7/skyeye/config/cli_config.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      803 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/config/config_center.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.004839 skyeye-3.4.7/skyeye/config/dex-tools-2.1/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     6148 2023-03-16 05:19:34.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/.DS_Store
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    11562 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/LICENSE.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      341 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/NOTICE.txt
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.006055 skyeye-3.4.7/skyeye/config/dex-tools-2.1/bin/
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     3277 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/bin/dex-tools.bat
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-baksmali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-baksmali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      845 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1371 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      843 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1369 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      847 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1373 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-access.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-access.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      831 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-smali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1357 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-smali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-std-apk.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-std-apk.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      326 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j_invoke.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1321 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j_invoke.sh
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.124702 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   239543 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1153819 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   167761 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1543336 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   374032 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   378662 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    17737 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174246 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   196809 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   237496 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    72149 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    76796 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174252 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   108508 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   104543 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1030064 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3210 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/open-source-license.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    25515 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  3238491 2023-03-16 09:25:15.000000 skyeye-3.4.7/skyeye/config/jd-gui-1.6.6.jar
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.138844 skyeye-3.4.7/skyeye/dto/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      104 2022-12-01 07:36:19.000000 skyeye-3.4.7/skyeye/dto/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      923 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/dto/class_desc_dto.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      592 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/dto/config_dto.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.145169 skyeye-3.4.7/skyeye/parse/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      122 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/parse/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     5107 2023-01-05 03:18:32.000000 skyeye-3.4.7/skyeye/parse/method_block_parser.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3742 2023-01-05 02:59:02.000000 skyeye-3.4.7/skyeye/parse/smali_parser.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1859 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/result_wirter.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:29.151155 skyeye-3.4.7/skyeye/utils/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       58 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/utils/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       85 2022-12-05 03:43:22.000000 skyeye-3.4.7/skyeye/utils/string_util.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      782 2022-12-01 07:00:01.000000 skyeye-3.4.7/skyeye/version_check.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-03-23 03:33:28.889129 skyeye-3.4.7/skyeye.egg-info/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/PKG-INFO
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3620 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/SOURCES.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/dependency_links.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       42 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/entry_points.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       16 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/requires.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        7 2023-03-23 03:33:28.000000 skyeye-3.4.7/skyeye.egg-info/top_level.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-03-16 08:06:34.000000 skyeye-3.4.7/skyeye.egg-info/zip-safe
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.635802 skyeye-3.4.8/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       36 2023-04-12 07:13:48.000000 skyeye-3.4.8/MANIFEST.in
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-04-24 06:40:26.636051 skyeye-3.4.8/PKG-INFO
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1883 2023-04-12 07:13:48.000000 skyeye-3.4.8/README.md
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      147 2023-04-24 06:40:26.637226 skyeye-3.4.8/setup.cfg
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      920 2023-04-12 07:13:48.000000 skyeye-3.4.8/setup.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.355383 skyeye-3.4.8/skyeye/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      209 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3857 2023-04-24 06:37:46.000000 skyeye-3.4.8/skyeye/apk_decompiling.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3546 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/apk_scanner.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2224 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/cli.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.377029 skyeye-3.4.8/skyeye/config/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      110 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/__init__.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.394754 skyeye-3.4.8/skyeye/config/__pycache__/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      271 2023-04-24 06:34:57.000000 skyeye-3.4.8/skyeye/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      182 2023-04-24 06:40:25.000000 skyeye-3.4.8/skyeye/config/__pycache__/cli_config.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1288 2023-04-24 06:34:57.000000 skyeye-3.4.8/skyeye/config/__pycache__/config_center.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1278692 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/baksmali-2.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       39 2023-04-24 06:38:29.000000 skyeye-3.4.8/skyeye/config/cli_config.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      803 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/config_center.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.530876 skyeye-3.4.8/skyeye/config/dex-tools-2.1/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    11562 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/LICENSE.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      341 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/NOTICE.txt
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.532352 skyeye-3.4.8/skyeye/config/dex-tools-2.1/bin/
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     3277 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/bin/dex-tools.bat
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-baksmali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-baksmali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      845 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1371 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      843 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1369 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      847 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1373 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-access.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-access.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      831 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-smali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1357 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-smali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-std-apk.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-std-apk.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      326 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j_invoke.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1321 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j_invoke.sh
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.619886 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   239543 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1153819 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   167761 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1543336 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   374032 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   378662 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    17737 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174246 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   196809 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   237496 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    72149 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    76796 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174252 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   108508 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   104543 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1030064 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3210 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/open-source-license.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    25515 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  3238491 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/config/jd-gui-1.6.6.jar
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.626328 skyeye-3.4.8/skyeye/dto/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      104 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/dto/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      923 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/dto/class_desc_dto.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      592 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/dto/config_dto.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.629938 skyeye-3.4.8/skyeye/parse/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      122 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/parse/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     5107 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/parse/method_block_parser.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3742 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/parse/smali_parser.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1859 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/result_wirter.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.633902 skyeye-3.4.8/skyeye/utils/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       58 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/utils/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       85 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/utils/string_util.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      782 2023-04-12 07:13:48.000000 skyeye-3.4.8/skyeye/version_check.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 06:40:26.365112 skyeye-3.4.8/skyeye.egg-info/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/PKG-INFO
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3558 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/SOURCES.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/dependency_links.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       42 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/entry_points.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       16 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/requires.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        7 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/top_level.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-04-24 06:40:26.000000 skyeye-3.4.8/skyeye.egg-info/zip-safe
```

### Comparing `skyeye-3.4.7/PKG-INFO` & `skyeye-3.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyeye
-Version: 3.4.7
+Version: 3.4.8
 Summary: APK扫描工具
 Home-page: https://github.com/wangshuwen1107/skyeye
 Author: wangshuwen
 Author-email: wnwn7375@outlook.com
 License: MIT
 Keywords: apk scanner
 Description-Content-Type: text/markdown
```

### Comparing `skyeye-3.4.7/README.md` & `skyeye-3.4.8/README.md`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/setup.py` & `skyeye-3.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/apk_decompiling.py` & `skyeye-3.4.8/skyeye/apk_decompiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,31 +37,31 @@
             #删除jar
             delFiles(jarPath)
     print("✅反编译目录->"+outputDirPath)
     openGUI(outputDirPath)
     
 def openGUI(openDirOrFilePath):
     firstClassFilePath = ""
-    if(isEmpty(openDirOrFilePath)):
-        return
-    if not os.path.exists(openDirOrFilePath):
+    # 指定了打开文件&&文件不存在
+    if not isEmpty(openDirOrFilePath) and not os.path.exists(openDirOrFilePath):
         print("❌文件不存在") 
         return
-    if os.path.isfile(openDirOrFilePath) and not openDirOrFilePath.endswith(".class"):
-        print("❌文件不是.class") 
-        return
-    if os.path.isdir(openDirOrFilePath):
+    # if os.path.isfile(openDirOrFilePath) and not openDirOrFilePath.endswith(".class"):
+    #     print("❌文件不是.class") 
+    #     return
+    if not isEmpty(openDirOrFilePath):
+      if os.path.isdir(openDirOrFilePath):
         walk = os.walk(openDirOrFilePath)
         for root,dir_list,file_list in walk:
             if root == openDirOrFilePath:
                 continue
             for file_name in file_list:
                 if file_name.endswith(".class") and  len(firstClassFilePath)==0:
                     firstClassFilePath = os.path.join(root,file_name)
-    else:
+      else:
         firstClassFilePath = openDirOrFilePath              
     current_file_dir = os.path.dirname(__file__)
     guiPath=  os.path.join(current_file_dir,'config/jd-gui-1.6.6.jar')
     command = None
     if(isEmpty(firstClassFilePath)):
         command ="java -jar "+guiPath
         print("✅正在打开JD-GUI")
```

### Comparing `skyeye-3.4.7/skyeye/apk_scanner.py` & `skyeye-3.4.8/skyeye/apk_scanner.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/cli.py` & `skyeye-3.4.8/skyeye/cli.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/__pycache__/config_center.cpython-310.pyc` & `skyeye-3.4.8/skyeye/config/__pycache__/config_center.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Dec  5 03:43:22 2022 UTC, .py size: 803 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 da68 8d63 2303 0000  o........h.c#...
+00000000: 6f0d 0d0a 0000 0000 2c5a 3664 2303 0000  o.......,Z6d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 5400 6400  d.l.Z.d.d.l.T.d.
 00000040: 6401 6c02 5a02 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 8302 5a03 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da01 2a63 0000 0000 0000 0000 0000  )...*c..........
 00000070: 0000 0000 0000 0300 0000 4000 0000 7338  ..........@...s8
```

### Comparing `skyeye-3.4.7/skyeye/config/baksmali-2.5.2.jar` & `skyeye-3.4.8/skyeye/config/baksmali-2.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/config_center.py` & `skyeye-3.4.8/skyeye/config/config_center.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/LICENSE.txt` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/bin/dex-tools.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/bin/dex-tools.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-baksmali.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-baksmali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-baksmali.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-baksmali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-access.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-access.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-access.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-access.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-smali.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-smali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-smali.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-smali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-std-apk.bat` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-std-apk.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j-std-apk.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j-std-apk.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/d2j_invoke.sh` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/d2j_invoke.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/open-source-license.txt` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/open-source-license.txt`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar` & `skyeye-3.4.8/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/config/jd-gui-1.6.6.jar` & `skyeye-3.4.8/skyeye/config/jd-gui-1.6.6.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/dto/class_desc_dto.py` & `skyeye-3.4.8/skyeye/dto/class_desc_dto.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/dto/config_dto.py` & `skyeye-3.4.8/skyeye/dto/config_dto.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/parse/method_block_parser.py` & `skyeye-3.4.8/skyeye/parse/method_block_parser.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/parse/smali_parser.py` & `skyeye-3.4.8/skyeye/parse/smali_parser.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/result_wirter.py` & `skyeye-3.4.8/skyeye/result_wirter.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye/version_check.py` & `skyeye-3.4.8/skyeye/version_check.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.7/skyeye.egg-info/PKG-INFO` & `skyeye-3.4.8/skyeye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyeye
-Version: 3.4.7
+Version: 3.4.8
 Summary: APK扫描工具
 Home-page: https://github.com/wangshuwen1107/skyeye
 Author: wangshuwen
 Author-email: wnwn7375@outlook.com
 License: MIT
 Keywords: apk scanner
 Description-Content-Type: text/markdown
```

### Comparing `skyeye-3.4.7/skyeye.egg-info/SOURCES.txt` & `skyeye-3.4.8/skyeye.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 skyeye.egg-info/PKG-INFO
 skyeye.egg-info/SOURCES.txt
 skyeye.egg-info/dependency_links.txt
 skyeye.egg-info/entry_points.txt
 skyeye.egg-info/requires.txt
 skyeye.egg-info/top_level.txt
 skyeye.egg-info/zip-safe
-skyeye/config/.DS_Store
 skyeye/config/__init__.py
 skyeye/config/baksmali-2.5.2.jar
 skyeye/config/cli_config.py
 skyeye/config/config_center.py
 skyeye/config/jd-gui-1.6.6.jar
 skyeye/config/__pycache__/__init__.cpython-310.pyc
 skyeye/config/__pycache__/cli_config.cpython-310.pyc
 skyeye/config/__pycache__/config_center.cpython-310.pyc
-skyeye/config/dex-tools-2.1/.DS_Store
 skyeye/config/dex-tools-2.1/LICENSE.txt
 skyeye/config/dex-tools-2.1/NOTICE.txt
 skyeye/config/dex-tools-2.1/d2j-apk-sign.bat
 skyeye/config/dex-tools-2.1/d2j-apk-sign.sh
 skyeye/config/dex-tools-2.1/d2j-asm-verify.bat
 skyeye/config/dex-tools-2.1/d2j-asm-verify.sh
 skyeye/config/dex-tools-2.1/d2j-baksmali.bat
```


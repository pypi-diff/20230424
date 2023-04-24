# Comparing `tmp/arrayfunc-8.5.0.tar.gz` & `tmp/arrayfunc-8.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayfunc-8.5.0.tar", last modified: Tue Dec 13 04:48:01 2022, max compression
+gzip compressed data, was "arrayfunc-8.5.1.tar", last modified: Sun Apr 23 02:30:47 2023, max compression
```

## Comparing `arrayfunc-8.5.0.tar` & `arrayfunc-8.5.1.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-13 04:48:01.877524 arrayfunc-8.5.0/
--rw-rw-r--   0 me        (1000) me        (1000)       99 2018-11-16 23:30:22.000000 arrayfunc-8.5.0/COPYRIGHT
--rw-rw-r--   0 me        (1000) me        (1000)    11354 2015-05-15 01:35:41.000000 arrayfunc-8.5.0/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      109 2022-12-06 06:27:06.000000 arrayfunc-8.5.0/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)    25413 2022-12-13 04:48:01.877524 arrayfunc-8.5.0/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)    24815 2022-12-13 04:46:48.000000 arrayfunc-8.5.0/README.rst
--rw-rw-r--   0 me        (1000) me        (1000)        6 2022-12-13 04:02:04.000000 arrayfunc-8.5.0/VERSION.TXT
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-13 04:48:01.741526 arrayfunc-8.5.0/arrayfunc/
--rw-rw-r--   0 me        (1000) me        (1000)     3050 2022-12-13 04:47:56.000000 arrayfunc-8.5.0/arrayfunc/__init__.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-13 04:48:01.741526 arrayfunc-8.5.0/arrayfunc.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)    25413 2022-12-13 04:48:01.000000 arrayfunc-8.5.0/arrayfunc.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     5677 2022-12-13 04:48:01.000000 arrayfunc-8.5.0/arrayfunc.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2022-12-13 04:48:01.000000 arrayfunc-8.5.0/arrayfunc.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)      492 2022-12-13 04:48:01.000000 arrayfunc-8.5.0/arrayfunc.egg-info/top_level.txt
--rw-rw-r--   0 me        (1000) me        (1000)       84 2022-11-08 08:03:58.000000 arrayfunc-8.5.0/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2022-12-13 04:48:01.877524 arrayfunc-8.5.0/setup.cfg
--rwxrwxr-x   0 me        (1000) me        (1000)    14573 2022-12-13 04:35:42.000000 arrayfunc-8.5.0/setup.py
--rw-rw-r--   0 me        (1000) me        (1000)     2186 2022-12-05 00:14:52.000000 arrayfunc-8.5.0/setupuser.bat
--rwxrwxr-x   0 me        (1000) me        (1000)      622 2022-12-05 00:12:51.000000 arrayfunc-8.5.0/setupuser.sh
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-13 04:48:01.877524 arrayfunc-8.5.0/src/
--rw-r--r--   0 me        (1000) me        (1000)    88603 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall.c
--rw-r--r--   0 me        (1000) me        (1000)    44808 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     3582 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    90774 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     5220 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    99911 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     5710 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aall_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    87019 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany.c
--rw-r--r--   0 me        (1000) me        (1000)    43920 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     3582 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    89178 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     5220 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    97046 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     5710 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/aany_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    18920 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs_.c
--rw-rw-r--   0 me        (1000) me        (1000)     2379 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    19523 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     2098 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    27742 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     2422 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    20780 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     2146 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/abs__simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/acos.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/acosh.c
--rw-rw-r--   0 me        (1000) me        (1000)   102044 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add.c
--rw-rw-r--   0 me        (1000) me        (1000)     7356 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    91605 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     6826 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)   142172 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     9068 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    98638 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     6159 2021-10-31 16:00:03.000000 arrayfunc-8.5.0/src/add_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    87503 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/afilter.c
--rw-r--r--   0 me        (1000) me        (1000)    20872 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax.c
--rw-r--r--   0 me        (1000) me        (1000)    11571 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    11601 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    13532 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     1760 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amax_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    20872 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin.c
--rw-r--r--   0 me        (1000) me        (1000)    11571 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    11601 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    13532 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     1760 2020-03-28 02:17:09.000000 arrayfunc-8.5.0/src/amin_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    44862 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and_.c
--rw-rw-r--   0 me        (1000) me        (1000)     2198 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    47281 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     4884 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    47423 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     4884 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    49760 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     4882 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/and__simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)     3999 2018-06-04 05:47:15.000000 arrayfunc-8.5.0/src/arrayerrs.c
--rw-rw-r--   0 me        (1000) me        (1000)     2872 2018-05-27 08:05:56.000000 arrayfunc-8.5.0/src/arrayerrs.h
--rw-rw-r--   0 me        (1000) me        (1000)     3880 2021-02-26 02:19:20.000000 arrayfunc-8.5.0/src/arrayguardbands.c
--rw-rw-r--   0 me        (1000) me        (1000)     5133 2018-06-04 05:47:15.000000 arrayfunc-8.5.0/src/arraylimits.c
--rw-rw-r--   0 me        (1000) me        (1000)     2017 2019-07-06 20:56:44.000000 arrayfunc-8.5.0/src/arrayops.c
--rw-rw-r--   0 me        (1000) me        (1000)     1358 2019-07-06 20:56:52.000000 arrayfunc-8.5.0/src/arrayops.h
--rw-rw-r--   0 me        (1000) me        (1000)     6498 2019-04-16 05:38:28.000000 arrayfunc-8.5.0/src/arrayparams_allany.c
--rw-rw-r--   0 me        (1000) me        (1000)     1896 2019-04-15 05:22:51.000000 arrayfunc-8.5.0/src/arrayparams_allany.h
--rw-rw-r--   0 me        (1000) me        (1000)     4882 2022-12-05 00:10:06.000000 arrayfunc-8.5.0/src/arrayparams_asum.c
--rw-rw-r--   0 me        (1000) me        (1000)     1820 2019-05-27 03:20:43.000000 arrayfunc-8.5.0/src/arrayparams_asum.h
--rw-rw-r--   0 me        (1000) me        (1000)    17605 2019-10-23 03:37:05.000000 arrayfunc-8.5.0/src/arrayparams_base.c
--rw-rw-r--   0 me        (1000) me        (1000)     4023 2019-05-11 04:30:01.000000 arrayfunc-8.5.0/src/arrayparams_base.h
--rw-rw-r--   0 me        (1000) me        (1000)     4838 2018-06-10 05:23:12.000000 arrayfunc-8.5.0/src/arrayparams_boolout.c
--rw-rw-r--   0 me        (1000) me        (1000)     1791 2018-06-10 05:14:43.000000 arrayfunc-8.5.0/src/arrayparams_boolout.h
--rw-rw-r--   0 me        (1000) me        (1000)     4835 2019-05-21 06:29:25.000000 arrayfunc-8.5.0/src/arrayparams_booloutsimd.c
--rw-rw-r--   0 me        (1000) me        (1000)     1838 2019-05-16 05:45:56.000000 arrayfunc-8.5.0/src/arrayparams_booloutsimd.h
--rw-r--r--   0 me        (1000) me        (1000)    17276 2019-06-10 04:52:42.000000 arrayfunc-8.5.0/src/arrayparams_cntcycrep.c
--rw-r--r--   0 me        (1000) me        (1000)     2197 2019-06-06 09:36:00.000000 arrayfunc-8.5.0/src/arrayparams_cntcycrep.h
--rw-rw-r--   0 me        (1000) me        (1000)     7886 2019-05-11 04:40:50.000000 arrayfunc-8.5.0/src/arrayparams_comp.c
--rw-rw-r--   0 me        (1000) me        (1000)     2039 2019-02-22 06:49:59.000000 arrayfunc-8.5.0/src/arrayparams_comp.h
--rw-r--r--   0 me        (1000) me        (1000)     7207 2019-06-27 03:04:37.000000 arrayfunc-8.5.0/src/arrayparams_compress.c
--rw-r--r--   0 me        (1000) me        (1000)     2009 2019-06-27 02:51:55.000000 arrayfunc-8.5.0/src/arrayparams_compress.h
--rw-r--r--   0 me        (1000) me        (1000)     6149 2019-06-28 03:11:17.000000 arrayfunc-8.5.0/src/arrayparams_convert.c
--rw-r--r--   0 me        (1000) me        (1000)     1879 2019-06-28 03:04:31.000000 arrayfunc-8.5.0/src/arrayparams_convert.h
--rw-rw-r--   0 me        (1000) me        (1000)     7765 2019-06-22 20:19:19.000000 arrayfunc-8.5.0/src/arrayparams_droptakefilter.c
--rw-rw-r--   0 me        (1000) me        (1000)     1982 2019-06-22 20:17:23.000000 arrayfunc-8.5.0/src/arrayparams_droptakefilter.h
--rw-r--r--   0 me        (1000) me        (1000)     7695 2019-06-25 01:54:11.000000 arrayfunc-8.5.0/src/arrayparams_findindices.c
--rw-r--r--   0 me        (1000) me        (1000)     1980 2019-06-24 00:24:51.000000 arrayfunc-8.5.0/src/arrayparams_findindices.h
--rw-rw-r--   0 me        (1000) me        (1000)     7051 2019-05-11 04:41:22.000000 arrayfunc-8.5.0/src/arrayparams_one.c
--rw-rw-r--   0 me        (1000) me        (1000)     1919 2018-06-09 06:50:35.000000 arrayfunc-8.5.0/src/arrayparams_one.h
--rw-rw-r--   0 me        (1000) me        (1000)     7192 2019-05-11 04:42:34.000000 arrayfunc-8.5.0/src/arrayparams_onesimd.c
--rw-rw-r--   0 me        (1000) me        (1000)     1938 2019-03-21 08:37:30.000000 arrayfunc-8.5.0/src/arrayparams_onesimd.h
--rw-rw-r--   0 me        (1000) me        (1000)     5503 2018-06-04 05:47:15.000000 arrayfunc-8.5.0/src/arrayparams_special.c
--rw-rw-r--   0 me        (1000) me        (1000)     1922 2018-04-30 01:08:31.000000 arrayfunc-8.5.0/src/arrayparams_special.h
--rw-rw-r--   0 me        (1000) me        (1000)    10300 2019-05-11 04:42:10.000000 arrayfunc-8.5.0/src/arrayparams_three.c
--rw-rw-r--   0 me        (1000) me        (1000)     2423 2019-04-13 05:26:34.000000 arrayfunc-8.5.0/src/arrayparams_three.h
--rw-rw-r--   0 me        (1000) me        (1000)    12674 2019-05-11 04:43:09.000000 arrayfunc-8.5.0/src/arrayparams_two.c
--rw-rw-r--   0 me        (1000) me        (1000)     2276 2019-03-13 08:04:47.000000 arrayfunc-8.5.0/src/arrayparams_two.h
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/asin.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/asinh.c
--rw-rw-r--   0 me        (1000) me        (1000)    27291 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum.c
--rw-rw-r--   0 me        (1000) me        (1000)     1698 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    19152 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     2034 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    19178 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     2034 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    21157 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1946 2022-07-04 17:35:50.000000 arrayfunc-8.5.0/src/asum_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/atan.c
--rw-r--r--   0 me        (1000) me        (1000)    14679 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/atan2.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/atanh.c
--rw-rw-r--   0 me        (1000) me        (1000)     9082 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/ceil.c
--rw-rw-r--   0 me        (1000) me        (1000)    13475 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/ceil_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1702 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/ceil_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    25171 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/compress.c
--rw-r--r--   0 me        (1000) me        (1000)    40551 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/convert.c
--rw-rw-r--   0 me        (1000) me        (1000)     3917 2021-02-26 02:20:14.000000 arrayfunc-8.5.0/src/convguardbands.h
--rw-r--r--   0 me        (1000) me        (1000)    14910 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/copysign.c
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/cos.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/cosh.c
--rw-r--r--   0 me        (1000) me        (1000)    17632 2020-03-06 07:22:57.000000 arrayfunc-8.5.0/src/count.c
--rw-r--r--   0 me        (1000) me        (1000)    22885 2020-03-06 07:22:57.000000 arrayfunc-8.5.0/src/cycle.c
--rw-rw-r--   0 me        (1000) me        (1000)    10103 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees.c
--rw-rw-r--   0 me        (1000) me        (1000)     8290 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)     8332 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    14481 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1732 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/degrees_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    91574 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/dropwhile.c
--rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq.c
--rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    38728 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/eq_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/erf.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/erfc.c
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/exp.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/expm1.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/fabs.c
--rw-r--r--   0 me        (1000) me        (1000)    25058 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/factorial.c
--rw-r--r--   0 me        (1000) me        (1000)    89306 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex.c
--rw-r--r--   0 me        (1000) me        (1000)    47306 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     3712 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    97112 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     5440 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)   106157 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     5960 2020-03-28 02:17:04.000000 arrayfunc-8.5.0/src/findindex_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    93660 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/findindices.c
--rw-rw-r--   0 me        (1000) me        (1000)     9127 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/floor.c
--rw-rw-r--   0 me        (1000) me        (1000)    13493 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/floor_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1712 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/floor_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    79045 2021-09-07 01:16:37.000000 arrayfunc-8.5.0/src/floordiv.c
--rw-r--r--   0 me        (1000) me        (1000)    18910 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/fma.c
--rw-r--r--   0 me        (1000) me        (1000)    14602 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/fmod.c
--rw-r--r--   0 me        (1000) me        (1000)     7232 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gamma.c
--rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge.c
--rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    41776 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ge_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    30875 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt.c
--rw-r--r--   0 me        (1000) me        (1000)    18024 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36907 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    41983 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/gt_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    14679 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/hypot.c
--rw-r--r--   0 me        (1000) me        (1000)    15342 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert.c
--rw-r--r--   0 me        (1000) me        (1000)    14832 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2176 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    14872 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2176 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    15989 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     2174 2020-03-28 02:17:17.000000 arrayfunc-8.5.0/src/invert_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)     5841 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/isfinite.c
--rw-r--r--   0 me        (1000) me        (1000)     5768 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/isinf.c
--rw-r--r--   0 me        (1000) me        (1000)     5760 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/isnan.c
--rw-r--r--   0 me        (1000) me        (1000)     7916 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/ldexp.c
--rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le.c
--rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    40264 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/le_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)     7259 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lgamma.c
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/log.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/log10.c
--rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/log1p.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/log2.c
--rw-rw-r--   0 me        (1000) me        (1000)    39261 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift.c
--rw-rw-r--   0 me        (1000) me        (1000)     2202 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    21501 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    21555 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    25046 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     2414 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/lshift_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    30875 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt.c
--rw-r--r--   0 me        (1000) me        (1000)    18024 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36907 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    43894 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/lt_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    80045 2021-10-01 16:10:01.000000 arrayfunc-8.5.0/src/mod.c
--rw-rw-r--   0 me        (1000) me        (1000)   111302 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul.c
--rw-rw-r--   0 me        (1000) me        (1000)    10833 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    97458 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     6371 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)   159373 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     8396 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    40117 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     3123 2021-10-31 16:00:30.000000 arrayfunc-8.5.0/src/mul_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne.c
--rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_armv7.c
--rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_armv7.h
--rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_armv8.c
--rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_armv8.h
--rw-r--r--   0 me        (1000) me        (1000)    38806 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_x86.c
--rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/ne_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    18332 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg.c
--rw-rw-r--   0 me        (1000) me        (1000)     2377 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    18818 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     2084 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    26693 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     2404 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    20503 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     2132 2021-10-31 16:00:37.000000 arrayfunc-8.5.0/src/neg_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    44676 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or_.c
--rw-rw-r--   0 me        (1000) me        (1000)     2196 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    47242 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    47384 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    49685 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     4844 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/or__simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)   101922 2021-10-15 00:12:28.000000 arrayfunc-8.5.0/src/pow.c
--rw-rw-r--   0 me        (1000) me        (1000)    22739 2021-10-15 00:12:41.000000 arrayfunc-8.5.0/src/pow2.c
--rw-rw-r--   0 me        (1000) me        (1000)    23230 2021-10-15 00:12:41.000000 arrayfunc-8.5.0/src/pow3.c
--rw-rw-r--   0 me        (1000) me        (1000)    10103 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians.c
--rw-rw-r--   0 me        (1000) me        (1000)     8277 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)     8319 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    14464 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1732 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/radians_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    10973 2020-03-06 07:22:57.000000 arrayfunc-8.5.0/src/repeat.c
--rw-rw-r--   0 me        (1000) me        (1000)    39207 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift.c
--rw-rw-r--   0 me        (1000) me        (1000)     2202 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    21507 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    21561 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    25821 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     2203 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/rshift_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)     4879 2022-05-31 02:56:47.000000 arrayfunc-8.5.0/src/simddefs.h
--rw-rw-r--   0 me        (1000) me        (1000)     4915 2022-04-23 05:47:53.000000 arrayfunc-8.5.0/src/simdsupport.c
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/sin.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/sinh.c
--rw-rw-r--   0 me        (1000) me        (1000)     9082 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/sqrt.c
--rw-rw-r--   0 me        (1000) me        (1000)    13411 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/sqrt_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1702 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/sqrt_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)   101596 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub.c
--rw-rw-r--   0 me        (1000) me        (1000)     8082 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    92455 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     6826 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)   145059 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     9068 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)   105347 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     6159 2021-10-31 16:00:22.000000 arrayfunc-8.5.0/src/sub_simd_x86.h
--rw-r--r--   0 me        (1000) me        (1000)    77808 2020-03-06 06:11:19.000000 arrayfunc-8.5.0/src/takewhile.c
--rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/tan.c
--rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.0/src/tanh.c
--rw-rw-r--   0 me        (1000) me        (1000)    63851 2021-09-07 01:16:29.000000 arrayfunc-8.5.0/src/truediv.c
--rw-rw-r--   0 me        (1000) me        (1000)     9127 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/trunc.c
--rw-rw-r--   0 me        (1000) me        (1000)    13493 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/trunc_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     1712 2021-10-31 16:00:15.000000 arrayfunc-8.5.0/src/trunc_simd_x86.h
--rw-rw-r--   0 me        (1000) me        (1000)    44676 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor.c
--rw-rw-r--   0 me        (1000) me        (1000)     2196 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_defs.h
--rw-rw-r--   0 me        (1000) me        (1000)    47242 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_armv7.c
--rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_armv7.h
--rw-rw-r--   0 me        (1000) me        (1000)    47384 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_armv8.c
--rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_armv8.h
--rw-rw-r--   0 me        (1000) me        (1000)    49721 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_x86.c
--rw-rw-r--   0 me        (1000) me        (1000)     4844 2021-09-07 01:16:10.000000 arrayfunc-8.5.0/src/xor_simd_x86.h
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:30:47.269478 arrayfunc-8.5.1/
+-rw-rw-r--   0 me        (1000) me        (1000)       99 2018-11-16 23:30:22.000000 arrayfunc-8.5.1/COPYRIGHT
+-rw-rw-r--   0 me        (1000) me        (1000)    11354 2015-05-15 01:35:41.000000 arrayfunc-8.5.1/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      109 2022-12-06 06:27:06.000000 arrayfunc-8.5.1/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)    26993 2023-04-23 02:30:47.265478 arrayfunc-8.5.1/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)    26395 2023-04-23 02:23:50.000000 arrayfunc-8.5.1/README.rst
+-rw-rw-r--   0 me        (1000) me        (1000)        6 2023-04-23 01:58:43.000000 arrayfunc-8.5.1/VERSION.TXT
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:30:47.109479 arrayfunc-8.5.1/arrayfunc/
+-rw-rw-r--   0 me        (1000) me        (1000)     3050 2023-04-23 02:30:42.000000 arrayfunc-8.5.1/arrayfunc/__init__.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:30:47.113479 arrayfunc-8.5.1/arrayfunc.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)    26993 2023-04-23 02:30:47.000000 arrayfunc-8.5.1/arrayfunc.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     5677 2023-04-23 02:30:47.000000 arrayfunc-8.5.1/arrayfunc.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-04-23 02:30:47.000000 arrayfunc-8.5.1/arrayfunc.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)      492 2023-04-23 02:30:47.000000 arrayfunc-8.5.1/arrayfunc.egg-info/top_level.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2022-11-08 08:03:58.000000 arrayfunc-8.5.1/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-04-23 02:30:47.269478 arrayfunc-8.5.1/setup.cfg
+-rwxrwxr-x   0 me        (1000) me        (1000)    14573 2022-12-13 04:35:42.000000 arrayfunc-8.5.1/setup.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2186 2022-12-05 00:14:52.000000 arrayfunc-8.5.1/setupuser.bat
+-rwxrwxr-x   0 me        (1000) me        (1000)      622 2022-12-05 00:12:51.000000 arrayfunc-8.5.1/setupuser.sh
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:30:47.265478 arrayfunc-8.5.1/src/
+-rw-r--r--   0 me        (1000) me        (1000)    88603 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall.c
+-rw-r--r--   0 me        (1000) me        (1000)    44808 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     3582 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    90774 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     5220 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    99911 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     5710 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aall_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    87019 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany.c
+-rw-r--r--   0 me        (1000) me        (1000)    43920 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     3582 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    89178 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     5220 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    97046 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     5710 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/aany_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    18920 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs_.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2379 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    19523 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2098 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    27742 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2422 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    20780 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2146 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/abs__simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/acos.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/acosh.c
+-rw-rw-r--   0 me        (1000) me        (1000)   102044 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add.c
+-rw-rw-r--   0 me        (1000) me        (1000)     7356 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    91605 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     6826 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)   142172 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9068 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    98638 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     6159 2021-10-31 16:00:03.000000 arrayfunc-8.5.1/src/add_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    87503 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/afilter.c
+-rw-r--r--   0 me        (1000) me        (1000)    20872 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax.c
+-rw-r--r--   0 me        (1000) me        (1000)    11571 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    11601 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    13532 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     1760 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amax_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    20872 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin.c
+-rw-r--r--   0 me        (1000) me        (1000)    11571 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    11601 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     1702 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    13532 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     1760 2020-03-28 02:17:09.000000 arrayfunc-8.5.1/src/amin_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    44862 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and_.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2198 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47281 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4884 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47423 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4884 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    49760 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4882 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/and__simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)     3999 2018-06-04 05:47:15.000000 arrayfunc-8.5.1/src/arrayerrs.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2872 2018-05-27 08:05:56.000000 arrayfunc-8.5.1/src/arrayerrs.h
+-rw-rw-r--   0 me        (1000) me        (1000)     3880 2021-02-26 02:19:20.000000 arrayfunc-8.5.1/src/arrayguardbands.c
+-rw-rw-r--   0 me        (1000) me        (1000)     5133 2018-06-04 05:47:15.000000 arrayfunc-8.5.1/src/arraylimits.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2017 2019-07-06 20:56:44.000000 arrayfunc-8.5.1/src/arrayops.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1358 2019-07-06 20:56:52.000000 arrayfunc-8.5.1/src/arrayops.h
+-rw-rw-r--   0 me        (1000) me        (1000)     6498 2019-04-16 05:38:28.000000 arrayfunc-8.5.1/src/arrayparams_allany.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1896 2019-04-15 05:22:51.000000 arrayfunc-8.5.1/src/arrayparams_allany.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4882 2022-12-05 00:10:06.000000 arrayfunc-8.5.1/src/arrayparams_asum.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1820 2019-05-27 03:20:43.000000 arrayfunc-8.5.1/src/arrayparams_asum.h
+-rw-rw-r--   0 me        (1000) me        (1000)    17605 2019-10-23 03:37:05.000000 arrayfunc-8.5.1/src/arrayparams_base.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4023 2019-05-11 04:30:01.000000 arrayfunc-8.5.1/src/arrayparams_base.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4838 2018-06-10 05:23:12.000000 arrayfunc-8.5.1/src/arrayparams_boolout.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1791 2018-06-10 05:14:43.000000 arrayfunc-8.5.1/src/arrayparams_boolout.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4835 2019-05-21 06:29:25.000000 arrayfunc-8.5.1/src/arrayparams_booloutsimd.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1838 2019-05-16 05:45:56.000000 arrayfunc-8.5.1/src/arrayparams_booloutsimd.h
+-rw-r--r--   0 me        (1000) me        (1000)    17276 2019-06-10 04:52:42.000000 arrayfunc-8.5.1/src/arrayparams_cntcycrep.c
+-rw-r--r--   0 me        (1000) me        (1000)     2197 2019-06-06 09:36:00.000000 arrayfunc-8.5.1/src/arrayparams_cntcycrep.h
+-rw-rw-r--   0 me        (1000) me        (1000)     7886 2019-05-11 04:40:50.000000 arrayfunc-8.5.1/src/arrayparams_comp.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2039 2019-02-22 06:49:59.000000 arrayfunc-8.5.1/src/arrayparams_comp.h
+-rw-r--r--   0 me        (1000) me        (1000)     7207 2019-06-27 03:04:37.000000 arrayfunc-8.5.1/src/arrayparams_compress.c
+-rw-r--r--   0 me        (1000) me        (1000)     2009 2019-06-27 02:51:55.000000 arrayfunc-8.5.1/src/arrayparams_compress.h
+-rw-r--r--   0 me        (1000) me        (1000)     6149 2019-06-28 03:11:17.000000 arrayfunc-8.5.1/src/arrayparams_convert.c
+-rw-r--r--   0 me        (1000) me        (1000)     1879 2019-06-28 03:04:31.000000 arrayfunc-8.5.1/src/arrayparams_convert.h
+-rw-rw-r--   0 me        (1000) me        (1000)     7765 2019-06-22 20:19:19.000000 arrayfunc-8.5.1/src/arrayparams_droptakefilter.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1982 2019-06-22 20:17:23.000000 arrayfunc-8.5.1/src/arrayparams_droptakefilter.h
+-rw-r--r--   0 me        (1000) me        (1000)     7695 2019-06-25 01:54:11.000000 arrayfunc-8.5.1/src/arrayparams_findindices.c
+-rw-r--r--   0 me        (1000) me        (1000)     1980 2019-06-24 00:24:51.000000 arrayfunc-8.5.1/src/arrayparams_findindices.h
+-rw-rw-r--   0 me        (1000) me        (1000)     7051 2019-05-11 04:41:22.000000 arrayfunc-8.5.1/src/arrayparams_one.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1919 2018-06-09 06:50:35.000000 arrayfunc-8.5.1/src/arrayparams_one.h
+-rw-rw-r--   0 me        (1000) me        (1000)     7192 2019-05-11 04:42:34.000000 arrayfunc-8.5.1/src/arrayparams_onesimd.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1938 2019-03-21 08:37:30.000000 arrayfunc-8.5.1/src/arrayparams_onesimd.h
+-rw-rw-r--   0 me        (1000) me        (1000)     5503 2018-06-04 05:47:15.000000 arrayfunc-8.5.1/src/arrayparams_special.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1922 2018-04-30 01:08:31.000000 arrayfunc-8.5.1/src/arrayparams_special.h
+-rw-rw-r--   0 me        (1000) me        (1000)    10300 2019-05-11 04:42:10.000000 arrayfunc-8.5.1/src/arrayparams_three.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2423 2019-04-13 05:26:34.000000 arrayfunc-8.5.1/src/arrayparams_three.h
+-rw-rw-r--   0 me        (1000) me        (1000)    12674 2019-05-11 04:43:09.000000 arrayfunc-8.5.1/src/arrayparams_two.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2276 2019-03-13 08:04:47.000000 arrayfunc-8.5.1/src/arrayparams_two.h
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/asin.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/asinh.c
+-rw-rw-r--   0 me        (1000) me        (1000)    27291 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1698 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    19152 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2034 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    19178 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2034 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    21157 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1946 2022-07-04 17:35:50.000000 arrayfunc-8.5.1/src/asum_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/atan.c
+-rw-r--r--   0 me        (1000) me        (1000)    14679 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/atan2.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/atanh.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9082 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/ceil.c
+-rw-rw-r--   0 me        (1000) me        (1000)    13475 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/ceil_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1702 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/ceil_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    25171 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/compress.c
+-rw-r--r--   0 me        (1000) me        (1000)    40551 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/convert.c
+-rw-rw-r--   0 me        (1000) me        (1000)     3917 2021-02-26 02:20:14.000000 arrayfunc-8.5.1/src/convguardbands.h
+-rw-r--r--   0 me        (1000) me        (1000)    14910 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/copysign.c
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/cos.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/cosh.c
+-rw-r--r--   0 me        (1000) me        (1000)    17632 2020-03-06 07:22:57.000000 arrayfunc-8.5.1/src/count.c
+-rw-r--r--   0 me        (1000) me        (1000)    22885 2020-03-06 07:22:57.000000 arrayfunc-8.5.1/src/cycle.c
+-rw-rw-r--   0 me        (1000) me        (1000)    10103 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees.c
+-rw-rw-r--   0 me        (1000) me        (1000)     8290 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)     8332 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    14481 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1732 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/degrees_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    91574 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/dropwhile.c
+-rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq.c
+-rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    38728 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/eq_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/erf.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/erfc.c
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/exp.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/expm1.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/fabs.c
+-rw-r--r--   0 me        (1000) me        (1000)    25058 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/factorial.c
+-rw-r--r--   0 me        (1000) me        (1000)    89306 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex.c
+-rw-r--r--   0 me        (1000) me        (1000)    47306 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     3712 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    97112 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     5440 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)   106157 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     5960 2020-03-28 02:17:04.000000 arrayfunc-8.5.1/src/findindex_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    93660 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/findindices.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9127 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/floor.c
+-rw-rw-r--   0 me        (1000) me        (1000)    13493 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/floor_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1712 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/floor_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    79045 2021-09-07 01:16:37.000000 arrayfunc-8.5.1/src/floordiv.c
+-rw-r--r--   0 me        (1000) me        (1000)    18910 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/fma.c
+-rw-r--r--   0 me        (1000) me        (1000)    14602 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/fmod.c
+-rw-r--r--   0 me        (1000) me        (1000)     7232 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gamma.c
+-rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge.c
+-rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    41776 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ge_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    30875 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt.c
+-rw-r--r--   0 me        (1000) me        (1000)    18024 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36907 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    41983 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/gt_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    14679 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/hypot.c
+-rw-r--r--   0 me        (1000) me        (1000)    15342 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert.c
+-rw-r--r--   0 me        (1000) me        (1000)    14832 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2176 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    14872 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2176 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    15989 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     2174 2020-03-28 02:17:17.000000 arrayfunc-8.5.1/src/invert_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)     5841 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/isfinite.c
+-rw-r--r--   0 me        (1000) me        (1000)     5768 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/isinf.c
+-rw-r--r--   0 me        (1000) me        (1000)     5760 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/isnan.c
+-rw-r--r--   0 me        (1000) me        (1000)     7916 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/ldexp.c
+-rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le.c
+-rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    40264 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/le_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)     7259 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lgamma.c
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/log.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/log10.c
+-rw-r--r--   0 me        (1000) me        (1000)     7224 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/log1p.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/log2.c
+-rw-rw-r--   0 me        (1000) me        (1000)    39261 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2202 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    21501 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    21555 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    25046 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2414 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/lshift_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    30875 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt.c
+-rw-r--r--   0 me        (1000) me        (1000)    18024 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36907 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    43894 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/lt_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    80045 2021-10-01 16:10:01.000000 arrayfunc-8.5.1/src/mod.c
+-rw-rw-r--   0 me        (1000) me        (1000)   111302 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul.c
+-rw-rw-r--   0 me        (1000) me        (1000)    10833 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    97458 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     6371 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)   159373 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     8396 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    40117 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     3123 2021-10-31 16:00:30.000000 arrayfunc-8.5.1/src/mul_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    30914 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne.c
+-rw-r--r--   0 me        (1000) me        (1000)    18036 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_armv7.c
+-rw-r--r--   0 me        (1000) me        (1000)     2256 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_armv7.h
+-rw-r--r--   0 me        (1000) me        (1000)    36928 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_armv8.c
+-rw-r--r--   0 me        (1000) me        (1000)     2997 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_armv8.h
+-rw-r--r--   0 me        (1000) me        (1000)    38806 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_x86.c
+-rw-r--r--   0 me        (1000) me        (1000)     3215 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/ne_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    18332 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2377 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    18818 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2084 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    26693 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2404 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    20503 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2132 2021-10-31 16:00:37.000000 arrayfunc-8.5.1/src/neg_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    44676 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or_.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2196 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47242 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47384 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    49685 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4844 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/or__simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)   101922 2021-10-15 00:12:28.000000 arrayfunc-8.5.1/src/pow.c
+-rw-rw-r--   0 me        (1000) me        (1000)    22739 2021-10-15 00:12:41.000000 arrayfunc-8.5.1/src/pow2.c
+-rw-rw-r--   0 me        (1000) me        (1000)    23230 2021-10-15 00:12:41.000000 arrayfunc-8.5.1/src/pow3.c
+-rw-rw-r--   0 me        (1000) me        (1000)    10103 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians.c
+-rw-rw-r--   0 me        (1000) me        (1000)     8277 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)     8319 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1438 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    14464 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1732 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/radians_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    10973 2020-03-06 07:22:57.000000 arrayfunc-8.5.1/src/repeat.c
+-rw-rw-r--   0 me        (1000) me        (1000)    39207 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2202 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    21507 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    21561 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2416 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    25821 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2203 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/rshift_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4879 2022-05-31 02:56:47.000000 arrayfunc-8.5.1/src/simddefs.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4915 2022-04-23 05:47:53.000000 arrayfunc-8.5.1/src/simdsupport.c
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/sin.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/sinh.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9082 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/sqrt.c
+-rw-rw-r--   0 me        (1000) me        (1000)    13411 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/sqrt_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1702 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/sqrt_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)   101596 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub.c
+-rw-rw-r--   0 me        (1000) me        (1000)     8082 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    92455 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     6826 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)   145059 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9068 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)   105347 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     6159 2021-10-31 16:00:22.000000 arrayfunc-8.5.1/src/sub_simd_x86.h
+-rw-r--r--   0 me        (1000) me        (1000)    77808 2020-03-06 06:11:19.000000 arrayfunc-8.5.1/src/takewhile.c
+-rw-r--r--   0 me        (1000) me        (1000)     7154 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/tan.c
+-rw-r--r--   0 me        (1000) me        (1000)     7189 2020-03-28 02:17:13.000000 arrayfunc-8.5.1/src/tanh.c
+-rw-rw-r--   0 me        (1000) me        (1000)    63851 2021-09-07 01:16:29.000000 arrayfunc-8.5.1/src/truediv.c
+-rw-rw-r--   0 me        (1000) me        (1000)     9127 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/trunc.c
+-rw-rw-r--   0 me        (1000) me        (1000)    13493 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/trunc_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1712 2021-10-31 16:00:15.000000 arrayfunc-8.5.1/src/trunc_simd_x86.h
+-rw-rw-r--   0 me        (1000) me        (1000)    44676 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2196 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_defs.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47242 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_armv7.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_armv7.h
+-rw-rw-r--   0 me        (1000) me        (1000)    47384 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_armv8.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4846 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_armv8.h
+-rw-rw-r--   0 me        (1000) me        (1000)    49721 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_x86.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4844 2021-09-07 01:16:10.000000 arrayfunc-8.5.1/src/xor_simd_x86.h
```

### Comparing `arrayfunc-8.5.0/LICENSE` & `arrayfunc-8.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/PKG-INFO` & `arrayfunc-8.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrayfunc
-Version: 8.5.0
+Version: 8.5.1
 Summary: Fast array processing functions
 Home-page: https://github.com/m1griffin/arrayfunc
 Author: M Griffin
 Author-email: m12.griffin@gmail.com
 License: Apache License V2.0
 Keywords: mathematical array functions
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,16 @@
 =========
 ArrayFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  8.5.0 for 2022-12-12
-:Copyright: 2014 - 2022
+:Version:  8.5.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -317,20 +317,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -392,18 +392,54 @@
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
 
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 8.5.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 8.5.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Removed duplicate assignment in
           parameter parsing return data in arrayparams_asum.c.
```

### Comparing `arrayfunc-8.5.0/README.rst` & `arrayfunc-8.5.1/arrayfunc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,33 @@
+Metadata-Version: 2.1
+Name: arrayfunc
+Version: 8.5.1
+Summary: Fast array processing functions
+Home-page: https://github.com/m1griffin/arrayfunc
+Author: M Griffin
+Author-email: m12.griffin@gmail.com
+License: Apache License V2.0
+Keywords: mathematical array functions
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 =========
 ArrayFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  8.5.0 for 2022-12-12
-:Copyright: 2014 - 2022
+:Version:  8.5.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -300,20 +317,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -375,18 +392,54 @@
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
 
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 8.5.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 8.5.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Removed duplicate assignment in
           parameter parsing return data in arrayparams_asum.c.
```

### Comparing `arrayfunc-8.5.0/arrayfunc/__init__.py` & `arrayfunc-8.5.1/arrayfunc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 for use with the standard Python array module. These functions are 
 patterned after the functions in the standard Python Itertools module 
 together with some additional ones import other sources.
 
 """
 
 # The version number should be updated automatically by the build script.
-__version__ = '8.5.0'
+__version__ = '8.5.1'
 
 from arrayfunc.count import count
 from arrayfunc.cycle import cycle
 from arrayfunc.repeat import repeat
 
 from arrayfunc.afilter import afilter
 from arrayfunc.takewhile import takewhile
```

### Comparing `arrayfunc-8.5.0/arrayfunc.egg-info/PKG-INFO` & `arrayfunc-8.5.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: arrayfunc
-Version: 8.5.0
-Summary: Fast array processing functions
-Home-page: https://github.com/m1griffin/arrayfunc
-Author: M Griffin
-Author-email: m12.griffin@gmail.com
-License: Apache License V2.0
-Keywords: mathematical array functions
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 =========
 ArrayFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  8.5.0 for 2022-12-12
-:Copyright: 2014 - 2022
+:Version:  8.5.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -317,20 +300,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -392,18 +375,54 @@
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
 
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 8.5.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 8.5.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Removed duplicate assignment in
           parameter parsing return data in arrayparams_asum.c.
```

### Comparing `arrayfunc-8.5.0/arrayfunc.egg-info/SOURCES.txt` & `arrayfunc-8.5.1/arrayfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/setup.py` & `arrayfunc-8.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/setupuser.bat` & `arrayfunc-8.5.1/setupuser.bat`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/setupuser.sh` & `arrayfunc-8.5.1/setupuser.sh`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall.c` & `arrayfunc-8.5.1/src/aall.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_armv7.c` & `arrayfunc-8.5.1/src/aall_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_armv7.h` & `arrayfunc-8.5.1/src/aall_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_armv8.c` & `arrayfunc-8.5.1/src/aall_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_armv8.h` & `arrayfunc-8.5.1/src/aall_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_x86.c` & `arrayfunc-8.5.1/src/aall_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aall_simd_x86.h` & `arrayfunc-8.5.1/src/aall_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany.c` & `arrayfunc-8.5.1/src/aany.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_armv7.c` & `arrayfunc-8.5.1/src/aany_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_armv7.h` & `arrayfunc-8.5.1/src/aany_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_armv8.c` & `arrayfunc-8.5.1/src/aany_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_armv8.h` & `arrayfunc-8.5.1/src/aany_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_x86.c` & `arrayfunc-8.5.1/src/aany_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/aany_simd_x86.h` & `arrayfunc-8.5.1/src/aany_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs_.c` & `arrayfunc-8.5.1/src/abs_.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__defs.h` & `arrayfunc-8.5.1/src/abs__defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_armv7.c` & `arrayfunc-8.5.1/src/abs__simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_armv7.h` & `arrayfunc-8.5.1/src/abs__simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_armv8.c` & `arrayfunc-8.5.1/src/abs__simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_armv8.h` & `arrayfunc-8.5.1/src/abs__simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_x86.c` & `arrayfunc-8.5.1/src/abs__simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/abs__simd_x86.h` & `arrayfunc-8.5.1/src/abs__simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/acos.c` & `arrayfunc-8.5.1/src/acos.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/acosh.c` & `arrayfunc-8.5.1/src/acosh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add.c` & `arrayfunc-8.5.1/src/add.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_defs.h` & `arrayfunc-8.5.1/src/add_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_armv7.c` & `arrayfunc-8.5.1/src/add_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_armv7.h` & `arrayfunc-8.5.1/src/add_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_armv8.c` & `arrayfunc-8.5.1/src/add_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_armv8.h` & `arrayfunc-8.5.1/src/add_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_x86.c` & `arrayfunc-8.5.1/src/add_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/add_simd_x86.h` & `arrayfunc-8.5.1/src/add_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/afilter.c` & `arrayfunc-8.5.1/src/afilter.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax.c` & `arrayfunc-8.5.1/src/amax.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_armv7.c` & `arrayfunc-8.5.1/src/amax_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_armv7.h` & `arrayfunc-8.5.1/src/amax_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_armv8.c` & `arrayfunc-8.5.1/src/amax_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_armv8.h` & `arrayfunc-8.5.1/src/amax_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_x86.c` & `arrayfunc-8.5.1/src/amax_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amax_simd_x86.h` & `arrayfunc-8.5.1/src/amax_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin.c` & `arrayfunc-8.5.1/src/amin.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_armv7.c` & `arrayfunc-8.5.1/src/amin_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_armv7.h` & `arrayfunc-8.5.1/src/amin_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_armv8.c` & `arrayfunc-8.5.1/src/amin_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_armv8.h` & `arrayfunc-8.5.1/src/amin_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_x86.c` & `arrayfunc-8.5.1/src/amin_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/amin_simd_x86.h` & `arrayfunc-8.5.1/src/amin_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and_.c` & `arrayfunc-8.5.1/src/and_.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__defs.h` & `arrayfunc-8.5.1/src/and__defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_armv7.c` & `arrayfunc-8.5.1/src/and__simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_armv7.h` & `arrayfunc-8.5.1/src/and__simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_armv8.c` & `arrayfunc-8.5.1/src/and__simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_armv8.h` & `arrayfunc-8.5.1/src/and__simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_x86.c` & `arrayfunc-8.5.1/src/and__simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/and__simd_x86.h` & `arrayfunc-8.5.1/src/and__simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayerrs.c` & `arrayfunc-8.5.1/src/arrayerrs.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayerrs.h` & `arrayfunc-8.5.1/src/arrayerrs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayguardbands.c` & `arrayfunc-8.5.1/src/arrayguardbands.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arraylimits.c` & `arrayfunc-8.5.1/src/arraylimits.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayops.c` & `arrayfunc-8.5.1/src/arrayops.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayops.h` & `arrayfunc-8.5.1/src/arrayops.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_allany.c` & `arrayfunc-8.5.1/src/arrayparams_allany.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_allany.h` & `arrayfunc-8.5.1/src/arrayparams_allany.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_asum.c` & `arrayfunc-8.5.1/src/arrayparams_asum.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_asum.h` & `arrayfunc-8.5.1/src/arrayparams_asum.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_base.c` & `arrayfunc-8.5.1/src/arrayparams_base.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_base.h` & `arrayfunc-8.5.1/src/arrayparams_base.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_boolout.c` & `arrayfunc-8.5.1/src/arrayparams_boolout.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_boolout.h` & `arrayfunc-8.5.1/src/arrayparams_boolout.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_booloutsimd.c` & `arrayfunc-8.5.1/src/arrayparams_booloutsimd.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_booloutsimd.h` & `arrayfunc-8.5.1/src/arrayparams_booloutsimd.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_cntcycrep.c` & `arrayfunc-8.5.1/src/arrayparams_cntcycrep.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_cntcycrep.h` & `arrayfunc-8.5.1/src/arrayparams_cntcycrep.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_comp.c` & `arrayfunc-8.5.1/src/arrayparams_comp.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_comp.h` & `arrayfunc-8.5.1/src/arrayparams_comp.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_compress.c` & `arrayfunc-8.5.1/src/arrayparams_compress.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_compress.h` & `arrayfunc-8.5.1/src/arrayparams_compress.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_convert.c` & `arrayfunc-8.5.1/src/arrayparams_convert.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_convert.h` & `arrayfunc-8.5.1/src/arrayparams_convert.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_droptakefilter.c` & `arrayfunc-8.5.1/src/arrayparams_droptakefilter.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_droptakefilter.h` & `arrayfunc-8.5.1/src/arrayparams_droptakefilter.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_findindices.c` & `arrayfunc-8.5.1/src/arrayparams_findindices.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_findindices.h` & `arrayfunc-8.5.1/src/arrayparams_findindices.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_one.c` & `arrayfunc-8.5.1/src/arrayparams_one.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_one.h` & `arrayfunc-8.5.1/src/arrayparams_one.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_onesimd.c` & `arrayfunc-8.5.1/src/arrayparams_onesimd.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_onesimd.h` & `arrayfunc-8.5.1/src/arrayparams_onesimd.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_special.c` & `arrayfunc-8.5.1/src/arrayparams_special.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_special.h` & `arrayfunc-8.5.1/src/arrayparams_special.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_three.c` & `arrayfunc-8.5.1/src/arrayparams_three.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_three.h` & `arrayfunc-8.5.1/src/arrayparams_three.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_two.c` & `arrayfunc-8.5.1/src/arrayparams_two.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/arrayparams_two.h` & `arrayfunc-8.5.1/src/arrayparams_two.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asin.c` & `arrayfunc-8.5.1/src/asin.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asinh.c` & `arrayfunc-8.5.1/src/asinh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum.c` & `arrayfunc-8.5.1/src/asum.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_defs.h` & `arrayfunc-8.5.1/src/asum_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_armv7.c` & `arrayfunc-8.5.1/src/asum_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_armv7.h` & `arrayfunc-8.5.1/src/asum_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_armv8.c` & `arrayfunc-8.5.1/src/asum_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_armv8.h` & `arrayfunc-8.5.1/src/asum_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_x86.c` & `arrayfunc-8.5.1/src/asum_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/asum_simd_x86.h` & `arrayfunc-8.5.1/src/asum_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/atan.c` & `arrayfunc-8.5.1/src/atan.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/atan2.c` & `arrayfunc-8.5.1/src/atan2.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/atanh.c` & `arrayfunc-8.5.1/src/atanh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ceil.c` & `arrayfunc-8.5.1/src/ceil.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ceil_simd_x86.c` & `arrayfunc-8.5.1/src/ceil_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ceil_simd_x86.h` & `arrayfunc-8.5.1/src/ceil_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/compress.c` & `arrayfunc-8.5.1/src/compress.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/convert.c` & `arrayfunc-8.5.1/src/convert.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/convguardbands.h` & `arrayfunc-8.5.1/src/convguardbands.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/copysign.c` & `arrayfunc-8.5.1/src/copysign.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/cos.c` & `arrayfunc-8.5.1/src/cos.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/cosh.c` & `arrayfunc-8.5.1/src/cosh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/count.c` & `arrayfunc-8.5.1/src/count.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/cycle.c` & `arrayfunc-8.5.1/src/cycle.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees.c` & `arrayfunc-8.5.1/src/degrees.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_armv7.c` & `arrayfunc-8.5.1/src/degrees_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_armv7.h` & `arrayfunc-8.5.1/src/degrees_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_armv8.c` & `arrayfunc-8.5.1/src/degrees_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_armv8.h` & `arrayfunc-8.5.1/src/degrees_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_x86.c` & `arrayfunc-8.5.1/src/degrees_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/degrees_simd_x86.h` & `arrayfunc-8.5.1/src/degrees_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/dropwhile.c` & `arrayfunc-8.5.1/src/dropwhile.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq.c` & `arrayfunc-8.5.1/src/eq.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_armv7.c` & `arrayfunc-8.5.1/src/eq_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_armv7.h` & `arrayfunc-8.5.1/src/eq_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_armv8.c` & `arrayfunc-8.5.1/src/eq_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_armv8.h` & `arrayfunc-8.5.1/src/eq_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_x86.c` & `arrayfunc-8.5.1/src/eq_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/eq_simd_x86.h` & `arrayfunc-8.5.1/src/eq_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/erf.c` & `arrayfunc-8.5.1/src/erf.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/erfc.c` & `arrayfunc-8.5.1/src/erfc.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/exp.c` & `arrayfunc-8.5.1/src/exp.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/expm1.c` & `arrayfunc-8.5.1/src/expm1.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/fabs.c` & `arrayfunc-8.5.1/src/fabs.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/factorial.c` & `arrayfunc-8.5.1/src/factorial.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex.c` & `arrayfunc-8.5.1/src/findindex.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_armv7.c` & `arrayfunc-8.5.1/src/findindex_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_armv7.h` & `arrayfunc-8.5.1/src/findindex_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_armv8.c` & `arrayfunc-8.5.1/src/findindex_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_armv8.h` & `arrayfunc-8.5.1/src/findindex_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_x86.c` & `arrayfunc-8.5.1/src/findindex_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindex_simd_x86.h` & `arrayfunc-8.5.1/src/findindex_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/findindices.c` & `arrayfunc-8.5.1/src/findindices.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/floor.c` & `arrayfunc-8.5.1/src/floor.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/floor_simd_x86.c` & `arrayfunc-8.5.1/src/floor_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/floor_simd_x86.h` & `arrayfunc-8.5.1/src/floor_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/floordiv.c` & `arrayfunc-8.5.1/src/floordiv.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/fma.c` & `arrayfunc-8.5.1/src/fma.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/fmod.c` & `arrayfunc-8.5.1/src/fmod.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gamma.c` & `arrayfunc-8.5.1/src/gamma.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge.c` & `arrayfunc-8.5.1/src/ge.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_armv7.c` & `arrayfunc-8.5.1/src/ge_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_armv7.h` & `arrayfunc-8.5.1/src/ge_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_armv8.c` & `arrayfunc-8.5.1/src/ge_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_armv8.h` & `arrayfunc-8.5.1/src/ge_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_x86.c` & `arrayfunc-8.5.1/src/ge_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ge_simd_x86.h` & `arrayfunc-8.5.1/src/ge_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt.c` & `arrayfunc-8.5.1/src/gt.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_armv7.c` & `arrayfunc-8.5.1/src/gt_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_armv7.h` & `arrayfunc-8.5.1/src/gt_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_armv8.c` & `arrayfunc-8.5.1/src/gt_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_armv8.h` & `arrayfunc-8.5.1/src/gt_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_x86.c` & `arrayfunc-8.5.1/src/gt_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/gt_simd_x86.h` & `arrayfunc-8.5.1/src/gt_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/hypot.c` & `arrayfunc-8.5.1/src/hypot.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert.c` & `arrayfunc-8.5.1/src/invert.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_armv7.c` & `arrayfunc-8.5.1/src/invert_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_armv7.h` & `arrayfunc-8.5.1/src/invert_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_armv8.c` & `arrayfunc-8.5.1/src/invert_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_armv8.h` & `arrayfunc-8.5.1/src/invert_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_x86.c` & `arrayfunc-8.5.1/src/invert_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/invert_simd_x86.h` & `arrayfunc-8.5.1/src/invert_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/isfinite.c` & `arrayfunc-8.5.1/src/isfinite.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/isinf.c` & `arrayfunc-8.5.1/src/isinf.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/isnan.c` & `arrayfunc-8.5.1/src/isnan.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ldexp.c` & `arrayfunc-8.5.1/src/ldexp.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le.c` & `arrayfunc-8.5.1/src/le.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_armv7.c` & `arrayfunc-8.5.1/src/le_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_armv7.h` & `arrayfunc-8.5.1/src/le_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_armv8.c` & `arrayfunc-8.5.1/src/le_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_armv8.h` & `arrayfunc-8.5.1/src/le_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_x86.c` & `arrayfunc-8.5.1/src/le_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/le_simd_x86.h` & `arrayfunc-8.5.1/src/le_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lgamma.c` & `arrayfunc-8.5.1/src/lgamma.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/log.c` & `arrayfunc-8.5.1/src/log.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/log10.c` & `arrayfunc-8.5.1/src/log10.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/log1p.c` & `arrayfunc-8.5.1/src/log1p.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/log2.c` & `arrayfunc-8.5.1/src/log2.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift.c` & `arrayfunc-8.5.1/src/lshift.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_defs.h` & `arrayfunc-8.5.1/src/lshift_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_armv7.c` & `arrayfunc-8.5.1/src/lshift_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_armv7.h` & `arrayfunc-8.5.1/src/lshift_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_armv8.c` & `arrayfunc-8.5.1/src/lshift_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_armv8.h` & `arrayfunc-8.5.1/src/lshift_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_x86.c` & `arrayfunc-8.5.1/src/lshift_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lshift_simd_x86.h` & `arrayfunc-8.5.1/src/lshift_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt.c` & `arrayfunc-8.5.1/src/lt.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_armv7.c` & `arrayfunc-8.5.1/src/lt_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_armv7.h` & `arrayfunc-8.5.1/src/lt_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_armv8.c` & `arrayfunc-8.5.1/src/lt_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_armv8.h` & `arrayfunc-8.5.1/src/lt_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_x86.c` & `arrayfunc-8.5.1/src/lt_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/lt_simd_x86.h` & `arrayfunc-8.5.1/src/lt_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mod.c` & `arrayfunc-8.5.1/src/mod.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul.c` & `arrayfunc-8.5.1/src/mul.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_defs.h` & `arrayfunc-8.5.1/src/mul_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_armv7.c` & `arrayfunc-8.5.1/src/mul_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_armv7.h` & `arrayfunc-8.5.1/src/mul_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_armv8.c` & `arrayfunc-8.5.1/src/mul_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_armv8.h` & `arrayfunc-8.5.1/src/mul_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_x86.c` & `arrayfunc-8.5.1/src/mul_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/mul_simd_x86.h` & `arrayfunc-8.5.1/src/mul_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne.c` & `arrayfunc-8.5.1/src/ne.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_armv7.c` & `arrayfunc-8.5.1/src/ne_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_armv7.h` & `arrayfunc-8.5.1/src/ne_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_armv8.c` & `arrayfunc-8.5.1/src/ne_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_armv8.h` & `arrayfunc-8.5.1/src/ne_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_x86.c` & `arrayfunc-8.5.1/src/ne_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/ne_simd_x86.h` & `arrayfunc-8.5.1/src/ne_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg.c` & `arrayfunc-8.5.1/src/neg.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_defs.h` & `arrayfunc-8.5.1/src/neg_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_armv7.c` & `arrayfunc-8.5.1/src/neg_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_armv7.h` & `arrayfunc-8.5.1/src/neg_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_armv8.c` & `arrayfunc-8.5.1/src/neg_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_armv8.h` & `arrayfunc-8.5.1/src/neg_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_x86.c` & `arrayfunc-8.5.1/src/neg_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/neg_simd_x86.h` & `arrayfunc-8.5.1/src/neg_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or_.c` & `arrayfunc-8.5.1/src/or_.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__defs.h` & `arrayfunc-8.5.1/src/or__defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_armv7.c` & `arrayfunc-8.5.1/src/or__simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_armv7.h` & `arrayfunc-8.5.1/src/or__simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_armv8.c` & `arrayfunc-8.5.1/src/or__simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_armv8.h` & `arrayfunc-8.5.1/src/or__simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_x86.c` & `arrayfunc-8.5.1/src/or__simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/or__simd_x86.h` & `arrayfunc-8.5.1/src/or__simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/pow.c` & `arrayfunc-8.5.1/src/pow.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/pow2.c` & `arrayfunc-8.5.1/src/pow2.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/pow3.c` & `arrayfunc-8.5.1/src/pow3.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians.c` & `arrayfunc-8.5.1/src/radians.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_armv7.c` & `arrayfunc-8.5.1/src/radians_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_armv7.h` & `arrayfunc-8.5.1/src/radians_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_armv8.c` & `arrayfunc-8.5.1/src/radians_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_armv8.h` & `arrayfunc-8.5.1/src/radians_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_x86.c` & `arrayfunc-8.5.1/src/radians_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/radians_simd_x86.h` & `arrayfunc-8.5.1/src/radians_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/repeat.c` & `arrayfunc-8.5.1/src/repeat.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift.c` & `arrayfunc-8.5.1/src/rshift.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_defs.h` & `arrayfunc-8.5.1/src/rshift_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_armv7.c` & `arrayfunc-8.5.1/src/rshift_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_armv7.h` & `arrayfunc-8.5.1/src/rshift_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_armv8.c` & `arrayfunc-8.5.1/src/rshift_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_armv8.h` & `arrayfunc-8.5.1/src/rshift_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_x86.c` & `arrayfunc-8.5.1/src/rshift_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/rshift_simd_x86.h` & `arrayfunc-8.5.1/src/rshift_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/simddefs.h` & `arrayfunc-8.5.1/src/simddefs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/simdsupport.c` & `arrayfunc-8.5.1/src/simdsupport.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sin.c` & `arrayfunc-8.5.1/src/sin.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sinh.c` & `arrayfunc-8.5.1/src/sinh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sqrt.c` & `arrayfunc-8.5.1/src/sqrt.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sqrt_simd_x86.c` & `arrayfunc-8.5.1/src/sqrt_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sqrt_simd_x86.h` & `arrayfunc-8.5.1/src/sqrt_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub.c` & `arrayfunc-8.5.1/src/sub.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_defs.h` & `arrayfunc-8.5.1/src/sub_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_armv7.c` & `arrayfunc-8.5.1/src/sub_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_armv7.h` & `arrayfunc-8.5.1/src/sub_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_armv8.c` & `arrayfunc-8.5.1/src/sub_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_armv8.h` & `arrayfunc-8.5.1/src/sub_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_x86.c` & `arrayfunc-8.5.1/src/sub_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/sub_simd_x86.h` & `arrayfunc-8.5.1/src/sub_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/takewhile.c` & `arrayfunc-8.5.1/src/takewhile.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/tan.c` & `arrayfunc-8.5.1/src/tan.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/tanh.c` & `arrayfunc-8.5.1/src/tanh.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/truediv.c` & `arrayfunc-8.5.1/src/truediv.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/trunc.c` & `arrayfunc-8.5.1/src/trunc.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/trunc_simd_x86.c` & `arrayfunc-8.5.1/src/trunc_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/trunc_simd_x86.h` & `arrayfunc-8.5.1/src/trunc_simd_x86.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor.c` & `arrayfunc-8.5.1/src/xor.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_defs.h` & `arrayfunc-8.5.1/src/xor_defs.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_armv7.c` & `arrayfunc-8.5.1/src/xor_simd_armv7.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_armv7.h` & `arrayfunc-8.5.1/src/xor_simd_armv7.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_armv8.c` & `arrayfunc-8.5.1/src/xor_simd_armv8.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_armv8.h` & `arrayfunc-8.5.1/src/xor_simd_armv8.h`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_x86.c` & `arrayfunc-8.5.1/src/xor_simd_x86.c`

 * *Files identical despite different names*

### Comparing `arrayfunc-8.5.0/src/xor_simd_x86.h` & `arrayfunc-8.5.1/src/xor_simd_x86.h`

 * *Files identical despite different names*


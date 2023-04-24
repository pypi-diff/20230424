# Comparing `tmp/refl1d-0.8.8.tar.gz` & `tmp/refl1d-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/refl1d-0.8.8.tar", last modified: Fri Sep  6 16:33:58 2019, max compression
+gzip compressed data, was "dist/refl1d-0.8.9.tar", last modified: Tue Oct 15 20:15:14 2019, max compression
```

## Comparing `refl1d-0.8.8.tar` & `refl1d-0.8.9.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:58.000000 refl1d-0.8.8/
--rwxr-xr-x   0 pkienzle (34766)    34766      830 2014-09-12 16:09:50.000000 refl1d-0.8.8/MANIFEST.in
--rw-r--r--   0 pkienzle (34766)    34766     2350 2019-09-06 16:33:58.000000 refl1d-0.8.8/PKG-INFO
--rwxr-xr-x   0 pkienzle (34766)    34766     1504 2018-08-28 16:24:05.000000 refl1d-0.8.8/README.rst
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:57.000000 refl1d-0.8.8/bin/
--rwxr-xr-x   0 pkienzle (34766)    34766      654 2013-12-13 15:57:45.000000 refl1d-0.8.8/bin/refl1d_cli.py
--rwxr-xr-x   0 pkienzle (34766)    34766     1676 2013-12-13 15:58:16.000000 refl1d-0.8.8/bin/refl1d_gui.py
--rwxr-xr-x   0 pkienzle (34766)    34766    19333 2017-12-01 14:32:12.000000 refl1d-0.8.8/master_builder.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:57.000000 refl1d-0.8.8/refl1d/
--rw-r--r--   0 pkienzle (34766)    34766      577 2019-03-01 20:58:01.000000 refl1d-0.8.8/refl1d/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     4162 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/abeles.py
--rw-r--r--   0 pkienzle (34766)    34766     2425 2017-05-18 22:27:56.000000 refl1d-0.8.8/refl1d/anstodata.py
--rw-r--r--   0 pkienzle (34766)    34766     9699 2017-12-04 21:03:21.000000 refl1d-0.8.8/refl1d/cheby.py
--rw-r--r--   0 pkienzle (34766)    34766     5035 2017-12-04 21:16:24.000000 refl1d-0.8.8/refl1d/composition.py
--rw-r--r--   0 pkienzle (34766)    34766     3020 2017-12-04 21:00:41.000000 refl1d-0.8.8/refl1d/corrtest.py
--rw-r--r--   0 pkienzle (34766)    34766     7939 2019-03-01 20:48:51.000000 refl1d-0.8.8/refl1d/dist.py
--rw-r--r--   0 pkienzle (34766)    34766    17224 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/errors.py
--rw-r--r--   0 pkienzle (34766)    34766    29808 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/experiment.py
--rw-r--r--   0 pkienzle (34766)    34766    15504 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/fasta.py
--rw-r--r--   0 pkienzle (34766)    34766     1931 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/fitplugin.py
--rw-r--r--   0 pkienzle (34766)    34766    10510 2018-02-09 22:54:54.000000 refl1d-0.8.8/refl1d/flayer.py
--rw-r--r--   0 pkienzle (34766)    34766     7800 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/freeform.py
--rw-r--r--   0 pkienzle (34766)    34766     3318 2019-02-19 23:06:29.000000 refl1d-0.8.8/refl1d/fresnel.py
--rw-r--r--   0 pkienzle (34766)    34766    10317 2018-12-18 19:40:07.000000 refl1d-0.8.8/refl1d/garefl.py
--rw-r--r--   0 pkienzle (34766)    34766    32040 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/instrument.py
--rw-r--r--   0 pkienzle (34766)    34766    14667 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/interface.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:58.000000 refl1d-0.8.8/refl1d/lib/
--rw-r--r--   0 pkienzle (34766)    34766     7378 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/calc_g_zs_cex.c
--rw-r--r--   0 pkienzle (34766)    34766    13622 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/contract_profile.cc
--rw-r--r--   0 pkienzle (34766)    34766     9417 2014-10-20 19:40:47.000000 refl1d-0.8.8/refl1d/lib/convolve.c
--rw-r--r--   0 pkienzle (34766)    34766     6807 2014-06-26 22:28:41.000000 refl1d-0.8.8/refl1d/lib/convolve_sampled.c
--rw-r--r--   0 pkienzle (34766)    34766    11400 2014-10-20 19:42:40.000000 refl1d-0.8.8/refl1d/lib/erf.c
--rw-r--r--   0 pkienzle (34766)    34766    16574 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/lib/magnetic.cc
--rwxr-xr-x   0 pkienzle (34766)    34766    11910 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/methods.cc
--rwxr-xr-x   0 pkienzle (34766)    34766     3983 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/methods.h
--rw-r--r--   0 pkienzle (34766)    34766     6150 2019-02-19 22:57:12.000000 refl1d-0.8.8/refl1d/lib/rebin.h
--rw-r--r--   0 pkienzle (34766)    34766     2701 2014-05-22 21:45:37.000000 refl1d-0.8.8/refl1d/lib/rebin2D.h
--rw-r--r--   0 pkienzle (34766)    34766     5499 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/reflcalc.h
--rwxr-xr-x   0 pkienzle (34766)    34766     5640 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/lib/reflectivity.cc
--rwxr-xr-x   0 pkienzle (34766)    34766     6781 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/lib/reflmodule.cc
--rw-r--r--   0 pkienzle (34766)    34766    11627 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/magnetic.py
--rw-r--r--   0 pkienzle (34766)    34766    11756 2018-05-17 21:14:27.000000 refl1d-0.8.8/refl1d/magnetism.py
--rw-r--r--   0 pkienzle (34766)    34766     1166 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/main.py
--rw-r--r--   0 pkienzle (34766)    34766    20517 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/material.py
--rw-r--r--   0 pkienzle (34766)    34766     1473 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/materialdb.py
--rw-r--r--   0 pkienzle (34766)    34766    24473 2019-02-25 23:03:24.000000 refl1d-0.8.8/refl1d/model.py
--rw-r--r--   0 pkienzle (34766)    34766     8796 2018-05-17 21:14:27.000000 refl1d-0.8.8/refl1d/mono.py
--rw-r--r--   0 pkienzle (34766)    34766     1989 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/names.py
--rw-r--r--   0 pkienzle (34766)    34766    11212 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/ncnrdata.py
--rw-r--r--   0 pkienzle (34766)    34766     3439 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/plottable.py
--rw-r--r--   0 pkienzle (34766)    34766    38347 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/polymer.py
--rw-r--r--   0 pkienzle (34766)    34766    64494 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/probe.py
--rw-r--r--   0 pkienzle (34766)    34766    24448 2018-02-12 22:48:41.000000 refl1d-0.8.8/refl1d/profile.py
--rw-r--r--   0 pkienzle (34766)    34766    10690 2018-12-10 17:07:16.000000 refl1d-0.8.8/refl1d/rebin.py
--rw-r--r--   0 pkienzle (34766)    34766    13372 2019-02-07 22:39:48.000000 refl1d-0.8.8/refl1d/reflectivity.py
--rw-r--r--   0 pkienzle (34766)    34766    12561 2018-09-26 15:50:42.000000 refl1d-0.8.8/refl1d/resolution.py
--rw-r--r--   0 pkienzle (34766)    34766     9375 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/snsdata.py
--rw-r--r--   0 pkienzle (34766)    34766    42103 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/staj.py
--rw-r--r--   0 pkienzle (34766)    34766    11501 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/stajconvert.py
--rw-r--r--   0 pkienzle (34766)    34766     4319 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/stitch.py
--rw-r--r--   0 pkienzle (34766)    34766     1410 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/support.py
--rw-r--r--   0 pkienzle (34766)    34766     1231 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/util.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:58.000000 refl1d-0.8.8/refl1d/view/
--rw-r--r--   0 pkienzle (34766)    34766       49 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766    15912 2018-06-14 19:20:12.000000 refl1d-0.8.8/refl1d/view/binder.py
--rw-r--r--   0 pkienzle (34766)    34766      348 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/config.py
--rwxr-xr-x   0 pkienzle (34766)    34766    10334 2019-09-06 16:32:52.000000 refl1d-0.8.8/refl1d/view/data_view.py
--rw-r--r--   0 pkienzle (34766)    34766      815 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/demo.py
--rw-r--r--   0 pkienzle (34766)    34766     9076 2013-12-24 20:15:53.000000 refl1d-0.8.8/refl1d/view/interactor.py
--rw-r--r--   0 pkienzle (34766)    34766     4221 2018-08-28 16:24:05.000000 refl1d-0.8.8/refl1d/view/interface.py
--rw-r--r--   0 pkienzle (34766)    34766     3570 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/layer.py
--rw-r--r--   0 pkienzle (34766)    34766    10506 2014-10-29 14:36:33.000000 refl1d-0.8.8/refl1d/view/layer_dialog.py
--rw-r--r--   0 pkienzle (34766)    34766     9545 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/view/model_view.py
--rw-r--r--   0 pkienzle (34766)    34766     6713 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/monoi.py
--rw-r--r--   0 pkienzle (34766)    34766     5453 2014-01-11 15:34:45.000000 refl1d-0.8.8/refl1d/view/polymeri.py
--rw-r--r--   0 pkienzle (34766)    34766     9731 2017-12-01 13:44:33.000000 refl1d-0.8.8/refl1d/view/profilei.py
--rw-r--r--   0 pkienzle (34766)    34766     1224 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/registry.py
--rw-r--r--   0 pkienzle (34766)    34766     5114 2013-12-13 13:41:07.000000 refl1d-0.8.8/refl1d/view/thickness.py
--rw-r--r--   0 pkienzle (34766)    34766     2120 2014-10-29 14:36:48.000000 refl1d-0.8.8/refl1d/view/util.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-09-06 16:33:57.000000 refl1d-0.8.8/refl1d.egg-info/
--rw-r--r--   0 pkienzle (34766)    34766     2350 2019-09-06 16:33:53.000000 refl1d-0.8.8/refl1d.egg-info/PKG-INFO
--rw-r--r--   0 pkienzle (34766)    34766     1689 2019-09-06 16:33:54.000000 refl1d-0.8.8/refl1d.egg-info/SOURCES.txt
--rw-r--r--   0 pkienzle (34766)    34766        1 2019-09-06 16:33:53.000000 refl1d-0.8.8/refl1d.egg-info/dependency_links.txt
--rw-r--r--   0 pkienzle (34766)    34766       88 2019-09-06 16:33:53.000000 refl1d-0.8.8/refl1d.egg-info/entry_points.txt
--rw-r--r--   0 pkienzle (34766)    34766       60 2019-09-06 16:33:53.000000 refl1d-0.8.8/refl1d.egg-info/requires.txt
--rw-r--r--   0 pkienzle (34766)    34766        7 2019-09-06 16:33:53.000000 refl1d-0.8.8/refl1d.egg-info/top_level.txt
--rwxr-xr-x   0 pkienzle (34766)    34766     9808 2016-06-13 16:32:34.000000 refl1d-0.8.8/refl1d.iss
--rw-r--r--   0 pkienzle (34766)    34766       38 2019-09-06 16:33:58.000000 refl1d-0.8.8/setup.cfg
--rwxr-xr-x   0 pkienzle (34766)    34766     4017 2019-09-06 16:32:52.000000 refl1d-0.8.8/setup.py
--rwxr-xr-x   0 pkienzle (34766)    34766    12010 2016-06-17 22:47:00.000000 refl1d-0.8.8/setup_py2exe.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:14.000000 refl1d-0.8.9/
+-rwxr-xr-x   0 pkienzle (34766)    34766      830 2014-09-12 16:09:50.000000 refl1d-0.8.9/MANIFEST.in
+-rw-r--r--   0 pkienzle (34766)    34766     2350 2019-10-15 20:15:14.000000 refl1d-0.8.9/PKG-INFO
+-rwxr-xr-x   0 pkienzle (34766)    34766     1504 2018-08-28 16:24:05.000000 refl1d-0.8.9/README.rst
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:13.000000 refl1d-0.8.9/bin/
+-rwxr-xr-x   0 pkienzle (34766)    34766      654 2013-12-13 15:57:45.000000 refl1d-0.8.9/bin/refl1d_cli.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     1676 2013-12-13 15:58:16.000000 refl1d-0.8.9/bin/refl1d_gui.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    19333 2017-12-01 14:32:12.000000 refl1d-0.8.9/master_builder.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:13.000000 refl1d-0.8.9/refl1d/
+-rw-r--r--   0 pkienzle (34766)    34766      577 2019-10-15 20:13:45.000000 refl1d-0.8.9/refl1d/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     4973 2019-09-12 17:58:02.000000 refl1d-0.8.9/refl1d/abeles.py
+-rw-r--r--   0 pkienzle (34766)    34766     2425 2017-05-18 22:27:56.000000 refl1d-0.8.9/refl1d/anstodata.py
+-rw-r--r--   0 pkienzle (34766)    34766     9699 2017-12-04 21:03:21.000000 refl1d-0.8.9/refl1d/cheby.py
+-rw-r--r--   0 pkienzle (34766)    34766     5035 2017-12-04 21:16:24.000000 refl1d-0.8.9/refl1d/composition.py
+-rw-r--r--   0 pkienzle (34766)    34766     3020 2017-12-04 21:00:41.000000 refl1d-0.8.9/refl1d/corrtest.py
+-rw-r--r--   0 pkienzle (34766)    34766     8498 2019-09-30 20:14:13.000000 refl1d-0.8.9/refl1d/dist.py
+-rw-r--r--   0 pkienzle (34766)    34766    17269 2019-09-06 16:35:13.000000 refl1d-0.8.9/refl1d/errors.py
+-rw-r--r--   0 pkienzle (34766)    34766    30928 2019-09-30 21:06:40.000000 refl1d-0.8.9/refl1d/experiment.py
+-rw-r--r--   0 pkienzle (34766)    34766    15504 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/fasta.py
+-rw-r--r--   0 pkienzle (34766)    34766     1931 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/fitplugin.py
+-rw-r--r--   0 pkienzle (34766)    34766    10510 2018-02-09 22:54:54.000000 refl1d-0.8.9/refl1d/flayer.py
+-rw-r--r--   0 pkienzle (34766)    34766     7800 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/freeform.py
+-rw-r--r--   0 pkienzle (34766)    34766     3318 2019-02-19 23:06:29.000000 refl1d-0.8.9/refl1d/fresnel.py
+-rw-r--r--   0 pkienzle (34766)    34766    10317 2018-12-18 19:40:07.000000 refl1d-0.8.9/refl1d/garefl.py
+-rw-r--r--   0 pkienzle (34766)    34766    32029 2019-09-06 16:35:13.000000 refl1d-0.8.9/refl1d/instrument.py
+-rw-r--r--   0 pkienzle (34766)    34766    14667 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/interface.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:14.000000 refl1d-0.8.9/refl1d/lib/
+-rw-r--r--   0 pkienzle (34766)    34766     7378 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/calc_g_zs_cex.c
+-rw-r--r--   0 pkienzle (34766)    34766    13622 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/contract_profile.cc
+-rw-r--r--   0 pkienzle (34766)    34766     9417 2014-10-20 19:40:47.000000 refl1d-0.8.9/refl1d/lib/convolve.c
+-rw-r--r--   0 pkienzle (34766)    34766     6807 2014-06-26 22:28:41.000000 refl1d-0.8.9/refl1d/lib/convolve_sampled.c
+-rw-r--r--   0 pkienzle (34766)    34766    11400 2014-10-20 19:42:40.000000 refl1d-0.8.9/refl1d/lib/erf.c
+-rw-r--r--   0 pkienzle (34766)    34766    16574 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/lib/magnetic.cc
+-rwxr-xr-x   0 pkienzle (34766)    34766    11910 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/methods.cc
+-rwxr-xr-x   0 pkienzle (34766)    34766     3983 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/methods.h
+-rw-r--r--   0 pkienzle (34766)    34766     6150 2019-02-19 22:57:12.000000 refl1d-0.8.9/refl1d/lib/rebin.h
+-rw-r--r--   0 pkienzle (34766)    34766     2701 2014-05-22 21:45:37.000000 refl1d-0.8.9/refl1d/lib/rebin2D.h
+-rw-r--r--   0 pkienzle (34766)    34766     5499 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/reflcalc.h
+-rwxr-xr-x   0 pkienzle (34766)    34766     5640 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/lib/reflectivity.cc
+-rwxr-xr-x   0 pkienzle (34766)    34766     6781 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/lib/reflmodule.cc
+-rw-r--r--   0 pkienzle (34766)    34766    11627 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/magnetic.py
+-rw-r--r--   0 pkienzle (34766)    34766    17257 2019-10-10 21:37:41.000000 refl1d-0.8.9/refl1d/magnetism.py
+-rw-r--r--   0 pkienzle (34766)    34766     1166 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/main.py
+-rw-r--r--   0 pkienzle (34766)    34766    22130 2019-10-10 21:16:17.000000 refl1d-0.8.9/refl1d/material.py
+-rw-r--r--   0 pkienzle (34766)    34766     1473 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/materialdb.py
+-rw-r--r--   0 pkienzle (34766)    34766    24308 2019-09-30 21:53:22.000000 refl1d-0.8.9/refl1d/model.py
+-rw-r--r--   0 pkienzle (34766)    34766     8796 2018-05-17 21:14:27.000000 refl1d-0.8.9/refl1d/mono.py
+-rw-r--r--   0 pkienzle (34766)    34766     1989 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/names.py
+-rw-r--r--   0 pkienzle (34766)    34766    11212 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/ncnrdata.py
+-rw-r--r--   0 pkienzle (34766)    34766     3439 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/plottable.py
+-rw-r--r--   0 pkienzle (34766)    34766    38032 2019-09-13 20:09:33.000000 refl1d-0.8.9/refl1d/polymer.py
+-rw-r--r--   0 pkienzle (34766)    34766    69653 2019-10-10 19:39:57.000000 refl1d-0.8.9/refl1d/probe.py
+-rw-r--r--   0 pkienzle (34766)    34766    24629 2019-10-10 21:05:19.000000 refl1d-0.8.9/refl1d/profile.py
+-rw-r--r--   0 pkienzle (34766)    34766    10690 2018-12-10 17:07:16.000000 refl1d-0.8.9/refl1d/rebin.py
+-rw-r--r--   0 pkienzle (34766)    34766    12093 2019-09-12 17:56:04.000000 refl1d-0.8.9/refl1d/refl_tr.py
+-rw-r--r--   0 pkienzle (34766)    34766    13372 2019-02-07 22:39:48.000000 refl1d-0.8.9/refl1d/reflectivity.py
+-rw-r--r--   0 pkienzle (34766)    34766    12561 2018-09-26 15:50:42.000000 refl1d-0.8.9/refl1d/resolution.py
+-rw-r--r--   0 pkienzle (34766)    34766     9375 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/snsdata.py
+-rw-r--r--   0 pkienzle (34766)    34766    42103 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/staj.py
+-rw-r--r--   0 pkienzle (34766)    34766    11501 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/stajconvert.py
+-rw-r--r--   0 pkienzle (34766)    34766     4319 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/stitch.py
+-rw-r--r--   0 pkienzle (34766)    34766     1410 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/support.py
+-rw-r--r--   0 pkienzle (34766)    34766     1389 2019-09-06 16:35:13.000000 refl1d-0.8.9/refl1d/util.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:14.000000 refl1d-0.8.9/refl1d/view/
+-rw-r--r--   0 pkienzle (34766)    34766       49 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766    15912 2018-06-14 19:20:12.000000 refl1d-0.8.9/refl1d/view/binder.py
+-rw-r--r--   0 pkienzle (34766)    34766      348 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/config.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    10566 2019-09-06 16:35:13.000000 refl1d-0.8.9/refl1d/view/data_view.py
+-rw-r--r--   0 pkienzle (34766)    34766      815 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/demo.py
+-rw-r--r--   0 pkienzle (34766)    34766     9076 2013-12-24 20:15:53.000000 refl1d-0.8.9/refl1d/view/interactor.py
+-rw-r--r--   0 pkienzle (34766)    34766     4221 2018-08-28 16:24:05.000000 refl1d-0.8.9/refl1d/view/interface.py
+-rw-r--r--   0 pkienzle (34766)    34766     3570 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/layer.py
+-rw-r--r--   0 pkienzle (34766)    34766    10506 2014-10-29 14:36:33.000000 refl1d-0.8.9/refl1d/view/layer_dialog.py
+-rw-r--r--   0 pkienzle (34766)    34766     9545 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/view/model_view.py
+-rw-r--r--   0 pkienzle (34766)    34766     6713 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/monoi.py
+-rw-r--r--   0 pkienzle (34766)    34766     5453 2014-01-11 15:34:45.000000 refl1d-0.8.9/refl1d/view/polymeri.py
+-rw-r--r--   0 pkienzle (34766)    34766     9731 2017-12-01 13:44:33.000000 refl1d-0.8.9/refl1d/view/profilei.py
+-rw-r--r--   0 pkienzle (34766)    34766     1224 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/registry.py
+-rw-r--r--   0 pkienzle (34766)    34766     5114 2013-12-13 13:41:07.000000 refl1d-0.8.9/refl1d/view/thickness.py
+-rw-r--r--   0 pkienzle (34766)    34766     2120 2014-10-29 14:36:48.000000 refl1d-0.8.9/refl1d/view/util.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2019-10-15 20:15:13.000000 refl1d-0.8.9/refl1d.egg-info/
+-rw-r--r--   0 pkienzle (34766)    34766     2350 2019-10-15 20:15:09.000000 refl1d-0.8.9/refl1d.egg-info/PKG-INFO
+-rw-r--r--   0 pkienzle (34766)    34766     1707 2019-10-15 20:15:10.000000 refl1d-0.8.9/refl1d.egg-info/SOURCES.txt
+-rw-r--r--   0 pkienzle (34766)    34766        1 2019-10-15 20:15:09.000000 refl1d-0.8.9/refl1d.egg-info/dependency_links.txt
+-rw-r--r--   0 pkienzle (34766)    34766       88 2019-10-15 20:15:09.000000 refl1d-0.8.9/refl1d.egg-info/entry_points.txt
+-rw-r--r--   0 pkienzle (34766)    34766       60 2019-10-15 20:15:09.000000 refl1d-0.8.9/refl1d.egg-info/requires.txt
+-rw-r--r--   0 pkienzle (34766)    34766        7 2019-10-15 20:15:09.000000 refl1d-0.8.9/refl1d.egg-info/top_level.txt
+-rwxr-xr-x   0 pkienzle (34766)    34766     9808 2016-06-13 16:32:34.000000 refl1d-0.8.9/refl1d.iss
+-rw-r--r--   0 pkienzle (34766)    34766       38 2019-10-15 20:15:14.000000 refl1d-0.8.9/setup.cfg
+-rwxr-xr-x   0 pkienzle (34766)    34766     4085 2019-09-06 16:35:13.000000 refl1d-0.8.9/setup.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    12010 2016-06-17 22:47:00.000000 refl1d-0.8.9/setup_py2exe.py
```

### Comparing `refl1d-0.8.8/MANIFEST.in` & `refl1d-0.8.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/PKG-INFO` & `refl1d-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: refl1d
-Version: 0.8.8
+Version: 0.8.9
 Summary: 1-D reflectometry modeling
 Home-page: http://www.reflectometry.org/danse/model1d.html
 Author: Paul Kienzle
 Author-email: pkienzle@nist.gov
 License: UNKNOWN
 Description: Refl1D
         ======
```

### Comparing `refl1d-0.8.8/README.rst` & `refl1d-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/bin/refl1d_cli.py` & `refl1d-0.8.9/bin/refl1d_cli.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/bin/refl1d_gui.py` & `refl1d-0.8.9/bin/refl1d_gui.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/master_builder.py` & `refl1d-0.8.9/master_builder.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/__init__.py` & `refl1d-0.8.9/refl1d/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 parameters adjusted to achieve the best fit.
 
 A graphical interface allows direct manipulation of the model profiles.
 
 See http://www.reflectometry.org/danse/reflectometry for online manuals.
 """
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
```

### Comparing `refl1d-0.8.8/refl1d/anstodata.py` & `refl1d-0.8.9/refl1d/anstodata.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/cheby.py` & `refl1d-0.8.9/refl1d/cheby.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/composition.py` & `refl1d-0.8.9/refl1d/composition.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/corrtest.py` & `refl1d-0.8.9/refl1d/corrtest.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/dist.py` & `refl1d-0.8.9/refl1d/dist.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,17 +67,21 @@
         self.args = [Parameter.default(a) for a in args]
 
     def parameters(self):
         return {'args': self.args, 'loc': self.loc, 'scale': self.scale}
 
     def to_dict(self):
         return {
+            'type': type(self).__name__,
+            'edges': self.edges.tolist(),
+            'cdf': self.cdf.__name__,  # TODO: can't lookup name
             'args': [s.to_dict() for s in self.args],
             'loc': self.loc.to_dict(),
             'scale': self.scale.to_dict(),
+            'truncated': self.truncated,
             }
 
     def __iter__(self):
         # Find weights and normalize the sum to 1
         centers = (self.edges[:-1]+self.edges[1:])/2
         loc = self.loc.value
         scale = self.scale.value
@@ -94,18 +98,20 @@
             idx = weights > 0
             return iter(zip(centers[idx], weights[idx]))
 
 class DistributionExperiment(ExperimentBase):
     """
     Compute reflectivity from a non-uniform sample.
 
-    The parameter *P* takes on the values from *distribution* in the
-    context of *experiment*. Clearly, *P* should not be a fitted
-    parameter, but the remaining experiment parameters can be fitted,
-    as can the parameters of the distribution.
+    *P* is the target parameter for the model, which takes on the values
+    from *distribution* in the context of the *experiment*.  The result
+    is the weighted sum of the theory curves after setting *P.value* to
+    each distribution value. Clearly, *P* should not be a fitted parameter,
+    but the remaining experiment parameters can be fitted, as can the
+    parameters of the distribution.
 
     If *coherent* is true, then the reflectivity of the mixture is computed
     from the coherent sum rather than the incoherent sum.
 
     See :class:`Weights` for a description of how to set up the distribution.
     """
     def __init__(self, experiment=None, P=None, distribution=None,
@@ -124,16 +130,20 @@
         return {
             'distribution': self.distribution.parameters(),
             'experiment': self.experiment.parameters(),
             }
 
     def to_dict(self):
         return {
+            'type': type(self).__name__,
+            'P': str(self.P),  # TODO: parameter name may not be unique
             'distribution': self.distribution.to_dict(),
             'experiment': self.experiment.to_dict(),
+            # Don't need self.probe since it is the experiment probe.
+            'coherent': self.coherent,
             }
 
     def reflectivity(self, resolution=True, interpolation=0):
         key = ("reflectivity", resolution, interpolation)
         if key not in self._cache:
             calc_R = 0
             for x, w in self.distribution:
```

### Comparing `refl1d-0.8.8/refl1d/errors.py` & `refl1d-0.8.9/refl1d/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,16 @@
            'show_errors', 'show_profiles', 'show_residuals',
           ]
 
 import numpy as np
 from bumps.plotutil import next_color, dhsv, plot_quantiles, form_quantiles
 from bumps.errplot import reload_errors
 
+from .util import asbytes
+
 #_CONTOURS = (68, 95, 100)
 #_CONTOURS = (57, 68, 84, 95, 100)
 _CONTOURS = (68, 95)
 
 def run_errors(**kw):
     """
     Argument parser for generating error plots from models.
@@ -325,17 +327,17 @@
         # TODO: should have columns for R, dR as well.
         data = np.vstack((x, r[:, 0], np.reshape(q, (-1, q.shape[2]))))
         columns = ["q", "best"] + list("%g%%"%v for v in 100*p.flatten())
         _write_file(save+"_resid_contour%d.dat"%k, data, title, columns)
         k += 1
 
 def _write_file(path, data, title, columns):
-    with open(path, "wt") as fid:
-        fid.write("# "+title+"\n")
-        fid.write("# "+" ".join(columns)+"\n")
+    with open(path, "wb") as fid:
+        fid.write(asbytes("# "+title+"\n"))
+        fid.write(asbytes("# "+" ".join(columns)+"\n"))
         np.savetxt(fid, data.T)
 
 
 # ===== Plotting functions =====
 
 def _profiles_labels(magnetic):
     import pylab
```

### Comparing `refl1d-0.8.8/refl1d/experiment.py` & `refl1d-0.8.9/refl1d/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 Experiment definition
 
 An experiment combines the sample definition with a measurement probe
 to create a fittable reflectometry model.
 """
 from __future__ import division, print_function
 
-from math import pi, log10, floor
+import sys
 import os
+from math import pi, log10, floor
 import traceback
 import json
 from warnings import warn
 
 import numpy
 from bumps import parameter
 
+from . import material, profile
+from . import __version__
 from .reflectivity import reflectivity_amplitude as reflamp
 from .reflectivity import magnetic_amplitude as reflmag
 #print("Using pure python reflectivity calculator")
 #from .abeles import refl as reflamp
-from . import material, profile
-from . import __version__
+from .util import asbytes
 
 def plot_sample(sample, instrument=None, roughness_limit=0):
     """
     Quick plot of a reflectivity sample and the corresponding reflectivity.
     """
     if instrument is None:
         from .probe import NeutronProbe
@@ -44,15 +46,15 @@
     _probe_cache = None
     _substrate = None
     _surface = None
     def parameters(self):
         raise NotImplementedError()
 
     def to_dict(self):
-        return None
+        raise NotImplementedError()
 
     def reflectivity(self, resolution=True, interpolation=0):
         raise NotImplementedError()
 
     def magnetic_step_profile(self):
         raise NotImplementedError()
 
@@ -184,23 +186,27 @@
         """Restore original data after resynthesis."""
         self.probe.restore_data()
 
     def write_data(self, filename, **kw):
         """Save simulated data to a file"""
         self.probe.write_data(filename, **kw)
 
-    def simulate_data(self, noise=2):
+    def simulate_data(self, noise=2.):
         """
-        Simulate a random data set for the model
+        Simulate a random data set for the model.
+
+        This sets R and dR according to the noise level given.
 
         **Parameters:**
 
-        *noise* = 2 : float | %
-            Percentage noise to add to the data.
+        *noise*: float or array or None | %
+            dR/R uncertainty as a percentage.  If noise is set to None, then
+            use dR from the data if present, otherwise default to 2%.
         """
+        # TODO: can't do perfect data while setting default uncertainty
         theory = self.reflectivity(resolution=True)
         self.probe.simulate_data(theory, noise=noise)
 
     def _set_name(self, name):
         self._name = name
 
     def _get_name(self):
@@ -233,64 +239,65 @@
             self._save_magnetic(basename)
         else:
             self._save_nonmagnetic(basename)
 
     def _save_magnetic(self, basename):
         # Slabs
         A = numpy.array(self.magnetic_slabs())
-        fid = open(basename+"-slabs.dat", "w")
-        fid.write("# %17s %20s %20s %20s %20s %20s\n"
-                  %("thickness (A)", "interface (A)", "rho (1e-6/A^2)", "irho (1e-6/A^2)",
+        header = ("# %17s %20s %20s %20s %20s %20s\n"
+                  %("thickness (A)", "interface (A)",
+                    "rho (1e-6/A^2)", "irho (1e-6/A^2)",
                     "rhoM (1e-6/A^2)", "theta (degrees)"))
-        numpy.savetxt(fid, A.T, fmt="%20.15g")
-        fid.close()
+        with open(basename+"-slabs.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%20.15g")
 
         # Step profile
         A = numpy.array(self.magnetic_step_profile())
-        fid = open(basename+"-steps.dat", "w")
-        fid.write("# %10s %12s %12s %12s %12s\n"
+        header = ("# %10s %12s %12s %12s %12s\n"
                   %("z (A)", "rho (1e-6/A2)", "irho (1e-6/A2)",
                     "rhoM (1e-6/A2)", "theta (degrees)"))
-        numpy.savetxt(fid, A.T, fmt="%12.8f")
-        fid.close()
+        with open(basename+"-steps.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%12.8f")
 
         # Smooth profile
         A = numpy.array(self.magnetic_smooth_profile())
-        fid = open(basename+"-profile.dat", "w")
-        fid.write("# %10s %12s %12s %12s %12s\n"
+        header = ("# %10s %12s %12s %12s %12s\n"
                   %("z (A)", "rho (1e-6/A2)", "irho (1e-6/A2)",
                     "rhoM (1e-6/A2)", "theta (degrees)"))
-        numpy.savetxt(fid, A.T, fmt="%12.8f")
-        fid.close()
+        with open(basename+"-profile.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%12.8f")
 
     def _save_nonmagnetic(self, basename):
         # Slabs
         A = numpy.array(self.slabs())
-        fid = open(basename+"-slabs.dat", "w")
-        fid.write("# %17s %20s %20s %20s\n"
+        header = ("# %17s %20s %20s %20s\n"
                   %("thickness (A)", "interface (A)", "rho (1e-6/A^2)",
                     "irho (1e-6/A^2)"))
-        numpy.savetxt(fid, A.T, fmt="%20.15g")
-        fid.close()
+        with open(basename+"-slabs.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%20.15g")
 
         # Step profile
         A = numpy.array(self.step_profile())
-        fid = open(basename+"-steps.dat", "w")
-        fid.write("# %10s %20s %20s\n"
+        header = ("# %10s %20s %20s\n"
                   %("z (A)", "rho (1e-6/A2)", "irho (1e-6/A2)"))
-        numpy.savetxt(fid, A.T, fmt="%12.8f")
-        fid.close()
+        with open(basename+"-steps.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%12.8f")
 
         # Smooth profile
         A = numpy.array(self.smooth_profile())
-        fid = open(basename+"-profile.dat", "w")
-        fid.write("# %10s %12s %12s\n"
+        header = ("# %10s %12s %12s\n"
                   %("z (A)", "rho (1e-6/A2)", "irho (1e-6/A2)"))
-        numpy.savetxt(fid, A.T, fmt="%12.8f")
-        fid.close()
+        with open(basename+"-profile.dat", "wb") as fid:
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%12.8f")
 
     def save_refl(self, basename):
         # Reflectivity
         theory = self.reflectivity()
         self.probe.save(filename=basename+"-refl.dat", theory=theory,
                         substrate=self._substrate, surface=self._surface)
         if self.interpolation > 0:
@@ -344,14 +351,16 @@
     maximum of the non-uniform profile within the slab will be smaller
     than *dA*.  A *dA* of 10 gives coarse slabs.  If *dA* is not provided
     then each profile step forms its own slab.  The *dA* condition will
     also apply to the slab approximation to the interfaces.
 
     *interpolation* indicates the number of points to plot in between
     existing points.
+
+    *smoothness* **DEPRECATED** This parameter is not used.
     """
     profile_shift = 0
     def __init__(self, sample=None, probe=None, name=None,
                  roughness_limit=0, dz=None, dA=None,
                  step_interfaces=None, smoothness=None,
                  interpolation=0):
         # Note: smoothness ignored
@@ -384,16 +393,23 @@
         return {
             'sample': self.sample.parameters(),
             'probe': self.probe.parameters(),
             }
 
     def to_dict(self):
         return {
+            'type': type(self).__name__,
             'sample': self.sample.to_dict(),
             'probe': self.probe.to_dict(),
+            'roughness_limit': self.roughness_limit,
+            'dz': self.dz,
+            'dA': self.dA,
+            'step_interfaces': self.step_interfaces,
+            'interpolation': self.interpolation,
+            'name': self.name,
             }
 
     def _render_slabs(self):
         """
         Build a slab description of the model from the individual layers.
         """
         key = 'rendered'
@@ -550,17 +566,18 @@
             if self.probe.R is not None:
                 datafile = getattr(self.probe, 'filename', basename+".refl")
             else:
                 datafile = None
             save_mlayer(self, basename+".staj", datafile=datafile)
             probe = self.probe
             datafile = os.path.join(os.path.dirname(basename), os.path.basename(datafile))
-            fid = open(datafile, "w")
-            fid.write("# Q R dR\n")
-            numpy.savetxt(fid, numpy.vstack((probe.Qo, probe.R, probe.dR)).T)
+            header = ("# Q R dR\n")
+            with open(datafile, "wb") as fid:
+                fid.write(asbytes(header))
+                numpy.savetxt(fid, numpy.vstack((probe.Qo, probe.R, probe.dR)).T)
             fid.close()
         except Exception:
             print("==== could not save staj file ====")
             traceback.print_exc()
 
     def plot_profile(self, plot_shift=None):
         import pylab
@@ -653,17 +670,22 @@
             'samples': [s.parameters() for s in self.samples],
             'ratio': self.ratio,
             'probe': self.probe.parameters(),
             }
 
     def to_dict(self):
         return {
+            'type': type(self).__name__,
             'samples': [s.to_dict() for s in self.samples],
             'ratio': [s.to_dict() for s in self.ratio],
             'probe': self.probe.to_dict(),
+            'parts': [s.to_dict() for s in self.parts],
+            'coherent': self.coherent,
+            'interpolation': self.interpolation,
+            'name': self.name,
             }
 
     def _reflamp(self):
         """
         Calculate the amplitude of the reflectivity...
 
         For an incoherent sum, we want to add the squares of the amplitudes,
```

### Comparing `refl1d-0.8.8/refl1d/fasta.py` & `refl1d-0.8.9/refl1d/fasta.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/fitplugin.py` & `refl1d-0.8.9/refl1d/fitplugin.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/flayer.py` & `refl1d-0.8.9/refl1d/flayer.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/freeform.py` & `refl1d-0.8.9/refl1d/freeform.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/fresnel.py` & `refl1d-0.8.9/refl1d/fresnel.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/garefl.py` & `refl1d-0.8.9/refl1d/garefl.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/instrument.py` & `refl1d-0.8.9/refl1d/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,15 @@
 
             if not normalize:
                 #Ci = 1./max(R)
                 R, dR = R*Ci, dR*Ci
                 probe.background.value *= Ci
                 probe.intensity.value = Ci
 
-            probe.Ro = probe.R = R
+            probe.R = R
             probe.dR = dR
             probes.append(probe)
 
         return Experiment(sample=sample, probe=ProbeSet(probes))
 
     def resolution(self, L, dL, **kw):
         """
```

### Comparing `refl1d-0.8.8/refl1d/interface.py` & `refl1d-0.8.9/refl1d/interface.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/calc_g_zs_cex.c` & `refl1d-0.8.9/refl1d/lib/calc_g_zs_cex.c`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/contract_profile.cc` & `refl1d-0.8.9/refl1d/lib/contract_profile.cc`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/convolve.c` & `refl1d-0.8.9/refl1d/lib/convolve.c`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/convolve_sampled.c` & `refl1d-0.8.9/refl1d/lib/convolve_sampled.c`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/erf.c` & `refl1d-0.8.9/refl1d/lib/erf.c`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/magnetic.cc` & `refl1d-0.8.9/refl1d/lib/magnetic.cc`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/methods.cc` & `refl1d-0.8.9/refl1d/lib/methods.cc`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/methods.h` & `refl1d-0.8.9/refl1d/lib/methods.h`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/rebin.h` & `refl1d-0.8.9/refl1d/lib/rebin.h`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/rebin2D.h` & `refl1d-0.8.9/refl1d/lib/rebin2D.h`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/reflcalc.h` & `refl1d-0.8.9/refl1d/lib/reflcalc.h`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/reflectivity.cc` & `refl1d-0.8.9/refl1d/lib/reflectivity.cc`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/lib/reflmodule.cc` & `refl1d-0.8.9/refl1d/lib/reflmodule.cc`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/magnetic.py` & `refl1d-0.8.9/refl1d/magnetic.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/magnetism.py` & `refl1d-0.8.9/refl1d/magnetism.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This program is public domain
 # Author: Paul Kienzle
-"""
+r"""
 Magnetic modeling for 1-D reflectometry.
 
 Magnetic properties are tied to the structural description of the
 but only loosely.
 
 There may be dead regions near the interfaces of magnetic materials.
 
@@ -42,22 +42,25 @@
 import numpy
 from numpy import inf
 from bumps.parameter import Parameter, flatten
 from bumps.mono import monospline
 
 from .model import Layer, Stack
 
+def _optional_dict(p):
+    return p.to_dict() if p is not None else None
+
 class BaseMagnetism(object):
     """
     Magnetic properties of the layer.
 
     Magnetism is attached to set of nuclear layers by setting the
     *magnetism* property of the first layer to the rendered for the
-    magnetic profile, and setting the *magnetism.extent* property to
-    say how many layers it extends over.
+    magnetic profile, and setting *extent* to the number of nuclear
+    layers attached to the magnetism object.
 
     *dead_below* and *dead_above* are dead regions within the magnetic
     extent, which allow you to shift the magnetic interfaces relative
     to the nuclear interfaces.
 
     *interface_below* and *interface_above* are the interface widths
     for the magnetic layer, which default to the interface widths for
@@ -81,19 +84,31 @@
                                                 name=name+"  interfaceM above")
         self.interface_below = interface_below
         self.interface_above = interface_above
         self.name = name
         self.extent = extent
 
     def parameters(self):
-        return {'dead_below':self.dead_below,
-                'dead_above':self.dead_above,
-                'interface_below':self.interface_below,
-                'interface_above':self.interface_above,
-               }
+        return {
+            'dead_below': self.dead_below,
+            'dead_above': self.dead_above,
+            'interface_below': self.interface_below,
+            'interface_above': self.interface_above,
+            }
+
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+            'extent': self.extent,
+            'name': self.name,
+            'dead_below': self.dead_below.to_dict(),
+            'dead_above': self.dead_above.to_dict(),
+            'interface_below': _optional_dict(self.interface_below),
+            'interface_above': _optional_dict(self.interface_above),
+        }
 
     def set_layer_name(self, name):
         """
         Update the names of the magnetic parameters with the name of the
         layer if it has not already been set.  This is necessary since we don't
         know the layer name until after we have constructed the magnetism object.
         """
@@ -101,96 +116,189 @@
             for p in flatten(self.parameters()):
                 p.name = p.name.replace("LAYER", name)
             self.name = name
 
 class Magnetism(BaseMagnetism):
     """
     Region of constant magnetism.
+
+    *rhoM* is the magnetic SLD the layer. Default is :code:`rhoM=0`.
+
+    *thetaM* is the magnetic angle for the layer. Default is :code:`thetaM=270`.
+
+    *name* is the base name for the various layer parameters.
+
+    *extent* defines the number of nuclear layers covered by the magnetic layer.
+
+    *dead_above* and *dead_below* define magnetically dead layers at the
+    nuclear boundaries.  These can be negative if magnetism extends beyond
+    the nuclear boundary.
+
+    *interface_above* and *interface_below* define the magnetic interface
+    at the boundaries, if it is different from the nuclear interface.
     """
     def __init__(self, rhoM=0, thetaM=270, name="LAYER", **kw):
         BaseMagnetism.__init__(self, name=name, **kw)
         self.rhoM = Parameter.default(rhoM, name=name+" rhoM")
         self.thetaM = Parameter.default(thetaM, limits=(0, 360),
                                         name=name+" thetaM")
 
     def parameters(self):
         parameters = BaseMagnetism.parameters(self)
         parameters.update(rhoM=self.rhoM, thetaM=self.thetaM)
         return parameters
 
+    def to_dict(self):
+        result = BaseMagnetism.to_dict(self)
+        result['rhoM'] = self.rhoM.to_dict()
+        result['thetaM'] = self.thetaM.to_dict()
+        return result
+
     def render(self, probe, slabs, thickness, anchor, sigma):
         slabs.add_magnetism(anchor=anchor,
                             w=[thickness],
                             rhoM=[self.rhoM.value],
                             thetaM=[self.thetaM.value],
                             sigma=sigma)
+
     def __str__(self):
         return "magnetism(%g)"%self.rhoM.value
 
     def __repr__(self):
         return ("Magnetism(rhoM=%g, thetaM=%g)"
                 %(self.rhoM.value, self.thetaM.value))
 
 class MagnetismStack(BaseMagnetism):
     """
     Magnetic slabs within a magnetic layer.
+
+    *weight* is the relative thickness of each layer relative to the nuclear
+    stack to which it is anchored.  Weights are automatically normalized to 1.
+    Default is :code:`weight=[1]` equal size layers.
+
+    *rhoM* is the magnetic SLD for each layer. Default is :code:`rhoM=[0]`
+    for shared magnetism in all the layers.
+
+    *thetaM* is the magnetic angle for each layer.  Default is
+    :code:`thetaM=[270]` for no magnetic twist.
+
+    **Not yet implemented.**
+    *interfaceM* is the magnetic interface for all but the last layer.  Default
+    is :code:`interfaceM=[0]` for equal width interfaces in all layers.
+
+    *name* is the base name for the various layer parameters.
+
+    *extent* defines the number of nuclear layers covered by the magnetic layer.
+
+    *dead_above* and *dead_below* define magnetically dead layers at the
+    nuclear boundaries.  These can be negative if magnetism extends beyond
+    the nuclear boundary.
+
+    *interface_above* and *interface_below* define the magnetic interface
+    at the boundaries, if it is different from the nuclear interface.
     """
-    def __init__(self, weight=(), rhoM=(), thetaM=(270,), interfaceM=(0,),
+    def __init__(self, weight=None, rhoM=None, thetaM=None, interfaceM=None,
                  name="LAYER", **kw):
-        if (len(thetaM) != 1 and len(thetaM) != len(weight)
-                and len(rhoM) != 1 and len(rhoM) != len(weight)
-                and len(interfaceM) != 1 and len(interfaceM) != len(weight)-1):
-            raise ValueError("Must have one rhoM, thetaM and intefaceM for each layer")
-        if interfaceM != [0]:
-            raise NotImplementedError("Doesn't support magnetic roughness")
+        weight_n = 0 if weight is None else len(weight)
+        rhoM_n = 0 if rhoM is None else len(rhoM)
+        thetaM_n = 0 if thetaM is None else len(thetaM)
+        interfaceM_n = 0 if interfaceM is None else (len(interfaceM) + 1)
+        n = max(weight_n, rhoM_n, thetaM_n, interfaceM_n)
+
+        if n == 0:
+            raise ValueError("Must specify one of weight, rhoM, thetaM or interfaceM as vector")
+        if ((weight_n > 1 and weight_n != n)
+                or (rhoM_n > 1 and rhoM_n != n)
+                or (thetaM_n > 1 and thetaM_n != n)
+                or (interfaceM_n > 1 and interfaceM_n != n)):
+            raise ValueError("Inconsistent lengths for weight, rhoM, thetaM and interfaceM")
+
+        # TODO: intefaces need to be implemented in profile.add_magnetism
+        if interfaceM is not None:
+            raise NotImplementedError("Doesn't yet support magnetic interfaces")
+
+        if weight is None:
+            weight = [1]
+        if rhoM is None:
+            rhoM = [0]
+        if thetaM is None:
+            thetaM = [270]
+        #if interfaceM is None:
+        #    interfaceM = [0]
 
-        BaseMagnetism.__init__(self, stack=stack, name=name, **kw)
+        BaseMagnetism.__init__(self, name=name, **kw)
         self.weight = [Parameter.default(v, name=name+" weight[%d]"%i)
                        for i, v in enumerate(weight)]
         self.rhoM = [Parameter.default(v, name=name+" rhoM[%d]"%i)
                      for i, v in enumerate(rhoM)]
         self.thetaM = [Parameter.default(v, name=name+" thetaM[%d]"%i)
                        for i, v in enumerate(thetaM)]
-        self.interfaceM = [Parameter.default(v, name=name+" interfaceM[%d]"%i)
-                           for i, v in enumerate(interfaceM)]
+        #self.interfaceM = [Parameter.default(v, name=name+" interfaceM[%d]"%i)
+        #                   for i, v in enumerate(interfaceM)]
 
     def parameters(self):
         parameters = BaseMagnetism.parameters(self)
         parameters.update(rhoM=self.rhoM,
                           thetaM=self.thetaM,
-                          interfaceM=self.interfaceM,
+                          #interfaceM=self.interfaceM,
                           weight=self.weight)
         return parameters
 
+    def to_dict(self):
+        result = BaseMagnetism.to_dict(self)
+        result['weight'] = [p.to_dict() for p in self.weight]
+        result['rhoM'] = [p.to_dict() for p in self.rhoM]
+        result['thetaM'] = [p.to_dict() for p in self.thetaM]
+        #result['interfaceM'] = [p.to_dict() for p in self.interfaceM]
+        return result
+
     def render(self, probe, slabs, thickness, anchor, sigma):
         w = numpy.array([p.value for p in self.weight])
         w *= thickness / numpy.sum(w)
         rhoM = [p.value for p in self.rhoM]
         thetaM = [p.value for p in self.thetaM]
-        sigmaM = [p.value for p in self.interfaceM]
+        #interfaceM = [p.value for p in self.interfaceM]
         if len(rhoM) == 1:
             rhoM = [rhoM[0]]*len(w)
         if len(thetaM) == 1:
             thetaM = [thetaM[0]]*len(w)
-        if len(sigmaM) == 1:
-            sigmaM = [sigmaM[0]]*(len(w)-1)
+        #if len(interfaceM) == 1:
+        #    interfaceM = [interfaceM[0]]*(len(w)-1)
 
         slabs.add_magnetism(anchor=anchor,
-                            w=w, rhoM=rhoM, thetaM=thetaM,
+                            w=w, rhoM=rhoM,
+                            thetaM=thetaM,
+                            #interfaceM=interfaceM,
                             sigma=sigma)
 
     def __str__(self):
         return "MagnetismStack(%d)"%(len(self.rhoM))
     def __repr__(self):
         return "MagnetismStack"
 
 
 class MagnetismTwist(BaseMagnetism):
     """
     Linear change in magnetism throughout layer.
+
+    *rhoM* contains the *(left, right)* values for the magnetic scattering
+    length density.  The number of steps is determined by the model *dz*.
+
+    *thetaM* contains the *(left, right)* values for the magnetic angle.
+
+    *name* is the base name for the various layer parameters.
+
+    *extent* defines the number of nuclear layers covered by the magnetic layer.
+
+    *dead_above* and *dead_below* define magnetically dead layers at the
+    nuclear boundaries.  These can be negative if magnetism extends beyond
+    the nuclear boundary.
+
+    *interface_above* and *interface_below* define the magnetic interface
+    at the boundaries, if it is different from the nuclear interface.
     """
     magnetic = True
     def __init__(self,
                  rhoM=(0, 0), thetaM=(270, 270),
                  name="LAYER", **kw):
         BaseMagnetism.__init__(self, name=name, **kw)
         self.rhoM = [Parameter.default(v, name=name+" rhoM[%d]"%i)
@@ -199,14 +307,20 @@
                        for i, v in enumerate(thetaM)]
 
     def parameters(self):
         parameters = BaseMagnetism.parameters(self)
         parameters.update(rhoM=self.rhoM, thetaM=self.thetaM)
         return parameters
 
+    def to_dict(self):
+        result = BaseMagnetism.to_dict(self)
+        result['rhoM'] = [p.to_dict() for p in self.rhoM]
+        result['thetaM'] = [p.to_dict() for p in self.thetaM]
+        return result
+
     def render(self, probe, slabs, thickness, anchor, sigma):
         w, z = slabs.microslabs(thickness)
         rhoM = numpy.linspace(self.rhoM[0].value,
                               self.rhoM[1].value, len(z))
         thetaM = numpy.linspace(self.thetaM[0].value,
                                 self.thetaM[1].value, len(z))
         slabs.add_magnetism(anchor=anchor,
@@ -218,14 +332,33 @@
     def __repr__(self):
         return "MagneticTwist"
 
 
 class FreeMagnetism(BaseMagnetism):
     """
     Spline change in magnetism throughout layer.
+
+    Defines monotonic splines for rhoM and thetaM with shared knot positions.
+
+    *z* is position of the knot in [0, 1] relative to the magnetic layer
+    thickness.  The *z* coordinates are automatically sorted before
+    rendering, leading to multiple equivalent solutions if knots are swapped.
+
+    *rhoM* gives the magnetic scattering length density for each knot.
+
+    *thetaM* gives the magnetic angle for each knot.
+
+    *name* is the base name for the various layer parameters.
+
+    *dead_above* and *dead_below* define magnetically dead layers at the
+    nuclear boundaries.  These can be negative if magnetism extends beyond
+    the nuclear boundary.
+
+    *interface_above* and *interface_below* define the magnetic interface
+    at the boundaries, if it is different from the nuclear interface.
     """
     magnetic = True
     def __init__(self, z=(), rhoM=(), thetaM=(),
                  name="LAYER", **kw):
         BaseMagnetism.__init__(self, name=name, **kw)
         def parvec(vector, name, limits):
             return [Parameter.default(p, name=name+"[%d]"%i, limits=limits)
@@ -243,14 +376,21 @@
             raise ValueError("must have one thetaM for each rhoM")
 
     def parameters(self):
         parameters = BaseMagnetism.parameters(self)
         parameters.update(rhoM=self.rhoM, thetaM=self.thetaM, z=self.z)
         return parameters
 
+    def to_dict(self):
+        result = BaseMagnetism.to_dict(self)
+        result['z'] = [p.to_dict() for p in self.z]
+        result['rhoM'] = [p.to_dict() for p in self.rhoM]
+        result['thetaM'] = [p.to_dict() for p in self.thetaM]
+        return result
+
     def profile(self, Pz, thickness):
         mbelow, tbelow = 0, (self.thetaM[0].value if self.thetaM else 270)
         mabove, tabove = 0, (self.thetaM[-1].value if self.thetaM else 270)
         z = numpy.sort([0]+[p.value for p in self.z]+[1])*thickness
 
         rhoM = numpy.hstack((mbelow, [p.value for p in self.rhoM], mabove))
         PrhoM = monospline(z, rhoM, Pz)
```

### Comparing `refl1d-0.8.8/refl1d/main.py` & `refl1d-0.8.9/refl1d/main.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/material.py` & `refl1d-0.8.9/refl1d/material.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 for X-ray, there is no need to scale by probe by electron radius.  In
 the end, sld is just the returned scattering factors times density.
 """
 __all__ = ['Material', 'Mixture', 'SLD', 'Vacuum', 'Scatterer', 'ProbeCache']
 import numpy
 from numpy import inf, NaN
 import periodictable
+from periodictable.constants import avogadro_number
 
 from bumps.parameter import Parameter as Par
 
 
 class Scatterer(object):
     """
     A generic scatterer separates the lookup of the scattering factors
@@ -57,14 +58,16 @@
     .. Note::
        the Scatterer base class is extended by
        :class:`_MaterialStacker <refl1d.model._MaterialStacker>` so that materials
        can be implicitly converted to slabs when used in stack construction
        expressions. It is not done directly to avoid circular dependencies
        between :mod:`model <refl1d.model>` and :mod:`material <refl1d.material>`.
     """
+    name = None
+
     def sld(self, sf):
         """
         Return the scattering length density expected for the given
         scattering factors, as returned from a call to scattering_factors()
         for a particular probe.
         """
         raise NotImplementedError()
@@ -95,14 +98,19 @@
     Empty layer
     """
     name = 'air'
 
     def parameters(self):
         return []
 
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+        }
+
     def sld(self, probe):
         return 0, 0
 
     def __repr__(self):
         return "Vacuum()"
 
 
@@ -131,14 +139,22 @@
         self.name = name
         self.rho = Par.default(rho, name=name+" rho")
         self.irho = Par.default(irho, name=name+" irho")
 
     def parameters(self):
         return {'rho':self.rho, 'irho':self.irho}
 
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+            'name': self.name,
+            'rho': self.rho.to_dict(),
+            'irho': self.irho.to_dict(),
+        }
+
     def sld(self, probe):
         return self.rho.value, self.irho.value
 
 # ============================ Substances =============================
 
 class Material(Scatterer):
     """
@@ -209,14 +225,16 @@
                 Density is *bulk_density*
             *natural_density* : |g/cm^3| or kg/L
                 Density is *natural_density* / (natural mass/isotope mass)
             *relative_density* : unitless
                 Density is *relative_density* * formula density
             *cell_volume* : |Ang^3|
                 Density is mass / *cell_volume*
+            *number_density*: [atoms/cm^3]
+                Density is *number_density* * molar mass / avogadro constant
 
         The resulting material will have a *density* attribute with the
         computed material density in addition to the *fitby*
         attribute specified.
 
         .. Note::
 
@@ -224,63 +242,79 @@
             material, so be sure to do so before using *density* in a
             parameter expression.  Using *bumps.parameter.WrappedParameter*
             for *density* is another alternative.
         """
 
         # Clean out old parameter
         for attr in ('bulk_density', 'natural_density', 'cell_volume',
-                     'relative_density'):
+                     'relative_density', 'number_density'):
             try:
                 delattr(self, attr)
             except Exception:
                 pass
 
         # Put in new parameters
-        if type is 'bulk_density':
+        if type == 'bulk_density':
             if value is None:
                 value = self.formula.density
             self.bulk_density = Par.default(value, name=self.name+" density",
                                             limits=(0, inf))
             self.density = self.bulk_density
-        elif type is 'natural_density':
+        elif type == "number_density":
+            if value is None:
+                value = avogadro_number / self.formula.mass * self.formula.density
+            self.number_density = Par.default(value, name=self.name+" number density", limits=(0, inf))
+            self.density = self.number_density / avogadro_number * self.formula.mass
+        elif type == 'natural_density':
             if value is None:
                 value = self.formula.natural_density
             self.natural_density = Par.default(value,
                                                name=self.name+" nat. density",
                                                limits=(0, inf))
             self.density = self.natural_density / self.formula.natural_mass_ratio()
-        elif type is 'relative_density':
+        elif type == 'relative_density':
             if value is None:
                 value = 1
             self.relative_density = Par.default(value,
                                                 name=self.name+" rel. density",
                                                 limits=(0, inf))
             self.density = self.formula.density*self.relative_density
         ## packing factor code should be correct, but radii are unreliable
         #elif type is 'packing_factor':
         #    max_density = self.formula.mass/self.formula.volume(packing_factor=1)
         #    if value is None:
         #        value = self.formula.density/max_density
         #    self.packing_factor = Par.default(value, name=self.name+" packing factor")
         #    self.density = self.packing_factor * max_density
-        elif type is 'cell_volume':
+        elif type == 'cell_volume':
             # Density is in grams/cm^3.
             # Mass is in grams.
             # Volume is in A^3 = 1e24*cm^3.
             if value is None:
                 value = (1e24*self.formula.molecular_mass)/self.formula.density
             self.cell_volume = Par.default(value,
                                            name=self.name+" cell volume",
                                            limits=(0, inf))
             self.density = (1e24*self.formula.molecular_mass)/self.cell_volume
         else:
             raise ValueError("Unknown density calculation type '%s'"%type)
 
     def parameters(self):
         return {'density': self.density}
+
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+            'name': self.name,
+            'formula': str(self.formula),
+            'density': self.density.to_dict(),
+            'use_incoherent': self.use_incoherent,
+            # TODO: what about fitby, natural_density and cell_volume?
+        }
+
     def sld(self, probe):
         rho, irho, incoh = probe.scattering_factors(self.formula,
                                                     density=self.density.value)
         if self.use_incoherent:
             raise NotImplementedError("incoherent scattering not supported")
             #irho += incoh
         return rho, irho
@@ -316,15 +350,22 @@
 
     def parameters(self):
         """
         Adjustable parameters are the fractions associated with each
         constituent and the relative scale fraction used to tweak
         the overall density.
         """
-        return {'count':self.count}
+        return {'count': self.count}
+
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+            'parts': [str(p) for p in self.formula],
+            'count': [p.to_dict() for p in self.count],
+        }
 
     def formula(self):
         return tuple((c.value, f) for c, f in zip(self.count, self.parts))
 
     def __str__(self):
         return "<%s>"%(", ".join(str(M) for M in self.formula()))
 
@@ -430,18 +471,27 @@
 
     def parameters(self):
         """
         Adjustable parameters are the fractions associated with each
         constituent and the relative scale fraction used to tweak
         the overall density.
         """
-        return {'base':self.base.parameters(),
-                'material':[m.parameters() for m in self.material],
-                'fraction':self.fraction,
-               }
+        return {
+            'base':self.base.parameters(),
+            'material':[m.parameters() for m in self.material],
+            'fraction':self.fraction,
+            }
+
+    def to_dict(self):
+        return {
+            'type': type(self).__name__,
+            'base': self.base.to_dict(),
+            'material': self.material.to_dict(),
+            'fraction': self.fraction.to_dict(),
+        }
 
     def _density(self):
         """
         Compute the density of the mixture from the density and proportion
         of the individual components.
         """
         fraction = numpy.array([0.]+[m.value for m in self.fraction])
```

### Comparing `refl1d-0.8.8/refl1d/materialdb.py` & `refl1d-0.8.9/refl1d/materialdb.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/model.py` & `refl1d-0.8.9/refl1d/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     interface (Parameter: angstrom)
         Interface for the top of the layer.
     magnetism (Magnetism info)
         Magnetic profile anchored to the layer.
     """
     thickness = None
     interface = None
+    name = None
 
     # Make magnetism a property so we can update the magnetism parameter
     # names with the layer name when we assign magnetism to the layer
     _magnetism = None
     @property
     def magnetism(self):
         return self._magnetism
@@ -86,16 +87,18 @@
         Returns a dictionary of parameters specific to the layer.  These will
         be added to the dictionary containing interface, thickness and magnetism
         parameters.
         """
 
     def layer_parameters(self):
         pars = {'thickness': self.thickness}
-        if self.interface: pars['interface'] = self.interface
-        if self.magnetism: pars['magnetism'] = self.magnetism.parameters()
+        if self.interface:
+            pars['interface'] = self.interface
+        if self.magnetism:
+            pars['magnetism'] = self.magnetism.parameters()
         pars.update(self.parameters())
         return pars
 
     def render(self, probe, slabs):
         """
         Use the probe to render the layer into a microslab representation.
         """
@@ -122,21 +125,20 @@
         return getattr(self, 'name', repr(self))
 
     def to_dict(self):
         """
             Return a dictionary representation of the Slab object
         """
         _layer_dict = dict(name=self.name, type=type(self).__name__)
-        if self.thickness: _layer_dict['thickness'] = self.thickness.to_dict()
-        if self.interface: _layer_dict['interface'] = self.interface.to_dict()
+        if self.thickness:
+            _layer_dict['thickness'] = self.thickness.to_dict()
+        if self.interface:
+            _layer_dict['interface'] = self.interface.to_dict()
         if self.magnetism:
-            _mag_parameters = self.magnetism.parameters()
-            if _mag_parameters:
-                for name, param in _mag_parameters.items():
-                    _layer_dict[name] = param.to_dict()
+            _layer_dict['magnetism'] = self.magnetism.to_dict()
         return _layer_dict
 
     # Define a little algebra for composing samples
     # Layers can be stacked, repeated, or have length/roughness/magnetism set
     def __or__(self, other):
         """Join two layers to make a stack"""
         stack = Stack()
@@ -687,15 +689,15 @@
         self.thickness = Par.default(thickness, limits=(0, inf),
                                      name=name+" thickness")
         self.interface = Par.default(interface, limits=(0, inf),
                                      name=name+" interface")
         self.magnetism = magnetism
 
     def parameters(self):
-        return {'material':self.material.parameters()}
+        return {'material': self.material.parameters()}
 
     def render(self, probe, slabs):
         rho, irho = self.material.sld(probe)
         w = self.thickness.value
         sigma = self.interface.value
         #print "rho", rho
         #print "irho", irho
@@ -715,12 +717,10 @@
         Return a dictionary representation of the Slab object
 
         #TODO: Add magnetism
         """
         _slab_dict = dict(name=self.name, type=type(self).__name__)
         _slab_dict['thickness'] = self.thickness.to_dict()
         _slab_dict['interface'] = self.interface.to_dict()
+        _slab_dict['material'] = self.material.to_dict()
         _material_parameters = self.material.parameters()
-        if _material_parameters:
-            for name, param in _material_parameters.items():
-                _slab_dict[name] = param.to_dict()
         return _slab_dict
```

### Comparing `refl1d-0.8.8/refl1d/mono.py` & `refl1d-0.8.9/refl1d/mono.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/names.py` & `refl1d-0.8.9/refl1d/names.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/ncnrdata.py` & `refl1d-0.8.9/refl1d/ncnrdata.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/plottable.py` & `refl1d-0.8.9/refl1d/plottable.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/polymer.py` & `refl1d-0.8.9/refl1d/polymer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This program is public domain
 # Authors Paul Kienzle, Richard Sheridan
-r"""
+"""
 Layer models for polymer systems.
 
 Analytic Self-consistent Field (SCF) Brush profile\ [#Zhulina]_\ [#Karim]_
 
 Analytical Self-consistent Field (SCF) Mushroom Profile\ [#Adamuti-Trache]_
 
 Numerical Self-consistent Field (SCF) End-Tethered Polymer
@@ -30,26 +30,28 @@
     a Monte Carlo model. Macromolecules, 20(7), 1692–1696.
     doi:10.1021/ma00173a041
 
 .. [#deVos] De Vos, W. M., & Leermakers, F. A. M. (2009). Modeling the
     structure of a polydisperse polymer brush. Polymer, 50(1), 305–316.
     doi:10.1016/j.polymer.2008.10.025
 
-.. [#Sheridan] Sheridan, R. J., Beers, K. L., et. al (2014). Direct observation
-    of "surface theta" conditions. [in prep]
+.. [#Sheridan] •	Sheridan, R. J., Orski, S. V., Jones, R. L., Satija, S.,
+    & Beers, K. L. (2017). Surface interaction parameter measurement of
+    solvated polymers via model end-tethered chains. [Submitted]
 
 ..  [#Vincent] Vincent, B., Edwards, J., Emmett, S., & Croot, R. (1988).
     Phase separation in dispersions of weakly-interacting particles in
     solutions of non-adsorbing polymer. Colloids and Surfaces, 31, 267–298.
     doi:10.1016/0166-6622(88)80200-2
 
 """
 
 from __future__ import division, print_function, unicode_literals
 
+
 __all__ = ["PolymerBrush", "PolymerMushroom", "EndTetheredPolymer",
            "VolumeProfile", "layer_thickness"]
 
 import inspect
 
 import numpy as np
 
@@ -61,27 +63,25 @@
 try:
     from collections import OrderedDict
 except ImportError:
     class OrderedDict(dict):
         def popitem(self, *args, **kw):
             return dict.popitem(self, *args)
 
-from numpy import real, imag, exp, log, sqrt, pi, hstack, ones_like, fabs
+from numpy import real, imag, exp, log, sqrt, pi, hstack, ones_like
 
 # This is okay to use as long as LAMBDA_ARRAY is symmetric,
 # otherwise a slice LAMBDA_ARRAY[::-1] is necessary
-from numpy.core.multiarray import correlate as raw_convolve
-
-from numpy.core import add
-addred = add.reduce
+from numpy.core.multiarray import correlate
 
 LAMBDA_1 = 1.0/6.0 #always assume cubic lattice (1/6) for now
 LAMBDA_0 = 1.0 - 2.0*LAMBDA_1
 LAMBDA_ARRAY = np.array([LAMBDA_1, LAMBDA_0, LAMBDA_1])
 MINLAT = 25
+MINBULK = 5
 SQRT_PI = sqrt(pi)
 
 class PolymerBrush(Layer):
     r"""
     Polymer brushes in a solvent
 
     :Parameters:
@@ -140,31 +140,31 @@
         self.power = Parameter.default(power, name=prefix+"power")
         self.sigma = Parameter.default(sigma, name=prefix+"sigma")
         self.solvent = solvent
         self.polymer = polymer
         self.name = name
         # Constraints:
         #   base_vf in [0, 1]
-        #   base, length, sigma, thickness, interface>0
-        #   base+length+3*sigma <= thickness
-
+        #   base, length, sigma, thickness, interface > 0
+        #   base + length + 3*sigma <= thickness
     def parameters(self):
-        return {'solvent':self.solvent.parameters(),
-                'polymer':self.polymer.parameters(),
-                'base_vf':self.base_vf,
-                'base':self.base,
-                'length':self.length,
-                'power':self.power,
-                'sigma':self.sigma,
-               }
+        return {
+            'solvent': self.solvent.parameters(),
+            'polymer': self.polymer.parameters(),
+            'base_vf': self.base_vf,
+            'base': self.base,
+            'length': self.length,
+            'power': self.power,
+            'sigma': self.sigma,
+        }
 
     def profile(self, z):
-        base_vf, base, length, power, sigma \
-            = [p.value for p in (self.base_vf, self.base, self.length,
-                                 self.power, self.sigma)]
+        base_vf, base, length, power, sigma = [
+            p.value for p in (self.base_vf, self.base,
+            self.length, self.power, self.sigma)]
         base_vf /= 100. # % to fraction
         L0 = base  # if base < thickness else thickness
         L1 = base+length # if base+length < thickness else thickness-L0
         if length == 0:
             v = np.ones_like(z)
         else:
             v = (1 - ((z-L0)/(L1-L0))**2)
@@ -285,17 +285,18 @@
             kw.setdefault(k, 0)
         for k, v in kw.items():
             setattr(self, k, Parameter.default(v, name=k))
 
         self._parameters = vars
 
     def parameters(self):
-        P = {'solvent':self.solvent.parameters(),
-             'material':self.material.parameters(),
-            }
+        P = {
+            'solvent': self.solvent.parameters(),
+            'material': self.material.parameters(),
+        }
         for k in self._parameters:
             P[k] = getattr(self, k)
         return P
 
     def render(self, probe, slabs):
         Mr, Mi = self.material.sld(probe)
         Sr, Si = self.solvent.sld(probe)
@@ -309,15 +310,15 @@
         #print(kw)
         phi = self.profile(Pz, **kw)
         try:
             if phi.shape != Pz.shape:
                 raise Exception
         except Exception:
             raise TypeError("profile function '%s' did not return array phi(z)"
-                            % self.profile.__name__)
+                            %self.profile.__name__)
         Pw, phi = util.merge_ends(Pw, phi, tol=1e-3)
         P = M*phi + S*(1-phi)
         slabs.extend(rho=[real(P)], irho=[imag(P)], w=Pw)
         #slabs.interface(self.interface.value)
 
 
 def smear(z, P, sigma):
@@ -342,15 +343,15 @@
         return P
     w = int(3*sigma/dz)
     G = exp(-0.5*(np.arange(-w, w+1)*(dz/sigma))**2)
     full = np.hstack(([P[0]]*w, P, [P[-1]]*w))
     return np.convolve(full, G/np.sum(G), 'valid')
 
 class PolymerMushroom(Layer):
-    r"""
+    """
     Polymer mushrooms in a solvent (volume profile)
 
     :Parameters:
         *delta* | real scalar
             interaction parameter
         *vf* | real scalar
             not quite volume fraction (dimensionless grafting density)
@@ -371,28 +372,29 @@
         self.interface = Parameter.default(interface, name="Mushroom interface")
         self.delta = Parameter.default(delta, name="delta")
         self.vf = Parameter.default(vf, name="vf")
         self.sigma = Parameter.default(sigma, name="sigma")
         self.solvent = solvent
         self.polymer = polymer
         self.name = name
-
     def parameters(self):
-        return {'solvent':self.solvent.parameters(),
-                'polymer':self.polymer.parameters(),
-                'delta':self.delta,
-                'vf':self.vf,
-                'sigma':self.sigma,
-                'thickness':self.thickness,
-                'interface':self.interface
-               }
+        return {
+            'solvent': self.solvent.parameters(),
+            'polymer': self.polymer.parameters(),
+            'delta': self.delta,
+            'vf': self.vf,
+            'sigma': self.sigma,
+            'thickness': self.thickness,
+            'interface': self.interface
+        }
 
     def profile(self, z):
-        delta, sigma, vf, thickness \
-            = [p.value for p in (self.delta, self.sigma, self.vf, self.thickness)]
+        delta, sigma, vf, thickness = [
+            p.value for p in (self.delta, self.sigma, self.vf, self.thickness)
+            ]
 
         return smear(z, MushroomProfile(z, delta, vf, sigma), sigma)
 
 
     def render(self, probe, slabs):
         thickness = self.thickness.value
         Pw, Pz = slabs.microslabs(thickness)
@@ -406,40 +408,38 @@
 
         Mr, Mi = self.polymer.sld(probe)
         Sr, Si = self.solvent.sld(probe)
         M = Mr + 1j*Mi
         S = Sr + 1j*Si
         try:
             M, S = M[0], S[0]  # Temporary hack
-        except KeyError:
+        except:
             pass
 
         phi = self.profile(Pz)
         Pw, phi = util.merge_ends(Pw, phi, tol=1e-3)
         P = M*phi + S*(1-phi)
         Pr, Pi = np.real(P), np.imag(P)
         slabs.extend(rho=[Pr], irho=[Pi], w=Pw)
 
 def MushroomProfile(z, delta=0.1, vf=1.0, sigma=1.0):
     thickness = layer_thickness(z)
     thresh = 1e-10
-
     base = 3.0*sigma # tail is erf, capture 95% of the mixing
     Rg = (thickness-base) / 4.0 # profile ends by ~4 RG, so we can tether these
     keep = (z-base) >= 0.0
     x = (z[keep] - base) / Rg
 
     """
     mushroom_profile_math has a divide by zero problem at delta=0.
     Fix it by weighted average of the profile above and below a threshold.
     No visual difference when delta is between +-0.001, and there's no
     floating point error until ~+-1e-14.
     """
-
-    if fabs(delta) > thresh:
+    if abs(delta) > thresh:
         mushroom_profile = mushroom_math(x, delta, vf)
     else: # we should RARELY get here
         scale = (delta+thresh)/2.0/thresh
         mushroom_profile = (scale*mushroom_math(x, thresh, vf)
                             + (1.0-scale)*mushroom_math(x, -thresh, vf))
 
     try:
@@ -453,53 +453,54 @@
 
 def mushroom_math(x, delta=.1, vf=.1):
     """
     new method, rewrite for numerical stability at high delta
     delta=0 causes divide by zero error!! Compensate elsewhere.
     http://ab-initio.mit.edu/wiki/index.php/Faddeeva_Package
     """
-
     from scipy.special import erfc, erfcx
 
     x_half = x/2.0
     delta_double = 2.0*delta
     return (
             (
              erfc(x_half)
-             - erfcx(delta_double+x_half)/exp(x_half*x_half)
-             - erfc(x)
+             -erfcx(delta_double+x_half)/exp(x_half*x_half)
+             -erfc(x)
              + (
                 (.25-delta*(x+delta_double))*erfcx(delta_double+x)
                 + delta/SQRT_PI
                ) * 4.0 / exp(x*x)
             ) * vf / (delta_double * erfcx(delta_double))
            )
 
 class EndTetheredPolymer(Layer):
     r"""
     Polymer end-tethered to an interface in a solvent
 
     Uses a numerical self-consistent field profile.\ [#Cosgrove]_\ [#deVos]_\ [#Sheridan]_
 
     **Parameters**
-
         *chi*
             solvent interaction parameter
         *chi_s*
             surface interaction parameter
         *h_dry*
             thickness of the neat polymer layer
         *l_lat*
             real length per lattice site
         *mn*
             Number average molecular weight
         *m_lat*
             real mass per lattice segment
         *pdi*
             Dispersity (Polydispersity index)
+        *phi_b*
+            volume fraction of free chains in solution. useful for associating
+            grafted films e.g. PS-COOH in Toluene with an SiO2 surface.
         *thickness*
             Slab thickness should be greater than the contour
             length of the polymer
         *interface*
             should be zero
         *material*
             the polymer material
@@ -509,16 +510,15 @@
     Previous layer should not have roughness! Use a spline to simulate it.
 
     According to [#Vincent]_, $l_\text{lat}$ and $m_\text{lat}$ should be
     calculated by the formulas:
 
     .. math::
 
-        l_\text{lat} &= \frac{a^2 m/l}{p_l}
-
+        l_\text{lat} &= \frac{a^2 m/l}{p_l} \\
         m_\text{lat} &= \frac{(a m/l)^2}{p_l}
 
     where $l$ is the real polymer's bond length, $m$ is the real segment mass,
     and $a$ is the ratio between molecular weight and radius of gyration at
     theta conditions. The lattice persistence, $p_l$, is:
 
     .. math::
@@ -526,52 +526,54 @@
         p_l = \frac16 \frac{1+1/Z}{1-1/Z}
 
     with coordination number $Z = 6$ for a cubic lattice, $p_l = .233$.
     """
 
     def __init__(self, thickness=0, interface=0, name="EndTetheredPolymer",
                  polymer=None, solvent=None, chi=0, chi_s=0, h_dry=None,
-                 l_lat=1, mn=None, m_lat=1, pdi=1):
+                 l_lat=1, mn=None, m_lat=1, pdi=1, phi_b=0):
         if interface != 0:
             raise NotImplementedError("interface not yet supported")
         if polymer is None or solvent is None or h_dry is None or mn is None:
             raise TypeError("Need polymer, solvent and profile")
 
         self.thickness = Parameter.default(thickness, name="SCF thickness")
         self.interface = Parameter.default(interface, name="SCF interface")
-        self.chi = Parameter.default(chi, name="chi")
-        self.chi_s = Parameter.default(chi_s, name="surface chi")
-        self.h_dry = Parameter.default(h_dry, name="dry thickness")
-        self.l_lat = Parameter.default(l_lat, name="lattice layer length")
-        self.mn = Parameter.default(mn, name="Num. Avg. MW")
-        self.m_lat = Parameter.default(m_lat, name="lattice segment mass")
-        self.pdi = Parameter.default(pdi, name="Dispersity")
+        self.chi = Parameter.default(chi, name="Chi")
+        self.chi_s = Parameter.default(chi_s, name="Surface chi")
+        self.h_dry = Parameter.default(h_dry, name="Dry thickness")
+        self.l_lat = Parameter.default(l_lat, name="Lattice layer length")
+        self.mn = Parameter.default(mn, name="Num. avg. MW")
+        self.m_lat = Parameter.default(m_lat, name="Lattice segegment mass")
+        self.pdi   = Parameter.default(pdi, name="Dispersity")
+        self.phi_b = Parameter.default(phi_b, name="Free polymer conc.")
         self.solvent = solvent
         self.polymer = polymer
         self.name = name
 
     def parameters(self):
-        return {'solvent':self.solvent.parameters(),
-                'polymer':self.polymer.parameters(),
-                'chi':self.chi,
-                'chi_s':self.chi_s,
-                'h_dry':self.h_dry,
-                'l_lat':self.l_lat,
-                'mn':self.mn,
-                'm_lat':self.m_lat,
-                'pdi':self.pdi,
-                'thickness':self.thickness,
-                'interface':self.interface
-               }
-
+        return {
+            'solvent': self.solvent.parameters(),
+            'polymer': self.polymer.parameters(),
+            'chi': self.chi,
+            'chi_s': self.chi_s,
+            'h_dry': self.h_dry,
+            'l_lat': self.l_lat,
+            'mn': self.mn,
+            'm_lat': self.m_lat,
+            'pdi': self.pdi,
+            'phi_b': self.phi_b,
+            'thickness': self.thickness,
+            'interface': self.interface
+        }
     def profile(self, z):
         return SCFprofile(z, chi=self.chi.value, chi_s=self.chi_s.value,
                           h_dry=self.h_dry.value, l_lat=self.l_lat.value,
                           mn=self.mn.value, m_lat=self.m_lat.value,
-                          pdi=self.pdi.value)
+                          pdi=self.pdi.value, phi_b=self.phi_b.value)
 
     def render(self, probe, slabs):
         thickness = self.thickness.value
         Pw, Pz = slabs.microslabs(thickness)
         # Skip layer if it falls to zero thickness.  This may lead to
         # problems in the fitter, since R(thickness) is non-differentiable
         # at thickness = 0.  "Clip to boundary" range handling will at
@@ -582,25 +584,26 @@
 
         Mr, Mi = self.polymer.sld(probe)
         Sr, Si = self.solvent.sld(probe)
         M = Mr + 1j*Mi
         S = Sr + 1j*Si
         try:
             M, S = M[0], S[0]  # Temporary hack
-        except KeyError:
+        except:
             pass
 
         phi = self.profile(Pz)
         Pw, phi = util.merge_ends(Pw, phi, tol=1e-3)
         P = M*phi + S*(1-phi)
         Pr, Pi = np.real(P), np.imag(P)
         slabs.extend(rho=[Pr], irho=[Pi], w=Pw)
 
+
 def SCFprofile(z, chi=None, chi_s=None, h_dry=None, l_lat=1, mn=None,
-               m_lat=1, pdi=1, disp=False):
+               m_lat=1, phi_b=0, pdi=1, disp=False):
     """
     Generate volume fraction profile for Refl1D based on real parameters.
 
     The field theory is a lattice-based one, so we need to move between lattice
     and real space. This is done using the parameters l_lat and m_lat, the
     lattice size and the mass of a lattice segment, respectivley. We use h_dry
     (dry thickness) as a convenient measure of surface coverage, along with mn
@@ -617,70 +620,79 @@
     theta = h_dry/l_lat
     segments = mn/m_lat
     sigma = theta/segments
 
     # solve the self consistent field equations using the cache
     if disp:
         print("\n=====Begin calculations=====\n")
-    phi_lat = SCFcache(chi, chi_s, pdi, sigma, segments, disp)
+    phi_lat = SCFcache(chi, chi_s, pdi, sigma, phi_b, segments, disp)
     if disp:
         print("\n============================\n")
 
+    # Chop edge effects out
+    for x, layer in enumerate(reversed(phi_lat)):
+        if abs(layer - phi_b) < 1e-6:
+            break
+    phi_lat = phi_lat[:-(x + 1)]
+
     # re-dimensionalize the solution
     layers = len(phi_lat)
     z_end = l_lat*layers
     z_lat = np.linspace(0.0, z_end, num=layers)
-    phi = np.interp(z, z_lat, phi_lat, right=0.0)
+    phi = np.interp(z, z_lat, phi_lat, right=phi_b)
 
     return phi
 
 
-def SCFcache(chi, chi_s, pdi, sigma, segments, disp=False, cache=OrderedDict()):
-    """
-    Return a memoized SCF result by walking from a previous solution.
+_SCFcache_dict = OrderedDict()
+
 
-    Using an OrderedDict (because I want to prune keys FIFO)
+def SCFcache(chi, chi_s, pdi, sigma, phi_b, segments, disp=False,
+             cache=_SCFcache_dict):
+    """Return a memoized SCF result by walking from a previous solution.
+
+    Using an OrderedDict because I want to prune keys FIFO
     """
-    # prime the cache with a known easy solution
+    from scipy.optimize.nonlin import NoConvergence
+    # prime the cache with a known easy solutions
     if not cache:
-        cache[(0, 0, 0, .1, .2)] = SCFsolve(sigma=.1, segments=100)
+        cache[(0, 0, 0, .1, .1, .1)] = SCFsolve(sigma=.1, phi_b=.1, segments=50, disp=disp)
+        cache[(0, 0, 0, 0, .1, .1)] = SCFsolve(sigma=0, phi_b=.1, segments=50, disp=disp)
+        cache[(0, 0, 0, .1, 0, .1)] = SCFsolve(sigma=.1, phi_b=0, segments=50, disp=disp)
 
     if disp:
         starttime = time()
 
     # Try to keep the parameters between 0 and 1. Factors are arbitrary.
-    scaled_parameters = (chi, chi_s*3, pdi-1, sigma, segments/500)
+    scaled_parameters = (chi, chi_s * 3, pdi - 1, sigma, phi_b, segments / 500)
 
     # longshot, but return a cached result if we hit it
     if scaled_parameters in cache:
         if disp:
             print('SCFcache hit at:', scaled_parameters)
-        phi = cache.pop(scaled_parameters) # pop and assign to shift the key
-        cache[scaled_parameters] = phi     # to the end as "recently used"
+        phi = cache[scaled_parameters] = cache.pop(scaled_parameters)
         return phi
 
     # Find the closest parameters in the cache: O(len(cache))
 
     # Numpy setup
-    cached_parameters = list(cache)
+    cached_parameters = tuple(dict.__iter__(cache))
     cp_array = np.array(cached_parameters)
     p_array = np.array(scaled_parameters)
 
     # Calculate distances to all cached parameters
     deltas = p_array - cp_array # Parameter space displacement vectors
-    norms = sqrt(addred(deltas*deltas, axis=1)) # and their magnitudes
-    closest_index = norms.argmin()
+    closest_index = np.sum(deltas * deltas, axis=1).argmin()
 
     # Organize closest point data for later use
     closest_cp = cached_parameters[closest_index]
     closest_cp_array = cp_array[closest_index]
     closest_delta = deltas[closest_index]
 
-    phi0 = cache.pop(closest_cp) # pop and assign to shift the key
-    cache[closest_cp] = phi0     # to the end as "recently used"
+    phi = cache[closest_cp] = cache.pop(closest_cp)
 
     if disp:
         print("Walking from nearest:", closest_cp_array)
         print("to:", p_array)
 
     """
     We must walk from the previously cached point to the desired region.
@@ -714,192 +726,153 @@
         else:
             p_tup = scaled_parameters
 
         if disp:
             print('Parameter step is', step)
             print('current parameters:', p_tup)
 
-        parameters = (p_tup[0], p_tup[1]/3, p_tup[2]+1,
-                      p_tup[3], p_tup[4]*500)
         try:
-            phi0 = SCFsolve(*parameters, phi0=phi0, disp=disp)
-            cache[p_tup] = phi0
+            phi = SCFsolve(p_tup[0], p_tup[1] / 3, p_tup[2] + 1, p_tup[3], p_tup[4],
+                           p_tup[5] * 500, disp=disp, phi0=phi)
+        except (NoConvergence, ValueError) as e:
+            if isinstance(e, ValueError):
+                if str(e) != "array must not contain infs or NaNs":
+                    raise
+            if disp:
+                print('Step failed')
+            flag = True  # Reset this so we don't quit if step=1.0 fails
+            dstep *= .5
+            step -= dstep
+            if dstep < 1e-5:
+                raise RuntimeError('Cache walk appears to be stuck')
+        else:  # Belongs to try, executes if no exception is raised
+            cache[p_tup] = phi
             dstep *= 1.05
             step += dstep
-        except RuntimeError as e:
-            if hasattr(e, 'message'):
-                message = e.message
-            elif hasattr(e, 'args'):
-                message = e.args[0]
-            else:
-                raise
-
-            if message != "solver couldn't converge":
-                raise
-            else:
-                flag = True # Reset this so we don't quit if step=1.0 fails
-                dstep *= .5
-                step -= dstep
 
     if disp:
         print('SCFcache execution time:', round(time()-starttime, 3), "s")
 
     # keep the cache from consuming all things
-    if len(cache) > 1000:
-        if disp:
-            print('pruning cache')
-        for i in range(100):
-            cache.popitem(last=False)
+    while len(cache) > 100:
+        cache.popitem(last=False)
 
-    return phi0
+    return phi
 
 
-def SCFsolve(chi=0, chi_s=0, pdi=1, sigma=None, segments=None,
-             disp=False, phi0=None, maxiter=15):
-    """
-    Solve SCF equations using an initial guess and lattice parameters
+def SCFsolve(chi=0, chi_s=0, pdi=1, sigma=None, phi_b=0, segments=None,
+             disp=False, phi0=None, maxiter=30):
+    """Solve SCF equations using an initial guess and lattice parameters
 
     This function finds a solution for the equations where the lattice size
     is sufficiently large.
 
-    The Newton-Krylov solver really makes this one. Krylov+gmres was faster
-    than the other scipy.optimize alternatives by quite a lot.
+    The Newton-Krylov solver really makes this one. With gmres, it was faster
+    than the other solvers by quite a lot.
     """
 
-    from scipy.optimize import root
+    from scipy.optimize import newton_krylov
 
     if sigma >= 1:
         raise ValueError('Chains that short cannot be squeezed that high')
 
     if disp:
         starttime = time()
 
     p_i = SZdist(pdi, segments)
 
     if phi0 is None:
         # TODO: Better initial guess for chi>.6
-        layers, phi0 = default_guess(segments, sigma)
+        phi0 = default_guess(segments, sigma)
         if disp:
-            print('No guess passed, using default phi0: layers =', layers)
+            print('No guess passed, using default phi0: layers =', len(phi0))
     else:
-        phi0 = fabs(phi0)
-        phi0[phi0 > .99999] = .99999
-        layers = len(phi0)
+        phi0 = abs(phi0)
+        phi0[phi0>.99999] = .99999
         if disp:
-            print("Initial guess passed: layers =", layers)
+            print("Initial guess passed: layers =", len(phi0))
 
-    # Loop resizing variables
-
-    # We tolerate up to 2ppm of our polymer in the last layer,
-    theta = sigma*segments
-    tol = 2e-6*theta
-    # otherwise we grow it by 20%.
-    ratio = .2
+    # resizing loop variables
+    jac_solve_method = 'gmres'
+    lattice_too_small = True
 
-    # callback to detect an undersized lattice early
-    def callback(x, fx):
-        short_circuit_callback(x, tol)
+    # We tolerate up to 1 ppm deviation from bulk phi
+    # when counting layers_near_phi_b
+    tol = 1e-6
 
-    # other loop variables
-    jac_solve_method = 'gmres'
+    def curried_SCFeqns(phi):
+        return SCFeqns(phi, chi, chi_s, sigma, segments, p_i, phi_b)
 
-    while True:
+    while lattice_too_small:
         if disp:
             print("Solving SCF equations")
 
         try:
-            result = root(
-                SCFeqns, phi0, args=(chi, chi_s, sigma, segments, p_i),
-                method='Krylov', callback=callback,
-                options={'disp':bool(disp), 'maxiter':maxiter,
-                         'jac_options':{'method':jac_solve_method}})
-            if disp:
-                print('Solver exit code:', result.status, result.message)
-
-            if result.status == 1:
-                # success! carry on to resize logic.
-                phi = fabs(result.x)
-            elif result.status == 2:
-                raise RuntimeError("solver couldn't converge")
-
-        except ShortCircuitError as e:
-            # dumping out to resize since we've exceeded resize tol by 4x
-            phi = fabs(e.x)
-            if disp:
-                print(e.value)
-
-        except ValueError as e:
-            if hasattr(e, 'message'):
-                message = e.message
-            elif hasattr(e, 'args'):
-                message = e.args[0]
-            else:
-                raise
-
-            if message == 'array must not contain infs or NaNs':
-                # TODO: Handle this error better. Caused by double overflows.
-                raise #RuntimeError("solver couldn't converge")
-            else:
-                raise
-
+            with np.errstate(invalid='ignore'):
+                phi = abs(newton_krylov(curried_SCFeqns,
+                                        phi0,
+                                        verbose=bool(disp),
+                                        maxiter=maxiter,
+                                        method=jac_solve_method,
+                                        ))
         except RuntimeError as e:
-            if hasattr(e, 'message'):
-                message = e.message
-            elif hasattr(e, 'args'):
-                message = e.args[0]
-            else:
-                raise
-            if message == 'gmres is not re-entrant':
+            if str(e) == 'gmres is not re-entrant':
                 # Threads are racing to use gmres. Lose the race and use
                 # something slower but thread-safe.
                 jac_solve_method = 'lgmres'
                 continue
             else:
                 raise
 
         if disp:
-            print('phi(M)/sum(phi) =', phi[-1] / theta * 1e6, '(ppm)')
+            print('lattice size:', len(phi))
 
-        if phi[-1] > tol:
-            # if the last layer is beyond tolerance, grow the lattice
-            newlayers = max(1, int(round(len(phi0)*ratio)))
+        phi_deviation = abs(phi - phi_b)
+        layers_near_phi_b = phi_deviation < tol
+        nbulk = np.sum(layers_near_phi_b)
+        lattice_too_small = nbulk < MINBULK
+
+        if lattice_too_small:
+            # if there aren't enough layers_near_phi_b, grow the lattice 20%
+            newlayers = max(1, round(len(phi0) * 0.2))
             if disp:
                 print('Growing undersized lattice by', newlayers)
-            phi0 = hstack((phi, np.linspace(phi[-1], 0, num=newlayers)))
-        else:
-            # otherwise, we are done for real
-            break
+            if nbulk:
+                i = np.diff(layers_near_phi_b).nonzero()[0].max()
+            else:
+                i = phi_deviation.argmin()
+            phi0 = np.insert(phi, i, np.linspace(phi[i - 1], phi[i], num=newlayers))
 
-    # chop off extra layers
-    chop = addred(phi > tol) + 1
-    phi = phi[:max(MINLAT, chop)]
+    if nbulk > 2 * MINBULK:
+        chop_end = np.diff(layers_near_phi_b).nonzero()[0].max()
+        chop_start = chop_end - MINBULK
+        i = np.arange(len(phi))
+        phi = phi[(i <= chop_start) | (i > chop_end)]
 
     if disp:
-        print('After chopping: phi(M)/sum(phi) =',
-              phi[-1] / theta * 1e6, '(ppm)')
-        print("lattice size:", len(phi))
         print("SCFsolve execution time:", round(time()-starttime, 3), "s")
 
     return phi
 
-def SZdist(pdi, nn, cache=OrderedDict()):
-    """
-    Calculate Shultz-Zimm distribution from PDI and number average DP
+
+_SZdist_dict = OrderedDict()
+
+
+def SZdist(pdi, nn, cache=_SZdist_dict):
+    """ Calculate Shultz-Zimm distribution from PDI and number average DP
 
     Shultz-Zimm is a "realistic" distribution for linear polymers. Numerical
     problems arise when the distribution gets too uniform, so if we find them,
     default to an exact uniform calculation.
     """
+    from scipy.special import gammaln
     args = pdi, nn
     if args in cache:
-        p_ni = cache.pop(args)
-        cache[args] = p_ni
-        return p_ni
-
-    from scipy.special import gammaln
+        cache[args] = cache.pop(args)
+        return cache[args]
 
     uniform = False
 
     if pdi == 1.0:
         uniform = True
     elif pdi < 1.0:
         raise ValueError('Invalid PDI')
@@ -913,15 +886,15 @@
         for i in range(max(1, int((100*nn)/chunk))):
             ni = np.arange(chunk*i+1, chunk*(i+1)+1, dtype=np.float64)
             r = ni/nn
             xr = x*r
 
             p_ni = exp(log(x/ni) - gammaln(x+1) + xr*(log(xr)/r-1))
 
-            pdi_underflow = (p_ni >= 1.0).any() # catch "too small PDI"
+            pdi_underflow = (p_ni>=1.0).any() # catch "too small PDI"
             if pdi_underflow:
                 break # and break out to uniform calculation
 
             # Stop calculating when species account for less than 1ppm
             keep = (r < 1.0) | (p_ni >= 1e-6)
             if keep.all():
                 p_ni_list.append(p_ni)
@@ -929,182 +902,204 @@
                 p_ni_list.append(p_ni[keep])
                 break
         else: # Belongs to the for loop. Executes if no break statement runs.
             raise RuntimeError('SZdist overflow')
 
     if uniform or pdi_underflow:
         # NOTE: rounding here allows nn to be a double in the rest of the logic
-        p_ni = np.zeros((1, int(round(nn))))
-        p_ni[0, -1] = 1.0
+        p_ni = np.zeros(int(round(nn)))
+        p_ni[-1] = 1.0
     else:
-        p_ni = hstack(p_ni_list).reshape(1, -1)
+        p_ni = np.concatenate(p_ni_list)
+        p_ni /= p_ni.sum()
+    cache[args]=p_ni
 
-    cache[args] = p_ni
-
-    if len(cache) > 9000:
-        for i in range(1000):
-            cache.popitem(last=False)
+    if len(cache)>9000:
+        cache.popitem(last=False)
 
     return p_ni
 
-def default_guess(segments=100, sigma=.5, chi=0, chi_s=0):
-    """
-    Produce an initial guess for phi via analytical approximants.
 
-    For now, a line using numbers from scaling theory
-    """
-    ss = sqrt(sigma)
-    default_layers = int(round(max(MINLAT, segments*ss)))
-    default_phi0 = np.linspace(ss, 0, num=default_layers)
-    return default_layers, default_phi0
+def default_guess(segments=100, sigma=.5, phi_b=.1, chi=0, chi_s=0):
+    """ Produce an initial guess for phi via analytical approximants.
 
-class ShortCircuitError(Exception):
-    """
-    Special error to stop root() before a solution is found.
+    For now, a line using numbers from scaling theory
     """
-    def __init__(self, value, x):
-        self.value = value
-        self.x = x
+    ss=sqrt(sigma)
+    default_layers = round(max(MINLAT, segments * ss))
+    default_phi0 = np.linspace(ss, phi_b, num=default_layers)
+    return default_phi0
 
-    def __str__(self):
-        return repr(self.value)
 
-def short_circuit_callback(x, tol):
-    """
-    Special callback to stop root() before solution is found.
+def SCFeqns(phi_z, chi, chi_s, sigma, n_avg, p_i, phi_b=0):
+    """ System of SCF equation for terminally attached polymers.
 
-    This kills root if the tolerances are exceeded by 4 times the tolerances
-    of the lattice resizing loop. This seems to work well empirically to
-    restart the solver when necessary without cutting out of otherwise
-    reasonable solver trajectories.
-    """
-    if abs(x[-1]) > 4*tol:
-        raise ShortCircuitError('Stopping, lattice too small!', x)
+        Formatted for input to a nonlinear minimizer or solver.
 
-def SCFeqns(phi_z, chi, chi_s, sigma, navgsegments, p_i):
-    """
-    System of SCF equation for terminally attached polymers.
-
-    Formatted for input to a nonlinear minimizer or solver.
+        The sign convention here on u is "backwards" and always has been.
+        It saves a few sign flips, and looks more like Cosgrove's.
     """
 
     # let the solver go negative if it wants
-    phi_z = fabs(phi_z)
+    phi_z = abs(phi_z)
 
-    # attempts to try fields with values greater than one are penalized
+    # penalize attempts that overfill the lattice
     toomuch = phi_z > .99999
-    if toomuch.any():
-        penalty = np.where(toomuch, 1e5*(phi_z-.99999), 0)
+    penalty_flag = toomuch.any()
+    if penalty_flag:
+        penalty = np.where(toomuch, phi_z - .99999, 0)
         phi_z[toomuch] = .99999
-    else:
-        penalty = 0.0
-
-    layers = phi_z.size
-    cutoff = p_i.size
-
-    # calculate all needed quantities for new g_z
-    delta = np.zeros(layers)
-    delta[0] = 1.0
-    phi_z_avg = calc_phi_z_avg(phi_z)
 
     # calculate new g_z (Boltzmann weighting factors)
-    g_z = (1.0 - phi_z)*exp(2*chi*phi_z_avg + delta*chi_s)
+    u_prime = log((1.0 - phi_z) / (1.0 - phi_b))
+    u_int = 2 * chi * (correlate(phi_z, LAMBDA_ARRAY, 1) - phi_b)
+    u_int[0] += chi_s
+    u_z = u_prime + u_int
+    g_z = exp(u_z)
 
     # normalize g_z for numerical stability
-    u = -log(g_z)
-    uavg = addred(u)/layers
-    g_z_norm = g_z*exp(uavg)
-
-    # calculate weighting factors for terminally attached chains
-    g_zs_ta_norm = calc_g_zs(g_z_norm, 0, layers, cutoff)
-
-    # calculate normalization constants from 1/(single chain partition fn)
-    if cutoff == round(navgsegments): # if uniform,
-        c_i_norm = sigma/addred(g_zs_ta_norm[:, -1]) # take a shortcut!
-    else:
-        c_i_norm = sigma*p_i/addred(g_zs_ta_norm, axis=0)
+    u_z_avg = np.mean(u_z)
+    g_z_norm = g_z / exp(u_z_avg)
 
-    # calculate weighting factors for free chains
-    g_zs_free_ngts_norm = calc_g_zs(g_z_norm, c_i_norm, layers, cutoff)
+    phi_z_new = calc_phi_z(g_z_norm, n_avg, sigma, phi_b, u_z_avg, p_i)
 
-    # calculate new polymer density field
-    phi_z_new = calc_phi_z(g_zs_ta_norm, g_zs_free_ngts_norm, g_z_norm)
+    eps_z = phi_z - phi_z_new
 
-    # Handle float overflows only if they show themselves
-    if np.isnan(phi_z_new).any():
-        maxfloat = _getmax(g_zs_ta_norm.dtype.type)
-        g_zs_ta_norm[np.isinf(g_zs_ta_norm)] = maxfloat
-        g_zs_free_ngts_norm[np.isinf(g_zs_free_ngts_norm)] = maxfloat
-        phi_z_new = calc_phi_z(g_zs_ta_norm, g_zs_free_ngts_norm, g_z_norm)
+    if penalty_flag:
+        np.copysign(penalty, eps_z, penalty)
+        eps_z += penalty
 
-    eps_z = phi_z - phi_z_new
-    return eps_z + penalty*np.sign(eps_z)
+    return eps_z
 
-def _getmax(t, seen_t={}):
-    try:
-        return seen_t[t]
-    except KeyError:
-        from numpy.core import getlimits
-        fmax = getlimits.finfo(t).max
-        seen_t[t] = fmax
-        return fmax
-
-def calc_phi_z_avg(phi_z):
-    return raw_convolve(phi_z, LAMBDA_ARRAY, 1)
-
-def calc_phi_z(g_ta, g_free, g_z):
-    return addred(g_ta*np.fliplr(g_free), axis=1)/g_z
-
-def calc_g_zs(g_z, c_i, layers, segments):
-    # initialize
-    g_zs = np.empty((layers, segments), dtype=np.float64, order='F')
-
-    # choose special case
-    if np.size(c_i) == 1:
-        if c_i:
-            # uniform chains
-            g_zs[:, 0] = c_i*g_z
+
+def calc_phi_z(g_z, n_avg, sigma, phi_b, u_z_avg=0, p_i=None):
+    if p_i is None:
+        segments = n_avg
+        uniform = True
+    else:
+        segments = p_i.size
+        uniform = segments == round(n_avg)
+
+    g_zs = Propagator(g_z, segments)
+
+    # for terminally attached chains
+    if sigma:
+        g_zs_ta = g_zs.ta()
+
+        if uniform:
+            c_i_ta = sigma / np.sum(g_zs_ta[:, -1])
+            g_zs_ta_ngts = g_zs.ngts_u(c_i_ta)
+        else:
+            c_i_ta = sigma * p_i / np.sum(g_zs_ta, axis=0)
+            g_zs_ta_ngts = g_zs.ngts(c_i_ta)
+
+        phi_z_ta = compose(g_zs_ta, g_zs_ta_ngts, g_z)
+    else:
+        phi_z_ta = 0
+
+    # for free chains
+    if phi_b:
+        g_zs_free = g_zs.free()
+
+        if uniform:
+            r_i = segments
+            c_free = phi_b / r_i
+            normalizer = exp(u_z_avg * r_i)
+            c_free = c_free * normalizer
+            g_zs_free_ngts = g_zs.ngts_u(c_free)
         else:
-            # terminally attached ends
-            g_zs[:, 0] = 0.0
-            g_zs[0, 0] = g_z[0]
-        from refl1d.calc_g_zs_cex import _calc_g_zs_uniform
-        _calc_g_zs_uniform(g_z, g_zs, LAMBDA_0, LAMBDA_1, layers, segments)
+            r_i = np.arange(1, segments + 1)
+            c_i_free = phi_b * p_i / r_i
+            normalizer = exp(u_z_avg * r_i)
+            c_i_free = c_i_free * normalizer
+            g_zs_free_ngts = g_zs.ngts(c_i_free)
 
+        phi_z_free = compose(g_zs_free, g_zs_free_ngts, g_z)
     else:
-        # free ends
-        g_zs[:, 0] = c_i[0, -1]*g_z
-        from refl1d.calc_g_zs_cex import _calc_g_zs
-        _calc_g_zs(g_z, c_i, g_zs, LAMBDA_0, LAMBDA_1, layers, segments)
-
-    # Older versions of inner loops
-
-#    if np.size(c_i)==1:
-#        c_i = np.zeros((1, int(round(segments))))
-#        g_zs[:, 0] = 0.0
-#        g_zs[0, 0] = g_z[0]
-#    else:
-#        # free chains
-#        g_zs[:, 0] = c_i[0, segments-1]*g_z
-
-    # FASTEST: call some custom C code identical to "SLOW" loop
-#    _calc_g_zs_pointers(g_z, c_i, g_zs, LAMBDA_0, LAMBDA_1, layers, segments)
-
-    # FASTER: use the convolve function to partially vectorize
-#    pg_zs=g_zs[:, 0]
-#    for r in range(1, segments):
-#        pg_zs=g_z*(c_i[0, segments-r-1]+raw_convolve(pg_zs, LAMBDA_ARRAY, 1))
-#        g_zs[:, r]=pg_zs
-
-    # SLOW: loop outright, pulling some slicing out of the innermost loop
-#    for r in range(1, segments):
-#        c=c_i[0, segments-r-1]
-#        g_zs[0, r]=(pg_zs[0]*LAMBDA_0+pg_zs[1]*LAMBDA_1+c)*g_z[0]
-#        for z in range(1, (layers-1)):
-#            g_zs[z, r]=(pg_zs[z-1]*LAMBDA_1
-#                       + pg_zs[z]*LAMBDA_0
-#                       + pg_zs[z+1]*LAMBDA_1
-#                       + c) * g_z[z]
-#        g_zs[-1, r]=(pg_zs[-1]*LAMBDA_0+pg_zs[-2]*LAMBDA_1+c)*g_z[-1]
-#        pg_zs=g_zs[:, r]
+        phi_z_free = 0
+
+    return phi_z_ta + phi_z_free
+
+
+def compose(g_zs, g_zs_ngts, g_z):
+    prod = g_zs * np.fliplr(g_zs_ngts)
+    prod[np.isnan(prod)] = 0
+    return np.sum(prod, axis=1) / g_z
+
+
+class Propagator(object):
+    cex = None
 
-    return g_zs
+    def __init__(self, g_z, segments):
+        self.g_z = g_z
+        self.shape = int(g_z.size), int(segments)
+        # keep all future instances from retrying this test
+        if self.cex is not None:
+            return
+
+        try:
+            import refl1d.calc_g_zs_cex as cex
+            Propagator.cex = cex
+        except ImportError:
+            import warnings
+            warnings.warn('Could not load C extension for EndTetheredPolymer. Continuing with slower NumPy code.\n'
+                          'Try rebuilding refl1d to remove this warning and speed things up!')
+            Propagator.cex = False
+
+    def ta(self):
+        # terminally attached beginnings
+        # forward propagator
+
+        g_zs = self._new()
+        g_zs[:, 0] = 0.0
+        g_zs[0, 0] = self.g_z[0]
+        self._calc_g_zs_uniform(self.g_z, g_zs)
+        return g_zs
+
+    def free(self):
+        # free beginnings
+        # forward propagator
+
+        g_zs = self._new()
+        g_zs[:, 0] = self.g_z
+        self._calc_g_zs_uniform(self.g_z, g_zs)
+        return g_zs
+
+    def ngts_u(self, c):
+        # free ends of uniform chains
+        # reverse propagator
+
+        g_zs = self._new()
+        g_zs[:, 0] = c * self.g_z
+        self._calc_g_zs_uniform(self.g_z, g_zs)
+        return g_zs
+
+    def ngts(self, c_i):
+        # free ends of disperse chains
+        # reverse propagator
+
+        g_zs = self._new()
+        g_zs[:, 0] = c_i[-1] * self.g_z
+        self._calc_g_zs(self.g_z, c_i, g_zs)
+        return g_zs
+
+    def _new(self):
+        return np.empty(self.shape, order='F')
+
+    def _calc_g_zs(self, g_z, c_i, g_zs):
+        if self.cex:
+            self.cex._calc_g_zs(g_z, c_i, g_zs, LAMBDA_0, LAMBDA_1, *self.shape)
+        else:
+            pg_zs = g_zs[:, 0]
+            segment_iterator = enumerate(c_i[::-1])
+            next(segment_iterator)
+            for r, c in segment_iterator:
+                g_zs[:, r] = pg_zs = (correlate(pg_zs, LAMBDA_ARRAY, 1) + c) * g_z
+
+    def _calc_g_zs_uniform(self, g_z, g_zs):
+        if self.cex:
+            self.cex._calc_g_zs_uniform(g_z, g_zs, LAMBDA_0, LAMBDA_1, *self.shape)
+        else:
+            segments = g_zs.shape[1]
+            pg_zs = g_zs[:, 0]
+            for r in range(1, segments):
+                g_zs[:, r] = pg_zs = correlate(pg_zs, LAMBDA_ARRAY, 1) * g_z
```

### Comparing `refl1d-0.8.8/refl1d/probe.py` & `refl1d-0.8.9/refl1d/probe.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 #   overlapping points are recalculated
 #   profiles are recalculated
 #
 # Unstitched seems like the better bet.
 
 import os
 import json
+import warnings
 
 import numpy
 from numpy import sqrt, pi, inf, sign, log
 
 from periodictable import nsf, xsf
 from bumps.parameter import Parameter, Constant
 from bumps.plotutil import coordinated_colors, auto_shift
@@ -51,14 +52,15 @@
 
 from . import fresnel
 from .material import Vacuum
 from .resolution import QL2T, QT2L, TL2Q, dQdL2dT, dQdT2dLoL, dTdL2dQ
 from .resolution import sigma2FWHM, FWHM2sigma
 from .stitch import stitch
 from .reflectivity import convolve
+from .util import asbytes
 
 PROBE_KW = ('T', 'dT', 'L', 'dL', 'data', 'name', 'filename',
             'intensity', 'background', 'back_absorption', 'sample_broadening',
             'theta_offset', 'back_reflectivity', 'data')
 
 
 def make_probe(**kw):
@@ -149,39 +151,41 @@
     Normally *view* is set directly in the class rather than the
     instance since it is not specific to the view.  Fresnel and Q4
     views are corrected for background and intensity; log and
     linear views show the uncorrected data.
     """
     polarized = False
     Aguide = 270  # default guide field for unpolarized measurements
-    view = "fresnel"
+    view = "log"
     plot_shift = 0
     residuals_shift = 0
 
     def __init__(self, T=None, dT=0, L=None, dL=0, data=None,
                  intensity=1, background=0, back_absorption=1, theta_offset=0,
                  sample_broadening=0,
                  back_reflectivity=False, name=None, filename=None):
         if T is None or L is None:
             raise TypeError("T and L required")
+        if sample_broadening is None:
+            sample_broadening = 0
+        if theta_offset is None:
+            theta_offset = 0
         if not name and filename:
             name = os.path.splitext(os.path.basename(filename))[0]
         qualifier = " "+name if name is not None else ""
-        self.intensity = Parameter.default(intensity,
-                                           name="intensity"+qualifier)
-        self.background = Parameter.default(background,
-                                            name="background"+qualifier,
-                                            limits=[0., inf])
-        self.back_absorption = Parameter.default(back_absorption,
-                                                 name="back_absorption"+qualifier,
-                                                 limits=[0., 1.])
-        self.theta_offset = Parameter.default(theta_offset,
-                                              name="theta_offset"+qualifier)
-        self.sample_broadening = Parameter.default(sample_broadening,
-                                              name="sample_broadening"+qualifier)
+        self.intensity = Parameter.default(
+            intensity, name="intensity"+qualifier)
+        self.background = Parameter.default(
+            background, name="background"+qualifier, limits=[0., inf])
+        self.back_absorption = Parameter.default(
+            back_absorption, name="back_absorption"+qualifier, limits=[0., 1.])
+        self.theta_offset = Parameter.default(
+            theta_offset, name="theta_offset"+qualifier)
+        self.sample_broadening = Parameter.default(
+            sample_broadening, name="sample_broadening"+qualifier)
         self.back_reflectivity = back_reflectivity
         if data is not None:
             R, dR = data
         else:
             R, dR = None, None
 
         self._set_TLR(T, dT, L, dL, R, dR)
@@ -193,29 +197,29 @@
         #    L = xsf.xray_wavelength(E)
         #    dL = L * dE/E
         #else:
         #    E = xsf.xray_energy(L)
         #    dE = E * dL/L
 
         Q = TL2Q(T=T, L=L)
-        dQ = dTdL2dQ(T=T, dT=dT + self.sample_broadening.value, L=L, dL=dL)
+        dQ = dTdL2dQ(T=T, dT=dT, L=L, dL=dL)
 
         # Make sure that we are dealing with vectors
         T, dT, L, dL = [numpy.ones_like(Q)*v for v in (T, dT, L, dL)]
 
         # Probe stores sorted values for convenience of resolution calculator
         idx = numpy.argsort(Q)
         self.T, self.dT = T[idx], dT[idx]
         self.L, self.dL = L[idx], dL[idx]
         self.Qo, self.dQo = Q[idx], dQ[idx]
         if R is not None:
             R = R[idx]
         if dR is not None:
             dR = dR[idx]
-        self.Ro = self.R = R
+        self.R = R
         self.dR = dR
 
         # By default the calculated points are the measured points.  Use
         # oversample() for a more accurate resolution calculations.
         self._set_calc(self.T, self.L)
 
     @staticmethod
@@ -243,81 +247,101 @@
         """
         Convert data from log to linear.
 
         Older reflectometry reduction code stored reflectivity in log base 10
         format.  Call probe.log10_to_linear() after loading this data to
         convert it to linear for subsequent display and fitting.
         """
-        if self.Ro is not None:
-            self.Ro = 10**self.Ro
+        if self.R is not None:
+            self.R = 10**self.R
             if self.dR is not None:
-                self.dR = self.Ro * self.dR * log(10)
-            self.R = self.Ro
+                self.dR = self.R * self.dR * log(10)
 
     def resynth_data(self):
         """
-        Generate new data according to the model R ~ N(Ro, dR).
+        Generate new data according to the model R' ~ N(R, dR).
 
         The resynthesis step is a precursor to refitting the data, as is
-        required for certain types of monte carlo error analysis.
-        """
-        self.R = self.Ro + numpy.random.randn(*self.Ro.shape)*self.dR
+        required for certain types of monte carlo error analysis.  The
+        first time it is run it will save the original R into Ro.  If you
+        reset R in the probe you will also need to reset Ro so that it
+        is used for subsequent resynth analysis.
+        """
+        if not hasattr(self, 'Ro'):
+            self._Ro = self.R
+        self.R = self._Ro + numpy.random.randn(*self._Ro.shape)*self.dR
 
     def restore_data(self):
         """
-        Restore the original data.
+        Restore the original data after resynth.
         """
-        self.R = self.Ro
+        self.R = self._Ro
+        del self._Ro
 
-    def simulate_data(self, theory, noise=None):
-        """
-        Set the data for the probe to R, adding random noise dR.
+    # CRUFT: Ro doesn't need to be part of the public interface.
+    @property
+    def Ro(self):
+        warnings.warn("Use probe.R instead of probe.Ro.", DeprecationWarning)
+        return getattr(self, '_Ro', self.R)
 
-        If noise is None, then use the uncertainty in the probe.
+    def simulate_data(self, theory, noise=2.):
+        r"""
+        Set the data for the probe to R + eps with eps ~ normal(dR^2).
 
-        As a hack, if noise<0, use the probe uncertainty but don't add
-        noise to the data.  Don't depend on this behavior.
-        """
-        self.Ro = theory[1]+0.
+        *theory* is (Q, R),
 
-        if numpy.isscalar(noise) and noise < 0:
-            # leave the probe uncertainty alone, and don't add noise to the data
-            self.R = self.Ro
-            return
+        If the percent *noise* is provided, set dR to R*noise/100 before
+        simulating.  *noise* defaults to 2% if no dR is present.
 
-        if noise is None:
-            pass
-        else:
-            self.dR = numpy.asarray(noise)
-            if len(self.dR.shape) == 0:  # noise is a scalar
-                self.dR = 0.01 * noise * self.Ro
-            self.dR[self.dR==0] = 1e-11
-
-        # Add noise to the theory function
-        self.resynth_data()
-
-        # Pretend the noisy theory function is the underlying measured data
-        # This allows us to resynthesize later, as needed.
-        self.Ro = self.R
+        Note that measured data estimates uncertainty from the number of
+        counts.  This means that points above the true value will have
+        larger uncertainty than points below the true value.  This bias
+        is not captured in the simulated data.
+        """
+        # Minimum value for dR after noise is added.
+        # TODO: does this need to be a parameter?
+        noise_floor = 1e-11
+
+        # Set the theory function.
+        R = numpy.asarray(theory[1], 'd')
+        assert R.shape == self.Q.shape
+        self.R = R
+
+        # Make sure scalar noise is positive.  This check is here to so that
+        # old interfaces will fail properly.
+        if numpy.isscalar(noise) and noise <= 0.:
+            raise ValueError("Noise level must be positive")
+
+        # If dR is missing then default noise to 2% so that dR will be set.
+        if self.dR is None and noise is None:
+            noise = 2.
+
+        # Set dR if noise was given or otherwise defaulted.
+        if noise is not None:
+            self.dR = 0.01 * numpy.asarray(noise) * self.R
+            self.dR[self.dR < noise_floor] = noise_floor
+
+        # Add noise according to dR.
+        self.R += numpy.random.randn(*self.R.shape)*self.dR
 
     def write_data(self, filename,
                    columns=('Q', 'R', 'dR'),
                    header=None):
         """
         Save the data to a file.
 
         *header* is a string with trailing \\n containing the file header.
         *columns* is a list of column names from Q, dQ, R, dR, L, dL, T, dT.
 
         The default is to write Q, R, dR data.
         """
         if header is None:
             header = "# %s\n"%' '.join(columns)
-        with open(filename, 'w') as fid:
-            fid.write(header)
+        with open(filename, 'wb') as fid:
+            fid.write(asbytes(header))
             data = numpy.vstack([getattr(self, c) for c in columns])
             numpy.savetxt(fid, data.T)
 
     def _set_calc(self, T, L):
         Q = TL2Q(T=T, L=L)
 
         idx = numpy.argsort(Q)
@@ -391,15 +415,17 @@
                     sample_broadening=self.sample_broadening.to_dict())
 
     def scattering_factors(self, material, density):
         """
         Returns the scattering factors associated with the material given
         the range of wavelengths/energies used in the probe.
         """
-        raise NotImplementedError
+        raise NotImplementedError(
+            "need radiation type in <%s> to compute sld for %s"
+            % (self.filename, material))
 
     def subsample(self, dQ):
         """
         Select points at most every dQ.
 
         Use this to speed up computation early in the fitting process.
 
@@ -419,15 +445,15 @@
         idx = numpy.unique(numpy.searchsorted(self.Qo, Q))
         #print len(idx), len(self.Qo)
 
         self.T, self.dT = self.T[idx], self.dT[idx]
         self.L, self.dL = self.L[idx], self.dL[idx]
         self.Qo, self.dQo = self.Qo[idx], self.dQo[idx]
         if self.R is not None:
-            self.Ro = self.R = self.R[idx]
+            self.R = self.R[idx]
         if self.dR is not None:
             self.dR = self.dR[idx]
         self._set_calc(self.T, self.L)
 
     def resolution_guard(self):
         r"""
         Make sure each measured $Q$ point has at least 5 calculated $Q$
@@ -584,36 +610,39 @@
                                      Vrho=Vrho*I, Virho=Virho*I)
         return calculator
 
     def save(self, filename, theory, substrate=None, surface=None):
         """
         Save the data and theory to a file.
         """
-        fresnel = self.fresnel(substrate, surface)
+        fresnel_calculator = self.fresnel(substrate, surface)
+        Q, FQ = self.apply_beam(self.calc_Q, fresnel_calculator(self.calc_Q))
         Q, R = theory
-        fid = open(filename, "w")
-        fid.write("# intensity: %.15g\n# background: %.15g\n"
-                  % (self.intensity.value, self.background.value))
         if len(Q) != len(self.Q):
             # Saving interpolated data
-            A = numpy.array((Q, R, fresnel(Q)))
-            fid.write("# %17s %20s %20s\n"
+            A = numpy.array((Q, R, numpy.interp(Q, self.Q, FQ)))
+            header = ("# %17s %20s %20s\n"
                       % ("Q (1/A)", "theory", "fresnel"))
         elif getattr(self, 'R', None) is not None:
             A = numpy.array((self.Q, self.dQ, self.R, self.dR,
-                             R, fresnel(self.Q)))
-            fid.write("# %17s %20s %20s %20s %20s %20s\n"
+                             R, FQ))
+            header = ("# %17s %20s %20s %20s %20s %20s\n"
                       % ("Q (1/A)", "dQ (1/A)", "R", "dR", "theory", "fresnel"))
         else:
-            A = numpy.array((self.Q, self.dQ, R, fresnel(self.Q)))
-            fid.write("# %17s %20s %20s %20s\n"
+            A = numpy.array((self.Q, self.dQ, R, FQ))
+            header = ("# %17s %20s %20s %20s\n"
                       % ("Q (1/A)", "dQ (1/A)", "theory", "fresnel"))
-        #print "A", self.Q.shape, A.shape
-        numpy.savetxt(fid, A.T, fmt="%20.15g")
-        fid.close()
+
+        header = ("# intensity: %.15g\n# background: %.15g\n"
+                    % (self.intensity.value, self.background.value)) + header
+
+        with open(filename, "wb") as fid:
+            #print("saving", A)
+            fid.write(asbytes(header))
+            numpy.savetxt(fid, A.T, fmt="%20.15g")
 
     def plot(self, view=None, **kwargs):
         """
         Plot theory against data.
 
         Need substrate/surface for Fresnel-normalized reflectivity
         """
@@ -871,41 +900,46 @@
         #return rho, irho[self._L_idx], rho_incoh
     scattering_factors.__doc__ = Probe.scattering_factors.__doc__
 
 
 class ProbeSet(Probe):
     def __init__(self, probes, name=None):
         self.probes = list(probes)
-        self.R = numpy.hstack(p.R for p in self.probes)
-        self.dR = numpy.hstack(p.dR for p in self.probes)
+        self.R = numpy.hstack([p.R for p in self.probes])
+        self.dR = numpy.hstack([p.dR for p in self.probes])
         self.name = name if name is not None else self.probes[0].name
 
         back_refls = [f.back_reflectivity for f in self.probes]
         if all(back_refls) or not any(back_refls):
             self.back_reflectivity = back_refls[0]
         else:
             raise ValueError("Cannot mix front and back reflectivity measurements")
 
     def parameters(self):
         return [p.parameters() for p in self.probes]
     parameters.__doc__ = Probe.parameters.__doc__
 
+    def to_dict(self):
+        """ Return a dictionary representation of the parameters """
+        return dict(type=type(self).__name__,
+                    pp=[p.to_dict() for p in self.probes])
+
     def resynth_data(self):
         for p in self.probes: p.resynth_data()
-        self.R = numpy.hstack(p.R for p in self.probes)
+        self.R = numpy.hstack([p.R for p in self.probes])
     resynth_data.__doc__ = Probe.resynth_data.__doc__
 
     def restore_data(self):
         for p in self.probes: p.restore_data()
-        self.R = numpy.hstack(p.R for p in self.probes)
+        self.R = numpy.hstack([p.R for p in self.probes])
     restore_data.__doc__ = Probe.restore_data.__doc__
 
-    def simulate_data(self, theory, noise=2):
+    def simulate_data(self, theory, noise=2.):
         """
-            Simulate data, allowing for noise to be a dR array for each Q point.
+        Simulate data, allowing for noise to be a dR array for each Q point.
         """
         Q, R = theory
         dR = numpy.asarray(noise)
         offset = 0
         for p in self.probes:
             n = len(p.Q)
             if len(self.dR.shape) > 0:
@@ -913,27 +947,27 @@
             p.simulate_data(theory=(Q[offset:offset+n], R[offset:offset+n]),
                             noise=noise)
             offset += n
     simulate_data.__doc__ = Probe.simulate_data.__doc__
 
     @property
     def Q(self):
-        return numpy.hstack(p.Q for p in self.probes)
+        return numpy.hstack([p.Q for p in self.probes])
 
     @property
     def calc_Q(self):
-        return numpy.unique(numpy.hstack(p.calc_Q for p in self.probes))
+        return numpy.unique(numpy.hstack([p.calc_Q for p in self.probes]))
 
     @property
     def dQ(self):
-        return numpy.hstack(p.dQ for p in self.probes)
+        return numpy.hstack([p.dQ for p in self.probes])
 
     @property
     def unique_L(self):
-        return numpy.unique(numpy.hstack(p.unique_L for p in self.probes))
+        return numpy.unique(numpy.hstack([p.unique_L for p in self.probes]))
 
     def oversample(self, **kw):
         for p in self.probes:
             p.oversample(**kw)
     oversample.__doc__ = Probe.oversample.__doc__
 
     def scattering_factors(self, material, density):
@@ -1086,18 +1120,18 @@
                       back_absorption=Po.back_absorption,
                       back_reflectivity=Po.back_reflectivity)
 
 
 def load4(filename, keysep=":", sep=None, comment="#", name=None,
           intensity=1, background=0, back_absorption=1,
           back_reflectivity=False, Aguide=270, H=0,
-          theta_offset=0, sample_broadening=0,
-          L=None, dL=None, T=None, dT=None,
+          theta_offset=None, sample_broadening=None,
+          L=None, dL=None, T=None, dT=None, dR=None,
           FWHM=False, radiation=None,
-          columns=None,
+          columns=None, data_range=(None, None),
          ):
     r"""
     Load in four column data Q, R, dR, dQ.
 
     The file is loaded with *bumps.data.parse_multi*.  *keysep*
     defaults to ':' so that header data looks like JSON key: value
     pairs.  *sep* is None so that the data uses white-space separated
@@ -1118,33 +1152,43 @@
     substrate or reflecting off the surface.
 
     *theta_offset* indicates sample alignment.  In order to use theta
     offset you need to be able to convert from Q to wavelength and angle
     by providing values for the wavelength or the angle, and the associated
     resolution.
 
-    For monochromatic sources you can supply *L*, *dLoL* when you call *load4*,
-    or you can store it in the header of the file::
+    *L*, *dL* in Angstroms can be used to recover angle and angular resolution
+    for monochromatic sources where wavelength is fixed and angle is varying.
+    These values can also be stored in the file header as::
 
         # wavelength: 4.75  # Ang
         # wavelength_resolution: 0.02  # Ang (1-sigma)
 
-    For time of flight sources, angle is fixed and wavelength is
-    varying, so you can supply *T*, *dT* in degrees when you call *load4*,
-    or you can store it in the header of the file::
+    *T*, *dT* in degrees can be used to recover wavelength and wavelength
+    dispersion for time of flight sources where angle is fixed and wavelength
+    is varying, or you can store them in the header of the file::
 
         # angle: 2  # degrees
         # angular_resolution: 0.2  # degrees (1-sigma)
 
     If both angle and wavelength are varying in the data, you can specify
     a separate value for each point, such the following::
 
         # wavelength: [1, 1.2, 1.5, 2.0, ...]
         # wavelength_resolution: [0.02, 0.02, 0.02, ...]
 
+    *dR* can be used to replace the uncertainty estimate for R in the
+    file with $\Delta R = R * \text{dR}$.  This allows files with only
+    two columns, *Q* and *R* to be loaded.  Note that points with *dR=0*
+    are automatically set to the minimum *dR>0* in the dataset.
+
+    Instead of constants, you can provide function, *dT = lambda T: f(T)*,
+    *dL = lambda L: f(L)* or *dR = lambda Q, R, dR: f(Q, R, dR)* for more
+    complex relationships (with *dR()* returning 1-$\sigma$ $\Delta R$).
+
     *sample_broadening* in degrees FWHM adds to the angular_resolution.
     Scale 1-$\sigma$ rms by $2 \surd(2 \ln 2) \approx 2.34$ to convert to FWHM.
 
     *Aguide* and *H* are parameters for polarized beam measurements
     indicating the magnitude and direction of the applied field.
 
     Polarized data is represented using a multi-section data file,
@@ -1153,119 +1197,188 @@
 
     *FWHM* is True if dQ, dT, dL are given as FWHM rather than 1-$\sigma$.
     *dR* is always 1-$\sigma$.  *sample_broadening* is always FWHM.
 
     *radiation* is 'xray' or 'neutron', depending on whether X-ray or
     neutron scattering length density calculator should be used for
     determining the scattering length density of a material.
+    Default is 'neutron'
 
     *columns* is a string giving the column order in the file.  Default
-    order is "Q R dR dQ".
+    order is "Q R dR dQ".  Note: include dR and dQ even if the file only
+    has two or three columns, but put the missing columns at the end.
+
+    *data_range* indicates which data rows to use.  Arguments are the
+    same as the list slice arguments, *(start, stop, step)*.  This follows
+    the usual semantics of list slicing, *L[start:stop:step]*, with
+    0-origin indices, stop is last plus one and step optional.  Use negative
+    numbers to count from the end.  Default is *(None, None)* for the entire
+    data set.
     """
-    data = parse_multi(filename, keysep=keysep, sep=sep, comment=comment)
+    entries = parse_multi(filename, keysep=keysep, sep=sep, comment=comment)
     if columns:
         actual = columns.split()
         natural = "Q R dR dQ".split()
-        order = [natural.index(k) for k in actual]
+        column_order = [natural.index(k) for k in actual]
     else:
-        order = [0, 1, 2, 3]
-    def _as_Qprobe(data):
-        Q, R, dR, dQ = (data[1][k] for k in order)
-
-        if FWHM: # dQ defaults to 1-sigma, if FWHM is not True
-            dQ = FWHM2sigma(dQ)
-
-        # support calculation of sld from material based on radiation type
-        if radiation is not None:
-            data_radiation = radiation
-        elif 'radiation' in data[0]:
-            data_radiation = json.loads(data[0]['radiation'])
-        else:
-            data_radiation = None
-        if data_radiation == 'xray':
-            make_probe = XrayProbe
-        elif data_radiation == 'neutron':
-            make_probe = NeutronProbe
-        else:
-            make_probe = Probe
-
-        # Get wavelength from header if it is not provided as an argument
-        data_L = data_T = None
-        if L is not None:
-            data_L = L
-        elif 'wavelength' in data[0]:
-            data_L = json.loads(data[0]['wavelength'])
-        if T is not None:
-            data_T = T
-        elif 'angle' in data[0]:
-            data_T = json.loads(data[0]['angle'])
-        if data_L is not None:
-            if dL is not None:
-                data_dL = dL
-            elif 'wavelength_resolution' in data[0]:
-                data_dL = json.loads(data[0]['wavelength_resolution'])
-            else:
-                raise ValueError("Need wavelength_resolution to determine dT")
-            data_dL = sigma2FWHM(data_dL) if not FWHM else data_dL
-            data_T = QL2T(Q, data_L)
-            data_dT = dQdL2dT(Q, dQ, data_L, data_dL)
-        elif data_T is not None:
-            if dT is not None:
-                data_dT = dT
-            elif 'angular_resolution' in data[0]:
-                data_dT = json.loads(data[0]['angular_resolution'])
-            else:
-                raise ValueError("Need angular_resolution to determine dL")
-            data_dT = sigma2FWHM(data_dT) if not FWHM else data_dT
-            data_L = QT2L(Q, data_T)
-            data_dLoL = dQdT2dLoL(Q, dQ, data_T, data_dT)
-            data_dL = data_dLoL * data_L
-
-        if data_L is not None:
-            probe = make_probe(
-                T=data_T, dT=data_dT,
-                L=data_L, dL=data_dL,
-                data=(R, dR),
-                name=name,
-                filename=filename,
-                intensity=intensity,
-                background=background,
-                back_absorption=back_absorption,
-                theta_offset=theta_offset,
-                sample_broadening=sample_broadening,
-                back_reflectivity=back_reflectivity,
-            )
-        else:
-            probe = QProbe(
-                Q, dQ, data=(R, dR),
-                name=name,
-                filename=filename,
-                intensity=intensity,
-                background=background,
-                back_absorption=back_absorption,
-                back_reflectivity=back_reflectivity,
-            )
-        return probe
-
-    if len(data) == 1:
-        probe = _as_Qprobe(data[0])
+        column_order = [0, 1, 2, 3]
+    index = slice(*data_range)
+    probe_args = dict(
+        name=name,
+        filename=filename,
+        intensity=intensity,
+        background=background,
+        back_absorption=back_absorption,
+        back_reflectivity=back_reflectivity,
+        theta_offset=theta_offset,
+        sample_broadening=sample_broadening,
+    )
+    data_args = dict(
+        radiation=radiation,
+        FWHM=FWHM,
+        T=T, L=L, dT=dT, dL=dL, dR=dR,
+        column_order=column_order,
+        index=index,
+    )
+    if len(entries) == 1:
+        probe = _data_as_probe(entries[0], probe_args, **data_args)
     else:
-        data_by_xs = dict((strip_quotes(d[0]["polarization"]), _as_Qprobe(d))
-                          for d in data)
+        data_by_xs = {strip_quotes(entry[0]["polarization"])
+                      : _data_as_probe(entry, probe_args, **data_args)
+                      for entry in entries}
         if not set(data_by_xs.keys()) <= set('-- -+ +- ++'.split()):
             raise ValueError("Unknown cross sections in: "
                              + ", ".join(sorted(data_by_xs.keys())))
         xs = [data_by_xs.get(xs, None) for xs in ('--', '-+', '+-', '++')]
 
         if any(isinstance(d, QProbe) for d in xs if d is not None):
             probe = PolarizedQProbe(xs, Aguide=Aguide, H=H)
         else:
             probe = PolarizedNeutronProbe(xs, Aguide=Aguide, H=H)
     return probe
 
+def _data_as_probe(entry, probe_args, T, L, dT, dL, dR, FWHM, radiation,
+                   column_order, index):
+    name = probe_args['filename']
+    header, data = entry
+    if len(data) == 2:
+        data_Q, data_R = (data[k][index] for k in column_order[:2])
+        data_dR, data_dQ = None, None
+        if dR is None:
+            raise ValueError("Need dR for two column data in %r" % name)
+    elif len(data) == 3:
+        data_Q, data_R, data_dR = (data[k][index] for k in column_order[:3])
+        data_dQ = None
+    else:
+        data_Q, data_R, data_dR, data_dQ = (data[k][index] for k in column_order)
+
+    if FWHM and data_dQ is not None: # dQ is already 1-sigma when not FWHM
+        data_dQ = FWHM2sigma(data_dQ)
+
+    # Override dR in the file if desired.
+    # Make sure the computed dR is positive (otherwise chisq is infinite) by
+    # choosing the smallest positive uncertainty to replace the invalid values.
+    if dR is not None:
+        data_dR = dR(data_Q, data_R, data_dR) if callable(dR) else data_R * dR
+        data_dR[data_dR <= 0] = numpy.min(data_dR[data_dR > 0])
+
+    # support calculation of sld from material based on radiation type
+    if radiation is not None:
+        data_radiation = radiation
+    elif 'radiation' in header:
+        data_radiation = json.loads(header['radiation'])
+    else:
+        # Default to neutron data if radiation not given in head.
+        data_radiation = 'neutron'
+        #data_radiation = None
+
+    if data_radiation == 'xray':
+        make_probe = XrayProbe
+    elif data_radiation == 'neutron':
+        make_probe = NeutronProbe
+    else:
+        make_probe = Probe
+
+    # Get T,dT,L,dL from header if it is not provided as an argument
+    def fetch_key(key, override):
+        if override is not None:
+            return override
+        elif key in header:
+            return json.loads(header[key])
+        else:
+            return None
+
+    # Get T and L, either from user input or from datafile.
+    data_T = fetch_key('angle', T)
+    data_L = fetch_key('wavelength', L)
+
+    # If one of T and L is missing, reconstruct it from Q
+    if data_T is None and data_L is not None:
+        data_T = QL2T(data_Q, data_L)
+    if data_L is None and data_T is not None:
+        data_L = QT2L(data_Q, data_T)
+
+
+    # Get dT and dL, either from user input or from datafile.
+    data_dL = fetch_key('wavelength_resolution', dL)
+    data_dT = fetch_key('angular_resolution', dT)
+
+    # Support dT = f(T), dL = f(L)
+    if callable(data_dT):
+        if data_T is None:
+            raise ValueError("Need T to determine dT for %r" % name)
+        data_dT = data_dT(data_T)
+    if callable(data_dL):
+        if data_L is None:
+            raise ValueError("Need L to determine dL for %r" % name)
+        data_dL = data_dL(data_L)
+
+    # Convert input dT,dL to FWHM if necessary.
+    if data_dL is not None and not FWHM:
+        data_dL = sigma2FWHM(data_dL)
+    if data_dT is not None and not FWHM:
+        data_dT = sigma2FWHM(data_dT)
+
+    # If one of T and L is missing, reconstruct it from Q.
+    if data_dT is None and not any(v is None for v in (data_L, data_dL, data_dQ)):
+        data_dT = dQdL2dT(data_Q, data_dQ, data_L, data_dL)
+    if data_dL is None and not any(v is None for v in (data_T, data_dT, data_dQ)):
+        data_dLoL = dQdT2dLoL(data_Q, data_dQ, data_T, data_dT)
+        data_dL = data_dLoL * data_L
+
+    # Check reconstruction if user provided any of T, L, dT, or dL.
+    # Also, sample_offset or sample_broadening.
+    offset = probe_args['theta_offset']
+    broadening = probe_args['sample_broadening']
+    if any(v is not None for v in (T, dT, L, dL, offset, broadening)):
+        if data_T is None:
+            raise ValueError("Need L to determine T from Q for %r" % name)
+        if data_L is None:
+            raise ValueError("Need T to determine L from Q for %r" % name)
+        if data_dT is None:
+            raise ValueError("Need dL to determine dT from dQ for %r" % name)
+        if data_dL is None:
+            raise ValueError("Need dT to determine dL from dQ for %r" % name)
+
+    # Build the probe, or the Q probe if we don't have angle and wavelength.
+    if all(v is not None for v in (data_T, data_L, data_dT, data_dL)):
+        probe = make_probe(
+            T=data_T, dT=data_dT,
+            L=data_L, dL=data_dL,
+            data=(data_R, data_dR),
+            **probe_args)
+    else:
+        # QProbe doesn't accept theta_offset or sample_broadening
+        qprobe_args = probe_args.copy()
+        qprobe_args.pop('theta_offset')
+        qprobe_args.pop('sample_broadening')
+        probe = QProbe(data_Q, data_dQ, data=(data_R, data_dR), **qprobe_args)
+
+    return probe
+
 
 class QProbe(Probe):
     """
     A pure Q, R probe
 
     This probe with no possibility of tricks such as looking up the
     scattering length density based on wavelength, or adjusting for
@@ -1291,20 +1404,26 @@
 
         if data is not None:
             R, dR = data
         else:
             R, dR = None, None
 
         self.Q, self.dQ = Q, dQ
-        self.Ro = self.R = R
+        self.R = R
         self.dR = dR
         self.unique_L = None
         self.calc_Qo = self.Qo
         self.name = name
 
+    def scattering_factors(self, material, density):
+        raise NotImplementedError(
+            "need radiation type and wavelength in <%s> to compute sld for %s"
+            % (self.filename, material))
+    scattering_factors.__doc__ = Probe.scattering_factors.__doc__
+
 
 def measurement_union(xs):
     """
     Determine the unique (T, dT, L, dL) across all datasets.
     """
 
     # First gather a set of unique tuples in angle and wavelength
@@ -1412,16 +1531,16 @@
 
     def restore_data(self):
         for p in self.xs:
             if p is not None:
                 p.restore_data()
     restore_data.__doc__ = Probe.restore_data.__doc__
 
-    def simulate_data(self, theory, noise=2):
-        if numpy.isscalar(noise):
+    def simulate_data(self, theory, noise=2.):
+        if noise is None or numpy.isscalar(noise):
             noise = [noise]*4
         for data_k, theory_k, noise_k in zip(self.xs, theory, noise):
             if data_k is not None:
                 data_k.simulate_data(theory=theory_k, noise=noise_k)
     simulate_data.__doc__ = Probe.simulate_data.__doc__
 
     def _check(self):
@@ -1676,17 +1795,17 @@
 def _interpolate_Q(Q, dQ, n):
     """
     Helper function to interpolate between data points.
 
     *n* is the number of points to show between existing points.
     """
     if n > 0:
-        # Extend the Q-range by one point on either side
-        Q = numpy.hstack((0.5*(Q[0]-Q[1]), Q, 0.5*(3.*Q[-1]-Q[-2])))
-        dQ = numpy.hstack((0.5*(dQ[0]-dQ[1]), dQ, 0.5*(3.*dQ[-1]-dQ[-2])))
+        # Extend the Q-range by 1/2 interval on either side
+        Q = numpy.hstack((0.5*(3.*Q[0]-Q[1]), Q, 0.5*(3.*Q[-1]-Q[-2])))
+        dQ = numpy.hstack((0.5*(3.*dQ[0]-dQ[1]), dQ, 0.5*(3.*dQ[-1]-dQ[-2])))
         index = numpy.arange(0, len(Q), dtype='d')
         subindex = numpy.arange(0, (n+1)*(len(Q)-1)+1, dtype='d')/(n+1.)
         Q = numpy.interp(subindex, index, Q)
         dQ = numpy.interp(subindex, index, dQ)
     return Q, dQ
 
 class PolarizedQProbe(PolarizedNeutronProbe):
```

### Comparing `refl1d-0.8.8/refl1d/profile.py` & `refl1d-0.8.9/refl1d/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,18 @@
         self._slabs_rho[self._num_slabs, :, 0] = rho
         self._slabs_rho[self._num_slabs, :, 1] = irho
         self._num_slabs += 1
 
     def add_magnetism(self, anchor, w, rhoM=0, thetaM=270., sigma=0):
         """
         Add magnetic layers.
+
+        Note that *sigma* is a pair *(interface_below, interface_above)*
+        representing the magnetic roughness, which may be different
+        from the nuclear roughness at the layer boundaries.
         """
         w = np.asarray(w, 'd')
         if np.isscalar(sigma):
             sigma = (sigma, sigma)
         self._magnetic_sections.append((np.vstack((w, rhoM, thetaM)),
                                         anchor, sigma))
 
@@ -545,15 +549,14 @@
         #   magnetism has been specified
         substrate_magnetism = isnan(sigmas[0][0])
         if substrate_magnetism:
             slices = [[[], [], []]]
         else:
             slices = [[[0], [0], [blocks[0][2, 0]]]]
         interfaces = []
-        sigma = None
         pos = 0
         for i, B in enumerate(blocks):
             anchor = offsets[i]
             w = anchor - pos
             if w >= gap_size:  # Big gap, so need spacer
                 # Target average theta between blocks.
                 if i == 0:
```

### Comparing `refl1d-0.8.8/refl1d/rebin.py` & `refl1d-0.8.9/refl1d/rebin.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/reflectivity.py` & `refl1d-0.8.9/refl1d/reflectivity.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/resolution.py` & `refl1d-0.8.9/refl1d/resolution.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/snsdata.py` & `refl1d-0.8.9/refl1d/snsdata.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/staj.py` & `refl1d-0.8.9/refl1d/staj.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/stajconvert.py` & `refl1d-0.8.9/refl1d/stajconvert.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/stitch.py` & `refl1d-0.8.9/refl1d/stitch.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/support.py` & `refl1d-0.8.9/refl1d/support.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/util.py` & `refl1d-0.8.9/refl1d/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 __all__ = ["merge_ends"]
 
+import sys
+
 import numpy
 
+# CRUFT: 2.7 support
+if sys.version_info[0] > 2:
+    def asbytes(s):
+        return s.encode('utf-8')
+else:
+    def asbytes(s):
+        return s
+
 def merge_ends(w, p, tol=1e-3):
     """
     join the leading and trailing ends of the profile together so fewer
     slabs are required and so that gaussian roughness can be used.
     """
     # TODO: accept rho, rhoi pairs as well
     # TODO: make sure we apply an interface to the right as well as the left
```

### Comparing `refl1d-0.8.8/refl1d/view/binder.py` & `refl1d-0.8.9/refl1d/view/binder.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/data_view.py` & `refl1d-0.8.9/refl1d/view/data_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,35 +69,40 @@
         # Grey out items that are not currently implemented.
         frame = wx.GetTopLevelParent(self)
         menu = wx.Menu()
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "&Fresnel",
                                           "Plot R/R_F")
         frame.Bind(wx.EVT_MENU, self.OnFresnel, _item)
-        _item.Check(True)
+        _item.Check(Probe.view == 'fresnel')
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "Log Fresnel",
                                           "Plot log R/R_F")
         frame.Bind(wx.EVT_MENU, self.OnLogFresnel, _item)
+        _item.Check(Probe.view == 'logfresnel')
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "Li&near",
                                           "Plot linear R")
         frame.Bind(wx.EVT_MENU, self.OnLinear, _item)
+        _item.Check(Probe.view == 'linear')
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "&Log",
                                           "Plot log R")
         frame.Bind(wx.EVT_MENU, self.OnLog, _item)
+        _item.Check(Probe.view == 'log')
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "&Q4",
                                           "Plot R * Q^4")
         frame.Bind(wx.EVT_MENU, self.OnQ4, _item)
+        _item.Check(Probe.view == 'q4')
         _item = menu.AppendRadioItem(wx.ID_ANY,
                                           "&SA",
                                           "Plot spin asymmetry")
         frame.Bind(wx.EVT_MENU, self.OnSA, _item)
+        _item.Check(Probe.view == 'SA')
 
         menu.AppendSeparator()
 
         _item = menu.Append(wx.ID_ANY,
                                  "&Residuals",
                                  "Plot residuals (R_theory - R)/dR")
         frame.Bind(wx.EVT_MENU, self.OnResiduals, _item)
```

### Comparing `refl1d-0.8.8/refl1d/view/demo.py` & `refl1d-0.8.9/refl1d/view/demo.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/interactor.py` & `refl1d-0.8.9/refl1d/view/interactor.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/interface.py` & `refl1d-0.8.9/refl1d/view/interface.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/layer.py` & `refl1d-0.8.9/refl1d/view/layer.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/layer_dialog.py` & `refl1d-0.8.9/refl1d/view/layer_dialog.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/model_view.py` & `refl1d-0.8.9/refl1d/view/model_view.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/monoi.py` & `refl1d-0.8.9/refl1d/view/monoi.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/polymeri.py` & `refl1d-0.8.9/refl1d/view/polymeri.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/profilei.py` & `refl1d-0.8.9/refl1d/view/profilei.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/registry.py` & `refl1d-0.8.9/refl1d/view/registry.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/thickness.py` & `refl1d-0.8.9/refl1d/view/thickness.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d/view/util.py` & `refl1d-0.8.9/refl1d/view/util.py`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/refl1d.egg-info/PKG-INFO` & `refl1d-0.8.9/refl1d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: refl1d
-Version: 0.8.8
+Version: 0.8.9
 Summary: 1-D reflectometry modeling
 Home-page: http://www.reflectometry.org/danse/model1d.html
 Author: Paul Kienzle
 Author-email: pkienzle@nist.gov
 License: UNKNOWN
 Description: Refl1D
         ======
```

### Comparing `refl1d-0.8.8/refl1d.egg-info/SOURCES.txt` & `refl1d-0.8.9/refl1d.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 refl1d/names.py
 refl1d/ncnrdata.py
 refl1d/plottable.py
 refl1d/polymer.py
 refl1d/probe.py
 refl1d/profile.py
 refl1d/rebin.py
+refl1d/refl_tr.py
 refl1d/reflectivity.py
 refl1d/resolution.py
 refl1d/snsdata.py
 refl1d/staj.py
 refl1d/stajconvert.py
 refl1d/stitch.py
 refl1d/support.py
```

### Comparing `refl1d-0.8.8/refl1d.iss` & `refl1d-0.8.9/refl1d.iss`

 * *Files identical despite different names*

### Comparing `refl1d-0.8.8/setup.py` & `refl1d-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         # minimum OSX version is bumped from the default 10.6 up
         # to 10.10.  Don't know if this is because of the mac
         # setup (older development libraries not installed) or
         # because of the anaconda build (targetted to 10.6) or
         # some combination.  Override by setting the deployment
         # target on the command line.  Curiously, Xcode can
         # target c++ code to 10.7 on the same machine.
-        os.environ.setdefault('MACOSX_DEPLOYMENT_TARGET', '10.10')
+        #os.environ.setdefault('MACOSX_DEPLOYMENT_TARGET', '10.10')
+        os.environ.setdefault('MACOSX_DEPLOYMENT_TARGET', '10.13')
 
     S = ("reflmodule.cc", "methods.cc",
          "reflectivity.cc", "magnetic.cc",
          "contract_profile.cc",
          "convolve.c", "convolve_sampled.c",
         )
```

### Comparing `refl1d-0.8.8/setup_py2exe.py` & `refl1d-0.8.9/setup_py2exe.py`

 * *Files identical despite different names*


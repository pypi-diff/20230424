# Comparing `tmp/bohra-1.2.9.tar.gz` & `tmp/bohra-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bohra-1.2.9.tar", last modified: Fri Mar 13 02:34:04 2020, max compression
+gzip compressed data, was "dist/bohra-2.2.0.tar", last modified: Mon Apr 24 04:09:57 2023, max compression
```

## Comparing `bohra-1.2.9.tar` & `bohra-2.2.0.tar`

### file list

```diff
@@ -1,62 +1,157 @@
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:04.000000 bohra-1.2.9/
--rw-r--r--   0 1424986825 1424491009    35149 2019-07-28 01:44:48.000000 bohra-1.2.9/LICENSE.txt
--rw-r--r--   0 1424986825 1424491009       71 2019-07-31 06:38:33.000000 bohra-1.2.9/MANIFEST.in
--rw-r--r--   0 1424986825 1424491009    16714 2020-03-13 02:34:04.000000 bohra-1.2.9/PKG-INFO
--rw-r--r--   0 1424986825 1424491009    13405 2020-03-11 05:04:16.000000 bohra-1.2.9/README.md
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:03.000000 bohra-1.2.9/bohra/
--rw-r--r--   0 1424986825 1424491009    37880 2020-03-13 02:32:55.000000 bohra-1.2.9/bohra/SnpDetection.py
--rw-r--r--   0 1424986825 1424491009     8434 2020-03-12 06:16:45.000000 bohra-1.2.9/bohra/Utils.py
--rw-r--r--   0 1424986825 1424491009      216 2019-08-07 06:34:59.000000 bohra-1.2.9/bohra/__init__.py
--rw-r--r--   0 1424986825 1424491009     9281 2020-03-12 19:12:36.000000 bohra-1.2.9/bohra/bohra.py
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:03.000000 bohra-1.2.9/bohra/templates/
--rw-r--r--   0 1424986825 1424491009      932 2019-09-21 05:50:22.000000 bohra-1.2.9/bohra/templates/cluster.tmpl
--rw-r--r--   0 1424986825 1424491009      724 2020-03-12 02:03:40.000000 bohra-1.2.9/bohra/templates/config_snippy.yaml
--rwxr-xr-x   0 1424986825 1424491009    23017 2020-02-27 03:19:09.000000 bohra-1.2.9/bohra/templates/index.html
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:03.000000 bohra-1.2.9/bohra/tests/
--rw-r--r--   0 1424986825 1424491009        0 2019-07-28 01:44:48.000000 bohra-1.2.9/bohra/tests/test.bed
--rw-r--r--   0 1424986825 1424491009  7163607 2019-07-28 01:44:48.000000 bohra-1.2.9/bohra/tests/test.gbk
--rw-r--r--   0 1424986825 1424491009      788 2019-07-28 01:44:48.000000 bohra-1.2.9/bohra/tests/test.tab
--rw-r--r--   0 1424986825 1424491009     4582 2020-03-06 05:21:05.000000 bohra-1.2.9/bohra/tests/test_bohra.py
--rw-r--r--   0 1424986825 1424491009        0 2019-07-28 01:44:48.000000 bohra-1.2.9/bohra/tests/test_file.txt
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:04.000000 bohra-1.2.9/bohra/utils/
--rw-r--r--   0 1424986825 1424491009     3160 2020-03-12 04:29:48.000000 bohra-1.2.9/bohra/utils/assemble.py
--rw-r--r--   0 1424986825 1424491009     2665 2020-03-11 05:12:59.000000 bohra-1.2.9/bohra/utils/assembly_combine.py
--rw-r--r--   0 1424986825 1424491009     2502 2020-03-12 04:30:45.000000 bohra-1.2.9/bohra/utils/assembly_stat.py
--rw-r--r--   0 1424986825 1424491009     8936 2020-03-12 19:00:10.000000 bohra-1.2.9/bohra/utils/bohra.smk
--rw-r--r--   0 1424986825 1424491009      911 2020-03-09 23:52:10.000000 bohra-1.2.9/bohra/utils/collate_tomls.py
--rw-r--r--   0 1424986825 1424491009     1472 2020-03-09 20:37:32.000000 bohra-1.2.9/bohra/utils/combine_kraken.py
--rw-r--r--   0 1424986825 1424491009     1864 2020-03-11 05:06:05.000000 bohra-1.2.9/bohra/utils/combine_mlst.py
--rw-r--r--   0 1424986825 1424491009     1392 2020-03-11 05:11:35.000000 bohra-1.2.9/bohra/utils/combine_resistome.py
--rw-r--r--   0 1424986825 1424491009     1411 2020-03-11 02:19:42.000000 bohra-1.2.9/bohra/utils/combine_seqdata.py
--rw-r--r--   0 1424986825 1424491009    17297 2020-03-11 05:11:24.000000 bohra-1.2.9/bohra/utils/compile.py
--rw-r--r--   0 1424986825 1424491009     1780 2020-03-12 04:34:58.000000 bohra-1.2.9/bohra/utils/gubbins.py
--rw-r--r--   0 1424986825 1424491009     1198 2019-07-30 02:34:20.000000 bohra-1.2.9/bohra/utils/iqtree_generator.sh
--rw-r--r--   0 1424986825 1424491009     3362 2020-03-12 04:38:18.000000 bohra-1.2.9/bohra/utils/kraken.py
--rw-r--r--   0 1424986825 1424491009     1459 2020-03-11 02:20:48.000000 bohra-1.2.9/bohra/utils/mash.py
--rw-r--r--   0 1424986825 1424491009     2277 2020-03-12 04:40:52.000000 bohra-1.2.9/bohra/utils/mlst.py
--rw-r--r--   0 1424986825 1424491009      730 2020-03-12 04:41:25.000000 bohra-1.2.9/bohra/utils/move_outputs.py
--rw-r--r--   0 1424986825 1424491009     1092 2020-03-12 04:46:54.000000 bohra-1.2.9/bohra/utils/pan_figure.py
--rw-r--r--   0 1424986825 1424491009     2002 2020-03-12 05:33:03.000000 bohra-1.2.9/bohra/utils/preview.py
--rw-r--r--   0 1424986825 1424491009     2043 2020-03-12 04:49:43.000000 bohra-1.2.9/bohra/utils/prokka.py
--rw-r--r--   0 1424986825 1424491009     2339 2020-03-12 04:52:47.000000 bohra-1.2.9/bohra/utils/resistome.py
--rw-r--r--   0 1424986825 1424491009     1617 2020-03-12 04:56:55.000000 bohra-1.2.9/bohra/utils/roary.py
--rw-r--r--   0 1424986825 1424491009     5179 2019-07-30 04:36:10.000000 bohra-1.2.9/bohra/utils/roary2svg.pl
--rw-r--r--   0 1424986825 1424491009     1482 2020-03-12 06:17:27.000000 bohra-1.2.9/bohra/utils/run_iqtree.py
--rw-r--r--   0 1424986825 1424491009     3922 2020-03-12 02:06:52.000000 bohra-1.2.9/bohra/utils/seqdata.py
--rw-r--r--   0 1424986825 1424491009     2733 2020-03-12 04:16:31.000000 bohra-1.2.9/bohra/utils/snippy.py
--rw-r--r--   0 1424986825 1424491009     3247 2020-03-12 04:25:47.000000 bohra-1.2.9/bohra/utils/snippy_core.py
--rw-r--r--   0 1424986825 1424491009     2697 2020-03-12 04:24:18.000000 bohra-1.2.9/bohra/utils/snippy_qc.py
--rw-r--r--   0 1424986825 1424491009      990 2020-03-10 00:08:34.000000 bohra-1.2.9/bohra/utils/snp_dists.py
--rw-r--r--   0 1424986825 1424491009       91 2020-02-19 05:01:20.000000 bohra-1.2.9/bohra/utils/tomls.py
--rw-r--r--   0 1424986825 1424491009     1614 2020-03-11 06:10:03.000000 bohra-1.2.9/bohra/utils/write_report.py
--rw-r--r--   0 1424986825 1424491009       17 2020-03-13 02:33:37.000000 bohra-1.2.9/bohra/version.py
-drwxr-xr-x   0 1424986825 1424491009        0 2020-03-13 02:34:03.000000 bohra-1.2.9/bohra.egg-info/
--rw-r--r--   0 1424986825 1424491009    16714 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/PKG-INFO
--rw-r--r--   0 1424986825 1424491009     1314 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/SOURCES.txt
--rw-r--r--   0 1424986825 1424491009        1 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/dependency_links.txt
--rw-r--r--   0 1424986825 1424491009       44 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/entry_points.txt
--rw-r--r--   0 1424986825 1424491009        1 2019-08-07 06:36:45.000000 bohra-1.2.9/bohra.egg-info/not-zip-safe
--rw-r--r--   0 1424986825 1424491009      126 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/requires.txt
--rw-r--r--   0 1424986825 1424491009        6 2020-03-13 02:34:02.000000 bohra-1.2.9/bohra.egg-info/top_level.txt
--rw-r--r--   0 1424986825 1424491009     1141 2020-03-13 02:34:04.000000 bohra-1.2.9/setup.cfg
--rw-r--r--   0 1424986825 1424491009       69 2020-03-06 03:52:01.000000 bohra-1.2.9/setup.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.2.0/LICENSE.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      202 2021-08-27 05:57:12.000000 bohra-2.2.0/MANIFEST.in
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    16293 2023-04-24 04:09:57.000000 bohra-2.2.0/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    13280 2023-03-31 02:22:29.000000 bohra-2.2.0/README.md
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/CustomLog.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    30708 2023-04-24 03:55:45.000000 bohra-2.2.0/bohra/SnpDetection.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.2.0/bohra/Utils.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.2.0/bohra/__init__.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9065 2023-04-24 03:56:33.000000 bohra-2.2.0/bohra/bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     5409 2023-04-04 03:44:06.000000 bohra-2.2.0/bohra/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/collation/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/collation/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.2.0/bohra/modules/collation/bin/add_header_mlst.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1480 2021-12-19 02:04:48.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_asm.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_kraken2.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      343 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_plasmids.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     2517 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/collate_stats.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    13486 2022-03-05 01:26:46.000000 bohra-2.2.0/bohra/modules/collation/bin/compile.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.2.0/bohra/modules/collation/bin/snippy_qc.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/bin/wrangle_mobsuite.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/collation/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     7114 2023-03-31 02:12:30.000000 bohra-2.2.0/bohra/modules/collation/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/csvtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/csvtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1140 2023-03-31 01:20:40.000000 bohra-2.2.0/bohra/modules/csvtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/csvtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/gubbins/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/gubbins/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1020 2023-03-31 01:20:31.000000 bohra-2.2.0/bohra/modules/gubbins/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/gubbins/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/iqtree/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/iqtree/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1212 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/bin/iqtree_generator.sh
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1229 2023-03-31 01:20:24.000000 bohra-2.2.0/bohra/modules/iqtree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/iqtree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/kraken2/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/kraken2/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1282 2023-03-31 01:20:15.000000 bohra-2.2.0/bohra/modules/kraken2/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/kraken2/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/sketch/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/sketch/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1415 2023-03-31 01:20:11.000000 bohra-2.2.0/bohra/modules/mash/sketch/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/sketch/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mash/triangle/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/triangle/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1069 2023-03-31 01:20:06.000000 bohra-2.2.0/bohra/modules/mash/triangle/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mash/triangle/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mlst/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mlst/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1427 2023-03-31 06:32:25.000000 bohra-2.2.0/bohra/modules/mlst/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1721 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mlst/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/mobsuite/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mobsuite/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-03-31 01:19:55.000000 bohra-2.2.0/bohra/modules/mobsuite/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/mobsuite/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/panaroo/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.2.0/bohra/modules/panaroo/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1414 2023-04-24 03:58:15.000000 bohra-2.2.0/bohra/modules/panaroo/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.2.0/bohra/modules/panaroo/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/prokka/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/prokka/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-03-31 01:19:42.000000 bohra-2.2.0/bohra/modules/prokka/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/prokka/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/quicktree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/quicktree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1090 2023-03-31 01:19:37.000000 bohra-2.2.0/bohra/modules/quicktree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/quicktree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/resistome/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/resistome/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.2.0/bohra/modules/resistome/bin/combine.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/bin/concat.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/bin/meta.yaml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2940 2023-03-31 01:19:31.000000 bohra-2.2.0/bohra/modules/resistome/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/resistome/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/roary2svg/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/roary2svg/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/bin/roary2svg.pl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/roary2svg/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1461 2023-03-31 01:19:19.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/fx2tab/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqkit/stats/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/stats/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1570 2023-03-31 01:19:14.000000 bohra-2.2.0/bohra/modules/seqkit/stats/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqkit/stats/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/seqtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1132 2023-03-31 01:21:08.000000 bohra-2.2.0/bohra/modules/seqtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/seqtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/shovill/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/shovill/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1295 2023-03-31 01:21:34.000000 bohra-2.2.0/bohra/modules/shovill/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/shovill/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/skesa/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/skesa/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1277 2023-03-31 01:21:53.000000 bohra-2.2.0/bohra/modules/skesa/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/skesa/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.2.0/bohra/modules/snippy/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1663 2023-04-13 00:09:28.000000 bohra-2.2.0/bohra/modules/snippy/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy_clean/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.2.0/bohra/modules/snippy_clean/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      944 2023-03-31 01:22:37.000000 bohra-2.2.0/bohra/modules/snippy_clean/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.2.0/bohra/modules/snippy_clean/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snippy_core/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy_core/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1350 2023-03-31 01:22:43.000000 bohra-2.2.0/bohra/modules/snippy_core/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snippy_core/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/snp_dists/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snp_dists/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1095 2023-03-31 01:23:35.000000 bohra-2.2.0/bohra/modules/snp_dists/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/snp_dists/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/modules/spades/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/spades/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1406 2023-03-31 01:23:33.000000 bohra-2.2.0/bohra/modules/spades/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/modules/spades/meta.yml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1963 2023-03-31 01:27:18.000000 bohra-2.2.0/bohra/nextflow.config
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/templates/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.2.0/bohra/templates/cluster.tmpl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.2.0/bohra/templates/config_snippy.yaml
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17031 2021-11-23 01:23:44.000000 bohra-2.2.0/bohra/templates/index.html
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    17104 2021-11-22 01:20:59.000000 bohra-2.2.0/bohra/templates/report_analysis.json
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/tests/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.bed
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.gbk
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test.tab
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.2.0/bohra/tests/test_bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.0/bohra/tests/test_file.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-04-24 04:02:07.000000 bohra-2.2.0/bohra/version.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra/workflows/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2577 2023-03-31 06:22:16.000000 bohra-2.2.0/bohra/workflows/assemble_typing.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/collation.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1519 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/common.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4714 2023-03-31 06:22:16.000000 bohra-2.2.0/bohra/workflows/default.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.2.0/bohra/workflows/pangenome.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      402 2021-08-24 07:45:44.000000 bohra-2.2.0/bohra/workflows/preview.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    16293 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3728 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/SOURCES.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/dependency_links.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/entry_points.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.2.0/bohra.egg-info/not-zip-safe
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      117 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/requires.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-04-24 04:09:57.000000 bohra-2.2.0/bohra.egg-info/top_level.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1131 2023-04-24 04:09:57.000000 bohra-2.2.0/setup.cfg
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.2.0/setup.py
```

### Comparing `bohra-1.2.9/LICENSE.txt` & `bohra-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/PKG-INFO` & `bohra-2.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 Metadata-Version: 2.1
 Name: bohra
-Version: 1.2.9
+Version: 2.2.0
 Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
 Home-page: https://github.com/kristyhoran/bohra
 Author: Kristy Horan
 Author-email: kristyhoran15@gmail.com
 License: UNKNOWN
 Description: [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra)
         [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
         
-        ![Image](https://github.com/kristyhoran/bohra/blob/master/bohra.png)
         
-        # Bohra 
         
-        Bohra has a new look! 
-        * A new preview mode for 'sneak peak' at your dataset. 
-        * `rerun` has been deprecated. If you would like to rerun a job etc; use the run command.
-        * If rerunning a job, a new --keep flag to archive previous report files.
-        * Built in filtering features to automatically remove isolates with low average coverage or alignment to your reference.
-        * Provide a standardised config file for commonly used settings.
+        # Bohra
         
-        Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. The pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+        Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+        
+        ## Bohra has a new look! Welcome to Bohra-NF
+        
+        **New features**
+        
+        * Pipeline written in [Nextflow](https://www.nextflow.io)
+        * Default mode
+            * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
+            * MobSuite integration.
+            * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
+        * Panaroo with visualisation of pan-genome.
+        * Improved support for different computing environments.
+        
+        **Comming soon**
+        
+        * Improved report structure
+        * Option to add your own modules
+        
+        
+        **Accreditation**
+        
+        * _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
+        * _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
         
         ### Motivation
         
-        Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Snakemake](https://snakemake.readthedocs.io/en/stable/). 
+        Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Nextflow](https://www.nextflow.io).
         
         ### Etymology
         
-        Bohra the name of an exinct species of tree kangaroo that lived on the nullarbor. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on *snippy* (named for a very famous kangaroo) and was inspired by *nullarbor*. 
+        Bohra the name of an exinct species of tree kangaroo that lived on the Nullarbor plain in Australia. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on [*snippy*](https://github.com/tseemann/snippy) (named for a very famous kangaroo) and was inspired by [*nullarbor*](https://github.com/tseemann/nullarbor). 
         
         
         ## Pipeline
         
-        Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports.
+        Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports. An addtional file can be porvided with the paths to any assemblies that have already been generated. This is a helpful saver of time.
+        
         ![Image](https://github.com/MDU-PHL/bohra/blob/master/workflow.png)
         
-        Bohra can be run in four modes
-        1. Preview (DEFAULT)
+        Bohra can be run in three modes
+        1. Preview
         * Calculate mash-distances
         * Build a mash-tree
+        * Report sequencing statistics
+        * Species identification (providing you have kraken2 database setup properly ;) )
         
-        2. SNPs, species ID and Assembly based tools (MLST, Resistome and annotation)
-        * Clean reads
+        2. Default SNPs, species ID, assemly, MLST, Resistome and annotation)
         * Call variants
         * Generate a phylogenetic tree
-        * Assemble
-        * Species identification
+        * Assemble 
         * MLST
         * Resistome
         * Annotate
+        * Plasmid prediction
+        * Species identification
         
-        4. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
-        * Clean reads
+        3. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
         * Call variants
         * Generate a phylogenetic tree
-        * Assemble
-        * Species identification
+        * Assemble 
         * MLST
         * Resistome
         * Annotate
+        * Plasmid prediction
+        * Species identification
         * Pan Genome
         
         ### Installation
         
+        **New installation instructions comming soon**
+        
         Bohra requires >=python3.7
         
         #### Conda (Highly recomended)
         
         Installing bohra with conda will ensure that all dependencies are present. See below for instructions on how to configure the databases for kraken2.
         
         Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
@@ -85,26 +106,27 @@
         conda activate <bohra_env_name>
         ```
         #### PyPi
         If installing with `pip` you will need to ensure other dependencies are also installed.
         ```
         pip3 install bohra
         ```
-        * [snakemake](https://snakemake.readthedocs.io/en/stable/getting_started/installation.html)
-        * [Snippy](https://github.com/tseemann/snippy)
+        * [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
         * [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
-        * [Roary](https://sanger-pathogens.github.io/Roary/)
+        * [Panaroo](https://github.com/gtonkinhill/panaroo)
         * [Prokka](https://github.com/tseemann/prokka)
         * [kraken2](https://ccb.jhu.edu/software/kraken/)
         * [abritamr](https://github.com/MDU-PHL/abritamr)
         * [mlst](https://github.com/tseemann/mlst)
         * [iqtree](http://www.iqtree.org/)
         * [seqtk](https://github.com/lh3/seqtk)
         * [snp-dists](https://github.com/tseemann/snp-dists)
         * [mash](https://github.com/lskatz/mashtree)
+        * [mob_suite](https://github.com/phac-nml/mob-suite)
+        * [csvtk](https://github.com/shenwei356/csvtk)
         
         
         #### Check installation
         
         Check that all dependencies are installed.
         
         ```
@@ -123,220 +145,161 @@
         Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
         ```
         export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
         ```
         
         ### Running bohra
         
+        **A word on resources**
+        
+        * A minimum of 8 cpus is required for running `bohra`
+        * `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
+        * Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
+        * If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
+        
         #### Using CLI
         
         ```
-        bohra run -h
-        usage: bohra run [-h] [--input_file INPUT_FILE] [-S]
-                         [--abritamr_singularity ABRITAMR_SINGULARITY]
-                         [--job_id JOB_ID] [--reference REFERENCE] [--mask MASK]
-                         [--kraken_db KRAKEN_DB] [--pipeline {preview,sa,all}]
-                         [--assembler {shovill,skesa,spades}] [--cpus CPUS]
-                         [--minaln MINALN] [--mincov MINCOV]
-                         [--prefillpath PREFILLPATH] [-mdu] [-workdir WORKDIR]
-                         [-resources RESOURCES] [-force] [-dry-run] [--cluster]
-                         [--json JSON] [--queue QUEUE] [--gubbins] [--keep {Y,N}]
+        $ bohra run -h
         
-        optional arguments:
-          -h, --help            show this help message and exit
+        Bohra - a bacterial genomics pipeline - version 2.0.0
+        
+         -h, --help            show this help message and exit
+          -v, --version         show program's version number and exit
+          --check               Check that dependencies are installed correctly.
+                                (default: False)
           --input_file INPUT_FILE, -i INPUT_FILE
-                                Input file = tab-delimited with 3 columns
-                                <isolatename> <path_to_read1> <path_to_read2>
-                                (default: )
-          -S, --use_singularity
-                                Set if you would like to use singularity containers to
-                                run bohra. (default: False)
-          --abritamr_singularity ABRITAMR_SINGULARITY
-                                The path to containers. If you want to use locally
-                                stored contianers please pull from
-                                dockerhub://mduphl/<toolname>. (default:
-                                docker://mduphl/abritamr:v0.2.2)
+                                Path to reads file, which is a tab-delimited with 3
+                                columns <isolatename> <path_to_read1> <path_to_read2>.
+                                REQUIRED (default: )
+          --contigs CONTIGS, -c CONTIGS
+                                Path to contigs file, which is a tab-delimited with 3
+                                columns <isolatename> <path_to_contigs>. OPTIONAL if
+                                you already have assemblies. (default: )
           --job_id JOB_ID, -j JOB_ID
                                 Job ID, will be the name of the output directory
                                 (default: )
           --reference REFERENCE, -r REFERENCE
                                 Path to reference (.gbk or .fa) (default: )
-          --mask MASK, -m MASK  Path to mask file if used (.bed) (default: False)
+          --mask MASK, -m MASK  Path to mask file if used (.bed) (default: )
+          --abritamr_args {Acinetobacter_baumannii,Campylobacter,Enterococcus_faecalis,Enterococcus_faecium,Escherichia,Klebsiella,Salmonella,Staphylococcus_aureus,Staphylococcus_pseudintermedius,Streptococcus_agalactiae,Streptococcus_pneumoniae,Streptococcus_pyogenes,Vibrio_cholerae}
+                                Set if you would like to use point mutations, please
+                                provide a valid species. (default: )
           --kraken_db KRAKEN_DB, -k KRAKEN_DB
                                 Path to DB for use with kraken2, if no DB present
-                                speciation will not be performed. [env var:
-                                KRAKEN2_DEFAULT_DB] (default: None)
-          --pipeline {preview,sa,all}, -p {preview,sa,all}
-                                The pipeline to run. Preview (--preview - default)
-                                will calculate mash-distances and a mash-tree for
-                                quick inspection of your dataset. SNPs and ASSEMBLIES
-                                ('sa') will perform SNPs and ASSEMBLIES. ALL ('all')
-                                will perform SNPS, ASSEMBLIES and ROARY for pan-genome
-                                analysis (default: preview)
+                                speciation will not be performed. (default:
+                                KRAKEN2_DEFAULT_DB)
+          --pipeline {preview,default,all}, -p {preview,default,all}
+                                The pipeline to run. `preview` - generates a rapid
+                                tree using mash distances | `default` - runs snippy,
+                                phylogenetic tree (if > 3 sequences), assemblies, mlst
+                                and amr gene detection | `all` - same as default but
+                                includes roary pangenome analysis (default: preview)
           --assembler {shovill,skesa,spades}, -a {shovill,skesa,spades}
-                                Assembler to use. (default: shovill)
-          --cpus CPUS, -c CPUS  Number of CPU cores to run, will define how many rules
-                                are run at a time (default: 16)
+                                Assembler to use. (default: spades)
+          --cpus CPUS           Number of max CPU cores to run, will define how many
+                                rules are run at a time (default: 72)
           --minaln MINALN, -ma MINALN
                                 Minimum percent alignment. Isolates which do not align
                                 to reference at this threshold will not be included in
-                                core phylogeny. (default: 80)
+                                core phylogeny. (default: 0)
+          --minqual MINQUAL, -mq MINQUAL
+                                Minimum Avg quality of reads (default: 0)
           --mincov MINCOV, -mc MINCOV
                                 Minimum percent alignment. Isolates which do not have
                                 average read coverage above this threshold will not be
-                                included further analysis. (default: 40)
-          --prefillpath PREFILLPATH, -pf PREFILLPATH
-                                Path to existing assemblies - in the form
-                                path_to_somewhere/isolatename/contigs.fa (default:
-                                None)
-          -mdu                  If running on MDU data (default: False)
-          -workdir WORKDIR, -w WORKDIR
+                                included further analysis. (default: 0)
+          --workdir WORKDIR, -w WORKDIR
                                 The directory where Bohra will be run, default is
                                 current directory (default:
-                                /home/khhor/dev/playground/bohra/20200218_/test_f)
-          -resources RESOURCES, -s RESOURCES
-                                Directory where templates are stored (default:
-                                /home/khhor/dev/bohra/bohra/templates)
-          -force, -f            Add if you would like to force a complete restart of
+                                /home/khhor/sandbox/bohra/weird_bugs)
+          --force, -f           Add if you would like to force a complete restart of
                                 the pipeline. All previous logs will be lost.
                                 (default: False)
-          -dry-run, -n          If you would like to see a dry run of commands to be
-                                executed. (default: False)
-          --cluster             If you are running Bohra on a cluster. (default:
-                                False)
-          --json JSON           Path to cluster.json - required if --cluster is set
+          --no_phylo            Set if you do NOT want to generate a phylogentic tree.
+                                (default: False)
+          --config CONFIG       An additional config file, required if running on a
+                                non-local machine, ie slurm, cloud. For help see
+                                documentation at https://github.com/MDU-PHL/bohra or
+                                https://www.nextflow.io/docs/latest/executor.html
                                 (default: )
-          --queue QUEUE         Type of queue (sbatch or qsub currently supported) -
-                                required if --cluster is set. (default: )
-          --gubbins, -g         Set to use gubbins for recombination correction.
+          --profile PROFILE     The resource profile to use. Defaults to local, if
+                                using an alternative config file, this calue should
+                                represent the name of a profile provided (default:
+                                lcl)
+          --gubbins             Set to use gubbins for recombination correction.
                                 (default: False)
           --keep {Y,N}          If you are rerunning bohra over an exisiting directory
                                 set --keep to 'Y' to archive report files - otherwise
                                 previous reprot files will be removed. (default: N)
         
         ```
         
-        #### Using a config file 
-        Arguments that start with '--' (eg. --input_file) can also be set in a config file. Please put your config file in the working directory and name it 'bohra.conf'
-        Config file syntax allows: key=value, flag=true,
-        stuff=[a,b,c] (for details, see syntax at https://goo.gl/R74nmi). If an arg is
-        specified in more than one place, then commandline values override environment
-        variables which override config file values which override defaults.
-        
-        ### Preview mode
-        
-        Bohra's preview mode (default mode) uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
-        
-        ### Set up
         
         **Input file**
         
         The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
         ```
         Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
         ```
         
+        In addition a file of contigs may also be provided if you have already generated assemblies you wish to use. This is also a tab-delimited file. 
+        
+        ```
+        Isolate-ID    /path/to/asm.fasta
+        ```
         **Reference**
         
         The choice of reference is important for the accuracy of SNP detection and therefore the investigation of genomic relatedness. Appropriate references should be chosen following the guidelines below.
         1. A closed reference from the same ST (where applicable) or a gold-standard reference (as may be used in M. tuberculosis).
         2. A pacbio or nanopore assembly from MDU that is of the same type as the query dataset
         3. A high quality de novo assembly of either an isolate in the dataset or an isolate of the same ST or type.
         
         **Mask**
         
         Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
         
         
-        ### Run
         
-        **Minimal command to run in preview mode**
+        ### Preview mode
+        
+        `bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
+        
+        ```
+        bohra run -i input.tab -r ref.fa -p preview -j job_id
+        ```
         
-        To use alternative modes, use `-p` with one of the following arguments.
+        ### Default
         
-        `sa` phylogeny and assembly associated tools
+        Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
         
-        `all` all functions (`sa` plus pan-genome analysis)
-        
-        
-        `bohra run -r path/to/reference -i path/to/inputfile -j unique_id -m path/to/maskfile (optional)`
-        
-        ### Running Bohra in a HPC environment
-        Bohra can be run in a HPC environment (currently only sbatch and qsub are supported). To do this some knowledge and experience in such environments is assumed. You will need to provide a file called `cluster.json`. This file will contain rule specifc and default settings for running the pipeline. An template is shown below (it is recommended that you use this template, settings have been established using a slurm queueing system), in addition you can see further documentation [here](https://snakemake.readthedocs.io/en/stable/snakefiles/configuration.html#cluster-configuration).
-        
-        *example command*
-        ```
-        bohra run -r <reference> -i <input_tab> -j <jobname> --cluster --json cluster.json --queue sbatch
-        ```
-        
-        ```
-        bohra rerun --cluster --queue sbatch
-        ```
-        
-        *cluster.json*
-        ```
-        {
-            "__default__" :
-            {
-                "account" : "AccountName",
-                "time" : "0-0:5:00",
-                "cpus-per-task": "2",
-                "partition" : "cloud",
-                "mem" : "2G",
-                "ntasks" : "4",
-                "job" : "{rule}"
-            },
-            "snippy" :
-            {
-                
-                "cpus-per-task" : "4",
-                "time" : "0-0:5:00",
-                "mem" : "8G" 
-            },
-            "assemble":
-            {
-                "cpus-per-task" : "4",
-                "time" : "0-0:20:00",
-                "mem" : "32G"
-        
-            },
-            "kraken" :
-            {
-                "cpus-per-task" : "8",
-                "time" : "0-0:20:00",
-                "mem"  : "32G"
-            },
-            "run_iqtree_core" :
-            {
-                "time": "0-0:20:00"
-            },
-            "roary" : 
-            {
-                "cpus-per-task" : "36",
-                "time" : "0-0:25:00",
-                "mem": "8G"
-            },
-            "run_prokka" :
-            {
-                "cpus-per-task" : "8",
-                "time" : "0-0:10:00"
-            },
-            "run_snippy_core" :
-            {
-                "time" : "0-0:15:00"
-            }
-        }
         ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
+        ```
+        
+        
+        ### Plus pangenome
+        
+        In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
+        
+        ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
+        ```
+        
+        ### Profile
+        
+        You can provide a specific profile for running `bohra` on various computing platforms (see https://www.nextflow.io/docs/latest/executor.html for available platforms). You will need to specify a `--profile`, which MUST be the same as the name of the profile in your `--config` file. An example structure is provided in `example.config` 
+        
         
         
         
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `bohra-1.2.9/README.md` & `bohra-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,86 @@
 [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 
-![Image](https://github.com/kristyhoran/bohra/blob/master/bohra.png)
 
-# Bohra 
 
-Bohra has a new look! 
-* A new preview mode for 'sneak peak' at your dataset. 
-* `rerun` has been deprecated. If you would like to rerun a job etc; use the run command.
-* If rerunning a job, a new --keep flag to archive previous report files.
-* Built in filtering features to automatically remove isolates with low average coverage or alignment to your reference.
-* Provide a standardised config file for commonly used settings.
+# Bohra
 
-Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. The pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+
+## Bohra has a new look! Welcome to Bohra-NF
+
+**New features**
+
+* Pipeline written in [Nextflow](https://www.nextflow.io)
+* Default mode
+    * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
+    * MobSuite integration.
+    * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
+* Panaroo with visualisation of pan-genome.
+* Improved support for different computing environments.
+
+**Comming soon**
+
+* Improved report structure
+* Option to add your own modules
+
+
+**Accreditation**
+
+* _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
+* _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
 
 ### Motivation
 
-Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Snakemake](https://snakemake.readthedocs.io/en/stable/). 
+Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Nextflow](https://www.nextflow.io).
 
 ### Etymology
 
-Bohra the name of an exinct species of tree kangaroo that lived on the nullarbor. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on *snippy* (named for a very famous kangaroo) and was inspired by *nullarbor*. 
+Bohra the name of an exinct species of tree kangaroo that lived on the Nullarbor plain in Australia. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on [*snippy*](https://github.com/tseemann/snippy) (named for a very famous kangaroo) and was inspired by [*nullarbor*](https://github.com/tseemann/nullarbor). 
 
 
 ## Pipeline
 
-Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports.
+Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports. An addtional file can be porvided with the paths to any assemblies that have already been generated. This is a helpful saver of time.
+
 ![Image](https://github.com/MDU-PHL/bohra/blob/master/workflow.png)
 
-Bohra can be run in four modes
-1. Preview (DEFAULT)
+Bohra can be run in three modes
+1. Preview
 * Calculate mash-distances
 * Build a mash-tree
+* Report sequencing statistics
+* Species identification (providing you have kraken2 database setup properly ;) )
 
-2. SNPs, species ID and Assembly based tools (MLST, Resistome and annotation)
-* Clean reads
+2. Default SNPs, species ID, assemly, MLST, Resistome and annotation)
 * Call variants
 * Generate a phylogenetic tree
-* Assemble
-* Species identification
+* Assemble 
 * MLST
 * Resistome
 * Annotate
+* Plasmid prediction
+* Species identification
 
-4. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
-* Clean reads
+3. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
 * Call variants
 * Generate a phylogenetic tree
-* Assemble
-* Species identification
+* Assemble 
 * MLST
 * Resistome
 * Annotate
+* Plasmid prediction
+* Species identification
 * Pan Genome
 
 ### Installation
 
+**New installation instructions comming soon**
+
 Bohra requires >=python3.7
 
 #### Conda (Highly recomended)
 
 Installing bohra with conda will ensure that all dependencies are present. See below for instructions on how to configure the databases for kraken2.
 
 Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
@@ -77,26 +98,27 @@
 conda activate <bohra_env_name>
 ```
 #### PyPi
 If installing with `pip` you will need to ensure other dependencies are also installed.
 ```
 pip3 install bohra
 ```
-* [snakemake](https://snakemake.readthedocs.io/en/stable/getting_started/installation.html)
-* [Snippy](https://github.com/tseemann/snippy)
+* [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
 * [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
-* [Roary](https://sanger-pathogens.github.io/Roary/)
+* [Panaroo](https://github.com/gtonkinhill/panaroo)
 * [Prokka](https://github.com/tseemann/prokka)
 * [kraken2](https://ccb.jhu.edu/software/kraken/)
 * [abritamr](https://github.com/MDU-PHL/abritamr)
 * [mlst](https://github.com/tseemann/mlst)
 * [iqtree](http://www.iqtree.org/)
 * [seqtk](https://github.com/lh3/seqtk)
 * [snp-dists](https://github.com/tseemann/snp-dists)
 * [mash](https://github.com/lskatz/mashtree)
+* [mob_suite](https://github.com/phac-nml/mob-suite)
+* [csvtk](https://github.com/shenwei356/csvtk)
 
 
 #### Check installation
 
 Check that all dependencies are installed.
 
 ```
@@ -115,209 +137,150 @@
 Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
 ```
 export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
 ```
 
 ### Running bohra
 
+**A word on resources**
+
+* A minimum of 8 cpus is required for running `bohra`
+* `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
+* Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
+* If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
+
 #### Using CLI
 
 ```
-bohra run -h
-usage: bohra run [-h] [--input_file INPUT_FILE] [-S]
-                 [--abritamr_singularity ABRITAMR_SINGULARITY]
-                 [--job_id JOB_ID] [--reference REFERENCE] [--mask MASK]
-                 [--kraken_db KRAKEN_DB] [--pipeline {preview,sa,all}]
-                 [--assembler {shovill,skesa,spades}] [--cpus CPUS]
-                 [--minaln MINALN] [--mincov MINCOV]
-                 [--prefillpath PREFILLPATH] [-mdu] [-workdir WORKDIR]
-                 [-resources RESOURCES] [-force] [-dry-run] [--cluster]
-                 [--json JSON] [--queue QUEUE] [--gubbins] [--keep {Y,N}]
+$ bohra run -h
 
-optional arguments:
-  -h, --help            show this help message and exit
+Bohra - a bacterial genomics pipeline - version 2.0.0
+
+ -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  --check               Check that dependencies are installed correctly.
+                        (default: False)
   --input_file INPUT_FILE, -i INPUT_FILE
-                        Input file = tab-delimited with 3 columns
-                        <isolatename> <path_to_read1> <path_to_read2>
-                        (default: )
-  -S, --use_singularity
-                        Set if you would like to use singularity containers to
-                        run bohra. (default: False)
-  --abritamr_singularity ABRITAMR_SINGULARITY
-                        The path to containers. If you want to use locally
-                        stored contianers please pull from
-                        dockerhub://mduphl/<toolname>. (default:
-                        docker://mduphl/abritamr:v0.2.2)
+                        Path to reads file, which is a tab-delimited with 3
+                        columns <isolatename> <path_to_read1> <path_to_read2>.
+                        REQUIRED (default: )
+  --contigs CONTIGS, -c CONTIGS
+                        Path to contigs file, which is a tab-delimited with 3
+                        columns <isolatename> <path_to_contigs>. OPTIONAL if
+                        you already have assemblies. (default: )
   --job_id JOB_ID, -j JOB_ID
                         Job ID, will be the name of the output directory
                         (default: )
   --reference REFERENCE, -r REFERENCE
                         Path to reference (.gbk or .fa) (default: )
-  --mask MASK, -m MASK  Path to mask file if used (.bed) (default: False)
+  --mask MASK, -m MASK  Path to mask file if used (.bed) (default: )
+  --abritamr_args {Acinetobacter_baumannii,Campylobacter,Enterococcus_faecalis,Enterococcus_faecium,Escherichia,Klebsiella,Salmonella,Staphylococcus_aureus,Staphylococcus_pseudintermedius,Streptococcus_agalactiae,Streptococcus_pneumoniae,Streptococcus_pyogenes,Vibrio_cholerae}
+                        Set if you would like to use point mutations, please
+                        provide a valid species. (default: )
   --kraken_db KRAKEN_DB, -k KRAKEN_DB
                         Path to DB for use with kraken2, if no DB present
-                        speciation will not be performed. [env var:
-                        KRAKEN2_DEFAULT_DB] (default: None)
-  --pipeline {preview,sa,all}, -p {preview,sa,all}
-                        The pipeline to run. Preview (--preview - default)
-                        will calculate mash-distances and a mash-tree for
-                        quick inspection of your dataset. SNPs and ASSEMBLIES
-                        ('sa') will perform SNPs and ASSEMBLIES. ALL ('all')
-                        will perform SNPS, ASSEMBLIES and ROARY for pan-genome
-                        analysis (default: preview)
+                        speciation will not be performed. (default:
+                        KRAKEN2_DEFAULT_DB)
+  --pipeline {preview,default,all}, -p {preview,default,all}
+                        The pipeline to run. `preview` - generates a rapid
+                        tree using mash distances | `default` - runs snippy,
+                        phylogenetic tree (if > 3 sequences), assemblies, mlst
+                        and amr gene detection | `all` - same as default but
+                        includes roary pangenome analysis (default: preview)
   --assembler {shovill,skesa,spades}, -a {shovill,skesa,spades}
-                        Assembler to use. (default: shovill)
-  --cpus CPUS, -c CPUS  Number of CPU cores to run, will define how many rules
-                        are run at a time (default: 16)
+                        Assembler to use. (default: spades)
+  --cpus CPUS           Number of max CPU cores to run, will define how many
+                        rules are run at a time (default: 72)
   --minaln MINALN, -ma MINALN
                         Minimum percent alignment. Isolates which do not align
                         to reference at this threshold will not be included in
-                        core phylogeny. (default: 80)
+                        core phylogeny. (default: 0)
+  --minqual MINQUAL, -mq MINQUAL
+                        Minimum Avg quality of reads (default: 0)
   --mincov MINCOV, -mc MINCOV
                         Minimum percent alignment. Isolates which do not have
                         average read coverage above this threshold will not be
-                        included further analysis. (default: 40)
-  --prefillpath PREFILLPATH, -pf PREFILLPATH
-                        Path to existing assemblies - in the form
-                        path_to_somewhere/isolatename/contigs.fa (default:
-                        None)
-  -mdu                  If running on MDU data (default: False)
-  -workdir WORKDIR, -w WORKDIR
+                        included further analysis. (default: 0)
+  --workdir WORKDIR, -w WORKDIR
                         The directory where Bohra will be run, default is
                         current directory (default:
-                        /home/khhor/dev/playground/bohra/20200218_/test_f)
-  -resources RESOURCES, -s RESOURCES
-                        Directory where templates are stored (default:
-                        /home/khhor/dev/bohra/bohra/templates)
-  -force, -f            Add if you would like to force a complete restart of
+                        /home/khhor/sandbox/bohra/weird_bugs)
+  --force, -f           Add if you would like to force a complete restart of
                         the pipeline. All previous logs will be lost.
                         (default: False)
-  -dry-run, -n          If you would like to see a dry run of commands to be
-                        executed. (default: False)
-  --cluster             If you are running Bohra on a cluster. (default:
-                        False)
-  --json JSON           Path to cluster.json - required if --cluster is set
+  --no_phylo            Set if you do NOT want to generate a phylogentic tree.
+                        (default: False)
+  --config CONFIG       An additional config file, required if running on a
+                        non-local machine, ie slurm, cloud. For help see
+                        documentation at https://github.com/MDU-PHL/bohra or
+                        https://www.nextflow.io/docs/latest/executor.html
                         (default: )
-  --queue QUEUE         Type of queue (sbatch or qsub currently supported) -
-                        required if --cluster is set. (default: )
-  --gubbins, -g         Set to use gubbins for recombination correction.
+  --profile PROFILE     The resource profile to use. Defaults to local, if
+                        using an alternative config file, this calue should
+                        represent the name of a profile provided (default:
+                        lcl)
+  --gubbins             Set to use gubbins for recombination correction.
                         (default: False)
   --keep {Y,N}          If you are rerunning bohra over an exisiting directory
                         set --keep to 'Y' to archive report files - otherwise
                         previous reprot files will be removed. (default: N)
 
 ```
 
-#### Using a config file 
-Arguments that start with '--' (eg. --input_file) can also be set in a config file. Please put your config file in the working directory and name it 'bohra.conf'
-Config file syntax allows: key=value, flag=true,
-stuff=[a,b,c] (for details, see syntax at https://goo.gl/R74nmi). If an arg is
-specified in more than one place, then commandline values override environment
-variables which override config file values which override defaults.
-
-### Preview mode
-
-Bohra's preview mode (default mode) uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
-
-### Set up
 
 **Input file**
 
 The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
 ```
 Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
 ```
 
+In addition a file of contigs may also be provided if you have already generated assemblies you wish to use. This is also a tab-delimited file. 
+
+```
+Isolate-ID    /path/to/asm.fasta
+```
 **Reference**
 
 The choice of reference is important for the accuracy of SNP detection and therefore the investigation of genomic relatedness. Appropriate references should be chosen following the guidelines below.
 1. A closed reference from the same ST (where applicable) or a gold-standard reference (as may be used in M. tuberculosis).
 2. A pacbio or nanopore assembly from MDU that is of the same type as the query dataset
 3. A high quality de novo assembly of either an isolate in the dataset or an isolate of the same ST or type.
 
 **Mask**
 
 Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
 
 
-### Run
 
-**Minimal command to run in preview mode**
+### Preview mode
+
+`bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
+
+```
+bohra run -i input.tab -r ref.fa -p preview -j job_id
+```
 
-To use alternative modes, use `-p` with one of the following arguments.
+### Default
 
-`sa` phylogeny and assembly associated tools
+Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
 
-`all` all functions (`sa` plus pan-genome analysis)
-
-
-`bohra run -r path/to/reference -i path/to/inputfile -j unique_id -m path/to/maskfile (optional)`
-
-### Running Bohra in a HPC environment
-Bohra can be run in a HPC environment (currently only sbatch and qsub are supported). To do this some knowledge and experience in such environments is assumed. You will need to provide a file called `cluster.json`. This file will contain rule specifc and default settings for running the pipeline. An template is shown below (it is recommended that you use this template, settings have been established using a slurm queueing system), in addition you can see further documentation [here](https://snakemake.readthedocs.io/en/stable/snakefiles/configuration.html#cluster-configuration).
-
-*example command*
-```
-bohra run -r <reference> -i <input_tab> -j <jobname> --cluster --json cluster.json --queue sbatch
-```
-
-```
-bohra rerun --cluster --queue sbatch
-```
-
-*cluster.json*
-```
-{
-    "__default__" :
-    {
-        "account" : "AccountName",
-        "time" : "0-0:5:00",
-        "cpus-per-task": "2",
-        "partition" : "cloud",
-        "mem" : "2G",
-        "ntasks" : "4",
-        "job" : "{rule}"
-    },
-    "snippy" :
-    {
-        
-        "cpus-per-task" : "4",
-        "time" : "0-0:5:00",
-        "mem" : "8G" 
-    },
-    "assemble":
-    {
-        "cpus-per-task" : "4",
-        "time" : "0-0:20:00",
-        "mem" : "32G"
-
-    },
-    "kraken" :
-    {
-        "cpus-per-task" : "8",
-        "time" : "0-0:20:00",
-        "mem"  : "32G"
-    },
-    "run_iqtree_core" :
-    {
-        "time": "0-0:20:00"
-    },
-    "roary" : 
-    {
-        "cpus-per-task" : "36",
-        "time" : "0-0:25:00",
-        "mem": "8G"
-    },
-    "run_prokka" :
-    {
-        "cpus-per-task" : "8",
-        "time" : "0-0:10:00"
-    },
-    "run_snippy_core" :
-    {
-        "time" : "0-0:15:00"
-    }
-}
 ```
+bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
+```
+
+
+### Plus pangenome
+
+In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
+
+```
+bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
+```
+
+### Profile
+
+You can provide a specific profile for running `bohra` on various computing platforms (see https://www.nextflow.io/docs/latest/executor.html for available platforms). You will need to specify a `--profile`, which MUST be the same as the name of the profile in your `--config` file. An example structure is provided in `example.config` 
+
```

### Comparing `bohra-1.2.9/bohra/Utils.py` & `bohra-2.2.0/bohra/Utils.py`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/bohra/bohra.py` & `bohra-2.2.0/bohra/bohra.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,132 +9,120 @@
 
 Bohra is modular allowing the user to choose between calling SNPs and generating a phylogenetic tree, perform assemblies and detect AMR, perform typing etc; Or use the full pipeline to call SNPs, generate phylogenies, assemble, type and detect the pan-geneome. The output of Bohra is a html report that can be distributed, with downloadable tables and data.
 """
 
 
 import logging
 import argparse
-import configargparse
 import pathlib
 import sys
 import os
 import shutil
-from bohra.SnpDetection import RunSnpDetection
-from bohra.Utils import Nulla2bohra, UpdateBohra, CheckDeps
+from bohra.SnpDetection import RunSnpDetection, SetupInputFiles
 from bohra.version import version
 
 
-#logging.basicConfig(filename='job.log',level=logging.INFO, format='[%(asctime)s] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p')
-
 def run_pipeline(args):
     '''
     Run the pipeline for the first time
     '''
+    
     R = RunSnpDetection(args)
     return(R.run_pipeline())
 
-def rerun_pipeline(args):
-    '''
-    Rerun the pipeline on a previous dataset, adding, removing isolates or changing reference or mask file
-    '''
-    R = ReRunSnpDetection(args)
-    return(R.run_pipeline())
+def find_reads(args):
 
-def nulla2bohra(args):
-    '''
-    ensure that bohra can be rerun over the top of an existing nullarbor directory
-    '''
-    N = Nulla2bohra(args)
-    return(N.update())
+    S = SetupInputFiles(args)
+    S.find_reads()
+
+def init_bohra():
+    pass
 
-def check_deps(args):
-    """
-    check that dependencies are all installed
-    """
-    C = CheckDeps(args)
-    return(C.check())
-    
 def main():
     # setup the parser
   
-    parser = configargparse.ArgumentParser(description=f'Bohra - a bacterial genomics pipeline - version {version}',formatter_class=configargparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(description=f'Bohra - a bacterial genomics pipeline - version {version}',formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + version)
-    # subparser for running the pipeline
-    subparsers = parser.add_subparsers(help="Task to perform")
-
-    
-
-    parser_sub_run = subparsers.add_parser('run', help='Initial run of Bohra', formatter_class=configargparse.ArgumentDefaultsHelpFormatter,default_config_files=[f"{pathlib.Path.cwd().absolute() / 'bohra.conf'}"])
-    
     # options for running
-    parser_sub_run.add_argument('--input_file','-i',help='Input file = tab-delimited with 3 columns <isolatename>  <path_to_read1> <path_to_read2>', default='')
-    parser_sub_run.add_argument('-S', '--use_singularity', action='store_true', help = 'Set if you would like to use singularity containers to run bohra.')
-    parser_sub_run.add_argument('--snippy_singularity', default='docker://mduphl/snippy', help='The path to containers. If you want to use locally stored contianers please pull from dockerhub://mduphl/<toolname>.')
-    parser_sub_run.add_argument('--abritamr_singularity', default='docker://mduphl/abritamr:v0.2.2', help='The path to containers. If you want to use locally stored contianers please pull from dockerhub://mduphl/<toolname>.')
-    parser_sub_run.add_argument('--job_id','-j',help='Job ID, will be the name of the output directory', default='')
-    parser_sub_run.add_argument('--reference','-r',help='Path to reference (.gbk or .fa)', default = '')
-    parser_sub_run.add_argument('--mask','-m',default = False, help='Path to mask file if used (.bed)')
-    parser_sub_run.add_argument('--kraken_db', '-k', env_var="KRAKEN2_DEFAULT_DB", help="Path to DB for use with kraken2, if no DB present speciation will not be performed.")
-    parser_sub_run.add_argument('--pipeline','-p', default = 'preview', choices=['preview','sa','all'], help=f"The pipeline to run. Preview (--preview - default) will calculate mash-distances and a mash-tree for quick inspection of your dataset. SNPs and ASSEMBLIES ('sa') will perform SNPs and ASSEMBLIES. ALL ('all') will perform SNPS, ASSEMBLIES and ROARY for pan-genome analysis")
-    parser_sub_run.add_argument('--assembler','-a', default = 'shovill', choices=['shovill','skesa','spades'], help=f"Assembler to use.")
-    parser_sub_run.add_argument('--cpus','-c',help='Number of CPU cores to run, will define how many rules are run at a time', default=16)
-    parser_sub_run.add_argument('--minaln','-ma',help='Minimum percent alignment. Isolates which do not align to reference at this threshold will not be included in core phylogeny.', default=80)
-    parser_sub_run.add_argument('--mincov','-mc',help='Minimum percent alignment. Isolates which do not have average read coverage above this threshold will not be included further analysis.', default=40)
-    parser_sub_run.add_argument('--prefillpath','-pf',help='Path to existing assemblies - in the form path_to_somewhere/isolatename/contigs.fa')
-    parser_sub_run.add_argument('-mdu', action = "store_true", help='If running on MDU data')
-    parser_sub_run.add_argument('-workdir','-w', default = f"{pathlib.Path.cwd().absolute()}", help='The directory where Bohra will be run, default is current directory')
-    parser_sub_run.add_argument('-resources','-s', default = f"{pathlib.Path(__file__).parent / 'templates'}", help='Directory where templates are stored')
-    parser_sub_run.add_argument('-force','-f', action="store_true", help = "Add if you would like to force a complete restart of the pipeline. All previous logs will be lost.")
-    parser_sub_run.add_argument('-dry-run','-n', action="store_true", help = "If you would like to see a dry run of commands to be executed.")
-    parser_sub_run.add_argument('--cluster', action="store_true", help = "If you are running Bohra on a cluster.")
-    parser_sub_run.add_argument('--json',help='Path to cluster.json - required if --cluster is set', default='')
-    parser_sub_run.add_argument('--queue',help='Type of queue (sbatch or qsub currently supported) - required if --cluster is set.', default='')
-    parser_sub_run.add_argument('--gubbins', '-g', action = 'store_true', help = 'Set to use gubbins for recombination correction.')
-    parser_sub_run.add_argument('--keep', default = 'N', choices= ['Y', 'N'], help = 'If you are rerunning bohra over an exisiting directory set --keep to \'Y\' to archive report files - otherwise previous reprot files will be removed.')
-    
-    # parser for update
-    parser_sub_nulla2bohra = subparsers.add_parser('nulla2bohra', help='Ensure that bohra can be rerun over an existing nullarbor folder. Can also be used to update older bohra directories. Must supply name of nullarbor directory, and your isolates.tab file', formatter_class=configargparse.ArgumentDefaultsHelpFormatter,default_config_files=[f"{pathlib.Path.cwd().absolute() / 'bohra.conf'}"])
 
-    parser_sub_nulla2bohra.add_argument('-workdir','-w', default = f"{pathlib.Path.cwd().absolute()}", help='Working directory, default is current directory')
-    parser_sub_nulla2bohra.add_argument('--job_id','-j',help='Job directory - the --name you used for nullarbor, will be the name of the output directory', default='')
-    parser_sub_nulla2bohra.add_argument('--input_file','-i',help='Input file = tab-delimited with 3 columns <isolatename>  <path_to_read1> <path_to_read2>', default='')
-    parser_sub_nulla2bohra.add_argument('--reference', '-r', help = 'The reference that was used in the previous run/ nullarbor job', default = '')
-    
-    # parser for checks
-    parser_sub_check = subparsers.add_parser('check', help = "Check that all dependencies for bohra have been installed.")
-    parser_sub_check.add_argument('--kraken_db', '-k', env_var="KRAKEN2_DEFAULT_DB", help="Path to DB for use with kraken2, if no DB present speciation will not be performed.")
-    parser_sub_run.set_defaults(func=run_pipeline)
-    parser_sub_nulla2bohra.set_defaults(func=nulla2bohra)
-    parser_sub_check.set_defaults(func = check_deps)
+    subparsers = parser.add_subparsers(help="Task to perform")
+    # run bohra pipeline
+    parser_run = subparsers.add_parser('run', help='Run bohra', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
+    parser_run.add_argument('--check',action="store_true", help = "Check that dependencies are installed correctly.")
+    parser_run.add_argument('--input_file','-i',help='Path to reads file, which is a tab-delimited with 3 columns <isolatename>  <path_to_read1> <path_to_read2>. REQUIRED', default='')
+    parser_run.add_argument('--contigs','-c',help='Path to contigs file, which is a tab-delimited with 3 columns <isolatename>  <path_to_contigs>. OPTIONAL if you already have assemblies.', default='')
+    parser_run.add_argument('--job_id','-j',help='Job ID is the name that will be displayed on your report', default='Bohra microbial genomics pipeline')
+    parser_run.add_argument('--reference','-r',help='Path to reference (.gbk or .fa)', default = '')
+    parser_run.add_argument('--mask','-m',default = '', help='Path to mask file if used (.bed)')
+    parser_run.add_argument("--abritamr_args",default="",help="Set if you would like to use point mutations, please provide a valid species.", choices= ['Neisseria', 'Acinetobacter_baumannii', "Campylobacter", "Enterococcus_faecalis", "Enterococcus_faecium", "Escherichia", "Klebsiella", "Salmonella", "Staphylococcus_aureus", "Staphylococcus_pseudintermedius", "Streptococcus_agalactiae", "Streptococcus_pneumoniae", "Streptococcus_pyogenes", "Vibrio_cholerae"])
+    parser_run.add_argument('--kraken_db', '-k', default="KRAKEN2_DEFAULT_DB", help="Path to DB for use with kraken2, if no DB present speciation will not be performed.")
+    parser_run.add_argument('--pipeline','-p', default = 'preview', choices=['preview','default','pluspan'], help=f"The pipeline to run. `preview` - generates a rapid tree using mash distances | `default` - runs snippy, phylogenetic tree (if > 3 sequences), assemblies, mlst and amr gene detection | `all` - same as default but includes roary pangenome analysis")
+    parser_run.add_argument('--assembler','-a', default = 'shovill', choices=['shovill','skesa','spades'], help=f"Assembler to use.")
+    parser_run.add_argument('--cpus',help='Number of max CPU cores to run, will define how many rules are run at a time, if 0 then the avail cpus will be determined at time of launch', default=0) # need to change
+    parser_run.add_argument('--minmap','-mp',help='Snippy - minimum read mapping quality to consider.', default='60')
+    parser_run.add_argument('--basequal','-bq',help='Snippy - Minimum base quality to consider.', default='13')
+    parser_run.add_argument('--minqual','-mq',help='Snippy - minumum QUALITY in VCF column 6', default='100')
+    parser_run.add_argument('--minfrac','-mf',help='Snippy - minumum proportion for variant evidence ', default='0')
+    parser_run.add_argument('--mincov','-mc',help='Snippy - minimum site depth to for calling alleles.', default='10')
+    parser_run.add_argument('--workdir','-w', default = f"{pathlib.Path.cwd().absolute()}", help='The directory where Bohra will be run, default is current directory') # don't need this
+    parser_run.add_argument('--force','-f', action="store_true", help = "Add if you would like to force a complete restart of the pipeline. All previous logs will be lost.")
+    parser_run.add_argument('--no_phylo',action="store_true", help = "Set if you do NOT want to generate a phylogentic tree.")
+    parser_run.add_argument('--config', default = f"", help='An additional config file, required if running on a non-local machine, ie slurm, cloud. For help see documentation at https://github.com/MDU-PHL/bohra or https://www.nextflow.io/docs/latest/executor.html') # don't need this
+    parser_run.add_argument('--profile', default = f"", help='The resource profile to use. Defaults to local, if using an alternative config file, this calue should represent the name of a profile provided') 
+    parser_run.add_argument('--conda_path', default = f"", help='The path to where your pre-installed conda envs are stored, defaults to installing conda envs in your work directory. This can be provided in your profiles settings as well - it assumes you have pre-configured all of your conda environments for each process run by bohra, this is an advanced setting. Please take care.') 
+    parser_run.add_argument('--blast_db', default = f"{os.getenv('BLAST_DB', '')}", help='Path to the mlst blast_db, defaults to what is installed in the environment.') 
+    parser_run.add_argument('--data_dir', default = f"{os.getenv('PUBMLST_DB','')}", help='Path to the mlst datadir, defaults to what is installed in the environment.') 
+    parser_run.add_argument('--mlst_exclude',default = f"", help='Space delimited list of mlst schemes to exclude.', nargs='+')
+    parser_run.add_argument('--proceed', action="store_true", help = "If you would like to proceed straigt to the pipeline.")
+    parser_run.add_argument('--gubbins',  action = 'store_true', help = 'Set to use gubbins for recombination correction.')
+    parser_run.add_argument('--keep', default = 'N', choices= ['Y', 'N'], help = 'If you are rerunning bohra over an exisiting directory set --keep to \'Y\' to archive report files - otherwise previous reprot files will be removed.')
+    parser_run.add_argument('--no-conda',action="store_true", help="Set if you DO NOT WANT to use separate conda environments for each nextflow process.")
+
+    # parser_check = subparsers.add_parser('check', help='Check bohra installation', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+
+    parser_setup = subparsers.add_parser('generate_input', help='Generate input files for bohra', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser_setup.add_argument(
+        '--read_path',
+        '-r',
+        default='',
+        help = 'Path to look for read files')
+    parser_setup.add_argument(
+        '--isolate_list',
+        '-i',
+        default= '',
+        help = 'List of isolates (one isolate name per line) to include in input file. If not provided all sequences in found will be included.'
+    )
+
+        
+    parser_run.set_defaults(func=run_pipeline)
+    parser_setup.set_defaults(func=find_reads)
 
         
     args = parser.parse_args()
     
-    if len(sys.argv) <= 1:
+    if len(sys.argv) <= 2 and sys.argv[1] != 'check':
         parser.print_help(sys.stderr)
-
-    elif len(sys.argv) == 2 and sys.argv[1] in ['run', 'nulla2bohra']:
-        parser.print_help(sys.stderr)
-    
+    # elif sys.argv[1] == 'check':
+    #     check_deps()
     else:
-        logger = logging.getLogger(__name__)
-        logger.setLevel(logging.INFO)
-        # create file handler which logs even debug messages
-        fh = logging.FileHandler('bohra.log')
-        fh.setLevel(logging.INFO)
-        # create console handler with a higher log level
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.INFO)
-        # create formatter and add it to the handlers
-        formatter = logging.Formatter('[%(levelname)s:%(asctime)s] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p')
-        fh.setFormatter(formatter)
-        ch.setFormatter(formatter)
-        # add the handlers to the logger
-        logger.addHandler(ch)
-        logger.addHandler(fh)
-        logger.info(f"Starting bohra pipeline using {' '.join(sys.argv)}")
+        # logger = logging.getLogger(__name__)
+        # logger.setLevel(logging.INFO)
+        # # create file handler which logs even debug messages
+        # fh = logging.FileHandler('bohra.log')
+        # fh.setLevel(logging.INFO)
+        # # create console handler with a higher log level
+        # ch = logging.StreamHandler()
+        # ch.setLevel(logging.INFO)
+        # # create formatter and add it to the handlers
+        # formatter = logging.Formatter('[%(levelname)s:%(asctime)s] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p')
+        # fh.setFormatter(formatter)
+        # ch.setFormatter(formatter)
+        # # add the handlers to the logger
+        # logger.addHandler(ch)
+        # logger.addHandler(fh)
+        # logger.info(f"Starting bohra pipeline using {' '.join(sys.argv)}")
         args.func(args)
 	
 if __name__ == '__main__':
     main()
```

### Comparing `bohra-1.2.9/bohra/templates/cluster.tmpl` & `bohra-2.2.0/bohra/templates/cluster.tmpl`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/bohra/templates/config_snippy.yaml` & `bohra-2.2.0/bohra/templates/config_snippy.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -24,16 +24,20 @@
         "{{assembler}}"
 template_path:
         "{{template_path}}"
 script_path:
         "{{script_path}}"
 preview:
         {{preview}}
+run_kraken:
+        "{{run_kraken}}"
 kraken_db:
         "{{kraken_db}}"
+kraken_threads:
+        "{{kraken_threads}}"
 min_cov:
         {{min_cov}}
 # snippy_singularity:
 #         "{{snippy_singularity}}"
 abritamr_singularity:
         "{{abritamr_singularity}}"
 snippy_singularity:
```

### Comparing `bohra-1.2.9/bohra/tests/test.gbk` & `bohra-2.2.0/bohra/tests/test.gbk`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/bohra/tests/test.tab` & `bohra-2.2.0/bohra/tests/test.tab`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/bohra/utils/iqtree_generator.sh` & `bohra-2.2.0/bohra/modules/iqtree/bin/iqtree_generator.sh`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 FASTA=$1
 if [ "x$FASTA" == "x" ]; then
   EXE=$(basename $0)
   echo "Usage: $EXE genome.fasta core.aln prefix max_cpus"
   exit 1
 fi
-
+any2fasta $FASTA > ref.fa
 RESULT="-fconst "
 for L in Aa Cc Gg Tt ; do
-  NUM=$(grep -v '>' "$FASTA" | tr -d -c "[$L]" | wc -c)
+  NUM=$(grep -v '>' ref.fa | tr -d -c "[$L]" | wc -c)
   if [ "x$NUM" == "x" ]; then
     echo "Error: could not count '$L' chars in $FASTA"
     exit 2
   fi
   RESULT="$RESULT$NUM,"
 done
 
@@ -40,8 +40,8 @@
 if [ "x$4" == "x" ]; then
     CPUS=$(getconf _NPROCESSORS_ONLN)
 else
     CPUS=$4
 fi
 
 
-echo "iqtree $RESULT -m GTR+G4 -bb 1000 -alrt 1000 -ntmax "$CPUS" -nt AUTO -st DNA -s $CORE -pre $PRE"
+iqtree $RESULT -m GTR+G4 -bb 1000 -alrt 1000 -ntmax $CPUS -nt AUTO -st DNA -s $CORE -pre $PRE
```

### Comparing `bohra-1.2.9/bohra/utils/roary2svg.pl` & `bohra-2.2.0/bohra/modules/roary2svg/bin/roary2svg.pl`

 * *Files identical despite different names*

### Comparing `bohra-1.2.9/bohra.egg-info/PKG-INFO` & `bohra-2.2.0/bohra.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 Metadata-Version: 2.1
 Name: bohra
-Version: 1.2.9
+Version: 2.2.0
 Summary: A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
 Home-page: https://github.com/kristyhoran/bohra
 Author: Kristy Horan
 Author-email: kristyhoran15@gmail.com
 License: UNKNOWN
 Description: [![CircleCI](https://circleci.com/gh/MDU-PHL/bohra.svg?style=svg&circle-token=530799cb0764519fc65966ab48bac7e0d02f3688)](https://circleci.com/gh/MDU-PHL/bohra)
         [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
         
-        ![Image](https://github.com/kristyhoran/bohra/blob/master/bohra.png)
         
-        # Bohra 
         
-        Bohra has a new look! 
-        * A new preview mode for 'sneak peak' at your dataset. 
-        * `rerun` has been deprecated. If you would like to rerun a job etc; use the run command.
-        * If rerunning a job, a new --keep flag to archive previous report files.
-        * Built in filtering features to automatically remove isolates with low average coverage or alignment to your reference.
-        * Provide a standardised config file for commonly used settings.
+        # Bohra
         
-        Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. The pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+        Bohra is microbial genomics pipeline, designed predominantly for use in public health, but may also be useful in research settings. At a minimum the pipeline takes as input a tab-delimited file with the isolate IDs followed by the path to READ1 and READ2, a reference for alignment and a unique identifier, where reads are illumina reads (other platforms are not supported at this stage).
+        
+        ## Bohra has a new look! Welcome to Bohra-NF
+        
+        **New features**
+        
+        * Pipeline written in [Nextflow](https://www.nextflow.io)
+        * Default mode
+            * Can be run on a single isolate (phylogenetic tree will not be generated if fewer than three sequences included in dataset)
+            * MobSuite integration.
+            * Updated [abriTAMR](https://github.com/MDU-PHL/abritamr) with support for point mutations and virulence factors (beta).
+        * Panaroo with visualisation of pan-genome.
+        * Improved support for different computing environments.
+        
+        **Comming soon**
+        
+        * Improved report structure
+        * Option to add your own modules
+        
+        
+        **Accreditation**
+        
+        * _snippy and snippy-core version 4.4.5 are NATA accredited for accurate detection of SNPs for reporting of genomic relationships at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
+        * _abritamr is accredited for detection of AMR genes at [MDU](https://biomedicalsciences.unimelb.edu.au/departments/microbiology-Immunology/research/services/microbiological-diagnostic-unit-public-health-laboratory#about-mdu-phl) Victoria Australia_ 
         
         ### Motivation
         
-        Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Snakemake](https://snakemake.readthedocs.io/en/stable/). 
+        Bohra was inspired by Nullarbor (https://github.com/tseemann/nullarbor) to be used in public health microbiology labs for analysis of short reads from microbiological samples. The pipeline is written in [Nextflow](https://www.nextflow.io).
         
         ### Etymology
         
-        Bohra the name of an exinct species of tree kangaroo that lived on the nullarbor. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on *snippy* (named for a very famous kangaroo) and was inspired by *nullarbor*. 
+        Bohra the name of an exinct species of tree kangaroo that lived on the Nullarbor plain in Australia. The name was chosen to reflect the fact that it will be predominantly used to build *trees*, relies on [*snippy*](https://github.com/tseemann/snippy) (named for a very famous kangaroo) and was inspired by [*nullarbor*](https://github.com/tseemann/nullarbor). 
         
         
         ## Pipeline
         
-        Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports.
+        Bohra takes raw sequencing reads and produces a standalone html file for simple distribution of reports. An addtional file can be porvided with the paths to any assemblies that have already been generated. This is a helpful saver of time.
+        
         ![Image](https://github.com/MDU-PHL/bohra/blob/master/workflow.png)
         
-        Bohra can be run in four modes
-        1. Preview (DEFAULT)
+        Bohra can be run in three modes
+        1. Preview
         * Calculate mash-distances
         * Build a mash-tree
+        * Report sequencing statistics
+        * Species identification (providing you have kraken2 database setup properly ;) )
         
-        2. SNPs, species ID and Assembly based tools (MLST, Resistome and annotation)
-        * Clean reads
+        2. Default SNPs, species ID, assemly, MLST, Resistome and annotation)
         * Call variants
         * Generate a phylogenetic tree
-        * Assemble
-        * Species identification
+        * Assemble 
         * MLST
         * Resistome
         * Annotate
+        * Plasmid prediction
+        * Species identification
         
-        4. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
-        * Clean reads
+        3. SNPs, Phylogeny, PanGenome and  Typing and Species Identification
         * Call variants
         * Generate a phylogenetic tree
-        * Assemble
-        * Species identification
+        * Assemble 
         * MLST
         * Resistome
         * Annotate
+        * Plasmid prediction
+        * Species identification
         * Pan Genome
         
         ### Installation
         
+        **New installation instructions comming soon**
+        
         Bohra requires >=python3.7
         
         #### Conda (Highly recomended)
         
         Installing bohra with conda will ensure that all dependencies are present. See below for instructions on how to configure the databases for kraken2.
         
         Set up conda - documentation for conda installation can be found [here](https://conda.io/en/latest/miniconda.html)
@@ -85,26 +106,27 @@
         conda activate <bohra_env_name>
         ```
         #### PyPi
         If installing with `pip` you will need to ensure other dependencies are also installed.
         ```
         pip3 install bohra
         ```
-        * [snakemake](https://snakemake.readthedocs.io/en/stable/getting_started/installation.html)
-        * [Snippy](https://github.com/tseemann/snippy)
+        * [Snippy (v4.4.5 recommended)](https://github.com/tseemann/snippy)
         * [Shovill (skesa and spades.py)](https://github.com/tseemann/shovill)
-        * [Roary](https://sanger-pathogens.github.io/Roary/)
+        * [Panaroo](https://github.com/gtonkinhill/panaroo)
         * [Prokka](https://github.com/tseemann/prokka)
         * [kraken2](https://ccb.jhu.edu/software/kraken/)
         * [abritamr](https://github.com/MDU-PHL/abritamr)
         * [mlst](https://github.com/tseemann/mlst)
         * [iqtree](http://www.iqtree.org/)
         * [seqtk](https://github.com/lh3/seqtk)
         * [snp-dists](https://github.com/tseemann/snp-dists)
         * [mash](https://github.com/lskatz/mashtree)
+        * [mob_suite](https://github.com/phac-nml/mob-suite)
+        * [csvtk](https://github.com/shenwei356/csvtk)
         
         
         #### Check installation
         
         Check that all dependencies are installed.
         
         ```
@@ -123,220 +145,161 @@
         Once you have the DB downloaded you will have to create an environment variable called `KRAKEN2_DEFAULT_DB`. This can be done by adding the following to your `$HOME/.bashrc`
         ```
         export KRAKEN_DEFAULT_DB=$HOME/minikraken2_v2_8GB_201904_UPDATE
         ```
         
         ### Running bohra
         
+        **A word on resources**
+        
+        * A minimum of 8 cpus is required for running `bohra`
+        * `bohra` has default settings for running at MDU (both on research and service systems). These ensure optimal running on these systems.
+        * Whether you are running `bohra` on MDU systems or not, you can override the default max cpus, by providing an upper limit for your job using the `--cpus` flag.
+        * If you are running on a queue or in the cloud you will need to provide an additional config file with details of your profile requirements.
+        
         #### Using CLI
         
         ```
-        bohra run -h
-        usage: bohra run [-h] [--input_file INPUT_FILE] [-S]
-                         [--abritamr_singularity ABRITAMR_SINGULARITY]
-                         [--job_id JOB_ID] [--reference REFERENCE] [--mask MASK]
-                         [--kraken_db KRAKEN_DB] [--pipeline {preview,sa,all}]
-                         [--assembler {shovill,skesa,spades}] [--cpus CPUS]
-                         [--minaln MINALN] [--mincov MINCOV]
-                         [--prefillpath PREFILLPATH] [-mdu] [-workdir WORKDIR]
-                         [-resources RESOURCES] [-force] [-dry-run] [--cluster]
-                         [--json JSON] [--queue QUEUE] [--gubbins] [--keep {Y,N}]
+        $ bohra run -h
         
-        optional arguments:
-          -h, --help            show this help message and exit
+        Bohra - a bacterial genomics pipeline - version 2.0.0
+        
+         -h, --help            show this help message and exit
+          -v, --version         show program's version number and exit
+          --check               Check that dependencies are installed correctly.
+                                (default: False)
           --input_file INPUT_FILE, -i INPUT_FILE
-                                Input file = tab-delimited with 3 columns
-                                <isolatename> <path_to_read1> <path_to_read2>
-                                (default: )
-          -S, --use_singularity
-                                Set if you would like to use singularity containers to
-                                run bohra. (default: False)
-          --abritamr_singularity ABRITAMR_SINGULARITY
-                                The path to containers. If you want to use locally
-                                stored contianers please pull from
-                                dockerhub://mduphl/<toolname>. (default:
-                                docker://mduphl/abritamr:v0.2.2)
+                                Path to reads file, which is a tab-delimited with 3
+                                columns <isolatename> <path_to_read1> <path_to_read2>.
+                                REQUIRED (default: )
+          --contigs CONTIGS, -c CONTIGS
+                                Path to contigs file, which is a tab-delimited with 3
+                                columns <isolatename> <path_to_contigs>. OPTIONAL if
+                                you already have assemblies. (default: )
           --job_id JOB_ID, -j JOB_ID
                                 Job ID, will be the name of the output directory
                                 (default: )
           --reference REFERENCE, -r REFERENCE
                                 Path to reference (.gbk or .fa) (default: )
-          --mask MASK, -m MASK  Path to mask file if used (.bed) (default: False)
+          --mask MASK, -m MASK  Path to mask file if used (.bed) (default: )
+          --abritamr_args {Acinetobacter_baumannii,Campylobacter,Enterococcus_faecalis,Enterococcus_faecium,Escherichia,Klebsiella,Salmonella,Staphylococcus_aureus,Staphylococcus_pseudintermedius,Streptococcus_agalactiae,Streptococcus_pneumoniae,Streptococcus_pyogenes,Vibrio_cholerae}
+                                Set if you would like to use point mutations, please
+                                provide a valid species. (default: )
           --kraken_db KRAKEN_DB, -k KRAKEN_DB
                                 Path to DB for use with kraken2, if no DB present
-                                speciation will not be performed. [env var:
-                                KRAKEN2_DEFAULT_DB] (default: None)
-          --pipeline {preview,sa,all}, -p {preview,sa,all}
-                                The pipeline to run. Preview (--preview - default)
-                                will calculate mash-distances and a mash-tree for
-                                quick inspection of your dataset. SNPs and ASSEMBLIES
-                                ('sa') will perform SNPs and ASSEMBLIES. ALL ('all')
-                                will perform SNPS, ASSEMBLIES and ROARY for pan-genome
-                                analysis (default: preview)
+                                speciation will not be performed. (default:
+                                KRAKEN2_DEFAULT_DB)
+          --pipeline {preview,default,all}, -p {preview,default,all}
+                                The pipeline to run. `preview` - generates a rapid
+                                tree using mash distances | `default` - runs snippy,
+                                phylogenetic tree (if > 3 sequences), assemblies, mlst
+                                and amr gene detection | `all` - same as default but
+                                includes roary pangenome analysis (default: preview)
           --assembler {shovill,skesa,spades}, -a {shovill,skesa,spades}
-                                Assembler to use. (default: shovill)
-          --cpus CPUS, -c CPUS  Number of CPU cores to run, will define how many rules
-                                are run at a time (default: 16)
+                                Assembler to use. (default: spades)
+          --cpus CPUS           Number of max CPU cores to run, will define how many
+                                rules are run at a time (default: 72)
           --minaln MINALN, -ma MINALN
                                 Minimum percent alignment. Isolates which do not align
                                 to reference at this threshold will not be included in
-                                core phylogeny. (default: 80)
+                                core phylogeny. (default: 0)
+          --minqual MINQUAL, -mq MINQUAL
+                                Minimum Avg quality of reads (default: 0)
           --mincov MINCOV, -mc MINCOV
                                 Minimum percent alignment. Isolates which do not have
                                 average read coverage above this threshold will not be
-                                included further analysis. (default: 40)
-          --prefillpath PREFILLPATH, -pf PREFILLPATH
-                                Path to existing assemblies - in the form
-                                path_to_somewhere/isolatename/contigs.fa (default:
-                                None)
-          -mdu                  If running on MDU data (default: False)
-          -workdir WORKDIR, -w WORKDIR
+                                included further analysis. (default: 0)
+          --workdir WORKDIR, -w WORKDIR
                                 The directory where Bohra will be run, default is
                                 current directory (default:
-                                /home/khhor/dev/playground/bohra/20200218_/test_f)
-          -resources RESOURCES, -s RESOURCES
-                                Directory where templates are stored (default:
-                                /home/khhor/dev/bohra/bohra/templates)
-          -force, -f            Add if you would like to force a complete restart of
+                                /home/khhor/sandbox/bohra/weird_bugs)
+          --force, -f           Add if you would like to force a complete restart of
                                 the pipeline. All previous logs will be lost.
                                 (default: False)
-          -dry-run, -n          If you would like to see a dry run of commands to be
-                                executed. (default: False)
-          --cluster             If you are running Bohra on a cluster. (default:
-                                False)
-          --json JSON           Path to cluster.json - required if --cluster is set
+          --no_phylo            Set if you do NOT want to generate a phylogentic tree.
+                                (default: False)
+          --config CONFIG       An additional config file, required if running on a
+                                non-local machine, ie slurm, cloud. For help see
+                                documentation at https://github.com/MDU-PHL/bohra or
+                                https://www.nextflow.io/docs/latest/executor.html
                                 (default: )
-          --queue QUEUE         Type of queue (sbatch or qsub currently supported) -
-                                required if --cluster is set. (default: )
-          --gubbins, -g         Set to use gubbins for recombination correction.
+          --profile PROFILE     The resource profile to use. Defaults to local, if
+                                using an alternative config file, this calue should
+                                represent the name of a profile provided (default:
+                                lcl)
+          --gubbins             Set to use gubbins for recombination correction.
                                 (default: False)
           --keep {Y,N}          If you are rerunning bohra over an exisiting directory
                                 set --keep to 'Y' to archive report files - otherwise
                                 previous reprot files will be removed. (default: N)
         
         ```
         
-        #### Using a config file 
-        Arguments that start with '--' (eg. --input_file) can also be set in a config file. Please put your config file in the working directory and name it 'bohra.conf'
-        Config file syntax allows: key=value, flag=true,
-        stuff=[a,b,c] (for details, see syntax at https://goo.gl/R74nmi). If an arg is
-        specified in more than one place, then commandline values override environment
-        variables which override config file values which override defaults.
-        
-        ### Preview mode
-        
-        Bohra's preview mode (default mode) uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
-        
-        ### Set up
         
         **Input file**
         
         The input file needs to be a tab-delimited file with three columns IsolateID, path to R1 and path to R2. 
         ```
         Isolate-ID    /path/to/reads/R1.fq.gz    /path/to/reads/R2.fq.gz
         ```
         
+        In addition a file of contigs may also be provided if you have already generated assemblies you wish to use. This is also a tab-delimited file. 
+        
+        ```
+        Isolate-ID    /path/to/asm.fasta
+        ```
         **Reference**
         
         The choice of reference is important for the accuracy of SNP detection and therefore the investigation of genomic relatedness. Appropriate references should be chosen following the guidelines below.
         1. A closed reference from the same ST (where applicable) or a gold-standard reference (as may be used in M. tuberculosis).
         2. A pacbio or nanopore assembly from MDU that is of the same type as the query dataset
         3. A high quality de novo assembly of either an isolate in the dataset or an isolate of the same ST or type.
         
         **Mask**
         
         Phage masking is important for to prevent the inflation of SNPs that can be introduced by horizontal transfer as opposed to vertical transfer. For closed genomes or those that are publicly available `phaster-query.pl` can be used to identify regions for masking. If a denovo assembly is used the website `phaster.ca` can be used. Regions for masking should be provided in `.bed` format.
         
         
-        ### Run
         
-        **Minimal command to run in preview mode**
+        ### Preview mode
+        
+        `bohra` preview mode uses `mash` to calculate mash distances between isolates and generate a mash tree to rapidly identify outliers in your dataset or identify clades of interest for a more focused analysis.
+        
+        ```
+        bohra run -i input.tab -r ref.fa -p preview -j job_id
+        ```
         
-        To use alternative modes, use `-p` with one of the following arguments.
+        ### Default
         
-        `sa` phylogeny and assembly associated tools
+        Default mode will perform SNP detection, assemblies (if contigs file not provided), mlst, abritamr and phylogeny (unless `--no_phylo` or < 4 samples used as input).
         
-        `all` all functions (`sa` plus pan-genome analysis)
-        
-        
-        `bohra run -r path/to/reference -i path/to/inputfile -j unique_id -m path/to/maskfile (optional)`
-        
-        ### Running Bohra in a HPC environment
-        Bohra can be run in a HPC environment (currently only sbatch and qsub are supported). To do this some knowledge and experience in such environments is assumed. You will need to provide a file called `cluster.json`. This file will contain rule specifc and default settings for running the pipeline. An template is shown below (it is recommended that you use this template, settings have been established using a slurm queueing system), in addition you can see further documentation [here](https://snakemake.readthedocs.io/en/stable/snakefiles/configuration.html#cluster-configuration).
-        
-        *example command*
-        ```
-        bohra run -r <reference> -i <input_tab> -j <jobname> --cluster --json cluster.json --queue sbatch
-        ```
-        
-        ```
-        bohra rerun --cluster --queue sbatch
-        ```
-        
-        *cluster.json*
-        ```
-        {
-            "__default__" :
-            {
-                "account" : "AccountName",
-                "time" : "0-0:5:00",
-                "cpus-per-task": "2",
-                "partition" : "cloud",
-                "mem" : "2G",
-                "ntasks" : "4",
-                "job" : "{rule}"
-            },
-            "snippy" :
-            {
-                
-                "cpus-per-task" : "4",
-                "time" : "0-0:5:00",
-                "mem" : "8G" 
-            },
-            "assemble":
-            {
-                "cpus-per-task" : "4",
-                "time" : "0-0:20:00",
-                "mem" : "32G"
-        
-            },
-            "kraken" :
-            {
-                "cpus-per-task" : "8",
-                "time" : "0-0:20:00",
-                "mem"  : "32G"
-            },
-            "run_iqtree_core" :
-            {
-                "time": "0-0:20:00"
-            },
-            "roary" : 
-            {
-                "cpus-per-task" : "36",
-                "time" : "0-0:25:00",
-                "mem": "8G"
-            },
-            "run_prokka" :
-            {
-                "cpus-per-task" : "8",
-                "time" : "0-0:10:00"
-            },
-            "run_snippy_core" :
-            {
-                "time" : "0-0:15:00"
-            }
-        }
         ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p default -j job_id
+        ```
+        
+        
+        ### Plus pangenome
+        
+        In addition to the default mode above, `all` will also run `panaroo` . If less than 4 samples are provided, `panaroo` will not be run and pipeline will revert to `default`
+        
+        ```
+        bohra run -i input.tab -c contigs.tab -r ref.fa -p pluspan -j job_id
+        ```
+        
+        ### Profile
+        
+        You can provide a specific profile for running `bohra` on various computing platforms (see https://www.nextflow.io/docs/latest/executor.html for available platforms). You will need to specify a `--profile`, which MUST be the same as the name of the profile in your `--config` file. An example structure is provided in `example.config` 
+        
         
         
         
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `bohra-1.2.9/setup.cfg` & `bohra-2.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [metadata]
 name = bohra
 author = Kristy Horan
 author_email = kristyhoran15@gmail.com
 description = A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
-version = 1.2.9
+version = 2.2.0
 url = https://github.com/kristyhoran/bohra
 classifiers = 
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.9
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = 
 	LICENSE.txt
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.9
 packages = find:
 zip_safe = False
 install_requires = 
 	pytest
+	altair
 	jinja2
 	biopython>=1.70
-	pandas>=0.25.0
-	numpy
+	pandas>=0.25.0,<=1.0.5
+	numpy==1.23.1
 	psutil
 	sh
 	packaging
-	snakemake>=5.9.1
-	configargparse
 include_package_data = True
 
 [options.extras_require]
 tests = 
 	pytest
 	flake8
```


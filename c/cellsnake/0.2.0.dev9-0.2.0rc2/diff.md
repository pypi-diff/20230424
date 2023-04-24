# Comparing `tmp/cellsnake-0.2.0.dev9.tar.gz` & `tmp/cellsnake-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellsnake-0.2.0.dev9.tar", last modified: Mon Apr 10 13:54:49 2023, max compression
+gzip compressed data, was "cellsnake-0.2.0rc2.tar", last modified: Sun Apr 23 23:04:33 2023, max compression
```

## Comparing `cellsnake-0.2.0.dev9.tar` & `cellsnake-0.2.0rc2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.687710 cellsnake-0.2.0.dev9/
--rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0.dev9/LICENSE
--rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0.dev9/MANIFEST.in
--rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-10 13:54:49.687497 cellsnake-0.2.0.dev9/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     4458 2023-04-04 13:27:36.000000 cellsnake-0.2.0.dev9/README.md
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.677093 cellsnake-0.2.0.dev9/cellsnake/
--rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0.dev9/cellsnake/__init__.py
--rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0.dev9/cellsnake/cellsnake_functions.py
--rwxr-xr-x   0 sium       (501) staff       (20)    13703 2023-04-10 13:53:11.000000 cellsnake-0.2.0.dev9/cellsnake/command_line.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678251 cellsnake-0.2.0.dev9/cellsnake/scrna/
--rw-r--r--   0 sium       (501) staff       (20)     2362 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/config.yaml
--rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/install_r_packages.sh
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678373 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/
--rw-r--r--   0 sium       (501) staff       (20)    23558 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/Snakefile
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.678527 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/
--rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.674775 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.680910 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.681055 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
--rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
--rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.682176 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/
--rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/extra_functions.smk
--rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/integration.smk
--rw-r--r--   0 sium       (501) staff       (20)     5712 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/microbiome.smk
--rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_detect.smk
--rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_write.smk
--rw-r--r--   0 sium       (501) staff       (20)    20702 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/seurat.smk
--rw-r--r--   0 sium       (501) staff       (20)      306 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/subset.smk
--rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/test.smk
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.687263 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/
--rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
--rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3319 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
--rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1241 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3449 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1714 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3563 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
--rwxr-xr-x   0 sium       (501) staff       (20)     7044 2023-04-10 13:12:21.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-functions.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3205 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-gsea.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-harmony.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4595 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kegg.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
--rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-metrics.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2835 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
--rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6808 2023-04-10 13:12:21.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6898 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3548 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1363 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-technicals.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1217 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-volcano.R
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-10 13:54:49.677996 cellsnake-0.2.0.dev9/cellsnake.egg-info/
--rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     3123 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/SOURCES.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/dependency_links.txt
--rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/entry_points.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/not-zip-safe
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/requires.txt
--rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-10 13:54:49.000000 cellsnake-0.2.0.dev9/cellsnake.egg-info/top_level.txt
--rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0.dev9/reqs.txt
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0.dev9/requirements.txt
--rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-10 13:54:49.687766 cellsnake-0.2.0.dev9/setup.cfg
--rw-r--r--   0 sium       (501) staff       (20)     1674 2023-04-10 13:53:06.000000 cellsnake-0.2.0.dev9/setup.py
--rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0.dev9/test_counts.txt
--rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0.dev9/test_meta.txt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.264800 cellsnake-0.2.0rc2/
+-rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0rc2/LICENSE
+-rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0rc2/MANIFEST.in
+-rw-r--r--   0 sium       (501) staff       (20)    10466 2023-04-23 23:04:33.264518 cellsnake-0.2.0rc2/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)    10020 2023-04-21 12:56:47.000000 cellsnake-0.2.0rc2/README.md
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.213246 cellsnake-0.2.0rc2/cellsnake/
+-rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0rc2/cellsnake/__init__.py
+-rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0rc2/cellsnake/cellsnake_functions.py
+-rwxr-xr-x   0 sium       (501) staff       (20)    18485 2023-04-23 23:03:36.000000 cellsnake-0.2.0rc2/cellsnake/command_line.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.214902 cellsnake-0.2.0rc2/cellsnake/scrna/
+-rw-r--r--   0 sium       (501) staff       (20)     2285 2023-04-20 08:38:42.000000 cellsnake-0.2.0rc2/cellsnake/scrna/config.yaml
+-rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0rc2/cellsnake/scrna/install_r_packages.sh
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.215474 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/
+-rw-r--r--   0 sium       (501) staff       (20)    24152 2023-04-22 13:11:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/Snakefile
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.216017 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/bundle/
+-rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.208386 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.220761 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.221023 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
+-rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.251516 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/
+-rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/extra_functions.smk
+-rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/integration.smk
+-rw-r--r--   0 sium       (501) staff       (20)     6067 2023-04-17 20:06:18.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/microbiome.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/params_detect.smk
+-rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/params_write.smk
+-rw-r--r--   0 sium       (501) staff       (20)    20983 2023-04-20 08:38:42.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/seurat.smk
+-rw-r--r--   0 sium       (501) staff       (20)      301 2023-04-18 12:20:01.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/subset.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/test.smk
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.264273 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/
+-rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
+-rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3961 2023-04-22 13:11:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
+-rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1241 2023-04-07 13:09:40.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3741 2023-04-22 13:11:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1714 2023-04-07 13:09:40.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3563 2023-04-07 13:09:40.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     7044 2023-04-10 13:12:21.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-functions.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3312 2023-04-23 23:02:52.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-gsea.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-harmony.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4701 2023-04-23 23:02:52.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kegg.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-metrics.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4076 2023-04-22 13:11:17.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
+-rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6808 2023-04-10 13:12:21.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6898 2023-04-07 13:09:40.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3587 2023-04-18 12:20:01.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1836 2023-04-20 08:38:42.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-technicals.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1217 2023-04-07 13:09:40.000000 cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-volcano.R
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-23 23:04:33.214455 cellsnake-0.2.0rc2/cellsnake.egg-info/
+-rw-r--r--   0 sium       (501) staff       (20)    10466 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)     3123 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/entry_points.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/not-zip-safe
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/requires.txt
+-rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-23 23:04:33.000000 cellsnake-0.2.0rc2/cellsnake.egg-info/top_level.txt
+-rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0rc2/reqs.txt
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0rc2/requirements.txt
+-rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-23 23:04:33.264843 cellsnake-0.2.0rc2/setup.cfg
+-rw-r--r--   0 sium       (501) staff       (20)     1673 2023-04-23 23:04:16.000000 cellsnake-0.2.0rc2/setup.py
+-rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0rc2/test_counts.txt
+-rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0rc2/test_meta.txt
```

### Comparing `cellsnake-0.2.0.dev9/LICENSE` & `cellsnake-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/command_line.py` & `cellsnake-0.2.0rc2/cellsnake/command_line.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 import random
 #from fuzzywuzzy import fuzz
 import timeit
 import errno
 import os
 import yaml
 from yaml.loader import SafeLoader
+from subprocess import call
+import pathlib
 
 
 #from schema import Schema, And, Or, Use, SchemaError
 
 from collections import defaultdict
 
 import cellsnake
 cellsnake_path=os.path.dirname(cellsnake.__file__)
 options = ["clustree","clusteringTree","minimal","standard","advanced"] #and integration
 
 
 __author__ = 'Sinan U. Umu'
-__version__= '0.2.0.dev9'
+__version__= '0.2.0.rc2'
 __logo__="""
              _  _                     _           
             | || |                   | |          
   ___   ___ | || | ___  _ __    __ _ | | __  ___  
  / __| / _ \| || |/ __|| '_ \  / _` || |/ / / _ \ 
 | (__ |  __/| || |\__ \| | | || (_| ||   < |  __/ 
  \___| \___||_||_||___/|_| |_| \__,_||_|\_\ \___| 
@@ -65,66 +67,127 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 __doc__=f"""Main cellsnake executable, version: {__version__}
 {__logo__} 
 Usage:
-    cellsnake <INPUT> [--resolution <text>] [--percent_mt <text>] [--configfile <text>] [--gene <text>] [--jobs <integer>] [--option <text>]... [--release-the-kraken <text>] [--taxa <text>] [--unlock|--remove] [--dry]
-    cellsnake <INPUT> [--unlock|--remove] [--dry]
+    cellsnake <command> <INPUT> [options] [--unlock|--remove] [--dry]
+    cellsnake integrated <command> <INPUT> [options] [--unlock|--remove] [--dry]
     cellsnake --generate-template
     cellsnake --install-packages
     cellsnake (-h | --help)
     cellsnake --version
 
-Arguments:
-    INPUT                                   Input directory or a file to process (if a directory given, batch mode is ON).
-    -c <text>, --configfile <text>          Config file name (if not supplied, it will use default settings, you may generate a template, change it and use it in your runs).
-    --resolution <text>                     Resolution for cluster detection, write "auto" for auto detection [default: 0.8].
-    --percent_mt <text>                     Maximum mitochondrial gene percentage cutoff, for example, 5 or 10, write "auto" for auto detection [default: 10].
-    --gene <text>                           Create publication ready plots for a gene or a list of genes from a text file.
-    --option <text>                         cellsnake run options: "minimal", "standard", "clustree", "advanced" [default: standard]. "integration" is to integrate and run on integrated samples.
-    --release-the-kraken <text>             Kraken database folder.
-    --taxa <text>                           Microbiome taxonomic level collapse to "domain", "kingdom", "phylum", "class", "order", "family", "genus", "species" [default: genus]
-    -j <integer>, --jobs <integer>          Total CPUs. [default: 2]
-
-Options:
-    --generate-template                Generate config file template in the current directory.
-    --install-packages                 Install, reinstall or check required R packages.
-    -u, --unlock                       Rescue stalled jobs (Try this if the previous job ended prematurely or currently failing).
-    -r, --remove                       Delete all output files (this won't affect input files).
-    -d, --dry                          Dry run, nothing will be generated.
-    -h, --help                         Show this screen.
-    --version                          Show version.
+commands:
+    minimal                                Run cellsnake with minimal workflow. 
+    standard                               Run cellsnake with standard workflow.
+    advanced                               Run cellsnake with advanced workflow.
+    clustree                               Run cellsnake with clustree workflow.
+    integrate                              Run cellsnake to integrate samples under analyses folder.
+                                           This option expects you have already finished processing multiple samples.
+
+main arguments:
+    INPUT                                  Input directory or a file to process (if a directory given, batch mode is ON).
+    --configfile <text>                    Config file name in YAML format, for example, "config.yaml". No default but can be created with --generate-template.
+    --metadata <text>                      Metadata file name in CSV, TSV or Excel format, for example, "metadata.csv", header required, first column sample name. No default but can be created with --generate-template.
+    --metadata_column <text>               Metadata column for differential expression analysis [default: condition].
 
+other arguments:
+    --gene <gene or filename>              Create publication ready plots for a gene or a list of genes from a text file.
+    
+main options:
+    --percent_mt <double>                  Maximum mitochondrial gene percentage cutoff, 
+                                           for example, 5 or 10, write "auto" for auto detection [default: 10].
+    --resolution <double>                  Resolution for cluster detection, write "auto" for auto detection [default: 0.8].
+
+other options:
+    --doublet_filter <bool>                [default: True] #this may fail on some samples
+    --percent_rp <double>                  [default: 0] #Ribosomal genes minimum percentage (0-100), default no filtering
+    --min_cells <integer>                  [default: 3] #seurat default, recommended
+    --min_features <integer>               [default: 200] #seurat default, recommended, nFeature_RNA
+    --max_features <integer>               [default: Inf] #seurat default, nFeature_RNA, 5000 can be a good cutoff
+    --min_molecules <integer>              [default: 0] #seurat default, nCount_RNA, min_features usually handles this so keep it 0
+    --max_molecules <integer>              [default: Inf] #seurat default, nCount_RNA, to filter potential doublets, doublet filtering is already default, so keep this Inf
+    --highly_variable_features <integer>   [default: 2000] #seurat defaults, recommended
+    --variable_selection_method <text>     [default: vst] #seurat defaults, recommended
+    
+    --normalization_method <text>          [default: LogNormalize]
+    --scale_factor <integer>               [default: 10000]
+    --logfc_threshold <double>             [default: 0.25]
+    --test_use <text>                      [default: wilcox]
+
+
+    --mapping <text>                       [default: org.Hs.eg.db] #you may install others from Bioconductor, this is for human
+    --organism <text>                      [default: hsa] #alternatives https://www.genome.jp/kegg/catalog/org_list.html
+    --species <text>                       [default: human] for cellchat, #only human or mouse is accepted
+
+plotting parameters:
+    --min_percentage_to_plot <double>        [default: 2] #only show clusters more than % of cells on the legend
+    --show_labels <bool>                     [default: True] #
+    --marker_plots_per_cluster_n <integer>   [default: 20] #plot summary marker plots for top markers
+    --umap_markers_plot <bool>               [default: True]
+    --tsne_markers_plot <bool>               [default: False]
+
+annotation options:
+    --singler_ref <text>                    [default: BlueprintEncodeData] # https://bioconductor.org/packages/release/data/experiment/vignettes/celldex/inst/doc/userguide.html#1_Overview
+    --celltypist_model <text>               [default: Immune_All_Low.pkl] #refer to Celltypist for another model 
+
+microbiome options:
+    --kraken_db_folder <text>              No default, you need to provide a folder with kraken2 database
+    --taxa <text>                          [default: genus] # available options "domain", "kingdom", "phylum", "class", "order", "family", "genus", "species"
+    --microbiome_min_cells <integer>       [default: 1]
+    --microbiome_min_features <integer>    [default: 3]
+    --confidence <double>                  [default: 0.05] #see kraken2 manual
+    --min_hit_groups <integer>             [default: 4] #see kraken2 manual
+
+integration options:
+    --dims <integer>                       [default: 30] #refer to Seurat for more details
+    --reduction <text>                     [default: cca] #refer to Seurat for more details
+
+others:
+    --generate-template                    Generate config file template and metadata template in the current directory.
+    --install-packages                     Install, reinstall or check required R packages.
+    -j <integer>, --jobs <integer>         Total CPUs. [default: 2]
+    -u, --unlock                           Rescue stalled jobs (Try this if the previous job ended prematurely or currently failing).
+    -r, --remove                           Delete all output files (this won't affect input files).
+    -d, --dry                              Dry run, nothing will be generated.
+    -h, --help                             Show this screen.
+    --version                              Show version.
+    
 """
 
 
 def check_command_line_arguments(arguments):
     if not os.path.exists(arguments["<INPUT>"]):
         print("File or input directory not found : ",arguments["<INPUT>"])
         return False
+    if arguments["integrated"] and os.path.isdir(arguments["<INPUT>"]):
+        print("You are running integrated option but you provided a directory, not a Seurat object file !")
+        print("The default Seurat object is usually here, analyses_integrated/seurat/integrated.rds")
+        print("""You can try something like: "cellsnake integrated standard analyses_integrated/seurat/integrated.rds""")
+        return False
+    if arguments["integrated"] and os.path.isfile(arguments["<INPUT>"]):
+        file_extension = pathlib.Path(arguments["<INPUT>"])
+        if (file_extension.suffix).lower() not in [".rds"]:
+            print("You are running integrated option but you provided not a Seurat object file !")
+            print("The default Seurat object is usually here, analyses_integrated/seurat/integrated.rds")
+            print("""You can try something like: \n cellsnake integrated standard analyses_integrated/seurat/integrated.rds""")
+            return False
     if arguments["--configfile"]:
          if not os.path.isfile(arguments["--configfile"]):
             print("Config file given not found : ",arguments["--configfile"])
             return False
-    if [o for o in arguments["--option"] if o not in ["minimal", "standard", "clustree", "integration", "advanced"]]:
-        print("Select a correct option for analyses : ",arguments["--option"])
-        print("Possible options : ",["minimal", "standard", "clustree", "advanced","integration"])
-        print("You may combine integration with others so the integrated sample will be processed accordingly.")
-        print("The default is : standard ")
-        return False
-    elif len(arguments["--option"]) > 1 and all(o  in arguments["--option"] for o in ["minimal", "standard", "clustree", "advanced"]):
-        print(arguments["--option"])
-        print("You cannot combine two options, except integration, choose one of these : ",["minimal", "standard", "clustree", "advanced"])
-        return False
-
-    if arguments["--release-the-kraken"]:
-        if not os.path.exists(arguments["--release-the-kraken"]) and not os.path.isfile(arguments["--release-the-kraken"] + "/inspect.txt"):
-            print("KrakenDB directory not found : ",arguments["--release-the-kraken"])
+    if arguments["--metadata"]:
+         if not os.path.isfile(arguments["--metadata"]):
+            print("Metadata file given not found : ",arguments["--metadata"])
+            return False
+    if arguments["--kraken_db_folder"]:
+        if not os.path.exists(arguments["--kraken_db_folder"]) and not os.path.isfile(arguments["--kraken_db_folder"] + "/inspect.txt"):
+            print("KrakenDB directory not found : ",arguments["--kraken_db_folder"])
             print("You should download a proper DB from this link (https://benlangmead.github.io/aws-indexes/k2), unpack it and point that directory.")
             return False
     if arguments["--taxa"] not in ["domain", "kingdom", "phylum", "class", "order", "family", "genus", "species"]:
         print("Select a correct taxa level for microbiome analysis:",arguments["--taxa"])
         print("Possible options : ",["domain", "kingdom", "phylum", "class", "order", "family", "genus", "species"])
         return False
     return True
@@ -135,14 +198,15 @@
         self.snakemake="snakemake --rerun-incomplete -k "
         self.runid="".join(random.choices("abcdefghisz",k=3) + random.choices("123456789",k=5))
         self.config=[]
         self.configfile_loaded=False
         self.is_integrated_sample=False
         self.is_this_an_integration_run=False
         self.parameters=dict()
+        self.log=True #if dry unlock etc, no logging
         
     def __str__(self):
         return self.snakemake
     def __repr__(self):
         return self.snakemake
     
 
@@ -150,164 +214,170 @@
 
         
 
     def add_config_argument(self):
         self.snakemake = self.snakemake + " --config " + " ".join(self.config)
 
 
-    def load_and_add_default_configfile_argument(self,arguments):
+    def load_configfile_if_available(self,arguments):
         if self.configfile_loaded is False:
             if arguments["--configfile"]:
                 self.snakemake = self.snakemake + " --configfile={}".format(arguments["--configfile"])
                 configfile=arguments["--configfile"]
-            else:
-                self.snakemake = self.snakemake + " --configfile={}".format(cellsnake_path + "/scrna/config.yaml")
-                configfile=cellsnake_path + "/scrna/config.yaml"
-
-            with open(configfile) as f:
-                self.parameters=yaml.load(f,Loader=SafeLoader)
-            self.configfile_loaded=True
+            #else:
+            #    self.snakemake = self.snakemake + " --configfile={}".format(cellsnake_path + "/scrna/config.yaml")
+            #    configfile=cellsnake_path + "/scrna/config.yaml"
+
+                with open(configfile) as f:
+                    self.parameters=yaml.load(f,Loader=SafeLoader)
+                self.configfile_loaded=True
         
-        self.change_parameters(arguments)
+                #self.change_parameters(arguments)
 
-    def change_parameters(self,arguments): #change parameters if there is a config file
-        if self.configfile_loaded is True and arguments["--configfile"]:
-            arguments["--resolution"] = self.parameters["resolution"]
-            arguments["--percent_mt"] = self.parameters["percent_mt"]
-            arguments["--taxa"] = self.parameters["taxa"]
+    #def change_parameters(self,arguments): #change parameters if there is a config file
+    #    if self.configfile_loaded is True and arguments["--configfile"]:
+    #        arguments["--resolution"] = self.parameters["resolution"]
+    #        arguments["--percent_mt"] = self.parameters["percent_mt"]
+    #        arguments["--taxa"] = self.parameters["taxa"]
 
 
 
 
 
 
         
 
     def prepare_arguments(self,arguments):
         self.snakemake = self.snakemake +  " -j {} ".format(arguments['--jobs']) #set CPU number
         self.snakemake = self.snakemake +  " -s {} ".format(f"{cellsnake_path}/scrna/workflow/Snakefile") #set Snakefile location
-        self.load_and_add_default_configfile_argument(arguments)
-        if self.is_this_an_integration_run is False and self.is_integrated_sample is False:
+        self.load_configfile_if_available(arguments)
+        if self.is_this_an_integration_run is False:
             self.config.append("datafolder={}".format(arguments['<INPUT>']))
 
         self.config.append(f"cellsnake_path={cellsnake_path}/scrna/")
-        self.config.append("resolution={}".format(arguments["--resolution"]))
-        self.config.append("percent_mt={}".format(arguments["--percent_mt"]))
-        self.config.append("taxa={}".format(arguments["--taxa"]))
+        for i,b in arguments.items():
+            if i not in ["--jobs","integrated","--configfile","--option","--gene","--kraken_db_folder","--unlock","--remove","--dry","--help","--version","<INPUT>","<command>","--install-packages","--generate-template"]:
+                k=i.lstrip("--")
+                if self.configfile_loaded is False: #if there is no config file, add all parameters given by the command line or defaults. command line parameters have priority over config file parameters
+                    self.config.append(k + "=" + str(b))
+                    self.parameters[k]=str(b)
+                else:
+                    if self.parameters.get(k) and i not in sys.argv:
+                        self.config.append(k + "=" + str(self.parameters.get(k)))
+                    else:
+                        self.config.append(k + "=" + str(b))
+                        self.parameters[k]=str(b)
+
+
+        
         self.config.append("runid={}".format(self.runid))
         if arguments["--gene"]:
             if os.path.isfile(arguments["--gene"]):
                 self.config.append("selected_gene_file={}".format(arguments["--gene"]))
             else:
                 self.config.append("gene_to_plot={}".format(arguments["--gene"]))
 
-        if arguments["--release-the-kraken"]:
-            self.config.append("kraken_db_folder={}".format(arguments["--release-the-kraken"]))
+        if arguments["--kraken_db_folder"]:
+            self.config.append("kraken_db_folder={}".format(arguments["--kraken_db_folder"]))
             
 
         if self.is_integrated_sample:
             self.config.append("is_integrated_sample={}".format("True"))
 
 
-        if any(x for x in arguments["--option"] if x in options) and self.is_this_an_integration_run is False:
-            self.config.append("option={}".format(arguments["--option"][0]))
+        if  self.is_this_an_integration_run is False:
+            self.config.append("option={}".format(arguments['<command>']))
          
         elif self.is_this_an_integration_run:
             self.config.append("option=integration")
         if arguments["--dry"]:
             self.snakemake = self.snakemake + " -n "
+            self.log=False
         if arguments["--unlock"]:
             self.snakemake = self.snakemake + " --unlock "
+            self.log=False
         if arguments["--remove"]:
             self.snakemake = self.snakemake + " --delete-all-output "
-        
+            self.log=False
         self.add_config_argument()
         
     
     def write_to_log(self,start):
         logname = "_".join(["cellsnake",self.runid, datetime.datetime.now().strftime("%y%m%d_%H%M%S"),"runlog"])
         stop = timeit.default_timer()
-        with open(logname,"w") as f:
-            f.write(__logo__ + "\n")
-            f.write("Run ID : " + __version__ + "\n")
-            f.write("Cellnake version : " + self.runid + "\n")
-            f.write("Cellsnake arguments : " + " ".join(sys.argv) + "\n\n")
-            f.write("------------------------------" + "\n")
-            f.write("Snakemake arguments : " + str(self.snakemake) + "\n\n")
-            f.write("------------------------------" + "\n")
-            f.write("Run parameters: " + str(self.parameters) + "\n\n")
-            f.write("Total run time: {t:.2f} mins \n".format(t=(stop-start)/60))
-
-
-
-
-
-
-def run_cellsnake(arguments):
-    start = timeit.default_timer()
-    if  "integration" in arguments["--option"]:
-        try:
-            snakemake_argument=run_integration(arguments)
-            snakemake_argument.write_to_log(start)
-        except:
-            pass
-            """
-            if not arguments["--dry"]:
-                print(arguments)
-                snakemake_argument=run_workflow(arguments,option=["minimal"])
-                print(arguments)
-                snakemake_argument.write_to_log(start)
-                snakemake_argument=run_integration(arguments)
-                snakemake_argument.write_to_log(start)
-            """
-
-    else:
-        snakemake_argument=run_workflow(arguments)
-        snakemake_argument.write_to_log(start)
+        if self.log:
+            with open(logname,"w") as f:
+                f.write(__logo__ + "\n")
+                f.write("Run ID : " + self.runid + "\n")
+                f.write("Cellnake version : " + __version__ + "\n")
+                f.write("Cellsnake arguments : " + " ".join(sys.argv) + "\n\n")
+                f.write("------------------------------" + "\n")
+                f.write("Snakemake arguments : " + str(self.snakemake) + "\n\n")
+                f.write("------------------------------" + "\n")
+                f.write("Run parameters: " + str(self.parameters) + "\n\n")
+                f.write("Total run time: {t:.2f} mins \n".format(t=(stop-start)/60))
 
 
 def run_integration(arguments):
 
-    if not arguments["--remove"]:
-        #first run integration
-        snakemake_argument=CommandLine()
-        snakemake_argument.is_this_an_integration_run = True
-        snakemake_argument.prepare_arguments(arguments)
-        subprocess.check_call(str(snakemake_argument),shell=True)
-
-    #then run workflow on integrated dataset
+    start = timeit.default_timer()
     snakemake_argument=CommandLine()
-    snakemake_argument.is_this_an_integration_run = False
-    snakemake_argument.is_integrated_sample = True
-    snakemake_argument.config.append("datafolder=analyses_integrated/seurat/integrated.rds")
-    try:
-        arguments["--option"].remove("integration")
-    except:
-        pass
+    snakemake_argument.is_this_an_integration_run = True
     snakemake_argument.prepare_arguments(arguments)
     subprocess.check_call(str(snakemake_argument),shell=True)
-    return snakemake_argument
+    snakemake_argument.write_to_log(start)
+
 
-def run_workflow(arguments,option=None):
+    #then run workflow on integrated dataset
+    #snakemake_argument=CommandLine()
+    #snakemake_argument.is_this_an_integration_run = False
+    #snakemake_argument.is_integrated_sample = True
+    #snakemake_argument.config.append("datafolder=analyses_integrated/seurat/integrated.rds")
+    #try:
+    #    arguments["--option"].remove("integration")
+    #except:
+    #    pass
+    #snakemake_argument.prepare_arguments(arguments)
+    #subprocess.check_call(str(snakemake_argument),shell=True)
+    #return snakemake_argument
+
+def run_workflow(arguments):
+    start = timeit.default_timer()
     snakemake_argument=CommandLine()
-    if option is not None:
-        arguments["--option"]=option
+    if arguments["integrated"]:
+        snakemake_argument.is_integrated_sample = True
     snakemake_argument.prepare_arguments(arguments)
     subprocess.check_call(str(snakemake_argument),shell=True)
-    return snakemake_argument
+    snakemake_argument.write_to_log(start)
 
 
 def main():
         cli_arguments = docopt(__doc__, version=__version__)
         if cli_arguments["--generate-template"]:
             print("Generating config.yaml file...")
             print("You can use this as a template for a cellsnake run. You may change the settings.")
             shutil.copyfile(cellsnake_path + "/scrna/config.yaml", 'config.yaml')
+            print("Generating metadata.csv file...")
+            with open("metadata.csv","w") as f:
+                f.write("sample,condition\n")
+                f.write("sample1,condition1\n")
+                f.write("sample2,condition2\n")
             return
         if cli_arguments["--install-packages"]:
             subprocess.check_call(cellsnake_path + "/scrna/workflow/scripts/scrna-install-packages.R")
             return
-        else:
-            if check_command_line_arguments(cli_arguments) is False:
-                return    
-            else:
-                run_cellsnake(arguments=cli_arguments)
+        
+        if not check_command_line_arguments(cli_arguments):
+            print("""Please check your command line arguments. Use "cellsnake --help" for more information""")
+            return
+
+
+        if cli_arguments['<command>'] == 'minimal':
+            run_workflow(cli_arguments)
+        if cli_arguments['<command>'] == 'standard':
+            run_workflow(cli_arguments)
+        if cli_arguments['<command>'] == 'advanced':
+            run_workflow(cli_arguments)
+        if cli_arguments['<command>'] == 'clustree':
+            run_workflow(cli_arguments)
+        if cli_arguments['<command>'] == 'integrate':
+            run_workflow(cli_arguments)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/config.yaml` & `cellsnake-0.2.0rc2/cellsnake/scrna/config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 #doublet filtering, True:T or False:F
 doublet_filter: T #this may fail on some samples
 
 #clustering and normalization paramaters
 normalization_method: "LogNormalize"
 scale_factor: 10000
-resolution: "0.8" #default is 0.8 and 0.3 for integrated samples, you can write "auto" for automatic detection
+resolution: "0.8" #seurat default
 
 #Differential expression paramaters
 logfc_threshold: 0.25
 test_use: "wilcox"
 marker_plots_per_cluster_n: 20 #plot summary marker plots for top markers
 umap_markers_plot: True
 tsne_markers_plot: False
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/Snakefile` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/Snakefile`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 max_molecules=config.get("max_molecules","Inf") #nCount_RNA
 min_molecules=config.get("min_molecules",0) #nCount_RNA
 percent_mt=str(config.get("percent_mt",10)) #if not automatic, this will be used for all samples
 percent_rp=config.get("percent_rp",0) #by default, no filtering on ribosomal genes percentage 
 highly_variable_features=config.get("highly_variable_features",2000)
 variable_selection_method=config.get("variable_selection_method","vst")
 doublet_filter= "--doublet.filter" if config.get("doublet_filter",True) in [True,"TRUE","True","T"] and is_integrated_sample is False else ""
-metadata_file=config.get("metadata_file","metadata.csv")
+metadata=config.get("metadata","metadata.csv")
 metadata_column=config.get("metadata_column","condition")
 keywords=config.get("keywords",1)
 exact="--exact" if config.get("exact",True) in [True,"TRUE","True","T"] else ""
 subset_file=config.get("subset_file","subset")
 subset_column=config.get("subset_column","seurat_clusters")
 
 min_percentage_to_plot=config.get("min_percentage_to_plot",5) #only plot clusters with more than 5% of cells
@@ -94,15 +94,16 @@
 
 #automatic cluster/resolution detection
 #detect_resolution=config.get("detect_resolution",True)
 
 #clustering and normalization paramaters
 normalization_method=config.get("normalization_method","LogNormalize")
 scale_factor=config.get("scale_factor",10000)
-resolution=config.get("resolution","0.8" if is_integrated_sample is False else "0.3") #a double or "auto", default is 0.8
+#resolution=config.get("resolution","0.8" if is_integrated_sample is False else "0.3") #a double or "auto", default is 0.8
+resolution=config.get("resolution","0.8") #a double or "auto", default is 0.8
 
 #dimension reduction options: by default both UMAP and TSNE will be plotted with predicted clusters
 umap_plot="--umap" if config.get("umap_plot",True) in [True,"TRUE","True","T"] else ""
 tsne_plot="--tsne" if config.get("tsne_plot",True) in [True,"TRUE","True","T"] else ""
 show_labels="--labels" if config.get("show_labels",True) in [True,"TRUE","True","T"] else ""
 
 #Each marker plot contains a DimPlot, by default only UMAP plots will be created (to save space and time), this behavior can be changed.
@@ -234,15 +235,15 @@
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-geneset_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-module_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-module_geneset_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
     return outs
 
 def metadata_pairwise_deseq_analysis(paramspace,metadata_column):
     outs=[]
-    if os.path.isfile(metadata_file) and is_integrated_sample:
+    if os.path.isfile(metadata) and is_integrated_sample:
         outs += expand([results_folder + "/" + s + "/{params}/metaplot_volcano-" + metadata_column + ".pdf" for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/metatable_positive-markers-" + metadata_column + ".xlsx" for s in files],params=list(paramspace.instance_patterns))
     return outs
 
 
 
 def kraken_predictions(paramspace,taxa,identity):
@@ -250,14 +251,15 @@
     outs=[]
     if kraken_db_folder is not None:
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_microbiome_full-" + taxa + "-level.pdf" for s in files],params=list(paramspace.instance_patterns))
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_microbiome_dimplot-" + taxa + "-" + x + ".pdf" for x in ["umap","tsne"] for s in files],params=list(paramspace.instance_patterns))
         outs = outs + ["analyses_integrated/seurat/" + integration_id + "-" + taxa + ".rds"]
     elif is_integrated_sample is True and os.path.isfile("analyses_integrated/seurat/" + integration_id + "-" + taxa + ".rds"):
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_integrated_microbiome_dimplot-" + taxa + "-" + x + ".pdf" for x in ["umap","tsne"] for s in files],params=list(paramspace.instance_patterns))
+        outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_integrated_total_microbiome-" + taxa + "-" + x + ".pdf" for x in ["umap","tsne"] for s in files],params=list(paramspace.instance_patterns))
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_integrated_significance-" + taxa + "-" + x + ".pdf" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/table_integrated_significance-" + taxa + "-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
     return outs
 
 
 def write_main_log(files):
 
@@ -342,14 +344,16 @@
                 selected_gene_plot(paramspace,gene_to_plot,identity_to_analysis),
                 metadata_pairwise_deseq_analysis(paramspace,metadata_column)
                 ]
     if option in ["clustree","clusteringTree","minimal","standard","advanced"]:
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_clustree.pdf" for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_nFeature.pdf" for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_nCount.pdf" for s in files],params=list(paramspace.instance_patterns))
+        outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_mt.percent.pdf" for s in files],params=list(paramspace.instance_patterns))
+        outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_rp.percent.pdf" for s in files],params=list(paramspace.instance_patterns))
     if option in ["advanced"]:
         outs += cellchat_plot(paramspace,[x for x in identity_to_analysis if x != "orig.ident"])
         outs += dim_reduction_and_marker_plots(paramspace,identity_to_analysis)
     if option not in ["clustree","clusteringTree","minimal","standard","advanced"]:
         print("Please select a correct option...")
 
     if not any(b in ["--dry-run", "--dryrun", "-n"] for b in sys.argv):
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/k2sc.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/k2sc.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/extra_functions.smk` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/extra_functions.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/microbiome.smk` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/microbiome.smk`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,18 @@
 
 
 rule dimplot_for_microbiome:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
         microbiome_rds=analyses_folder + "/kraken/" + f"{paramspace.wildcard_pattern}" + "/{sample}/microbiome-full-{taxa}-level.rds"
     output:
-        results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_microbiome_dimplot-{taxa}-{reduction}.pdf"
+        dimplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_microbiome_dimplot-{taxa}-{reduction}.pdf",
+        tplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_total_microbiome-{taxa}-{reduction}.pdf"
     shell:
-        "{cellsnake_path}workflow/scripts/scrna-microbiome-dimplot.R --rds {input.rds} --microbiome.rds {input.microbiome_rds} --dimplot {output} --reduction.type {wildcards.reduction} --taxa {wildcards.taxa}"
+        "{cellsnake_path}workflow/scripts/scrna-microbiome-dimplot.R --rds {input.rds} --microbiome.rds {input.microbiome_rds} --dimplot {output.dimplot} --tplot {output.tplot} --reduction.type {wildcards.reduction} --taxa {wildcards.taxa}"
 
 
 rule combine_microbiome_files_for_later:
     input:
         lambda wildcards : expand([analyses_folder + "/kraken/" + "{params}" + "/" + s + "/microbiome-full-" + wildcards.taxa + "-level.rds" for s in files],params=list(paramspace.instance_patterns))
     output:
         "analyses_integrated/seurat/" + integration_id + "-{taxa}.rds"
@@ -74,17 +75,18 @@
 
 
 rule dimplot_for_combined_microbiome:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
         microbiome_rds="analyses_integrated/seurat/" + integration_id + "-{taxa}.rds"
     output:
-        dimplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_integrated_microbiome_dimplot-{taxa}-{reduction}.pdf"
+        dimplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_integrated_microbiome_dimplot-{taxa}-{reduction}.pdf",
+        tplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_integrated_total_microbiome-{taxa}-{reduction}.pdf"
     shell:
-        "{cellsnake_path}workflow/scripts/scrna-microbiome-dimplot.R --rds {input.rds} --microbiome.rds {input.microbiome_rds} --dimplot {output.dimplot} --reduction.type {wildcards.reduction} --taxa {wildcards.taxa}"
+        "{cellsnake_path}workflow/scripts/scrna-microbiome-dimplot.R --rds {input.rds} --microbiome.rds {input.microbiome_rds} --dimplot {output.dimplot} --tplot {output.tplot} --reduction.type {wildcards.reduction} --taxa {wildcards.taxa}"
 
 rule sigplot_for_combined_microbiome:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
         microbiome_rds="analyses_integrated/seurat/" + integration_id + "-{taxa}.rds"
     output:
         dimplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/microbiome/plot_integrated_significance-{taxa}-{i}.pdf",
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/params_detect.smk` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/params_detect.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/seurat.smk` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/seurat.smk`

 * *Files 0% similar despite different names*

```diff
@@ -87,18 +87,20 @@
         "{cellsnake_path}workflow/scripts/scrna-metrics.R --rds {input.rds} --ccplot {output.ccplot} --ccbarplot {output.ccbarplot} --html {output.html} --idents {wildcards.i}"
 
 rule plot_some_technicals:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds"
     output:
         fplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/technicals/plot_nFeature.pdf",
-        cplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/technicals/plot_nCount.pdf"
+        cplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/technicals/plot_nCount.pdf",
+        mtplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/technicals/plot_mt.percent.pdf",
+        rpplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/technicals/plot_rp.percent.pdf"
 
     shell:
-        "{cellsnake_path}workflow/scripts/scrna-technicals.R --rds {input.rds} --fplot {output.fplot} --cplot {output.cplot}"
+        "{cellsnake_path}workflow/scripts/scrna-technicals.R --rds {input.rds} --fplot {output.fplot} --cplot {output.cplot} --mtplot {output.mtplot} --rpplot {output.rpplot}"
 
 
 
 rule plot_dimplots:
     input:
         analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds"
     output:
@@ -264,15 +266,15 @@
     shell:
         "{cellsnake_path}workflow/scripts/scrna-go_analysis.R --xlsx {input} --output.rds {output.rds} --mapping {mapping} --output.go {output.go} --output.gse {output.gse}"
 
 
 rule deseq_analysis_from_metadata_file:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
-        metadata=metadata_file
+        metadata=metadata
     output:
         rds=analyses_folder + "/markers/" + f"{paramspace.wildcard_pattern}" + "/deseq_{sample}-{i}.rds"
     shell:
         "{cellsnake_path}workflow/scripts/scrna-find-pairwise-markers.R --rds {input.rds} --logfc.threshold {logfc_threshold} --test.use {test_use} --output.rds {output.rds} --metadata {input.metadata} --metadata.column {wildcards.i}"
 
 rule create_deseq_metadata_tables:
     input:
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/rules/test.smk` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/rules/test.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-cellchat.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-dimplot.R`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,114 @@
 #!/usr/bin/env Rscript
 
+
 option_list <- list(
-      optparse::make_option(c("--sampleid"),
-            type = "character", default = NULL,
-            help = "Sample ID", metavar = "character"
-      ),
       optparse::make_option(c("--rds"),
             type = "character", default = NULL,
-            help = "A list of RDS files of Seurat objects", metavar = "character"
+            help = "Processed rds file of a Seurat object", metavar = "character"
       ),
-      optparse::make_option(c("--csv"),
-            type = "character", default = NULL,
-            help = "Celltypist prediction file", metavar = "character"
+      optparse::make_option(c("--reduction.type"),
+            type = "character", default = "umap",
+            help = "Reduction type, umap or tsne", metavar = "character"
       ),
-      optparse::make_option(c("--output.tsne.plot"),
-            type = "character", default = NULL,
-            help = "Output tsne file name", metavar = "character"
+      optparse::make_option(c("--pdfplot"),
+            type = "character", default = "reduction.pdf",
+            help = "Plot file name", metavar = "character"
       ),
-      optparse::make_option(c("--output.umap.plot"),
+      optparse::make_option(c("--htmlplot"),
+            type = "character", default = "reduction.html",
+            help = "Plot file name", metavar = "character"
+      ),
+      optparse::make_option(c("--csv"),
             type = "character", default = NULL,
-            help = "Output umap file name", metavar = "character"
+            help = "CSV meta file", metavar = "character"
+      ),
+      optparse::make_option(c("--idents"),
+            type = "character", default = "seurat_clusters",
+            help = "Meta data column name for marker analysis", metavar = "character"
       ),
       optparse::make_option(c("--percentage"),
             type = "double", default = 5,
             help = "Cluster mimnimum percentage to plot", metavar = "double"
-      ), optparse::make_option(c("--labels"), action = "store_true", default = FALSE, help = "Print labels on the plot")
+      ),
+      optparse::make_option(c("--labels"), action = "store_true", default = FALSE, help = "Print labels on the plot")
 )
 
+
+
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
-if (is.null(opt$rds) || is.null(opt$csv)) {
+if (is.null(opt$rds)) {
       optparse::print_help(opt_parser)
-      stop("At least one argument must be supplied (rds and sampleid)", call. = FALSE)
+      stop("At least one argument must be supplied (rds file)", call. = FALSE)
 }
 
-require(tidyverse)
+require(patchwork)
+require(plotly)
 require(Seurat)
-
+require(tidyverse)
 
 tryCatch(
       {
             source("workflow/scripts/scrna-functions.R")
       },
       error = function(cond) {
             source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
       }
 )
 
 
+
 scrna <- readRDS(file = opt$rds)
 DefaultAssay(scrna) <- "RNA"
 
-celltypist <- read.csv(
-      opt$csv,
-      row.names = 1
-)
 
-scrna@meta.data <- scrna@meta.data %>%
-      tibble::rownames_to_column("barcodes") %>%
-      dplyr::left_join(celltypist %>% as.data.frame() %>% rownames_to_column("barcodes"), by = "barcodes") %>%
-      tibble::column_to_rownames("barcodes")
+if (!is.null(opt$csv)) {
+      metadata <- read.csv(
+            opt$csv,
+            row.names = 1
+      )
+
+      scrna@meta.data <- scrna@meta.data %>%
+            tibble::rownames_to_column("barcodes") %>%
+            dplyr::left_join(metadata %>% as.data.frame() %>% rownames_to_column("barcodes"), by = "barcodes") %>%
+            tibble::column_to_rownames("barcodes")
+}
 
+Idents(object = scrna) <- scrna@meta.data[[opt$idents]]
 
-n <- length(scrna@meta.data %>% pull(majority_voting) %>% unique())
+n <- length(Idents(scrna) %>% unique())
 
 palette <- function_color_palette(n)
-palette <- function_color_palette(n)
-palette <- setNames(palette, scrna@meta.data %>% pull(majority_voting) %>% unique())
+palette <- setNames(palette, Idents(scrna) %>% unique())
 
 breaks <- scrna@meta.data %>%
-      dplyr::select(majority_voting) %>%
-      dplyr::count(majority_voting) %>%
+      dplyr::select(opt$idents) %>%
+      dplyr::count(get(opt$idents)) %>%
       dplyr::mutate(perc = (n * 100) / sum(n)) %>%
       dplyr::filter(perc >= opt$percentage) %>%
       dplyr::select(-n, -perc) %>%
       distinct() %>%
       pull() %>%
       as.character()
 
-p1 <- DimPlot(scrna, reduction = "tsne", label = opt$labels, group.by = "majority_voting", repel = TRUE) & scale_color_manual(values = palette, breaks = breaks)
-p2 <- DimPlot(scrna, reduction = "umap", label = opt$labels, group.by = "majority_voting", repel = TRUE) & scale_color_manual(values = palette, breaks = breaks)
 
+p1 <- DimPlot(scrna, reduction = opt$reduction.type) & scale_color_manual(values = palette)
 
-m <- max(str_count(breaks))
+ggplotly(p1) -> p1_plotly
 
-w <- c(7.5 + (m * 0.08) * (floor(length(breaks) / 11) + 1))
+p1_plotly %>% htmlwidgets::saveWidget(file = opt$htmlplot, selfcontained = T)
+
+m <- max(str_count(breaks))
 
+w <- c(8 + (m * 0.09) * (floor(length(breaks) / 11) + 1))
 
-ggsave(plot = p1, filename = opt$output.tsne.plot, width = w, height = 7)
-ggsave(plot = p2, filename = opt$output.umap.plot, width = w, height = 7)
 
+p1 <- DimPlot(scrna, reduction = opt$reduction.type, label = opt$labels, repel = TRUE) &
+      scale_color_manual(values = palette, breaks = breaks) &
+      theme(legend.direction = "horizontal", legend.text = element_text(size = 7)) &
+      guides(colour = guide_legend(ncol = 2, override.aes = list(size = 7)))
 
+(p1 / guide_area()) + plot_layout(heights = c(2.5, 1), widths = c(1, 0.6), guides = "collect") -> p1
 
-# saveRDS(scrna,file = opt$output)
+ggsave(plot = p1, filename = opt$pdfplot, width = 7.5, height = 8)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-celltypist.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-celltypist.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dimplot.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,92 @@
 #!/usr/bin/env Rscript
 
-
 option_list <- list(
-      optparse::make_option(c("--rds"),
-            type = "character", default = NULL,
-            help = "Processed rds file of a Seurat object", metavar = "character"
-      ),
-      optparse::make_option(c("--reduction.type"),
-            type = "character", default = "umap",
-            help = "Reduction type, umap or tsne", metavar = "character"
-      ),
-      optparse::make_option(c("--pdfplot"),
-            type = "character", default = "reduction.pdf",
-            help = "Plot file name", metavar = "character"
-      ),
-      optparse::make_option(c("--htmlplot"),
-            type = "character", default = "reduction.html",
-            help = "Plot file name", metavar = "character"
-      ),
-      optparse::make_option(c("--csv"),
-            type = "character", default = NULL,
-            help = "CSV meta file", metavar = "character"
-      ),
-      optparse::make_option(c("--idents"),
-            type = "character", default = "seurat_clusters",
-            help = "Meta data column name for marker analysis", metavar = "character"
-      ),
-      optparse::make_option(c("--percentage"),
-            type = "double", default = 5,
-            help = "Cluster mimnimum percentage to plot", metavar = "double"
-      ),
-      optparse::make_option(c("--labels"), action = "store_true", default = FALSE, help = "Print labels on the plot")
+  optparse::make_option(c("--min.cells"),
+    type = "integer", default = 1,
+    help = "Min cells [default= %default]", metavar = "integer"
+  ),
+  optparse::make_option(c("--min.features"),
+    type = "integer", default = 3,
+    help = "Min features [default= %default]", metavar = "character"
+  ),
+  optparse::make_option(c("--data.dir"),
+    type = "character", default = NULL,
+    help = "Data directory", metavar = "character"
+  ),
+  optparse::make_option(c("--h5seurat"),
+    type = "character", default = NULL,
+    help = "Data directory", metavar = "character"
+  ),
+  optparse::make_option(c("--sampleid"),
+    type = "character", default = NULL,
+    help = "Sample ID", metavar = "character"
+  ),
+  optparse::make_option(c("--output.rds"),
+    type = "character", default = "output.rds",
+    help = "Output RDS file name [default= %default]", metavar = "character"
+  ),
+  optparse::make_option(c("--output.plot"),
+    type = "character", default = "output.pdf",
+    help = "Output barplot file name [default= %default]", metavar = "character"
+  ),
+  optparse::make_option(c("--taxa"),
+    type = "character", default = "genus",
+    help = "Taxonomic level", metavar = "character"
+  )
 )
 
-
-
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
-if (is.null(opt$rds)) {
-      optparse::print_help(opt_parser)
-      stop("At least one argument must be supplied (rds file)", call. = FALSE)
+if (is.null(opt$h5seurat)) {
+  optparse::print_help(opt_parser)
+  stop("At least one argument must be supplied (data.dir and sampleid)", call. = FALSE)
 }
 
-require(plotly)
-require(Seurat)
+require(optparse)
 require(tidyverse)
-
+require(Seurat)
+require(SeuratDisk)
 tryCatch(
-      {
-            source("workflow/scripts/scrna-functions.R")
-      },
-      error = function(cond) {
-            source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
-      }
+  {
+    source("workflow/scripts/scrna-functions.R")
+  },
+  error = function(cond) {
+    source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
+  }
 )
+# nFeature_RNA is the number of genes detected in each cell. nCount_RNA is the total number of molecules detected within a cell.
 
 
+# CreateSeuratObject(scrna.data,min.cells = 1,min.features = 5) -> scrna
 
-scrna <- readRDS(file = opt$rds)
-DefaultAssay(scrna) <- "RNA"
-
-
-if (!is.null(opt$csv)) {
-      metadata <- read.csv(
-            opt$csv,
-            row.names = 1
-      )
-
-      scrna@meta.data <- scrna@meta.data %>%
-            tibble::rownames_to_column("barcodes") %>%
-            dplyr::left_join(metadata %>% as.data.frame() %>% rownames_to_column("barcodes"), by = "barcodes") %>%
-            tibble::column_to_rownames("barcodes")
-}
-
-Idents(object = scrna) <- scrna@meta.data[[opt$idents]]
-
-n <- length(Idents(scrna) %>% unique())
-
-palette <- function_color_palette(n)
-palette <- setNames(palette, Idents(scrna) %>% unique())
-
-breaks <- scrna@meta.data %>%
-      dplyr::select(opt$idents) %>%
-      dplyr::count(get(opt$idents)) %>%
-      dplyr::mutate(perc = (n * 100) / sum(n)) %>%
-      dplyr::filter(perc >= opt$percentage) %>%
-      dplyr::select(-n, -perc) %>%
-      distinct() %>%
-      pull() %>%
-      as.character()
-
-
-p1 <- DimPlot(scrna, reduction = opt$reduction.type) & scale_color_manual(values = palette)
+CreateSeuratObject(LoadH5Seurat(opt$h5seurat)[["RNA"]]@counts, min.cells = opt$min.cells, min.features = opt$min.features) -> scrna
 
-ggplotly(p1) -> p1_plotly
+scrna <- RenameCells(object = scrna, add.cell.id = make.names(opt$sampleid)) # add cell.id to cell name
 
-p1_plotly %>% htmlwidgets::saveWidget(file = opt$htmlplot, selfcontained = T)
 
-m <- max(str_count(breaks))
+scrna[["RNA"]]@counts %>%
+  as.matrix() %>%
+  t() %>%
+  as.data.frame() %>%
+  select(-starts_with("Homo")) -> df
 
-w <- c(7.5 + (m * 0.08) * (floor(length(breaks) / 11) + 1))
+df %>%
+  rownames_to_column("barcode") %>%
+  gather(group, umi, -barcode) %>%
+  group_by(group) %>%
+  summarise(sum = log(sum(umi))) %>%
+  arrange(desc(sum)) %>%
+  slice_max(n = 50, order_by = sum) %>%
+  ggplot(aes(reorder(group, sum), sum)) +
+  geom_col() +
+  coord_flip() +
+  ggthemes::theme_few() +
+  ylab("log-total UMI") +
+  xlab(opt$taxa) +
+  ggtitle(opt$sampleid) +
+  theme(axis.title = element_text(size = 12)) -> p1
 
+ggsave(plot = p1, filename = opt$output.plot, width = 6, height = 9)
 
-p1 <- DimPlot(scrna, reduction = opt$reduction.type, label = opt$labels, repel = TRUE) & scale_color_manual(values = palette, breaks = breaks)
-ggsave(plot = p1, filename = opt$pdfplot, width = w, height = 7)
+saveRDS(df, file = opt$output.rds)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-dotplot.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-dotplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-markers.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-find-markers.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-functions.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-functions.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,19 @@
     type = "double", default = 1.5,
     help = "LogFC [default= %default]", metavar = "character"
   )
 )
 # require(clusterProfiler)
 require(tidyverse)
 
+try({
+  if (!requireNamespace(opt$mapping, quietly = TRUE)) {
+    BiocManager::install(opt$mapping)
+  }
+})
 
 
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
 require(opt$mapping, character.only = T)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-gsea.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-gsea.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-harmony.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-harmony.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-install-packages.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-install-packages.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kegg.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kegg.R`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,19 @@
     type = "double", default = 1,
     help = "LogFC [default= %default]", metavar = "character"
   )
 )
 # require(clusterProfiler)
 require(tidyverse)
 
-
+try({
+  if (!requireNamespace(opt$mapping, quietly = TRUE)) {
+    BiocManager::install(opt$mapping)
+  }
+})
 
 
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 require(opt$mapping, character.only = T)
 if (is.null(opt$xlsx)) {
   optparse::print_help(opt_parser)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-metrics.R`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,74 @@
 #!/usr/bin/env Rscript
-
 option_list <- list(
-  optparse::make_option(c("--min.cells"),
-    type = "integer", default = 1,
-    help = "Min cells [default= %default]", metavar = "integer"
-  ),
-  optparse::make_option(c("--min.features"),
-    type = "integer", default = 3,
-    help = "Min features [default= %default]", metavar = "character"
-  ),
-  optparse::make_option(c("--data.dir"),
+  optparse::make_option(c("--rds"),
     type = "character", default = NULL,
-    help = "Data directory", metavar = "character"
-  ),
-  optparse::make_option(c("--h5seurat"),
-    type = "character", default = NULL,
-    help = "Data directory", metavar = "character"
+    help = "Processed rds file of a Seurat object", metavar = "character"
   ),
   optparse::make_option(c("--sampleid"),
     type = "character", default = NULL,
     help = "Sample ID", metavar = "character"
   ),
-  optparse::make_option(c("--output.rds"),
-    type = "character", default = "output.rds",
-    help = "Output RDS file name [default= %default]", metavar = "character"
-  ),
-  optparse::make_option(c("--output.plot"),
-    type = "character", default = "output.pdf",
-    help = "Output barplot file name [default= %default]", metavar = "character"
-  ),
-  optparse::make_option(c("--taxa"),
-    type = "character", default = "genus",
-    help = "Taxonomic level", metavar = "character"
+  optparse::make_option(c("--idents"),
+    type = "character", default = "seurat_clusters",
+    help = "Meta data column name for marker analysis", metavar = "character"
+  ),
+  optparse::make_option(c("--ccplot"),
+    type = "character", default = "ccplot.pdf",
+    help = "Cell cluster count plot", metavar = "character"
+  ),
+  optparse::make_option(c("--ccbarplot"),
+    type = "character", default = "ccbarplot.pdf",
+    help = "Cell cluster count plot", metavar = "character"
+  ),
+  optparse::make_option(c("--htmlplot"),
+    type = "character", default = "htmlplot.pdf",
+    help = "Cell cluster html plot", metavar = "character"
   )
 )
 
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
-if (is.null(opt$h5seurat)) {
+if (is.null(opt$rds)) {
   optparse::print_help(opt_parser)
-  stop("At least one argument must be supplied (data.dir and sampleid)", call. = FALSE)
+  stop("At least one argument must be supplied (rds file and sampleid)", call. = FALSE)
 }
 
-require(optparse)
-require(tidyverse)
+require(plotly)
+require(ggpubr)
 require(Seurat)
-require(SeuratDisk)
-tryCatch(
-  {
-    source("workflow/scripts/scrna-functions.R")
-  },
-  error = function(cond) {
-    source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
-  }
-)
-# nFeature_RNA is the number of genes detected in each cell. nCount_RNA is the total number of molecules detected within a cell.
+require(tidyverse)
+# try({source("workflow/scripts/scrna-functions.R")})
+# try({source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE),"/scrna/workflow/scripts/scrna-functions.R"))})
 
 
-# CreateSeuratObject(scrna.data,min.cells = 1,min.features = 5) -> scrna
 
-CreateSeuratObject(LoadH5Seurat(opt$h5seurat)[["RNA"]]@counts, min.cells = opt$min.cells, min.features = opt$min.features) -> scrna
+scrna <- readRDS(file = opt$rds)
 
-scrna <- RenameCells(object = scrna, add.cell.id = make.names(opt$sampleid)) # add cell.id to cell name
 
 
-scrna[["RNA"]]@counts %>%
-  as.matrix() %>%
-  t() %>%
-  as.data.frame() %>%
-  select(-starts_with("Homo")) -> df
+scrna@meta.data %>%
+  dplyr::add_count(orig.ident) %>%
+  dplyr::mutate(total_clusters = length(unique(get(opt$idents)))) %>%
+  distinct(orig.ident, n, total_clusters) %>%
+  dplyr::select("Sample Name" = orig.ident, "Total Cells" = n, "Total Clusters" = total_clusters) %>%
+  ggtexttable(rows = NULL, theme = ttheme("light")) -> p1
 
-df %>%
-  rownames_to_column("barcode") %>%
-  gather(group, umi, -barcode) %>%
-  group_by(group) %>%
-  summarise(sum = log(sum(umi))) %>%
-  arrange(desc(sum)) %>%
-  slice_max(n = 50, order_by = sum) %>%
-  ggplot(aes(reorder(group, sum), sum)) +
+ggsave(opt$ccplot, p1)
+
+scrna@meta.data %>%
+  dplyr::group_by(orig.ident, get(opt$idents)) %>%
+  dplyr::count() %>%
+  dplyr::select("Sample Name" = 1, "Cluster" = 2, "Total Cells" = 3) %>%
+  ggplot(aes(x = Cluster, y = `Total Cells`, fill = `Sample Name`)) +
   geom_col() +
-  coord_flip() +
-  ggthemes::theme_few() +
-  ylab("log-total UMI") +
-  xlab(opt$taxa) +
-  ggtitle(opt$sampleid) +
-  theme(axis.title = element_text(size = 12)) -> p1
+  ggthemes::theme_hc() +
+  theme(legend.title = element_blank()) -> p2
+n <- length(unique(scrna@meta.data[opt$idents]))
+
+ggsave(opt$ccbarplot, p2, height = 5, width = 5 + (n * 0.12))
+
 
-ggsave(plot = p1, filename = opt$output.plot, width = 6, height = 9)
+ggplotly(p2) -> p1_plotly
 
-saveRDS(df, file = opt$output.rds)
+p1_plotly %>% htmlwidgets::saveWidget(file = opt$htmlplot, selfcontained = T)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-metrics.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,85 @@
 #!/usr/bin/env Rscript
+
 option_list <- list(
-  optparse::make_option(c("--rds"),
-    type = "character", default = NULL,
-    help = "Processed rds file of a Seurat object", metavar = "character"
-  ),
-  optparse::make_option(c("--sampleid"),
-    type = "character", default = NULL,
-    help = "Sample ID", metavar = "character"
-  ),
-  optparse::make_option(c("--idents"),
-    type = "character", default = "seurat_clusters",
-    help = "Meta data column name for marker analysis", metavar = "character"
-  ),
-  optparse::make_option(c("--ccplot"),
-    type = "character", default = "ccplot.pdf",
-    help = "Cell cluster count plot", metavar = "character"
-  ),
-  optparse::make_option(c("--ccbarplot"),
-    type = "character", default = "ccbarplot.pdf",
-    help = "Cell cluster count plot", metavar = "character"
-  ),
-  optparse::make_option(c("--htmlplot"),
-    type = "character", default = "htmlplot.pdf",
-    help = "Cell cluster html plot", metavar = "character"
-  )
+      optparse::make_option(c("--rds"),
+            type = "character", default = NULL,
+            help = "A list of RDS files of Seurat objects", metavar = "character"
+      ),
+      optparse::make_option(c("--sheplot"),
+            type = "character", default = "sheplot.pdf",
+            help = "Output score heatmap plot file name", metavar = "character"
+      ),
+      optparse::make_option(c("--sheplottop"),
+            type = "character", default = "sheplot.pdf",
+            help = "Output score heatmap plot file name, top 20", metavar = "character"
+      ),
+      optparse::make_option(c("--pheplot"),
+            type = "character", default = "pheplot.pdf",
+            help = "Output heatmap plot file name", metavar = "character"
+      ),
+      optparse::make_option(c("--idents"),
+            type = "character", default = "seurat_clusters",
+            help = "Meta data column name", metavar = "character"
+      ),
+      optparse::make_option(c("--csv"),
+            type = "character", default = NULL,
+            help = "A meta data table", metavar = "character"
+      ),
+      optparse::make_option(c("--reference"),
+            type = "character", default = "HumanPrimaryCellAtlasData",
+            help = "SingleR reference", metavar = "character"
+      )
 )
 
+
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
 if (is.null(opt$rds)) {
-  optparse::print_help(opt_parser)
-  stop("At least one argument must be supplied (rds file and sampleid)", call. = FALSE)
+      optparse::print_help(opt_parser)
+      stop("At least one argument must be supplied (rds and sampleid)", call. = FALSE)
 }
 
-require(plotly)
-require(ggpubr)
-require(Seurat)
+
+require(optparse)
+require(SingleR)
+require(SingleCellExperiment)
+# require(celldex)
 require(tidyverse)
-# try({source("workflow/scripts/scrna-functions.R")})
-# try({source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE),"/scrna/workflow/scripts/scrna-functions.R"))})
+require(pheatmap)
+require(Seurat)
 
+scrna <- readRDS(file = opt$rds)
+DefaultAssay(scrna) <- "RNA"
 
+if (!is.null(opt$tsv)) {
+      markers <- read_tsv(opt$tsv, col_names = FALSE) %>% pull()
+}
+
+
+# celltype annotation with SingleR
+ref <- get(opt$reference)()
+
+smObjSCE <- as.SingleCellExperiment(scrna)
+pred <- SingleR(test = smObjSCE, ref = ref, labels = ref$label.fine)
+
+
+plotScoreHeatmap(pred) -> p1
+ggsave(plot = p1, filename = opt$sheplot, width = 15, height = 8)
+
+
+plotScoreHeatmap(pred, show.labels = F, max.labels = 20) -> p1
+ggsave(plot = p1, filename = opt$sheplottop, width = 7, height = 4)
 
-scrna <- readRDS(file = opt$rds)
 
+tab <- table(Assigned = pred$pruned.labels, Cluster = smObjSCE[[opt$idents]])
 
 
-scrna@meta.data %>%
-  dplyr::add_count(orig.ident) %>%
-  dplyr::mutate(total_clusters = length(unique(get(opt$idents)))) %>%
-  distinct(orig.ident, n, total_clusters) %>%
-  dplyr::select("Sample Name" = orig.ident, "Total Cells" = n, "Total Clusters" = total_clusters) %>%
-  ggtexttable(rows = NULL, theme = ttheme("light")) -> p1
-
-ggsave(opt$ccplot, p1)
-
-scrna@meta.data %>%
-  dplyr::group_by(orig.ident, get(opt$idents)) %>%
-  dplyr::count() %>%
-  dplyr::select("Sample Name" = 1, "Cluster" = 2, "Total Cells" = 3) %>%
-  ggplot(aes(x = Cluster, y = `Total Cells`, fill = `Sample Name`)) +
-  geom_col() +
-  ggthemes::theme_hc() +
-  theme(legend.title = element_blank()) -> p2
-n <- length(unique(scrna@meta.data[opt$idents]))
+pheatmap(log2(tab + 10), color = colorRampPalette(c("white", "blue"))(101)) -> p1
 
-ggsave(opt$ccbarplot, p2, height = 5, width = 5 + (n * 0.12))
 
 
-ggplotly(p2) -> p1_plotly
+n1 <- length(unique(smObjSCE$seurat_clusters))
+n2 <- length(unique(pred$pruned.labels))
 
-p1_plotly %>% htmlwidgets::saveWidget(file = opt$htmlplot, selfcontained = T)
+ggsave(plot = p1, filename = opt$pheplot, width = 6 + (n1 * 0.10), height = 4 + (n2 * 0.10))
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,29 @@
     type = "character", default = NULL,
     help = "Processed rds file of a Seurat object", metavar = "character"
   ),
   optparse::make_option(c("--microbiome.rds"),
     type = "character", default = NULL,
     help = "Microbiome rds file", metavar = "character"
   ),
-  optparse::make_option(c("--reduction.type"),
-    type = "character", default = "umap",
-    help = "Reduction type, umap or tsne", metavar = "character"
-  ),
-  optparse::make_option(c("--dimplot"),
-    type = "character", default = "micdimplot.pdf",
+  optparse::make_option(c("--sigplot"),
+    type = "character", default = "sigplot.pdf",
     help = "Plot file name", metavar = "character"
   ),
+  optparse::make_option(c("--sigtable"),
+    type = "character", default = NULL,
+    help = "Excel table of positive markers", metavar = "character"
+  ),
   optparse::make_option(c("--taxa"),
     type = "character", default = "genus",
     help = "Taxonomic level", metavar = "character"
+  ),
+  optparse::make_option(c("--idents"),
+    type = "character", default = "seurat_clusters",
+    help = "Meta data column name", metavar = "character"
   )
 )
 
 
 
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
@@ -64,24 +68,38 @@
 AddMetaData(scrna, microbiome %>% rownames_to_column("barcodes") %>% gather(taxa, umi, -barcodes) %>% dplyr::group_by(taxa) %>% dplyr::mutate(sum = sum(umi, na.rm = T)) %>% ungroup() %>%
   dplyr::mutate(taxa = ifelse(sum >= min(sort(unique(sum), decreasing = T)[1:11], na.rm = T), paste0(opt$taxa, "_", taxa), paste0(opt$taxa, "_", "others"))) %>%
   dplyr::select(-sum) %>% dplyr::group_by(barcodes, taxa) %>% dplyr::summarise(sum = sum(umi, na.rm = T)) %>% ungroup() %>% spread(taxa, sum) %>% column_to_rownames("barcodes")) -> scrna
 
 
 # p1 <- DimPlot(scrna, reduction = opt$reduction.type, label = TRUE) & theme_cellsnake_classic() & scale_color_manual(values = palette)
 
-
 scrna %>%
-  dplyr::select(barcodes = .cell, orig.ident, contains(opt$taxa), starts_with(opt$reduction.type)) %>%
+  dplyr::select(one_of(opt$idents), starts_with(opt$taxa)) %>%
   gather(taxa, umi, starts_with(opt$taxa)) %>%
-  dplyr::select(barcodes, orig.ident, x = 3, y = 4, taxa, umi) %>%
-  replace(is.na(.), 0) %>%
-  ggplot(aes(x = x, y = y, color = log(umi + 1))) +
-  geom_point(size = 0.2) +
-  labs(color = "Log-UMI") +
-  theme(axis.text = element_text(size = 12)) +
-  scale_color_viridis(option = "magma", direction = -1, alpha = 0.8, na.value = "white") +
-  # ggthemes::theme_few() +
-  facet_wrap(~taxa) -> p1
+  group_by(across(opt$idents), taxa) %>%
+  dplyr::mutate(total = sum(umi, na.rm = T)) %>%
+  group_by(taxa, across(opt$idents)) %>%
+  dplyr::mutate(cell = n()) %>%
+  dplyr::ungroup() %>%
+  distinct(across(opt$idents), taxa, total, cell) %>%
+  group_by(taxa) %>%
+  dplyr::mutate(v3 = sum(total) - total, v4 = sum(cell) - cell) %>%
+  rowwise() %>%
+  dplyr::mutate(p = fisher.test(matrix(c(total, cell, v3, v4), ncol = 2), alternative = "greater")$p.value) %>%
+  ungroup() %>%
+  dplyr::mutate(p = p.adjust(p)) %>%
+  arrange(p) -> df
+
+
+df %>% ggplot(aes(x = get(opt$idents), y = -log10(p + 1e-200))) +
+  geom_col() +
+  geom_hline(yintercept = -log10(0.05), color = "red") +
+  facet_wrap(~taxa) +
+  theme_bw() +
+  coord_flip() +
+  ylab("Adjusted log P value") +
+  xlab("Identity") -> p1
 
+ggsave(plot = p1, filename = opt$sigplot, width = 12, height = 8)
 
 
-ggsave(plot = p1, filename = opt$dimplot, width = 13, height = 9)
+openxlsx::write.xlsx(df, file = opt$sigtable)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-celltypist.R`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 #!/usr/bin/env Rscript
 
-
 option_list <- list(
-  optparse::make_option(c("--rds"),
-    type = "character", default = NULL,
-    help = "Processed rds file of a Seurat object", metavar = "character"
-  ),
-  optparse::make_option(c("--microbiome.rds"),
-    type = "character", default = NULL,
-    help = "Microbiome rds file", metavar = "character"
-  ),
-  optparse::make_option(c("--sigplot"),
-    type = "character", default = "sigplot.pdf",
-    help = "Plot file name", metavar = "character"
-  ),
-  optparse::make_option(c("--sigtable"),
-    type = "character", default = NULL,
-    help = "Excel table of positive markers", metavar = "character"
-  ),
-  optparse::make_option(c("--taxa"),
-    type = "character", default = "genus",
-    help = "Taxonomic level", metavar = "character"
-  ),
-  optparse::make_option(c("--idents"),
-    type = "character", default = "seurat_clusters",
-    help = "Meta data column name", metavar = "character"
-  )
+      optparse::make_option(c("--sampleid"),
+            type = "character", default = NULL,
+            help = "Sample ID", metavar = "character"
+      ),
+      optparse::make_option(c("--rds"),
+            type = "character", default = NULL,
+            help = "A list of RDS files of Seurat objects", metavar = "character"
+      ),
+      optparse::make_option(c("--csv"),
+            type = "character", default = NULL,
+            help = "Celltypist prediction file", metavar = "character"
+      ),
+      optparse::make_option(c("--output.tsne.plot"),
+            type = "character", default = NULL,
+            help = "Output tsne file name", metavar = "character"
+      ),
+      optparse::make_option(c("--output.umap.plot"),
+            type = "character", default = NULL,
+            help = "Output umap file name", metavar = "character"
+      ),
+      optparse::make_option(c("--percentage"),
+            type = "double", default = 5,
+            help = "Cluster mimnimum percentage to plot", metavar = "double"
+      ), optparse::make_option(c("--labels"), action = "store_true", default = FALSE, help = "Print labels on the plot")
 )
 
-
-
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
-if (is.null(opt$rds)) {
-  optparse::print_help(opt_parser)
-  stop("At least one argument must be supplied (rds file)", call. = FALSE)
+if (is.null(opt$rds) || is.null(opt$csv)) {
+      optparse::print_help(opt_parser)
+      stop("At least one argument must be supplied (rds and sampleid)", call. = FALSE)
 }
 
-require(Seurat)
-# require(randomcoloR)
-require(tidyseurat)
-require(viridis)
+require(patchwork)
 require(tidyverse)
+require(Seurat)
 
-try(
-  {
-    source("workflow/scripts/scrna-functions.R")
-  },
-  silent = TRUE
-)
-try(
-  {
-    source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
-  },
-  silent = TRUE
+
+tryCatch(
+      {
+            source("workflow/scripts/scrna-functions.R")
+      },
+      error = function(cond) {
+            source(paste0(system("python -c 'import os; import cellsnake; print(os.path.dirname(cellsnake.__file__))'", intern = TRUE), "/scrna/workflow/scripts/scrna-functions.R"))
+      }
 )
 
+
 scrna <- readRDS(file = opt$rds)
 DefaultAssay(scrna) <- "RNA"
 
+celltypist <- read.csv(
+      opt$csv,
+      row.names = 1
+)
+
+scrna@meta.data <- scrna@meta.data %>%
+      tibble::rownames_to_column("barcodes") %>%
+      dplyr::left_join(celltypist %>% as.data.frame() %>% rownames_to_column("barcodes"), by = "barcodes") %>%
+      tibble::column_to_rownames("barcodes")
+
+
+n <- length(scrna@meta.data %>% pull(majority_voting) %>% unique())
 
-microbiome <- readRDS(file = opt$microbiome.rds)
+palette <- function_color_palette(n)
+palette <- function_color_palette(n)
+palette <- setNames(palette, scrna@meta.data %>% pull(majority_voting) %>% unique())
 
+breaks <- scrna@meta.data %>%
+      dplyr::select(majority_voting) %>%
+      dplyr::count(majority_voting) %>%
+      dplyr::mutate(perc = (n * 100) / sum(n)) %>%
+      dplyr::filter(perc >= opt$percentage) %>%
+      dplyr::select(-n, -perc) %>%
+      distinct() %>%
+      pull() %>%
+      as.character()
 
+p1 <- DimPlot(scrna, reduction = "tsne", label = opt$labels, group.by = "majority_voting", repel = TRUE) &
+      scale_color_manual(values = palette, breaks = breaks) & theme(plot.title = element_blank()) &
+      theme(legend.direction = "horizontal", legend.text = element_text(size = 7)) &
+      guides(colour = guide_legend(ncol = 2, override.aes = list(size = 7)))
+p2 <- DimPlot(scrna, reduction = "umap", label = opt$labels, group.by = "majority_voting", repel = TRUE) &
+      scale_color_manual(values = palette, breaks = breaks) & theme(plot.title = element_blank()) &
+      theme(legend.direction = "horizontal", legend.text = element_text(size = 7)) &
+      guides(colour = guide_legend(ncol = 2, override.aes = list(size = 7)))
 
-AddMetaData(scrna, microbiome %>% rownames_to_column("barcodes") %>% gather(taxa, umi, -barcodes) %>% dplyr::group_by(taxa) %>% dplyr::mutate(sum = sum(umi, na.rm = T)) %>% ungroup() %>%
-  dplyr::mutate(taxa = ifelse(sum >= min(sort(unique(sum), decreasing = T)[1:11], na.rm = T), paste0(opt$taxa, "_", taxa), paste0(opt$taxa, "_", "others"))) %>%
-  dplyr::select(-sum) %>% dplyr::group_by(barcodes, taxa) %>% dplyr::summarise(sum = sum(umi, na.rm = T)) %>% ungroup() %>% spread(taxa, sum) %>% column_to_rownames("barcodes")) -> scrna
 
+m <- max(str_count(breaks))
 
-# p1 <- DimPlot(scrna, reduction = opt$reduction.type, label = TRUE) & theme_cellsnake_classic() & scale_color_manual(values = palette)
+w <- c(7.5 + (m * 0.08) * (floor(length(breaks) / 11) + 1))
 
-scrna %>%
-  dplyr::select(one_of(opt$idents), starts_with(opt$taxa)) %>%
-  gather(taxa, umi, starts_with(opt$taxa)) %>%
-  group_by(across(opt$idents), taxa) %>%
-  dplyr::mutate(total = sum(umi, na.rm = T)) %>%
-  group_by(taxa, across(opt$idents)) %>%
-  dplyr::mutate(cell = n()) %>%
-  dplyr::ungroup() %>%
-  distinct(across(opt$idents), taxa, total, cell) %>%
-  group_by(taxa) %>%
-  dplyr::mutate(v3 = sum(total) - total, v4 = sum(cell) - cell) %>%
-  rowwise() %>%
-  dplyr::mutate(p = fisher.test(matrix(c(total, cell, v3, v4), ncol = 2), alternative = "greater")$p.value) %>%
-  ungroup() %>%
-  dplyr::mutate(p = p.adjust(p)) %>%
-  arrange(p) -> df
+(p1 / guide_area()) + plot_layout(heights = c(2.5, 1), widths = c(1, 0.6), guides = "collect") -> p1
+(p2 / guide_area()) + plot_layout(heights = c(2.5, 1), widths = c(1, 0.6), guides = "collect") -> p2
 
 
-df %>% ggplot(aes(x = get(opt$idents), y = -log10(p + 1e-200))) +
-  geom_col() +
-  geom_hline(yintercept = -log10(0.05), color = "red") +
-  facet_wrap(~taxa) +
-  theme_bw() +
-  coord_flip() +
-  ylab("Adjusted log P value") +
-  xlab("Identity") -> p1
+ggsave(plot = p1, filename = opt$output.tsne.plot, width = 7.5, height = 8)
+ggsave(plot = p2, filename = opt$output.umap.plot, width = 7.5, height = 8)
 
-ggsave(plot = p1, filename = opt$sigplot, width = 12, height = 8)
 
 
-openxlsx::write.xlsx(df, file = opt$sigtable)
+# saveRDS(scrna,file = opt$output)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-monocle3.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-monocle3.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-read-qc.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-read-qc.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R`

 * *Files 3% similar despite different names*

```diff
@@ -114,8 +114,10 @@
     }
 }
 
 
 
 function_subset_by_idents(scrna, opt) -> scrna
 
-head(scrna)
+head(scrna)
+
+saveRDS(scrna, file = opt$output.rds)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-technicals.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-technicals.R`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,22 @@
   optparse::make_option(c("--fplot"),
     type = "character", default = NULL,
     help = "nFeature plot", metavar = "character"
   ),
   optparse::make_option(c("--cplot"),
     type = "character", default = NULL,
     help = "nCount plot", metavar = "character"
+  ),
+  optparse::make_option(c("--mtplot"),
+    type = "character", default = NULL,
+    help = "Percent MT plot", metavar = "character"
+  ),
+  optparse::make_option(c("--rpplot"),
+    type = "character", default = NULL,
+    help = "Ribo plot", metavar = "character"
   )
 )
 
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
 if (is.null(opt$rds)) {
@@ -40,8 +48,17 @@
 
 ggsave(opt$fplot, width = 7, height = 5)
 
 
 
 FeaturePlot(scrna, features = "nCount_RNA", pt.size = 0.1)
 
-ggsave(opt$cplot, width = 7, height = 5)
+ggsave(opt$cplot, width = 7, height = 5)
+
+
+FeaturePlot(scrna, features = "percent.mt", pt.size = 0.1)
+
+ggsave(opt$mtplot, width = 7, height = 5)
+
+FeaturePlot(scrna, features = "percent.rp", pt.size = 0.1)
+
+ggsave(opt$rpplot, width = 7, height = 5)
```

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake/scrna/workflow/scripts/scrna-volcano.R` & `cellsnake-0.2.0rc2/cellsnake/scrna/workflow/scripts/scrna-volcano.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/cellsnake.egg-info/SOURCES.txt` & `cellsnake-0.2.0rc2/cellsnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev9/setup.py` & `cellsnake-0.2.0rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 with open("README.md","r") as readme:
     long_description=readme.read()
 
 setup(
     name="cellsnake",
-    version="0.2.0.dev9",
+    version="0.2.0.rc2",
     packages=find_packages(exclude=('tests*','testing*')),
     long_description=long_description,
     long_description_content_type="text/markdown",
     #extras_require={"dev":["pytest>=3.7"]},
     install_requires=requirements,
     include_package_data=True,
     zip_safe=False,
```

### Comparing `cellsnake-0.2.0.dev9/test_counts.txt` & `cellsnake-0.2.0rc2/test_counts.txt`

 * *Files identical despite different names*


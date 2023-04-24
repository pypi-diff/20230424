# Comparing `tmp/spacemake-0.7.tar.gz` & `tmp/spacemake-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacemake-0.7.tar", last modified: Fri Dec  2 12:48:20 2022, max compression
+gzip compressed data, was "spacemake-0.7.2.tar", last modified: Mon Apr 24 14:20:29 2023, max compression
```

## Comparing `spacemake-0.7.tar` & `spacemake-0.7.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      137 2022-12-02 12:46:36.000000 spacemake-0.7/.readthedocs.yaml
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18092 2022-12-02 12:46:36.000000 spacemake-0.7/COPYING
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      957 2022-12-02 12:46:36.000000 spacemake-0.7/LICENSE
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       49 2022-12-02 12:46:36.000000 spacemake-0.7/MANIFEST.in
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1350 2022-12-02 12:48:20.781468 spacemake-0.7/PKG-INFO
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      648 2022-12-02 12:46:36.000000 spacemake-0.7/README.md
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.777468 spacemake-0.7/docs/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      919 2022-12-02 12:46:36.000000 spacemake-0.7/docs/conf.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      846 2022-12-02 12:46:37.000000 spacemake-0.7/environment.yaml
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      103 2022-12-02 12:46:37.000000 spacemake-0.7/pyproject.toml
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1212 2022-12-02 12:48:20.781468 spacemake-0.7/setup.cfg
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       73 2022-12-02 12:46:37.000000 spacemake-0.7/setup.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.777468 spacemake-0.7/spacemake/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      106 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/__init__.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    16898 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/alnstats.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18300 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/annotator.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    27708 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/config.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    20173 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/cutadapt_bam.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.777468 spacemake-0.7/spacemake/data/
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/data/config/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2506 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/config/config.yaml
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3702 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/config/longread.yaml
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      521 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/config/species_data_url.yaml
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/data/test/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    38033 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/test/test_bc1.csv
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    38075 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/test/test_bc2.csv
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)   190098 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/data/visium_barcode_positions.csv
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5254 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/errors.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/longread/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       93 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/__main__.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18801 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/annotation.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15747 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/cache.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    24586 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/cmdline.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7983 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/overview.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15423 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/report.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5084 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/longread/signature.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     4452 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/parallel.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/preprocess/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      230 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/preprocess/__init__.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1029 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/preprocess/cmdline.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7954 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/preprocess/dge.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    36757 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/preprocess/fastq.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    58232 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/project_df.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    25587 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/quant.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5434 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/reporting.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    19939 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/smk.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/snakemake/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/__init__.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2659 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/downsample.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1578 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/dropseq.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     6847 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/longread.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    22128 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/main.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    20410 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/mapping.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1932 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/merge_samples.smk
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/snakemake/scripts/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3020 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/automated_analysis.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3373 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/automated_analysis_create_processed_data_files.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15435 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/automated_analysis_create_report.Rmd
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1208 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/clean_top_barcodes.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1436 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/create_sample_db.R
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7970 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/create_sample_overview.Rmd
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1014 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/create_spatial_dge.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2750 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/filter_mm_reads.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2058 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/fix_bam_header.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1746 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/kmer_stats_from_fastq.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1853 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/parse_ribo_log.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    25363 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/qc_sequencing_create_sheet.Rmd
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    11334 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/saturation_analysis.Rmd
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      401 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/shared_functions.R
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    24306 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/snakemake_helper_functions.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3770 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/splice_bam_header.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2812 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/scripts/split_reads_by_strand_info.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1013 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/species_init.smk
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     8484 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/variables.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2470 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/snakemake/visium.smk
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.781468 spacemake-0.7/spacemake/spatial/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      282 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/spatial/__init__.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3164 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/spatial/cmdline.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    21700 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/spatial/he_integration.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    12290 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/spatial/novosparc_integration.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    16500 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/spatial/util.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     9753 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/tag_alignments.py
--rwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)     8822 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/unittests.py
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7417 2022-12-02 12:46:37.000000 spacemake-0.7/spacemake/util.py
-drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2022-12-02 12:48:20.777468 spacemake-0.7/spacemake.egg-info/
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1350 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/PKG-INFO
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2593 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/SOURCES.txt
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        1 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/dependency_links.txt
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      181 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/entry_points.txt
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        1 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/not-zip-safe
--rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       10 2022-12-02 12:48:20.000000 spacemake-0.7/spacemake.egg-info/top_level.txt
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.518967 spacemake-0.7.2/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      137 2023-04-24 14:18:16.000000 spacemake-0.7.2/.readthedocs.yaml
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18092 2023-04-24 14:18:16.000000 spacemake-0.7.2/COPYING
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      957 2023-04-24 14:18:16.000000 spacemake-0.7.2/LICENSE
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       49 2023-04-24 14:18:16.000000 spacemake-0.7.2/MANIFEST.in
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2291 2023-04-24 14:20:29.518967 spacemake-0.7.2/PKG-INFO
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1587 2023-04-24 14:18:16.000000 spacemake-0.7.2/README.md
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.510967 spacemake-0.7.2/docs/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      919 2023-04-24 14:18:16.000000 spacemake-0.7.2/docs/conf.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      854 2023-04-24 14:18:17.000000 spacemake-0.7.2/environment.yaml
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      103 2023-04-24 14:18:17.000000 spacemake-0.7.2/pyproject.toml
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1214 2023-04-24 14:20:29.518967 spacemake-0.7.2/setup.cfg
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       73 2023-04-24 14:18:17.000000 spacemake-0.7.2/setup.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.510967 spacemake-0.7.2/spacemake/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      106 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/__init__.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    16898 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/alnstats.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18300 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/annotator.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    28353 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/config.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    20173 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/cutadapt_bam.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/data/
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/data/config/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2431 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/config/config.yaml
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3702 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/config/longread.yaml
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      521 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/config/species_data_url.yaml
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/data/test/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    38033 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/test/test_bc1.csv
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    38075 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/test/test_bc2.csv
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)   190098 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/data/visium_barcode_positions.csv
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5254 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/errors.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/longread/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       93 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/__main__.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18801 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/annotation.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15747 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/cache.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    24586 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/cmdline.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7983 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/overview.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15423 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/report.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5084 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/longread/signature.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     4452 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/parallel.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/preprocess/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      230 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/preprocess/__init__.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1029 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/preprocess/cmdline.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7954 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/preprocess/dge.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    36757 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/preprocess/fastq.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    58232 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/project_df.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    25587 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/quant.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     5434 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/reporting.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    19939 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/smk.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/snakemake/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/__init__.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2659 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/downsample.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1578 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/dropseq.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     6847 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/longread.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    22128 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/main.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    20410 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/mapping.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1932 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/merge_samples.smk
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake/snakemake/scripts/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3020 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3373 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis_create_processed_data_files.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    15435 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis_create_report.Rmd
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1208 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/clean_top_barcodes.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1436 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/create_sample_db.R
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7970 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/create_sample_overview.Rmd
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1014 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/create_spatial_dge.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2750 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/filter_mm_reads.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2058 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/fix_bam_header.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1746 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/kmer_stats_from_fastq.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1853 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/parse_ribo_log.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    25363 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/qc_sequencing_create_sheet.Rmd
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    11334 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/saturation_analysis.Rmd
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      401 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/shared_functions.R
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    24305 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/snakemake_helper_functions.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3770 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/splice_bam_header.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2812 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/scripts/split_reads_by_strand_info.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     1013 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/species_init.smk
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     8484 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/variables.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2470 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/snakemake/visium.smk
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.518967 spacemake-0.7.2/spacemake/spatial/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      282 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/spatial/__init__.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     3164 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/spatial/cmdline.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    21700 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/spatial/he_integration.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    12290 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/spatial/novosparc_integration.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)    18051 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/spatial/util.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     9753 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/tag_alignments.py
+-rwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)     8822 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/unittests.py
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     7417 2023-04-24 14:18:17.000000 spacemake-0.7.2/spacemake/util.py
+drwxr-xr-x   0 nkarais  (23074) nkarais_usr (23074)        0 2023-04-24 14:20:29.514967 spacemake-0.7.2/spacemake.egg-info/
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2291 2023-04-24 14:20:29.000000 spacemake-0.7.2/spacemake.egg-info/PKG-INFO
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)     2593 2023-04-24 14:20:29.000000 spacemake-0.7.2/spacemake.egg-info/SOURCES.txt
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        1 2023-04-24 14:20:29.000000 spacemake-0.7.2/spacemake.egg-info/dependency_links.txt
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)      181 2023-04-24 14:20:29.000000 spacemake-0.7.2/spacemake.egg-info/entry_points.txt
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)        1 2023-04-24 14:19:52.000000 spacemake-0.7.2/spacemake.egg-info/not-zip-safe
+-rw-r--r--   0 nkarais  (23074) nkarais_usr (23074)       10 2023-04-24 14:20:29.000000 spacemake-0.7.2/spacemake.egg-info/top_level.txt
```

### Comparing `spacemake-0.7/COPYING` & `spacemake-0.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/LICENSE` & `spacemake-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/docs/conf.py` & `spacemake-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/environment.yaml` & `spacemake-0.7.2/environment.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     - r-hexbin
     - r-scales
     - pysam>=0.16.0.1
     - pot
     - openjdk==11.0.15
     - pigz
     - pip:
-        - pandas>=1.3.0
+        - pandas>=1.3.0,<=1.5.1
         - scanpy>=1.8.1
         - leidenalg>=0.8.1
         - numpy>=1.18.1
         - more-itertools>=8.7.0
         - biopython>=1.78
         - scipy>=1.5.0
         - scikit-misc>=0.1.3
```

### Comparing `spacemake-0.7/setup.cfg` & `spacemake-0.7.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spacemake
-version = 0.7
+version = 0.7.2
 author = Tamas Ryszard Sztanka-Toth, Marvin Jens, Nikos Karaiskos, Nikolaus Rajewsky
 author_email = TamasRyszard.Sztanka-Toth@mdc-berlin.de
 description = A bioinformatic pipeline for the analysis of spatial transcriptomic data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rajewsky-lab/spacemake
 project_urls =
```

### Comparing `spacemake-0.7/spacemake/alnstats.py` & `spacemake-0.7.2/spacemake/alnstats.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/annotator.py` & `spacemake-0.7.2/spacemake/annotator.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/config.py` & `spacemake-0.7.2/spacemake/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,22 +72,22 @@
         choices=bool_in_str,
         type=str,
         help="By default only beads having at least umi_cutoff UMI counts are analysed "
         + "during the automated analysis, all other beads are filtered out. If this "
         + "parameter is set, contiguous islands within umi_cutoff passing beads will "
         + "also be included in the analysis",
     )
-    parser.add_argument(
-        "--polyA_adapter_trimming",
-        required=False,
-        choices=bool_in_str,
-        type=str,
-        help="if set, reads will have polyA stretches and adapter sequence overlaps trimmed "
-        + "BEFORE mapping.",
-    )
+    # parser.add_argument(
+    #     "--polyA_adapter_trimming",
+    #     required=False,
+    #     choices=bool_in_str,
+    #     type=str,
+    #     help="if set, reads will have polyA stretches and adapter sequence overlaps trimmed "
+    #     + "BEFORE mapping.",
+    # )
     parser.add_argument(
         "--count_intronic_reads",
         required=False,
         choices=bool_in_str,
         type=str,
         help="if set, INTRONIC reads will also be countsed (apart from UTR and CDS)",
     )
@@ -577,14 +577,26 @@
         # correct run modes
         for run_mode_name, run_mode_variables in self.variables["run_modes"].items():
             variables = run_mode_variables.copy()
             for var in run_mode_variables:
                 if not var in RunMode.variable_types:
                     del variables[var]
 
+            if ("polyA_adapter_trimming" in variables) and (
+                variables["polyA_adapter_trimming"] == False
+            ):
+                import logging
+
+                logger = logging.getLogger("spacemake.config")
+                logger.warning(
+                    f"WARNING: run_mode {run_mode_name} lists polyA_adapter_trimming=false. This is no longer supported and will be overriden with true"
+                )
+                variables["polyA_adapter_trimming"] = True
+
+            # print(f"assigning run mode {run_mode_name}: {variables}")
             self.variables["run_modes"][run_mode_name] = variables
 
     def dump(self):
         with open(self.file_path, "w") as fo:
             fo.write(yaml.dump(self.variables))
 
     def set_file_path(self, file_path):
@@ -719,15 +731,15 @@
 
     def add_variable(self, variable, name, **kwargs):
         kwargs["name"] = name
         # It's not very clear that a cmdline arg
         # --name is absolutely REQUIRED and its value has to map somehow onto
         # an internal function name
         # @TAMAS: can you help?
-        print(f"add_variable() called with variable={variable} name={name} kw={kwargs}")
+        # print(f"add_variable() called with variable={variable} name={name} kw={kwargs}")
 
         if variable == "species":
             # for the species command, collision check is on the reference name, not the species name
             if "genome" in kwargs:
                 # deprecated cmdline option --genome ... was used. Translate to
                 # --sequence ... --reference=genome
                 kwargs["sequence"] = kwargs["genome"]
@@ -765,14 +777,15 @@
                 variable = variable[:-1]
 
             raise ConfigVariableNotFoundError(variable, name)
 
         return variable_data
 
     def get_variable(self, variable, name):
+        # print(f"config.get_variable({variable}, {name})")
         if not self.variable_exists(variable, name):
             raise ConfigVariableNotFoundError(variable, name)
         else:
             return self.variables[variable][name]
 
     def get_run_mode(self, name):
         # first load the default values
```

### Comparing `spacemake-0.7/spacemake/cutadapt_bam.py` & `spacemake-0.7.2/spacemake/cutadapt_bam.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/data/config/config.yaml` & `spacemake-0.7.2/spacemake/data/config/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -31,27 +31,25 @@
         mesh_spot_diameter_um: 55
         mesh_spot_distance_um: 100
     visium:
         n_beads: 10000
         umi_cutoff: [1000]
         clean_dge: False
         detect_tissue: True
-        polyA_adapter_trimming: False
         count_intronic_reads: False
         count_mm_reads: True
     slide_seq:
         n_beads: 100000
         umi_cutoff: [50]
         clean_dge: False
         detect_tissue: False
     scRNA_seq:
         n_beads: 10000
         umi_cutoff: [500]
         detect_tissue: False
-        polyA_adapter_trimming: True
         count_intronic_reads: True
         count_mm_reads: False
     seq_scope:
         clean_dge: false
         count_intronic_reads: false
         count_mm_reads: false
         detect_tissue: false
```

### Comparing `spacemake-0.7/spacemake/data/config/longread.yaml` & `spacemake-0.7.2/spacemake/data/config/longread.yaml`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/data/config/species_data_url.yaml` & `spacemake-0.7.2/spacemake/data/config/species_data_url.yaml`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/data/test/test_bc1.csv` & `spacemake-0.7.2/spacemake/data/test/test_bc1.csv`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/data/test/test_bc2.csv` & `spacemake-0.7.2/spacemake/data/test/test_bc2.csv`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/data/visium_barcode_positions.csv` & `spacemake-0.7.2/spacemake/data/visium_barcode_positions.csv`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/errors.py` & `spacemake-0.7.2/spacemake/errors.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/annotation.py` & `spacemake-0.7.2/spacemake/longread/annotation.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/cache.py` & `spacemake-0.7.2/spacemake/longread/cache.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/cmdline.py` & `spacemake-0.7.2/spacemake/longread/cmdline.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/overview.py` & `spacemake-0.7.2/spacemake/longread/overview.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/report.py` & `spacemake-0.7.2/spacemake/longread/report.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/longread/signature.py` & `spacemake-0.7.2/spacemake/longread/signature.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/parallel.py` & `spacemake-0.7.2/spacemake/parallel.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/preprocess/cmdline.py` & `spacemake-0.7.2/spacemake/preprocess/cmdline.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/preprocess/dge.py` & `spacemake-0.7.2/spacemake/preprocess/dge.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/preprocess/fastq.py` & `spacemake-0.7.2/spacemake/preprocess/fastq.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/project_df.py` & `spacemake-0.7.2/spacemake/project_df.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/quant.py` & `spacemake-0.7.2/spacemake/quant.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/reporting.py` & `spacemake-0.7.2/spacemake/reporting.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/smk.py` & `spacemake-0.7.2/spacemake/smk.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/downsample.smk` & `spacemake-0.7.2/spacemake/snakemake/downsample.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/dropseq.smk` & `spacemake-0.7.2/spacemake/snakemake/dropseq.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/longread.smk` & `spacemake-0.7.2/spacemake/snakemake/longread.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/main.smk` & `spacemake-0.7.2/spacemake/snakemake/main.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/mapping.smk` & `spacemake-0.7.2/spacemake/snakemake/mapping.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/merge_samples.smk` & `spacemake-0.7.2/spacemake/snakemake/merge_samples.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/automated_analysis.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/automated_analysis_create_processed_data_files.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis_create_processed_data_files.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/automated_analysis_create_report.Rmd` & `spacemake-0.7.2/spacemake/snakemake/scripts/automated_analysis_create_report.Rmd`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/clean_top_barcodes.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/clean_top_barcodes.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/create_sample_db.R` & `spacemake-0.7.2/spacemake/snakemake/scripts/create_sample_db.R`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/create_sample_overview.Rmd` & `spacemake-0.7.2/spacemake/snakemake/scripts/create_sample_overview.Rmd`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/create_spatial_dge.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/create_spatial_dge.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/filter_mm_reads.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/filter_mm_reads.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/fix_bam_header.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/fix_bam_header.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/kmer_stats_from_fastq.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/kmer_stats_from_fastq.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/parse_ribo_log.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/parse_ribo_log.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/qc_sequencing_create_sheet.Rmd` & `spacemake-0.7.2/spacemake/snakemake/scripts/qc_sequencing_create_sheet.Rmd`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/saturation_analysis.Rmd` & `spacemake-0.7.2/spacemake/snakemake/scripts/saturation_analysis.Rmd`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/snakemake_helper_functions.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/snakemake_helper_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         ][0]
 
         if non_spatial_pbf_id not in puck_barcode_file_ids:
             puck_barcode_file_ids.append(non_spatial_pbf_id)
 
         for run_mode in row["run_mode"]:
             run_mode_variables = project_df.config.get_run_mode(run_mode).variables
-
             if "polyA_adapter_trimmed" in kwargs:
                 polyA_adapter_trimmed = kwargs["polyA_adapter_trimmed"]
             else:
                 if run_mode_variables["polyA_adapter_trimming"]:
                     polyA_adapter_trimmed = ".polyA_adapter_trimmed"
                 else:
                     polyA_adapter_trimmed = ""
```

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/splice_bam_header.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/splice_bam_header.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/scripts/split_reads_by_strand_info.py` & `spacemake-0.7.2/spacemake/snakemake/scripts/split_reads_by_strand_info.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/species_init.smk` & `spacemake-0.7.2/spacemake/snakemake/species_init.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/variables.py` & `spacemake-0.7.2/spacemake/snakemake/variables.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/snakemake/visium.smk` & `spacemake-0.7.2/spacemake/snakemake/visium.smk`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/spatial/cmdline.py` & `spacemake-0.7.2/spacemake/spatial/cmdline.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/spatial/he_integration.py` & `spacemake-0.7.2/spacemake/spatial/he_integration.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/spatial/novosparc_integration.py` & `spacemake-0.7.2/spacemake/spatial/novosparc_integration.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/spatial/util.py` & `spacemake-0.7.2/spacemake/spatial/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 from anndata import AnnData
 from spacemake.preprocess import calculate_adata_metrics
 
+
 def compute_neighbors(adata, min_dist=None, max_dist=None):
-    '''Compute all direct neighbors of all spots in the adata. Currently
+    """Compute all direct neighbors of all spots in the adata. Currently
         tailored for 10X Visium.
     Args:
         adata: an AnnData object
         min_dist: int, minimum distance to consider neighbors
         max_dist: int, maximum distance to consider neighbors
     Returns:
         neighbors: a dictionary holding the spot IDs for every spot
-    '''
+    """
     import numpy as np
     from scipy.spatial.distance import cdist
 
     # Calculate all Euclidean distances on the adata
-    dist_mtrx = cdist(adata.obsm['spatial'],
-                      adata.obsm['spatial'])
+    dist_mtrx = cdist(adata.obsm["spatial"], adata.obsm["spatial"])
     neighbors = dict()
 
     for i in range(adata.obs.shape[0]):
-        neighbors[i] = np.where((dist_mtrx[i,:] > min_dist) & (dist_mtrx[i,:] < max_dist))[0]
+        neighbors[i] = np.where(
+            (dist_mtrx[i, :] > min_dist) & (dist_mtrx[i, :] < max_dist)
+        )[0]
 
     return neighbors
 
+
 def compute_islands(adata, min_umi):
-    '''Find contiguity islands
+    """Find contiguity islands
 
     Args:
         adata: an AnnData object
         cluster: a cell type label to compute the islands for
     Returns:
         islands: A list of lists of spots forming contiguity islands
-    '''
+    """
     import numpy as np
     import itertools
 
     # this is hard coded for now for visium, to have 6 neighbors per spot
-    # TODO: define an iterative approach where the key is to have around 6 
+    # TODO: define an iterative approach where the key is to have around 6
     # neighbors per spot on average
-    neighbors = compute_neighbors(adata, min_dist = 0, max_dist=3)
-    spots_cluster = np.where(np.array(adata.obs['total_counts']) < min_umi)[0]
+    neighbors = compute_neighbors(adata, min_dist=0, max_dist=3)
+    spots_cluster = np.where(np.array(adata.obs["total_counts"]) < min_umi)[0]
 
     # create a new dict holding only neighbors of the cluster
     islands = []
 
     for spot in neighbors:
         if spot not in spots_cluster:
             continue
         islands.append({spot}.union({x for x in neighbors[spot] if x in spots_cluster}))
 
     # merge islands with common spots
-    island_spots = set(itertools.chain.from_iterable(islands)) 
+    island_spots = set(itertools.chain.from_iterable(islands))
 
     for each in island_spots:
         components = [x for x in islands if each in x]
         for i in components:
             islands.remove(i)
         islands += [list(set(itertools.chain.from_iterable(components)))]
 
     return islands
 
+
 def nonsingular(vmin, vmax, expander=0.001, tiny=1e-15, increasing=True):
     """
     Modify the endpoints of a range as needed to avoid singularities.
 
     This code was adapted from matplotlib.transforms
     "Copyright (c) 2012- Matplotlib Development Team; All Rights Reserved"
 
     Args
         vmin, vmax: float, the initial endpoints.
-        expander: float, default: 0.001, fractional amount by which *vmin* and 
+        expander: float, default: 0.001, fractional amount by which *vmin* and
                   *vmax* are expanded if the original interval is too small,
                   based on *tiny*.
-        tiny : float, default: 1e-15, hreshold for the ratio of the interval to 
-            the maximum absolute value of its endpoints. 
-            If the interval is smaller than this, it will be expanded. 
-            This value should be around 1e-15 or larger; 
+        tiny : float, default: 1e-15, hreshold for the ratio of the interval to
+            the maximum absolute value of its endpoints.
+            If the interval is smaller than this, it will be expanded.
+            This value should be around 1e-15 or larger;
             otherwise the interval will be approaching the double precision
             resolution limit.
         increasing: bool, default: True, if True, swap *vmin*, *vmax* if *vmin* > *vmax*.
     Returns:
         vmin, vmax: float, endpoints, expanded and/or swapped if necessary.
                     If either input is inf or NaN, or if both inputs are 0 or very
                     close to zero, it returns -*expander*, *expander*.
@@ -103,93 +107,90 @@
         vmax = expander
 
     elif vmax - vmin <= maxabsvalue * tiny:
         if vmax == 0 and vmin == 0:
             vmin = -expander
             vmax = expander
         else:
-            vmin -= expander*abs(vmin)
-            vmax += expander*abs(vmax)
+            vmin -= expander * abs(vmin)
+            vmax += expander * abs(vmax)
 
     if swapped and not increasing:
         vmin, vmax = vmax, vmin
     return vmin, vmax
 
+
 def detect_tissue(adata, min_umi):
-    ''' Detect tissue: first find beads with at least min_umi UMIs, then detect island in the rest
-    
+    """Detect tissue: first find beads with at least min_umi UMIs, then detect island in the rest
+
     Args
         adata: an AnnData object, with spatial coordinates
         min_umi: integer, the min umi to be assigned as tissue bead by default
     Returns:
         tissue_indices: a list of indices which should be kept for this AnnData object
-    '''
+    """
     import numpy as np
 
     islands = compute_islands(adata, min_umi)
 
     # find the sizes of the islands. remove the biggest, as either the tissue has a big hole in it
     # or there are not so many big islands in which case removal is OK.
     # to be evaluated later...
     island_sizes = [len(island) for island in islands]
 
     tissue_islands = np.delete(islands, np.argmax(island_sizes))
 
     # get the indices of the islands
-    tissue_indices = np.where(np.array(adata.obs['total_counts']) >= min_umi)[0]
+    tissue_indices = np.where(np.array(adata.obs["total_counts"]) >= min_umi)[0]
 
     tissue_indices = np.append(tissue_indices, np.hstack(tissue_islands))
 
     adata = adata[tissue_indices, :]
 
     return adata
 
-def create_mesh(
-    width,
-    height,
-    diameter,
-    distance,
-    push_x = 0,
-    push_y = 0):
+
+def create_mesh(width, height, diameter, distance, push_x=0, push_y=0):
     import numpy as np
 
     distance_y = np.sqrt(3) * distance
-    
+
     x_coord = np.arange(push_x, width + diameter, distance)
     y_coord = np.arange(push_y, height + diameter, distance_y)
-    
+
     X, Y = np.meshgrid(x_coord, y_coord)
     xy = np.vstack((X.flatten(), Y.flatten())).T
-    
+
     return xy
 
+
 def binning_hexagon(x, y, gridsize, extent=None, last_row=False):
-    ''' Bins x,y points into a mesh of gridsize (across x axis, or xy axes). 
+    """Bins x,y points into a mesh of gridsize (across x axis, or xy axes).
     Points are assigned to the closest hexagon, without explicitly calculating
     pairwise distances.
-    
+
     Does not require to create a mesh beforehand, this function handles the
     mesh and nearest neighbor.
 
     This code was adapted from matplotlib
     "Copyright (c) 2012- Matplotlib Development Team; All Rights Reserved"
-    
+
     Args
         x, y: numpy.ndarray, x, y spatial coordinates of points
         gridsize: float or tuple, the amount of hexagons in x direction (float);
                   y direction is automatically computed; or specified if gridsize is
                   a tuple.
         extent: tuple, of (x_min, x_max, y_min, y_max)
         last_row: bool, whether a last row is created in mesh or not
     Returns:
         coordinates: numpy.ndarray, a (x_mesh x y_mesh) x 2 matrix, with the coordinates
                      (centres) of each hexagon in the binned mesh
         accumulated: list, contains the indices from the x, y arrays that were binned
                      to each hexagon in the mesh.
-    '''
+    """
     import numpy as np
 
     if np.iterable(gridsize):
         nx, ny = gridsize
     else:
         nx = gridsize
         ny = int(nx / np.sqrt(3))
@@ -218,87 +219,177 @@
         ny1 = ny
     nx2 = nx
     ny2 = ny
     n = nx1 * ny1 + nx2 * ny2
 
     # In the x-direction, the hexagons exactly cover the region from
     # xmin to xmax. Need some padding to avoid roundoff errors.
-    padding = 1.e-9 * (xmax - xmin)
+    padding = 1.0e-9 * (xmax - xmin)
     xmin -= padding
     xmax += padding
     sx = (xmax - xmin) / nx
     sy = (ymax - ymin) / ny
 
     # Positions in hexagon index coordinates.
     ix = (tx - xmin) / sx
     iy = (ty - ymin) / sy
     ix1 = np.round(ix).astype(int)
     iy1 = np.round(iy).astype(int)
     ix2 = np.floor(ix).astype(int)
     iy2 = np.floor(iy).astype(int)
 
     # flat indices, plus one so that out-of-range points go to position 0.
-    i1 = np.where((0 <= ix1) & (ix1 < nx1) & (0 <= iy1) & (iy1 < ny1),
-                    ix1 * ny1 + iy1 + 1, 0)
-    i2 = np.where((0 <= ix2) & (ix2 < nx2) & (0 <= iy2) & (iy2 < ny2),
-                    ix2 * ny2 + iy2 + 1, 0)
+    i1 = np.where(
+        (0 <= ix1) & (ix1 < nx1) & (0 <= iy1) & (iy1 < ny1), ix1 * ny1 + iy1 + 1, 0
+    )
+    i2 = np.where(
+        (0 <= ix2) & (ix2 < nx2) & (0 <= iy2) & (iy2 < ny2), ix2 * ny2 + iy2 + 1, 0
+    )
 
     d1 = (ix - ix1) ** 2 + 3.0 * (iy - iy1) ** 2
     d2 = (ix - ix2 - 0.5) ** 2 + 3.0 * (iy - iy2 - 0.5) ** 2
-    bdist = (d1 < d2)
+    bdist = d1 < d2
 
     Cs_at_i1 = [[] for _ in range(1 + nx1 * ny1)]
     Cs_at_i2 = [[] for _ in range(1 + nx2 * ny2)]
     for i in range(len(x)):
         if bdist[i]:
             Cs_at_i1[i1[i]].append(i)
         else:
             Cs_at_i2[i2[i]].append(i)
 
-    accumulated = [acc
-                   for Cs_at_i in [Cs_at_i1, Cs_at_i2]
-                   for acc in Cs_at_i[1:]]
+    accumulated = [acc for Cs_at_i in [Cs_at_i1, Cs_at_i2] for acc in Cs_at_i[1:]]
 
     coordinates = np.zeros((n, 2), float)
-    coordinates[:nx1 * ny1, 0] = np.repeat(np.arange(nx1), ny1)
-    coordinates[:nx1 * ny1, 1] = np.tile(np.arange(ny1), nx1)
-    coordinates[nx1 * ny1:, 0] = np.repeat(np.arange(nx2) + 0.5, ny2)
-    coordinates[nx1 * ny1:, 1] = np.tile(np.arange(ny2), nx2) + 0.5
+    coordinates[: nx1 * ny1, 0] = np.repeat(np.arange(nx1), ny1)
+    coordinates[: nx1 * ny1, 1] = np.tile(np.arange(ny1), nx1)
+    coordinates[nx1 * ny1 :, 0] = np.repeat(np.arange(nx2) + 0.5, ny2)
+    coordinates[nx1 * ny1 :, 1] = np.tile(np.arange(ny2), nx2) + 0.5
     coordinates[:, 0] *= sx
     coordinates[:, 1] *= sy
     coordinates[:, 0] += xmin
     coordinates[:, 1] += ymin
 
     return coordinates, accumulated
 
-def create_meshed_adata(adata,
-        px_by_um,
-        spot_diameter_um = 55,
-        spot_distance_um = 100,
-        bead_diameter_um = 10,
-        mesh_type = 'circle',
-        start_at_minimum=False,
-        optimized_binning=True
-    ):
+
+def aggregate_adata_by_indices(
+    adata, idx_to_aggregate, idx_aggregated, coordinates_aggregated
+):
     import pandas as pd
-    import scanpy as sc
     import numpy as np
     import anndata
 
+    from scipy.sparse import csr_matrix, csc_matrix, vstack, dok_matrix
+
+    joined_C = adata.X[idx_to_aggregate]
+
+    # at which indices does the index in the newly created matrix change
+    change_ix = np.where(idx_aggregated[:-1] != idx_aggregated[1:])[0] + 1
+
+    # array of indices, split by which row they should go together
+
+    ix_array = np.asarray(
+        np.split(np.arange(idx_aggregated.shape[0]), change_ix, axis=0), dtype="object"
+    )
+
+    joined_C_sumed = vstack(
+        [
+            csr_matrix(joined_C[ix_array[n].astype(int), :].sum(0))
+            for n in range(len(ix_array))
+        ]
+    )
+
+    aggregated_adata = anndata.AnnData(
+        csc_matrix(joined_C_sumed),
+        obs=pd.DataFrame(
+            {
+                "x_pos": coordinates_aggregated[:, 0],
+                "y_pos": coordinates_aggregated[:, 1],
+            }
+        ),
+        var=adata.var,
+    )
+
+    aggregated_adata.obsm["spatial"] = coordinates_aggregated
+
+    # rename index
+    aggregated_adata.obs.index.name = "cell_bc"
+
+    def summarise_adata_obs_column(adata, column, summary_fun=sum):
+        vals_to_join = adata.obs[column].to_numpy()[idx_to_aggregate]
+        vals_joined = np.array(
+            [
+                summary_fun(vals_to_join[ix_array[n].astype(int)])
+                for n in range(len(ix_array))
+            ]
+        )
+        return vals_joined
+
+    print(adata)
+
+    # summarise and attach n_reads, calculate metrics (incl. pcr)
+    calculate_adata_metrics(
+        aggregated_adata,
+        # provide the n_reads as a parameter
+        n_reads=summarise_adata_obs_column(adata, "n_reads"),
+    )
+
+    aggregated_adata.obs["n_joined"] = [len(x) for x in ix_array]
+    
+    mesh_bc_ilocs = np.arange(len(idx_to_aggregate))[idx_to_aggregate]
+
+    joined_dict = {i: mesh_bc_ilocs[x] for i, x in enumerate(ix_array)}
+
+    indices_joined_spatial_units = dok_matrix(
+        (len(joined_dict), len(adata.obs_names)), dtype=np.int8
+    )
+
+    for obs_name_aggregate, obs_name_to_aggregate in joined_dict.items():
+        indices_joined_spatial_units[obs_name_aggregate, obs_name_to_aggregate] = 1
+
+    indices_joined_spatial_units = indices_joined_spatial_units.tocsr()
+    aggregated_adata.uns["spatial_units_obs_names"] = np.array(adata.obs_names)
+    aggregated_adata.uns["indices_joined_spatial_units"] = indices_joined_spatial_units
+
+    from statistics import mean
+
+    for column in [
+        "exact_entropy",
+        "theoretical_entropy",
+        "exact_compression",
+        "theoretical_compression",
+    ]:
+        aggregated_adata.obs[column] = summarise_adata_obs_column(adata, column, mean)
+
+    return aggregated_adata
+
+
+def create_meshed_adata(
+    adata,
+    px_by_um,
+    spot_diameter_um=55,
+    spot_distance_um=100,
+    bead_diameter_um=10,
+    mesh_type="circle",
+    start_at_minimum=False,
+    optimized_binning=True,
+):
+    import numpy as np
+
     from sklearn.metrics.pairwise import euclidean_distances
-    from scipy.sparse import csr_matrix, csc_matrix, vstack
 
-    if not mesh_type in ['circle', 'hexagon']:
-        raise ValueError(f'unrecognised mesh type {mesh_type}')
+    if not mesh_type in ["circle", "hexagon"]:
+        raise ValueError(f"unrecognised mesh type {mesh_type}")
 
-    if mesh_type == 'hexagon': 
+    if mesh_type == "hexagon":
         spot_diameter_um = np.sqrt(3) * spot_diameter_um
         spot_distance_um = spot_diameter_um
 
-    coords = adata.obsm['spatial']
+    coords = adata.obsm["spatial"]
 
     if start_at_minimum:
         top_left_corner = np.min(coords, axis=0)
     else:
         top_left_corner = [0, 0]
 
     bottom_right_corner = np.max(coords, axis=0)
@@ -313,139 +404,133 @@
     spot_diameter_px = spot_diameter_um / um_by_px
     spot_radius_px = spot_radius_um / um_by_px
     spot_distance_px = spot_distance_um / um_by_px
 
     height_um = height_px * um_by_px
 
     # create meshgrid with one radius push
-    xy = create_mesh(width_um,
+    xy = create_mesh(
+        width_um,
         height_um,
         spot_diameter_um,
         spot_distance_um,
-        push_x = spot_radius_um,
-        push_y = spot_radius_um)
-    # create pushed meshgrid, pushed by 
-    xy_pushed = create_mesh(width_um,
+        push_x=spot_radius_um,
+        push_y=spot_radius_um,
+    )
+    # create pushed meshgrid, pushed by
+    xy_pushed = create_mesh(
+        width_um,
         height_um,
         spot_diameter_um,
         spot_distance_um,
-        push_x = spot_radius_um + spot_distance_um / 2,
-        push_y = spot_radius_um + np.sqrt(3) * spot_distance_um / 2)
+        push_x=spot_radius_um + spot_distance_um / 2,
+        push_y=spot_radius_um + np.sqrt(3) * spot_distance_um / 2,
+    )
 
     mesh = np.vstack((xy, xy_pushed))
-    mesh_px = mesh/um_by_px
+    mesh_px = mesh / um_by_px
     # add the top_left_corner
     mesh_px = mesh_px + top_left_corner
 
     # example: the diameter of one visium spot is 55um. if we take any bead, which center
     # falls into that, assuming that a bead is 10um, we would in fact take all beads
     # within 65um diameter. for this reason, the max distance should be 45um/2 between
     # visium spot center and other beads
-    max_distance_px = (spot_diameter_um - bead_diameter_um)/um_by_px/2
+    max_distance_px = (spot_diameter_um - bead_diameter_um) / um_by_px / 2
 
-    def _create_optimized_hex_mesh_properties(mesh):
+    def _create_optimized_hex_mesh_properties(mesh_px):
         _y_values = np.unique(mesh_px[:, 1])
         _x_values = np.unique(mesh_px[:, 0])
         grid_x = len(mesh_px[mesh_px[:, 1] == _y_values[1]])
         grid_y = len(mesh_px[mesh_px[:, 0] == _x_values[1]])
 
         # Calculating the extent
         if len(mesh_px[mesh_px[:, 0] == _x_values[0]]) == grid_y:
-            _offset = (np.diff(_y_values[0:2]))
+            _offset = np.diff(_y_values[0:2])
             _last_row = False
         else:
             _offset = 0
             _last_row = True
 
-        _extent = (mesh_px[:, 0].min(), mesh_px[:, 0].max(),
-                    mesh_px[:, 1].min(), mesh_px[:, 1].max()+_offset)
+        _extent = (
+            mesh_px[:, 0].min(),
+            mesh_px[:, 0].max(),
+            mesh_px[:, 1].min(),
+            mesh_px[:, 1].max() + _offset,
+        )
 
         return grid_x, grid_y, _extent, _last_row
 
-    if mesh_type == 'circle':
+    if mesh_type == "circle":
         if optimized_binning:
-            grid_x, grid_y, _extent, _last_row = _create_optimized_hex_mesh_properties(mesh_px)
-            mesh_px, accum = binning_hexagon(coords[:, 0], coords[:, 1], gridsize=(grid_x, grid_y), extent=_extent, last_row=_last_row)
+            grid_x, grid_y, _extent, _last_row = _create_optimized_hex_mesh_properties(
+                mesh_px
+            )
+            mesh_px, accum = binning_hexagon(
+                coords[:, 0],
+                coords[:, 1],
+                gridsize=(grid_x, grid_y),
+                extent=_extent,
+                last_row=_last_row,
+            )
 
-            new_ilocs = [[i]*len(accum[i]) for i in range(len(accum))]
+            new_ilocs = [[i] * len(accum[i]) for i in range(len(accum))]
             new_ilocs = np.array([n for new_iloc in new_ilocs for n in new_iloc])
             original_ilocs = np.array([a for acc in accum for a in acc])
 
-            distance_filter = np.linalg.norm(np.array(coords[original_ilocs])-np.array(mesh_px[new_ilocs]), axis=1) < max_distance_px
-            
+            distance_filter = (
+                np.linalg.norm(
+                    np.array(coords[original_ilocs]) - np.array(mesh_px[new_ilocs]),
+                    axis=1,
+                )
+                < max_distance_px
+            )
+
             new_ilocs = new_ilocs[distance_filter]
             original_ilocs = original_ilocs[distance_filter]
         else:
             distance_M = euclidean_distances(mesh_px, coords)
             # circle mesh type: we create spots in a hexagonal mesh
             # new_ilocs contains the indices of the columns of the sparse matrix to be created
             # original_ilocs contains the column location of the original adata.X (csr_matrix)
             new_ilocs, original_ilocs = np.nonzero(distance_M < max_distance_px)
-    elif mesh_type == 'hexagon':
+    elif mesh_type == "hexagon":
         if optimized_binning:
-            grid_x, grid_y, _extent, _last_row = _create_optimized_hex_mesh_properties(mesh_px)
-            mesh_px, accum = binning_hexagon(coords[:, 0], coords[:, 1], gridsize=(grid_x, grid_y), extent=_extent, last_row=_last_row)
+            grid_x, grid_y, _extent, _last_row = _create_optimized_hex_mesh_properties(
+                mesh_px
+            )
+            mesh_px, accum = binning_hexagon(
+                coords[:, 0],
+                coords[:, 1],
+                gridsize=(grid_x, grid_y),
+                extent=_extent,
+                last_row=_last_row,
+            )
 
             new_ilocs = np.zeros(len(coords), dtype=int)
             for i in range(len(accum)):
                 new_ilocs[accum[i]] = i
         else:
-            # we simply create a hex mesh, without holes. For each spot, we find the 
+            # we simply create a hex mesh, without holes. For each spot, we find the
             # hexagon it belongs to.
             # Not recommended this non-optimized approach; high memory
             # usage if spot distance is low -> O(n^2) complexity!
             # Kept for reproducibility with legacy runs of spacemake
             distance_M = euclidean_distances(mesh_px, coords)
             new_ilocs = np.argmin(distance_M, axis=0)
-        
+
         original_ilocs = np.arange(new_ilocs.shape[0])
         # we need to sort the new ilocs so that they are in increasing order
         sorted_ix = np.argsort(new_ilocs)
         new_ilocs = new_ilocs[sorted_ix]
         original_ilocs = original_ilocs[sorted_ix]
 
-    joined_C = adata.X[original_ilocs]
-
-    # at which indices does the index in the newly created matrix change
-    change_ix = np.where(new_ilocs[:-1] != new_ilocs[1:])[0] + 1
-
-    #array of indices, split by which row they should go together
-
-    ix_array = np.asarray(np.split(np.arange(new_ilocs.shape[0]), change_ix, axis=0), dtype='object')
-
-    joined_C_sumed = vstack([csr_matrix(joined_C[ix_array[n].astype(int), :].sum(0)) for n in range(len(ix_array))])
-
     joined_coordinates = mesh_px[np.unique(new_ilocs)]
 
-    adata_out = anndata.AnnData(csc_matrix(joined_C_sumed), 
-        obs = pd.DataFrame({'x_pos': joined_coordinates[:, 0],
-                            'y_pos': joined_coordinates[:, 1]}),
-        var = adata.var)
-
-    adata_out.obsm['spatial'] = joined_coordinates
-    
-    # rename index
-    adata_out.obs.index.name = 'cell_bc'
-
-    def summarise_adata_obs_column(adata, column, summary_fun=sum):
-        vals_to_join = adata.obs[column].to_numpy()[original_ilocs]
-        vals_joined = np.array(
-            [summary_fun(vals_to_join[ix_array[n].astype(int)])
-                for n in range(len(ix_array))])
-        return vals_joined
-    print(adata)
-
-    # summarise and attach n_reads, calculate metrics (incl. pcr)
-    calculate_adata_metrics(adata_out,
-        # provide the n_reads as a parameter
-        n_reads = summarise_adata_obs_column(adata, 'n_reads'))
-
-    adata_out.obs['n_joined'] = [len(x) for x in ix_array]
-
-    from statistics import mean
-
-    for column in ['exact_entropy', 'theoretical_entropy', 'exact_compression',\
-        'theoretical_compression']:
-        adata_out.obs[column] = summarise_adata_obs_column(adata, column, mean)
-
-    return adata_out
+    meshed_adata = aggregate_adata_by_indices(
+        adata,
+        idx_to_aggregate=original_ilocs,
+        idx_aggregated=new_ilocs,
+        coordinates_aggregated=joined_coordinates,
+    )
 
+    return meshed_adata
```

### Comparing `spacemake-0.7/spacemake/tag_alignments.py` & `spacemake-0.7.2/spacemake/tag_alignments.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/unittests.py` & `spacemake-0.7.2/spacemake/unittests.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake/util.py` & `spacemake-0.7.2/spacemake/util.py`

 * *Files identical despite different names*

### Comparing `spacemake-0.7/spacemake.egg-info/SOURCES.txt` & `spacemake-0.7.2/spacemake.egg-info/SOURCES.txt`

 * *Files identical despite different names*


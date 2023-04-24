# Comparing `tmp/CodonU-0.0.1.tar.gz` & `tmp/CodonU-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodonU-0.0.1.tar", last modified: Mon Feb 20 19:14:59 2023, max compression
+gzip compressed data, was "CodonU-1.0.2.tar", last modified: Mon Apr 24 07:19:54 2023, max compression
```

## Comparing `CodonU-0.0.1.tar` & `CodonU-1.0.2.tar`

### file list

```diff
@@ -1,66 +1,80 @@
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.140627 CodonU-0.0.1/
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.132627 CodonU-0.0.1/CodonU/
--rw-rw-r--   0 souro     (1000) souro     (1000)        0 2023-02-05 14:22:18.000000 CodonU-0.0.1/CodonU/__init__.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.132627 CodonU-0.0.1/CodonU/analyzer/
--rw-rw-r--   0 souro     (1000) souro     (1000)      146 2023-02-05 17:23:55.000000 CodonU-0.0.1/CodonU/analyzer/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1500 2023-02-05 11:01:20.000000 CodonU-0.0.1/CodonU/analyzer/cai_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1505 2023-02-05 10:29:57.000000 CodonU-0.0.1/CodonU/analyzer/cbi_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1052 2023-02-05 11:37:00.000000 CodonU-0.0.1/CodonU/analyzer/enc_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     8204 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/analyzer/internal_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1069 2023-02-05 11:26:55.000000 CodonU-0.0.1/CodonU/analyzer/rscu_comp.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.132627 CodonU-0.0.1/CodonU/correspondence_analysis/
--rw-rw-r--   0 souro     (1000) souro     (1000)       43 2023-02-20 12:50:52.000000 CodonU-0.0.1/CodonU/correspondence_analysis/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1621 2023-02-20 12:56:38.000000 CodonU-0.0.1/CodonU/correspondence_analysis/mca_codon_freq.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.136627 CodonU-0.0.1/CodonU/cua_errors/
--rw-rw-r--   0 souro     (1000) souro     (1000)      231 2023-02-05 14:45:00.000000 CodonU-0.0.1/CodonU/cua_errors/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      226 2023-02-05 14:22:18.000000 CodonU-0.0.1/CodonU/cua_errors/codon_usage_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      302 2023-02-05 14:45:01.000000 CodonU-0.0.1/CodonU/cua_errors/file_not_empty_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      421 2023-02-05 14:45:01.000000 CodonU-0.0.1/CodonU/cua_errors/internal_stop_codon_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      662 2023-02-05 14:45:01.000000 CodonU-0.0.1/CodonU/cua_errors/no_prot_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      616 2023-02-05 14:45:01.000000 CodonU-0.0.1/CodonU/cua_errors/nucleotide_err.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      478 2023-02-05 14:45:01.000000 CodonU-0.0.1/CodonU/cua_errors/ter_seq_err.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.136627 CodonU-0.0.1/CodonU/cua_warnings/
--rw-rw-r--   0 souro     (1000) souro     (1000)      220 2023-02-20 12:36:45.000000 CodonU-0.0.1/CodonU/cua_warnings/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      361 2023-02-05 14:34:03.000000 CodonU-0.0.1/CodonU/cua_warnings/api_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      165 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/cua_warnings/codon_usage_warns.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      355 2023-02-05 14:34:03.000000 CodonU-0.0.1/CodonU/cua_warnings/email_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      435 2023-02-05 14:22:19.000000 CodonU-0.0.1/CodonU/cua_warnings/missing_codon_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      443 2023-02-20 12:36:46.000000 CodonU-0.0.1/CodonU/cua_warnings/no_codon_warn.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      374 2023-02-05 14:22:18.000000 CodonU-0.0.1/CodonU/cua_warnings/no_syn_codon_warn.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.140627 CodonU-0.0.1/CodonU/extractor/
--rw-rw-r--   0 souro     (1000) souro     (1000)      162 2023-02-05 17:20:46.000000 CodonU-0.0.1/CodonU/extractor/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      772 2023-02-05 17:20:46.000000 CodonU-0.0.1/CodonU/extractor/extract_cds.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      466 2023-02-05 17:20:46.000000 CodonU-0.0.1/CodonU/extractor/extract_cds_lst.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      770 2023-02-05 17:20:45.000000 CodonU-0.0.1/CodonU/extractor/extract_exome.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      876 2023-02-05 17:20:45.000000 CodonU-0.0.1/CodonU/extractor/extract_prot.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      622 2023-02-05 17:20:46.000000 CodonU-0.0.1/CodonU/extractor/internal_comp.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.140627 CodonU-0.0.1/CodonU/file_handler/
--rw-rw-r--   0 souro     (1000) souro     (1000)      244 2023-02-07 16:38:04.000000 CodonU-0.0.1/CodonU/file_handler/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      563 2023-02-07 16:28:20.000000 CodonU-0.0.1/CodonU/file_handler/get_gb.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1580 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/file_handler/internal_comp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      282 2023-02-07 16:29:21.000000 CodonU-0.0.1/CodonU/file_handler/make_dir.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      258 2023-02-07 16:31:13.000000 CodonU-0.0.1/CodonU/file_handler/read_file.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      452 2023-02-07 16:52:57.000000 CodonU-0.0.1/CodonU/file_handler/set_entrez_param.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      793 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/file_handler/write_exome_fasta.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      968 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/file_handler/write_nucleotide_fasta.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      847 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/file_handler/write_protein_fasta.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      641 2022-09-14 18:21:45.000000 CodonU-0.0.1/CodonU/main.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      203 2023-02-20 12:52:25.000000 CodonU-0.0.1/CodonU/temp.py
--rw-rw-r--   0 souro     (1000) souro     (1000)      485 2023-02-20 11:53:23.000000 CodonU-0.0.1/CodonU/temp2.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     3353 2023-02-20 12:39:35.000000 CodonU-0.0.1/CodonU/temp3.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.140627 CodonU-0.0.1/CodonU/vizualizer/
--rw-rw-r--   0 souro     (1000) souro     (1000)      107 2023-02-17 14:11:34.000000 CodonU-0.0.1/CodonU/vizualizer/__init__.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1378 2023-02-20 11:53:23.000000 CodonU-0.0.1/CodonU/vizualizer/plot_enc.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     7540 2023-02-19 10:54:15.000000 CodonU-0.0.1/CodonU/vizualizer/plot_funcs.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1358 2023-02-20 11:53:25.000000 CodonU-0.0.1/CodonU/vizualizer/plot_neutrality.py
--rw-rw-r--   0 souro     (1000) souro     (1000)     1538 2023-02-20 11:53:24.000000 CodonU-0.0.1/CodonU/vizualizer/plot_pr2.py
-drwxrwxr-x   0 souro     (1000) souro     (1000)        0 2023-02-20 19:14:59.132627 CodonU-0.0.1/CodonU.egg-info/
--rw-rw-r--   0 souro     (1000) souro     (1000)     2635 2023-02-20 19:14:59.000000 CodonU-0.0.1/CodonU.egg-info/PKG-INFO
--rw-rw-r--   0 souro     (1000) souro     (1000)     1700 2023-02-20 19:14:59.000000 CodonU-0.0.1/CodonU.egg-info/SOURCES.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)        1 2023-02-20 19:14:59.000000 CodonU-0.0.1/CodonU.egg-info/dependency_links.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)        7 2023-02-20 19:14:59.000000 CodonU-0.0.1/CodonU.egg-info/top_level.txt
--rw-rw-r--   0 souro     (1000) souro     (1000)     1077 2023-02-01 15:01:49.000000 CodonU-0.0.1/LICENSE.md
--rw-rw-r--   0 souro     (1000) souro     (1000)     2635 2023-02-20 19:14:59.140627 CodonU-0.0.1/PKG-INFO
--rw-rw-r--   0 souro     (1000) souro     (1000)     1344 2023-02-20 17:59:17.000000 CodonU-0.0.1/README.md
--rw-rw-r--   0 souro     (1000) souro     (1000)       38 2023-02-20 19:14:59.140627 CodonU-0.0.1/setup.cfg
--rw-rw-r--   0 souro     (1000) souro     (1000)     2477 2023-02-20 19:14:56.000000 CodonU-0.0.1/setup.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.859822 CodonU-1.0.2/
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.841822 CodonU-1.0.2/CodonU/
+-rw-rw-r--   0 souro     (1000) souro     (1000)        0 2023-03-05 07:31:25.000000 CodonU-1.0.2/CodonU/__init__.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.846822 CodonU-1.0.2/CodonU/analyzer/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      344 2023-04-23 09:03:35.000000 CodonU-1.0.2/CodonU/analyzer/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2379 2023-04-18 11:47:53.000000 CodonU-1.0.2/CodonU/analyzer/aromaticity_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2882 2023-04-18 11:47:53.000000 CodonU-1.0.2/CodonU/analyzer/cai_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2912 2023-04-18 12:20:27.000000 CodonU-1.0.2/CodonU/analyzer/cbi_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2427 2023-04-18 12:20:27.000000 CodonU-1.0.2/CodonU/analyzer/enc_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     6524 2023-03-26 14:18:02.000000 CodonU-1.0.2/CodonU/analyzer/generate_report.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     5901 2023-03-27 11:31:56.000000 CodonU-1.0.2/CodonU/analyzer/generate_report_summary.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2372 2023-04-18 12:20:27.000000 CodonU-1.0.2/CodonU/analyzer/gravy_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     8876 2023-03-21 06:22:22.000000 CodonU-1.0.2/CodonU/analyzer/internal_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1237 2023-04-16 18:32:20.000000 CodonU-1.0.2/CodonU/analyzer/rscu_comp.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.847822 CodonU-1.0.2/CodonU/correspondence_analysis/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      123 2023-03-06 12:33:30.000000 CodonU-1.0.2/CodonU/correspondence_analysis/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1774 2023-03-05 12:14:39.000000 CodonU-1.0.2/CodonU/correspondence_analysis/mca_aa_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2127 2023-03-05 12:06:51.000000 CodonU-1.0.2/CodonU/correspondence_analysis/mca_codon_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1633 2023-03-05 12:06:51.000000 CodonU-1.0.2/CodonU/correspondence_analysis/mca_codon_rscu.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.849822 CodonU-1.0.2/CodonU/cua_errors/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      277 2023-03-08 17:10:24.000000 CodonU-1.0.2/CodonU/cua_errors/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      226 2023-02-05 14:22:18.000000 CodonU-1.0.2/CodonU/cua_errors/codon_usage_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      302 2023-02-05 14:45:01.000000 CodonU-1.0.2/CodonU/cua_errors/file_not_empty_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      421 2023-02-05 14:45:01.000000 CodonU-1.0.2/CodonU/cua_errors/internal_stop_codon_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      662 2023-02-05 14:45:01.000000 CodonU-1.0.2/CodonU/cua_errors/no_prot_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      616 2023-02-05 14:45:01.000000 CodonU-1.0.2/CodonU/cua_errors/nucleotide_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      478 2023-02-05 14:45:01.000000 CodonU-1.0.2/CodonU/cua_errors/ter_seq_err.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      463 2023-03-08 17:18:27.000000 CodonU-1.0.2/CodonU/cua_errors/unsupported_type.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.850822 CodonU-1.0.2/CodonU/cua_warnings/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      262 2023-04-24 07:10:51.000000 CodonU-1.0.2/CodonU/cua_warnings/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      361 2023-02-05 14:34:03.000000 CodonU-1.0.2/CodonU/cua_warnings/api_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      165 2023-02-20 11:53:24.000000 CodonU-1.0.2/CodonU/cua_warnings/codon_usage_warns.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      355 2023-02-05 14:34:03.000000 CodonU-1.0.2/CodonU/cua_warnings/email_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      435 2023-02-05 14:22:19.000000 CodonU-1.0.2/CodonU/cua_warnings/missing_codon_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      443 2023-02-20 12:36:46.000000 CodonU-1.0.2/CodonU/cua_warnings/no_codon_warn.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      374 2023-02-05 14:22:18.000000 CodonU-1.0.2/CodonU/cua_warnings/no_syn_codon_warn.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.852822 CodonU-1.0.2/CodonU/extractor/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      162 2023-02-05 17:20:46.000000 CodonU-1.0.2/CodonU/extractor/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      772 2023-02-05 17:20:46.000000 CodonU-1.0.2/CodonU/extractor/extract_cds.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      466 2023-02-05 17:20:46.000000 CodonU-1.0.2/CodonU/extractor/extract_cds_lst.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      770 2023-02-05 17:20:45.000000 CodonU-1.0.2/CodonU/extractor/extract_exome.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      876 2023-02-05 17:20:45.000000 CodonU-1.0.2/CodonU/extractor/extract_prot.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      622 2023-02-05 17:20:46.000000 CodonU-1.0.2/CodonU/extractor/internal_comp.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.854822 CodonU-1.0.2/CodonU/file_handler/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      299 2023-04-24 07:10:51.000000 CodonU-1.0.2/CodonU/file_handler/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      563 2023-02-07 16:28:20.000000 CodonU-1.0.2/CodonU/file_handler/get_gb.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1580 2023-02-20 11:53:24.000000 CodonU-1.0.2/CodonU/file_handler/internal_comp.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      282 2023-02-07 16:29:21.000000 CodonU-1.0.2/CodonU/file_handler/make_dir.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      258 2023-02-07 16:31:13.000000 CodonU-1.0.2/CodonU/file_handler/read_file.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      452 2023-03-06 12:48:19.000000 CodonU-1.0.2/CodonU/file_handler/set_entrez_param.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      793 2023-02-20 11:53:24.000000 CodonU-1.0.2/CodonU/file_handler/write_exome_fasta.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      968 2023-02-20 11:53:24.000000 CodonU-1.0.2/CodonU/file_handler/write_nucleotide_fasta.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)      847 2023-02-20 11:53:24.000000 CodonU-1.0.2/CodonU/file_handler/write_protein_fasta.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.855822 CodonU-1.0.2/CodonU/phylogenetic_analysis/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      129 2023-04-23 10:39:14.000000 CodonU-1.0.2/CodonU/phylogenetic_analysis/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1314 2023-04-09 16:04:34.000000 CodonU-1.0.2/CodonU/phylogenetic_analysis/clustal_o.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1295 2023-04-09 16:04:53.000000 CodonU-1.0.2/CodonU/phylogenetic_analysis/clustal_w.py
+-rw-r--r--   0 souro     (1000) souro     (1000)     1373 2023-04-23 10:39:14.000000 CodonU-1.0.2/CodonU/phylogenetic_analysis/generate_phylo_input.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.858822 CodonU-1.0.2/CodonU/vizualizer/
+-rw-rw-r--   0 souro     (1000) souro     (1000)      377 2023-04-13 13:58:13.000000 CodonU-1.0.2/CodonU/vizualizer/__init__.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1378 2023-02-23 15:35:26.000000 CodonU-1.0.2/CodonU/vizualizer/plot_enc.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     7969 2023-04-13 13:45:08.000000 CodonU-1.0.2/CodonU/vizualizer/plot_funcs.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2596 2023-03-07 05:32:05.000000 CodonU-1.0.2/CodonU/vizualizer/plot_mca_aa_aroma.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2585 2023-03-07 05:27:47.000000 CodonU-1.0.2/CodonU/vizualizer/plot_mca_aa_gravy.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2535 2023-03-06 12:33:30.000000 CodonU-1.0.2/CodonU/vizualizer/plot_mca_codon_freq.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2502 2023-03-07 05:27:47.000000 CodonU-1.0.2/CodonU/vizualizer/plot_mca_rscu.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1358 2023-02-23 15:35:27.000000 CodonU-1.0.2/CodonU/vizualizer/plot_neutrality.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1000 2023-04-13 13:55:32.000000 CodonU-1.0.2/CodonU/vizualizer/plot_phy_dnd.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1283 2023-04-13 13:55:32.000000 CodonU-1.0.2/CodonU/vizualizer/plot_phy_nex.py
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1538 2023-02-23 15:35:27.000000 CodonU-1.0.2/CodonU/vizualizer/plot_pr2.py
+drwxr-xr-x   0 souro     (1000) souro     (1000)        0 2023-04-24 07:19:54.843822 CodonU-1.0.2/CodonU.egg-info/
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3072 2023-04-24 07:19:54.000000 CodonU-1.0.2/CodonU.egg-info/PKG-INFO
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2315 2023-04-24 07:19:54.000000 CodonU-1.0.2/CodonU.egg-info/SOURCES.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)        1 2023-04-24 07:19:54.000000 CodonU-1.0.2/CodonU.egg-info/dependency_links.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)        7 2023-04-24 07:19:54.000000 CodonU-1.0.2/CodonU.egg-info/top_level.txt
+-rw-rw-r--   0 souro     (1000) souro     (1000)     1077 2023-02-01 15:01:49.000000 CodonU-1.0.2/LICENSE.md
+-rw-r--r--   0 souro     (1000) souro     (1000)     3072 2023-04-24 07:19:54.858822 CodonU-1.0.2/PKG-INFO
+-rw-rw-r--   0 souro     (1000) souro     (1000)     3468 2023-04-24 07:10:52.000000 CodonU-1.0.2/README.md
+-rw-r--r--   0 souro     (1000) souro     (1000)       38 2023-04-24 07:19:54.859822 CodonU-1.0.2/setup.cfg
+-rw-rw-r--   0 souro     (1000) souro     (1000)     2178 2023-04-24 07:19:50.000000 CodonU-1.0.2/setup.py
```

### Comparing `CodonU-0.0.1/CodonU/analyzer/cai_comp.py` & `CodonU-1.0.2/CodonU/analyzer/rscu_comp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from CAI import CAI
-from warnings import filterwarnings
-from Bio.Data.CodonTable import unambiguous_dna_by_id
+from cai2 import RSCU
 from .internal_comp import filter_reference
+from Bio.SeqIO import parse
 
 
-def calculate_cai(records, genetic_code_num: int, min_len_threshold: int = 200, gene_analysis: bool = False) -> \
-        dict[str, float] | dict[str, dict[str, float]]:
+def calculate_rscu(handle: str, genetic_code_num: int, min_len_threshold: int = 200, gene_analysis: bool = False) -> \
+        dict[str, float | dict[str, float]]:
     """
-    Calculates cai values for each codon
+    Calculates rscu values for each codon
 
-    :param records: The generator object containing sequence object
+    :param handle: Handle to the file, or the filename as a string
     :param genetic_code_num: Genetic table number for codon table
     :param min_len_threshold: Minimum length of nucleotide sequence to be considered as gene
     :param gene_analysis: Option if gene analysis (True) or genome analysis (False) (optional)
-    :return: The dictionary containing codon and cai value pairs
+    :return: The dictionary containing codon and rscu value pairs if gene_analysis is false, otherwise the dictionary containing the gene name and the codon & rscu value pairs
     """
-    filterwarnings('ignore')
-    cai_dict = dict()
-    reference = filter_reference(records, min_len_threshold)
+    records = parse(handle, 'fasta')
+    references = filter_reference(records, min_len_threshold)
     if gene_analysis:
-        for i, seq in enumerate(reference):
-            cai_val_dict = dict()
-            for codon in unambiguous_dna_by_id[genetic_code_num].forward_table:
-                cai_val = CAI(codon, reference=[seq], genetic_code=genetic_code_num)
-                cai_val_dict.update({codon: cai_val})
-            cai_dict.update({f'gene_{i + 1}': cai_val_dict})
+        rscu_dict = dict()
+        for i, seq in enumerate(references):
+            rscu_dict.update({f'gene_{i + 1}': RSCU([seq], genetic_code_num)})
+        return rscu_dict
     else:
-        for codon in unambiguous_dna_by_id[genetic_code_num].forward_table:
-            cai_val = CAI(codon, reference=reference, genetic_code=genetic_code_num)
-            cai_dict.update({codon: cai_val})
-    return cai_dict
+        reference = filter_reference(records, min_len_threshold)
+        return RSCU(reference, genetic_code_num)
```

### Comparing `CodonU-0.0.1/CodonU/analyzer/internal_comp.py` & `CodonU-1.0.2/CodonU/analyzer/internal_comp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import Counter
 from itertools import chain
 from math import nan, isnan
 from statistics import mean
 from Bio.Data.CodonTable import NCBICodonTableDNA, unambiguous_dna_by_id
 from Bio.Seq import Seq
 from Bio.SeqUtils import seq3, GC123
+from Bio.SeqUtils.ProtParam import ProteinAnalysis
 from CodonU.cua_warnings import NoSynonymousCodonWarning, MissingCodonWarning
 from CodonU.cua_errors import NoProteinError
 
 
 def g3(seq: Seq | str) -> float:
     """
     Calculates percentage of G content for third position
@@ -110,15 +111,15 @@
     return sorted_sf_dict
 
 
 def cbi(prot_seq: Seq | str, reference: list[Seq], genetic_code: int) -> tuple[float, str]:
     """
     Calculates codon bias index (CBI) for a given protein seq based on Bennetzen and Hall (1982)
 
-    :param prot_seq: The Amino Acid
+    :param prot_seq: The Protein Sequence
     :param reference: List of reference nucleotide sequences
     :param genetic_code: Genetic table number for codon table
     :return: A tuple of CBI val and the optimal codon
     :raises NoSynonymousCodonWarning: When there is no synonymous codons
     :raises MissingCodonWarning: When no codons translate to provided Amino acid
     """
     sequences = ((sequence[i:i + 3].upper() for i in range(0, len(sequence), 3)) for sequence in reference)
@@ -211,7 +212,33 @@
                     ((2 / (5 * f_6)) + (3 / 5)) ** -1)) / 3.0
         else:
             raise NoProteinError(references[0])
         F_val_avg_lst[2] = f_3
     # [sf_6 avg, sf_4 avg, sf_3 avg, sf_2 avg, sf_1 avg]
     enc_val = 2 + (9 / F_val_avg_lst[3]) + (1 / F_val_avg_lst[2]) + (5 / F_val_avg_lst[1]) + (3 / F_val_avg_lst[0])
     return enc_val if enc_val < 61 else 61.00
+
+
+def gravy(seq: Seq | str) -> float:
+    """
+    Computes the GRAVY score according to Kyte and Doolittle (1982)
+
+    :param seq: Protein sequence
+    :return: The GRAVY score
+    """
+    if not isinstance(seq, str):
+        _seq = str(seq)
+        seq = _seq
+    return ProteinAnalysis(seq).gravy()
+
+
+def aromaticity(seq: Seq | str) -> float:
+    """
+    Calculate the aromaticity score according to Lobry (1994).
+
+    :param seq: Protein sequence
+    :return: The aromaticity score
+    """
+    if not isinstance(seq, str):
+        _seq = str(seq)
+        seq = _seq
+    return ProteinAnalysis(seq).aromaticity()
```

### Comparing `CodonU-0.0.1/CodonU/cua_errors/no_prot_err.py` & `CodonU-1.0.2/CodonU/cua_errors/no_prot_err.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/cua_errors/nucleotide_err.py` & `CodonU-1.0.2/CodonU/cua_errors/nucleotide_err.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/extractor/extract_cds.py` & `CodonU-1.0.2/CodonU/extractor/extract_cds.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/extractor/extract_exome.py` & `CodonU-1.0.2/CodonU/extractor/extract_exome.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/extractor/extract_prot.py` & `CodonU-1.0.2/CodonU/extractor/extract_prot.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/extractor/internal_comp.py` & `CodonU-1.0.2/CodonU/extractor/internal_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/file_handler/get_gb.py` & `CodonU-1.0.2/CodonU/file_handler/get_gb.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/file_handler/internal_comp.py` & `CodonU-1.0.2/CodonU/file_handler/internal_comp.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/file_handler/write_exome_fasta.py` & `CodonU-1.0.2/CodonU/file_handler/write_exome_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/file_handler/write_nucleotide_fasta.py` & `CodonU-1.0.2/CodonU/file_handler/write_nucleotide_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/file_handler/write_protein_fasta.py` & `CodonU-1.0.2/CodonU/file_handler/write_protein_fasta.py`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/CodonU/vizualizer/plot_enc.py` & `CodonU-1.0.2/CodonU/vizualizer/plot_enc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def plot_enc(handle: str | Any, genetic_table_num: int, min_len_threshold: int = 200, organism_name: None | str = None,
              save_image: bool = False, folder_path: str = '', gene_analysis: bool = True):
     """
     Plots ENc curve from given fasta file
 
-    :param handle: handle to the file, or the filename as a string
+    :param handle: Handle to the file, or the filename as a string
     :param genetic_table_num: Genetic table number for codon table
     :param min_len_threshold: Minimum length of nucleotide sequence to be considered as gene
     :param organism_name: Name of organism (optional)
     :param save_image: Options for saving the image (optional)
     :param folder_path: Folder path where image should be saved (optional)
     :param gene_analysis: Option if gene analysis (True) or genome analysis (False) (optional)
     """
```

### Comparing `CodonU-0.0.1/CodonU/vizualizer/plot_funcs.py` & `CodonU-1.0.2/CodonU/vizualizer/plot_funcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
-from os.path import join
+from os.path import join, abspath
 from scipy.stats import linregress
+from CodonU.file_handler.internal_comp import is_file_empty
 
 
 def _enc(x: int) -> float:
     """
     Calculates Theoretical ENC value based on Wright (1989)
 
     :param x: GC3 value
@@ -43,15 +44,18 @@
     plt.ylabel(r"$EN_c$ Value")
     plt.grid(True, linestyle=':')
     c_bar = plt.colorbar()
     c_bar.set_label(r'$EN_c values$')
     if save_image:
         name = 'ENc_plot.png' if organism_name is None else f"ENc_plot_{organism_name}.png"
         file_name = join(folder_path, name)
+        if is_file_empty(file_name):
+            pass
         plt.savefig(file_name, dpi=500)
+        print(f'Saved file can be found as {abspath(file_name)}')
     plt.show()
     plt.close()
 
 
 def _plot_pr2(gc_val_lst: list, at_val_lst: list, g3_val_lst: list, a3_val_lst: list, organism_name: str | None = None,
               save_image: bool = False, folder_path: str = '', gene_analysis: bool = True):
     """
@@ -128,15 +132,18 @@
     suptitle = r'Parity Rule 2 plot' if organism_name is None else f"Parity Rule 2 plot for {organism_name}"
     plt.suptitle(suptitle, fontsize=16)
     title = f'Total genes: {N}' if gene_analysis else f'Total genome: {N}'
     plt.title(title, fontsize=12)
     if save_image:
         name = 'PR2_plot.png' if organism_name is None else f"PR2_plot_{organism_name}.png"
         file_name = join(folder_path, name)
+        if is_file_empty(file_name):
+            pass
         plt.savefig(file_name, dpi=500)
+        print(f'Saved file can be found as {abspath(file_name)}')
     plt.show()
     plt.close()
 
 
 def _plot_neutrality(gc12_lst: list, gc3_lst: list, organism_name: None | str = None, save_image: bool = False,
                      folder_path: str = '', gene_analysis: bool = True):
     """
@@ -175,10 +182,13 @@
     suptitle = r'Neutrality Plot' if organism_name is None else f"Neutrality plot for {organism_name}"
     plt.suptitle(suptitle, fontsize=16)
     title = f'Total genes: {N}, $R^2$ value: {round(r ** 2, 4)}' if gene_analysis else f'Total genome: {N}, $R^2$ value: {round(r ** 2, 4)}'
     plt.title(title, fontsize=14)
     if save_image:
         name = 'Neutrality_plot.png' if organism_name is None else f"Neutrality_plot_{organism_name}.png"
         file_name = join(folder_path, name)
+        if is_file_empty(file_name):
+            pass
         plt.savefig(file_name, dpi=500)
+        print(f'Saved file can be found as {abspath(file_name)}')
     plt.show()
     plt.close()
```

### Comparing `CodonU-0.0.1/CodonU/vizualizer/plot_neutrality.py` & `CodonU-1.0.2/CodonU/vizualizer/plot_neutrality.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def plot_neutrality(handle: str | Any, min_len_threshold: int, organism_name: str | None = None,
                     save_image: bool = False, folder_path: str = '', gene_analysis: bool = True):
     """
     Plots neutrality plot from given fasta file
 
-    :param handle: handle to the file, or the filename as a string
+    :param handle: Handle to the file, or the filename as a string
     :param min_len_threshold: Minimum length of nucleotide sequence to be considered as gene
     :param organism_name: Name of organism (optional)
     :param save_image: Options for saving the image (optional)
     :param folder_path: Folder path where image should be saved (optional)
     :param gene_analysis: Option if gene analysis (True) or genome analysis (False) (optional)
     """
     filterwarnings('ignore')
```

### Comparing `CodonU-0.0.1/CodonU/vizualizer/plot_pr2.py` & `CodonU-1.0.2/CodonU/vizualizer/plot_pr2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def plot_pr2(handle: str | Any, min_len_threshold: int, organism_name: str | None = None, save_image: bool = False,
              folder_path: str = '', gene_analysis: bool = True):
     """
     Plots A3/AT3 values against G3/GC3 values from given fasta file
 
-    :param handle: handle to the file, or the filename as a string
+    :param handle: Handle to the file, or the filename as a string
     :param min_len_threshold: Minimum length of nucleotide sequence to be considered as gene
     :param organism_name: Name of organism (optional)
     :param save_image: Options for saving the image (optional)
     :param folder_path: Folder path where image should be saved (optional)
     :param gene_analysis: Option if gene analysis (True) or genome analysis (False) (optional)
     """
     filterwarnings('ignore')
```

### Comparing `CodonU-0.0.1/CodonU.egg-info/PKG-INFO` & `CodonU-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,83 @@
-Metadata-Version: 2.1
-Name: CodonU
-Version: 0.0.1
-Summary: This package is designed for helping in genomic analysis
-Home-page: https://github.com/SouradiptoC/codon_usage
-Author: Souradipto Choudhuri
-Author-email: sourochaudhuri@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/SouradiptoC/codon_usage/issues
-Project-URL: Documentation, https://github.com/SouradiptoC/codon_usage/wiki
-Project-URL: Source Code, https://github.com/SouradiptoC/codon_usage
-Keywords: bioinformatics,bioinformatics-analysis,bioinformatics-tool,codon-usage,codon,codon-bias,genomic-analysis,genome,souradipto choudhuri
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
+[//]: # (# CodonU)
 
-# README
+![CodonU](https://github.com/SouradiptoC/CodonU/blob/master/images/CODON_U_Background.png)
 
 [![PyPI - License](https://img.shields.io/pypi/l/CodonU)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/536583655.svg)](https://zenodo.org/badge/latestdoi/536583655)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CodonU)](https://pypi.org/project/CodonU)
 [![PyPI](https://img.shields.io/pypi/v/CodonU)](https://pypi.org/project/CodonU)
-![GitHub repo size](https://img.shields.io/github/repo-size/SouradiptoC/codon_usage)
 [![PyPI - Format](https://img.shields.io/pypi/format/CodonU)](https://pypi.org/project/CodonU)
+[![Downloads](https://static.pepy.tech/personalized-badge/codonu?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/codonu)
+[![CodeFactor](https://www.codefactor.io/repository/github/souradiptoc/codonu/badge/master)](https://www.codefactor.io/repository/github/souradiptoc/codonu/overview/master)
+[![Docs](https://img.shields.io/badge/docs-passing-brightgreen)](https://souradiptoc.github.io/CodonU/)
 
-The package can easily can help in various ways from fetching genebank files from NCBI with the help of accession id to
-calculating cai, cbi, rscu, enc values and also can generate good quality graphics such as enc plot, or correspondence
-analysis plot
-<br>
-Updates will be done on a regular basis.
+# Introduction
 
-A complete doumentation is available [here](https://github.com/SouradiptoC/codon_usage/wiki).
+Welcome to CodonU!
+
+This is an integrated package for codon usage analysis.
+
+# Functionalities
+
+Various functionalities can be found below. For gene/genome analysis, this package can:
+
+- For Nucleotide sequences
+    - Calculate RSCU
+    - Calculate CAI
+    - Calculate CBI
+    - Calculate ENc
+- For Protein sequences
+    - Calculate Aromaticity
+    - Calculate gravy
+
+One can also can calculate the multivariate analysis, popularly known as correspondence analysis (COA) for the codons
+easily.
+Supported calculations are:
+
+- For Nucleotide sequences
+    - COA using codon frequency with scale set to length of gene
+    - COA using codon RSCU values with scale set to length of gene
+- For Protein sequences
+    - COA using amino acid frequency with scale set to gravy score
+    - COA using amino acid frequency with scale set to aromaticity score
+
+Phylogenetic analysis and tree building now can be done.
+
+Detailed instructions on how to use the functions can be found in
+the [examples](https://github.com/SouradiptoC/CodonU/tree/master/Examples)
+
+# Graphics!!
+
+Also, can generate beautiful graphics for publication purpose or otherwise. Some plots are:
+
+ENc plot for human chromosome 2
+
+![ENc plot for human chromosome 2](https://github.com/SouradiptoC/CodonU/blob/master/images/ENc_plot_Human%20Cr%202.png)
+
+Neutrality plot for human chromosome 2
+
+![Neutrality plot for human chromosome 2](https://github.com/SouradiptoC/CodonU/blob/master/images/Neutrality_plot_Human%20Cr%202.png)
+
+Correspondence analysis of protein frequency using gravy score
+
+![Correspondence analysis of protein frequency using gravy score](https://github.com/SouradiptoC/CodonU/blob/master/images/Multivariate_analysis_aa_gravy_agnetis.png)
+
+Examples for other plots cans be found in the [images](https://github.com/SouradiptoC/CodonU/tree/master/images)
+
+# Installation
+
+    pip install CodonU
+
+# Future Plans
+
+None. If you would like recommend one, please mail
+at [sourochaudhuri@gmail.com](mailto:sourochaudhuri@gmail.com)
+
+# Citation
 
 Please cite the work as
 
     @software{souradipto_choudhuri_2023_7657797,
       author       = {Souradipto Choudhuri},
       title        = {CodonU},
       month        = feb,
```

### Comparing `CodonU-0.0.1/CodonU.egg-info/SOURCES.txt` & `CodonU-1.0.2/CodonU.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 LICENSE.md
 README.md
 setup.py
 CodonU/__init__.py
-CodonU/main.py
-CodonU/temp.py
-CodonU/temp2.py
-CodonU/temp3.py
 CodonU.egg-info/PKG-INFO
 CodonU.egg-info/SOURCES.txt
 CodonU.egg-info/dependency_links.txt
 CodonU.egg-info/top_level.txt
 CodonU/analyzer/__init__.py
+CodonU/analyzer/aromaticity_comp.py
 CodonU/analyzer/cai_comp.py
 CodonU/analyzer/cbi_comp.py
 CodonU/analyzer/enc_comp.py
+CodonU/analyzer/generate_report.py
+CodonU/analyzer/generate_report_summary.py
+CodonU/analyzer/gravy_comp.py
 CodonU/analyzer/internal_comp.py
 CodonU/analyzer/rscu_comp.py
 CodonU/correspondence_analysis/__init__.py
+CodonU/correspondence_analysis/mca_aa_freq.py
 CodonU/correspondence_analysis/mca_codon_freq.py
+CodonU/correspondence_analysis/mca_codon_rscu.py
 CodonU/cua_errors/__init__.py
 CodonU/cua_errors/codon_usage_err.py
 CodonU/cua_errors/file_not_empty_err.py
 CodonU/cua_errors/internal_stop_codon_err.py
 CodonU/cua_errors/no_prot_err.py
 CodonU/cua_errors/nucleotide_err.py
 CodonU/cua_errors/ter_seq_err.py
+CodonU/cua_errors/unsupported_type.py
 CodonU/cua_warnings/__init__.py
 CodonU/cua_warnings/api_warn.py
 CodonU/cua_warnings/codon_usage_warns.py
 CodonU/cua_warnings/email_warn.py
 CodonU/cua_warnings/missing_codon_warn.py
 CodonU/cua_warnings/no_codon_warn.py
 CodonU/cua_warnings/no_syn_codon_warn.py
@@ -43,12 +46,22 @@
 CodonU/file_handler/internal_comp.py
 CodonU/file_handler/make_dir.py
 CodonU/file_handler/read_file.py
 CodonU/file_handler/set_entrez_param.py
 CodonU/file_handler/write_exome_fasta.py
 CodonU/file_handler/write_nucleotide_fasta.py
 CodonU/file_handler/write_protein_fasta.py
+CodonU/phylogenetic_analysis/__init__.py
+CodonU/phylogenetic_analysis/clustal_o.py
+CodonU/phylogenetic_analysis/clustal_w.py
+CodonU/phylogenetic_analysis/generate_phylo_input.py
 CodonU/vizualizer/__init__.py
 CodonU/vizualizer/plot_enc.py
 CodonU/vizualizer/plot_funcs.py
+CodonU/vizualizer/plot_mca_aa_aroma.py
+CodonU/vizualizer/plot_mca_aa_gravy.py
+CodonU/vizualizer/plot_mca_codon_freq.py
+CodonU/vizualizer/plot_mca_rscu.py
 CodonU/vizualizer/plot_neutrality.py
+CodonU/vizualizer/plot_phy_dnd.py
+CodonU/vizualizer/plot_phy_nex.py
 CodonU/vizualizer/plot_pr2.py
```

### Comparing `CodonU-0.0.1/LICENSE.md` & `CodonU-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CodonU-0.0.1/setup.py` & `CodonU-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,38 +24,36 @@
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 
 PACK_NAME = 'CodonU'
 AUTHOR_NAME = 'Souradipto Choudhuri'
 AUTHOR_EMAIL = 'sourochaudhuri@gmail.com'
-VERSION = '0.0.1'
+VERSION = '1.0.2'
 DESC = 'This package is designed for helping in genomic analysis'
-# LONG_DESC = 'The package can easily can help in various ways from fetching genebank files from NCBI with the help of ' \
-#             'accession id to calculating cai, cbi, rscu, enc values and also can generate good quality graphics ' \
-#             'such as enc plot, or correspondence analysis plot'
 
 setup(
     name='CodonU',
     version=VERSION,
     url='https://github.com/SouradiptoC/codon_usage',
     project_urls={
         "Bug Tracker": "https://github.com/SouradiptoC/codon_usage/issues",
-        "Documentation": "https://github.com/SouradiptoC/codon_usage/wiki",
+        "Documentation": "https://souradiptoc.github.io/CodonU/",
         "Source Code": "https://github.com/SouradiptoC/codon_usage"
     },
     author=AUTHOR_NAME,
     author_email=AUTHOR_EMAIL,
     description=DESC,
-    long_description=read("README.md"),
+    long_description=read("README_pypi.md"),
     long_description_content_type="text/markdown",
+    license='MIT License',
     packages=find_packages(exclude=["tests", ".github"]),
     install_requirements=read_requirements('requirements.txt'),
     keywords=['bioinformatics', 'bioinformatics-analysis', 'bioinformatics-tool', 'codon-usage', 'codon', 'codon-bias',
-              'genomic-analysis', 'genome', 'souradipto choudhuri'],
+              'genomic-analysis', 'genome', 'codonW'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```


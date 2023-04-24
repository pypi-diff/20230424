# Comparing `tmp/cladeomatic-0.0.1.tar.gz` & `tmp/cladeomatic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jrobertson/PycharmProjects/cladeomatic/dist/tmp_ukj_z1y/cladeomatic-0.0.1.tar", last modified: Fri Oct 21 19:20:36 2022, max compression
+gzip compressed data, was "cladeomatic-0.1.0.tar", last modified: Mon Apr 24 17:18:22 2023, max compression
```

## Comparing `cladeomatic-0.0.1.tar` & `cladeomatic-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/
--rw-r--r--   0 jrobertson   (502) staff       (20)    11357 2022-06-27 19:03:32.000000 cladeomatic-0.0.1/LICENSE
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-27 19:04:06.000000 cladeomatic-0.0.1/MANIFEST.in
--rw-r--r--   0 jrobertson   (502) staff       (20)      969 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)     6887 2022-10-21 19:15:28.000000 cladeomatic-0.0.1/README.md
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 18:18:38.000000 cladeomatic-0.0.1/cladeomatic/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    12087 2022-10-21 16:54:14.000000 cladeomatic-0.0.1/cladeomatic/benchmark.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1052 2022-10-18 13:43:09.000000 cladeomatic-0.0.1/cladeomatic/constants.py
--rw-rw-rw-   0 jrobertson   (502) staff       (20)    80644 2022-10-20 20:48:05.000000 cladeomatic-0.0.1/cladeomatic/create.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     1361 2022-09-13 17:28:01.000000 cladeomatic-0.0.1/cladeomatic/main.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     6970 2022-10-13 17:45:55.000000 cladeomatic-0.0.1/cladeomatic/simulate_genomes.py
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 17:34:28.000000 cladeomatic-0.0.1/cladeomatic/test.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic/utils/
--rw-r--r--   0 jrobertson   (502) staff       (20)     1961 2022-08-17 18:28:22.000000 cladeomatic-0.0.1/cladeomatic/utils/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      890 2022-08-18 15:05:23.000000 cladeomatic-0.0.1/cladeomatic/utils/jellyfish.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     5273 2022-10-18 18:06:57.000000 cladeomatic-0.0.1/cladeomatic/utils/kmerSearch.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     7885 2022-10-18 13:43:56.000000 cladeomatic-0.0.1/cladeomatic/utils/phylo_tree.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     7676 2022-10-20 19:18:11.000000 cladeomatic-0.0.1/cladeomatic/utils/seqdata.py
--rw-r--r--   0 jrobertson   (502) staff       (20)     2008 2022-09-07 15:20:56.000000 cladeomatic-0.0.1/cladeomatic/utils/vcfhelper.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      310 2022-06-29 15:08:41.000000 cladeomatic-0.0.1/cladeomatic/utils/visualization.py
--rw-r--r--   0 jrobertson   (502) staff       (20)       21 2022-08-10 14:56:16.000000 cladeomatic-0.0.1/cladeomatic/version.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/
--rw-r--r--   0 jrobertson   (502) staff       (20)      969 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)      661 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/SOURCES.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)        1 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/dependency_links.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       54 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/entry_points.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)      119 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/requires.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       12 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/cladeomatic.egg-info/top_level.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       38 2022-10-21 19:20:36.000000 cladeomatic-0.0.1/setup.cfg
--rw-r--r--   0 jrobertson   (502) staff       (20)     1907 2022-09-12 18:14:44.000000 cladeomatic-0.0.1/setup.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.354730 cladeomatic-0.1.0/
+-rw-r--r--   0 jrobertson   (502) staff       (20)    11357 2022-06-27 19:03:32.000000 cladeomatic-0.1.0/LICENSE
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-27 19:04:06.000000 cladeomatic-0.1.0/MANIFEST.in
+-rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-24 17:18:22.353746 cladeomatic-0.1.0/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)     9241 2023-03-31 20:37:18.000000 cladeomatic-0.1.0/README.md
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.337570 cladeomatic-0.1.0/cladeomatic/
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 18:18:38.000000 cladeomatic-0.1.0/cladeomatic/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    12959 2022-11-14 20:52:10.000000 cladeomatic-0.1.0/cladeomatic/benchmark.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    51241 2023-04-20 20:04:29.000000 cladeomatic-0.1.0/cladeomatic/clades.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2545 2023-04-20 19:54:43.000000 cladeomatic-0.1.0/cladeomatic/constants.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    51815 2023-04-19 17:46:08.000000 cladeomatic-0.1.0/cladeomatic/create.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    17214 2023-04-20 20:07:06.000000 cladeomatic-0.1.0/cladeomatic/genotype.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    34892 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/kmers.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1602 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/main.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2694 2022-12-08 20:22:59.000000 cladeomatic-0.1.0/cladeomatic/namer.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     7514 2023-04-19 15:06:51.000000 cladeomatic-0.1.0/cladeomatic/snps.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)        0 2022-06-09 17:34:28.000000 cladeomatic-0.1.0/cladeomatic/test.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.352278 cladeomatic-0.1.0/cladeomatic/utils/
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3440 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/__init__.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      961 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/jellyfish.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     6588 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/kmerSearch.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     9377 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/phylo_tree.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)    10264 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/seqdata.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)      742 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/snpdists.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     3207 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/vcfhelper.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1308 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/utils/visualization.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)       21 2023-04-21 13:45:27.000000 cladeomatic-0.1.0/cladeomatic/version.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     1071 2023-04-04 17:14:30.000000 cladeomatic-0.1.0/cladeomatic/visualize.py
+-rw-r--r--   0 jrobertson   (502) staff       (20)     5491 2023-04-19 14:55:01.000000 cladeomatic-0.1.0/cladeomatic/writers.py
+drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-04-24 17:18:22.343284 cladeomatic-0.1.0/cladeomatic.egg-info/
+-rw-r--r--   0 jrobertson   (502) staff       (20)      969 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/PKG-INFO
+-rw-r--r--   0 jrobertson   (502) staff       (20)      815 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       54 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/entry_points.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)      283 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/requires.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       12 2023-04-24 17:18:22.000000 cladeomatic-0.1.0/cladeomatic.egg-info/top_level.txt
+-rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-04-24 17:18:22.355036 cladeomatic-0.1.0/setup.cfg
+-rw-r--r--   0 jrobertson   (502) staff       (20)     2152 2023-04-24 17:18:06.000000 cladeomatic-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cladeomatic-0.0.1/LICENSE` & `cladeomatic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cladeomatic-0.0.1/PKG-INFO` & `cladeomatic-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cladeomatic
-Version: 0.0.1
+Version: 0.1.0
 Summary: Clade-O-Matic: Automatic recognition of population structures based on canonical SNPs
 Home-page: https://github.com/phac-nml/cladeomaticc
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Keywords: Genotyping,population structure,kmer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cladeomatic-0.0.1/README.md` & `cladeomatic-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [![PyPI](https://img.shields.io/badge/Install%20with-PyPI-blue)](https://pypi.org/project/chewBBACA/#description)
 [![Bioconda](https://img.shields.io/badge/Install%20with-bioconda-green)](https://anaconda.org/bioconda/chewbbaca)
-[![Conda](https://img.shields.io/conda/dn/bioconda/chewbbaca?color=green)](https://anaconda.org/bioconda/chewbbaca)
-[![chewBBACA](https://github.com/B-UMMI/chewBBACA/workflows/chewbbaca/badge.svg)](https://github.com/B-UMMI/chewBBACA/actions?query=workflow%3Achewbbaca)
-[![Documentation Status](https://readthedocs.org/projects/chewbbaca/badge/?version=latest)](https://chewbbaca.readthedocs.io/en/latest/?badge=latest)
-[![License: GPL v3](https://img.shields.io/github/license/B-UMMI/chewBBACA)](https://www.gnu.org/licenses/gpl-3.0)
-[![DOI:10.1099/mgen.0.000166](https://img.shields.io/badge/DOI-10.1099%2Fmgen.0.000166-blue)](http://mgen.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000166)
+[![Conda](https://img.shields.io/conda/dn/bioconda/cladeomatic?color=green)](https://anaconda.org/bioconda/chewbbaca)
+[![License: GPL v3](https://img.shields.io/github/license/phac-nml/cladeomatic)](https://www.apache.org/licenses/LICENSE-2.0)
+[![DOI:10.1099/](https://img.shields.io/badge/DOI-10.1099%2F-blue)]
 
 <p align="left"><img src="logo.png" alt="Clade-o-matic" height="150" width="400"></p>
 
 ## Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
@@ -38,15 +36,15 @@
 
 Install using pip:
 
         pip install cladeomatic
 
 Install the latest master branch version directly from Github:
 
-        conda install jellyfish
+        conda install jellyfish snp-dists
         pip install git+https://github.com/phac-nml/cladeomatic.git
 
 
 
 ## Usage
 If you run ``cladeomatic``, you should see the following usage statement:
 
@@ -71,24 +69,38 @@
 =====
 **Create scheme:**
 
 Option 1 - De novo tree-based <br />
 This mode will discover clades and lineages which meet membership size and SNP requirements. 
 Input requirements are: 
 * newick formatted tree
-* VCF
-* Reference sequence (.fasta / .gbk)
-* Name of outgroup sequence
+* Reference (Outgroup) sequence (.fasta / .gbk)
+* VCF (Must use the same reference sequence as above)
+* Name of Reference (Outgroup) sequence (Must be the same as the reference sequence)
 * Metadata file<br />
   
 
     cladeomatic create --in_nwk tree.nwk  --in_var variants.vcf --in_meta metadata.txt --outdir scheme/ --root_name ref --reference ref.gbk
 
 Option 2 - Predefined groups <br />
-This mode will attempt to define a scheme based on a group manifest which meet membership size and SNP requirements. 
+This mode will attempt to define a scheme based on a group manifest which meet membership size and SNP requirements.
+Note every group id must be unique accross all ranks to use this feature.Cladeomatic uses this for internal representation 
+of the genotypes but they can be mapped to whatever nomenclature is desired to have as an output
+
+| sample_id     | invalid_genotype | valid_genotype |
+| ----------- | ----------- |----------- | 
+| A      | 0.1      |   0.1         |
+| B   | 0.1.1.1        |     0.2.4.7       |
+| C     | 0.1.1.2       |    0.2.4.8        |
+| D   | 0.1.1.2        |       0.2.4.8       |
+| E      | 0.2      |       0.3     |
+| F   | 0.2.1        |      0.3.5     |
+| G   | 0.2.2        |       0.3.6   |
+| H   | 0.2.2        |      0.3.6      |
+
 Input requirements are: 
 * TSV formatted group file (sample_id, genotype)
 * VCF
 * Reference sequence (.fasta / .gbk)
 * Name of outgroup sequence
 * Metadata file<br />
   
@@ -96,37 +108,64 @@
     cladeomatic create --in_groups groups.tsv --in_var variants.vcf --in_meta metadata.txt --outdir scheme/ --root_name ref --reference ref.gbk
   
 
 **Outputs:**
 
 ```
 OutputFolderName
-├── {prefix}-clade.snp.histo.html [Tree Mode Only]
-├── {prefix}-clades.info.txt
-├── {prefix}-filt.kmers.txt
-├── {prefix}-genotypes.raw.txt
-├── {prefix}-genotypes.supported.txt
-├── {prefix}-genotypes.selected.txt
-├── {prefix}-genotype.consenus.fasta
-├── {prefix}-jellyfish.counts.txt
-├── {prefix}-scheme.txt
-├── {prefix}-snps.all.txt
-├── pseudo.seqs.fasta
-├── samples.dists.matrix.csv [Tree Mode Only]
+├── {prefix}-params.log - Selected parameters for the run
+├── {prefix}-clades.info.txt - Information on each individual clade, including supporting SNPs and metadata associations
+├── {prefix}-extracted.kmers.txt - Raw kmer output of extracted kmers with positions mapped
+├── {prefix}-genotypes.raw.txt - Tree or group file without filtering
+├── {prefix}-genotypes.supported.txt - Nodes which meet the user criteria
+├── {prefix}-genotypes.selected.txt - Nodes which were selected based on the supported nodes
+├── {prefix}-sample.distances.html - Histogram of node distances
+├── {prefix}-scheme.txt - Cladeomatic kmer based scheme
+├── {prefix}-snp.scheme.txt - Cladeomatic SNP based scheme
+├── {prefix}-filtered.vcf - VCF file where invalid sites have been removed
+├── pseudo.seqs.fasta - reconstructed fasta sequences based on reference sequence and vcf
+├── {prefix}-dist.mat.txt - tab delimeted distance matrix from snp-dists
+├── {prefix}-biohansel.fasta - biohansel formatted kmer fasta file
+├── {prefix}-biohansel.meta.txt - descriptions of biohansel kmers: kmername,target_position,target_base
+├── {prefix}-genotypes.distance.txt - defined threshold {single,average,complete}-linkage clusters
 └──
 ```
 
-**Benchmark Scheme:**
-Benchmark the scheme using the original input VCF file and the set of genomes used to construct the scheme.
+**Genotype:**
+Genotype samples using the developed scheme based on a VCF file with the same reference selected to build the scheme
 Input requirements are: 
 * VCF
 * Clade-O-Matic Scheme
-* Metadata file (sample_id,genotype) * Produced by "create" {prefix}-genotypes.selected.txt
+* (Optional) Metadata file (sample_id,genotype) * Produced by "create" {prefix}-genotypes.selected.txt
   
 
+    cladeomatic genotype --in_var variants.vcf --in_scheme cladeomatic-scheme.txt --in_meta metadata.txt --outdir benchmark/ 
+
+VCF files will not include positions which are exclusively the reference sequence or missing and this poses an issue for calling
+genotypes based on the VCF file where missing and reference state cannot be distinguished. A work around for this issue is the inclusion 
+of a sequence which is different from the reference sequence for every position targeted by the scheme. The create module generates a sequence 
+where every position used by the scheme is flipped to be a different base from the reference. This is not an ideal solution but it will allow
+users to use the genotype module using SNIPPY-CORE with their query sequence and the "alt" sequence.
+
+
+**Outputs:**
+Outputs a file with the genotype calls for each input sample
+```
+OutputFolderName
+└──  {prefix}.txt
+```
+
+
+
+**Benchmark Scheme:**
+Benchmark the scheme based on the output of genotype tool. At this point only vcf based genotyping is supported
+Input requirements are: 
+* TXT file produced by genotype module with predicted and expected genotypes
+
+
     cladeomatic benchmark --in_var variants.vcf --in_scheme cladeomatic-scheme.txt --in_meta metadata.txt --outdir benchmark/ 
 
 Evaluate the results for any conflicting genotypes
 
 
 **Outputs:**
```

### Comparing `cladeomatic-0.0.1/cladeomatic/benchmark.py` & `cladeomatic-0.1.0/cladeomatic/benchmark.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import sys
+
 import ray
 from cladeomatic.version import __version__
 from cladeomatic.utils.vcfhelper import vcfReader
 from cladeomatic.utils import init_console_logger
 from cladeomatic.utils import parse_metadata
 import pandas as pd
 from argparse import (ArgumentParser, ArgumentDefaultsHelpFormatter, RawDescriptionHelpFormatter)
@@ -64,55 +66,82 @@
     return profiles
 
 def parse_scheme_genotypes(scheme_file):
     scheme = {}
     df = pd.read_csv(scheme_file, sep="\t", header=0, low_memory=False)
     variant_positions = list(df['variant_start'].unique())
     geno_seqs = {}
+    snp_states = {}
     for row in df.itertuples():
         target_variant = row.target_variant
         variant_start = int(row.variant_start)
         positive_genotypes = row.positive_genotypes
         if isinstance(positive_genotypes,float):
             positive_genotypes = []
         else:
             positive_genotypes = positive_genotypes.split(',')
-        if len(positive_genotypes) == 0:
-            continue
+
         genotypes = positive_genotypes
         for genotype in positive_genotypes:
 
             if not genotype in scheme:
-                scheme[genotype] = {'positive':{},'partial':{}}
-            scheme[genotype]['positive'][variant_start] = target_variant
+                scheme[genotype] = {'positive':{},'partial':{},'allowed':{}}
+            if not variant_start in scheme[genotype]['positive']:
+                scheme[genotype]['positive'][variant_start] = set()
+            scheme[genotype]['positive'][variant_start].add(target_variant)
 
         partial_genotypes = row.partial_genotypes
 
+        if not variant_start in snp_states:
+            snp_states[variant_start] = set()
+        snp_states[variant_start].add(target_variant)
+
         if isinstance(partial_genotypes,float):
             partial_genotypes = []
         else:
             partial_genotypes = partial_genotypes.split(',')
         genotypes+= partial_genotypes
         if len(partial_genotypes) == 0:
             continue
         for genotype in partial_genotypes:
             if not genotype in scheme:
-                scheme[genotype] = {'positive':{},'partial':{}}
-            scheme[genotype]['partial'][variant_start] = target_variant
+                scheme[genotype] = {'positive':{},'partial':{},'allowed':{}}
+            if not variant_start in scheme[genotype]['partial']:
+                scheme[genotype]['partial'][variant_start] = set()
+            scheme[genotype]['partial'][variant_start].add(target_variant)
+
+
+    for genotype in scheme:
+        for pos in snp_states:
+            allowed_bases = set()
+            if pos in scheme[genotype]['partial']:
+                allowed_bases = allowed_bases | set(scheme[genotype]['partial'][pos])
+            if pos in scheme[genotype]['positive']:
+                allowed_bases = allowed_bases | set(scheme[genotype]['positive'][pos])
+            if len(allowed_bases) == 0:
+                allowed_bases = snp_states[pos]
+            scheme[genotype]['allowed'][pos] = allowed_bases
+
+
+    genotypes = list(scheme.keys())
+
+    for i in range(0,len(genotypes)):
+        g1 = genotypes[i]
+        a1 = scheme[g1]['allowed']
+        for k in range(i+1,len(genotypes)):
+            g2 = genotypes[k]
+            dist = 0
+            a2 = scheme[g2]['allowed']
+            for pos in a1:
+                int1 = a1[pos] & a2[pos]
+                if len(int1) == 1:
+                    dist+=1
+            if dist == 0:
+                print("{}\t{}\t{}".format(g1,g2,dist))
 
-        for genotype in genotypes:
-            if not genotype in geno_seqs:
-                geno_seqs[genotype] = {}
-                for pos in variant_positions:
-                    geno_seqs[genotype][pos] = 'N'
-            if geno_seqs[genotype][variant_start] == 'N':
-                geno_seqs[genotype][variant_start] = target_variant
-            else:
-                if geno_seqs[genotype][variant_start] != target_variant:
-                    geno_seqs[genotype][variant_start] = "N"
     return scheme
 
 @ray.remote
 def call_genotypes(genotype_rules,metadata,variants,max_dist=0):
     result = {}
     for sample_id in metadata:
         if not 'genotype' in metadata[sample_id]:
@@ -130,39 +159,43 @@
         genoytpe_results = {}
         dists = {}
         for genotype in genotype_rules:
             genoytpe_results[genotype] = {'match':{},'mismatch':{}}
             dists[genotype] = 1
 
         for pos in variants[sample_id]:
-            found_base = variants[sample_id][pos]
+            found_base = set(variants[sample_id][pos])
+            if '*' in found_base  or '-' in found_base or 'N' in found_base:
+
+                continue
+
             for genotype in genotype_rules:
-                if pos in genotype_rules[genotype]['positive']:
-                    target_base = genotype_rules[genotype]['positive'][pos]
-                    if found_base == target_base:
-                        genoytpe_results[genotype]['match'][pos] = found_base
-                    else:
-                        genoytpe_results[genotype]['mismatch'][pos] = found_base
-                elif pos in genotype_rules[genotype]['partial']:
-                    target_base = genotype_rules[genotype]['partial'][pos]
-                    if found_base == target_base:
-                        genoytpe_results[genotype]['match'][pos] = found_base
+                allowed_bases = genotype_rules[genotype]['allowed'][pos]
+
+                if len(found_base & allowed_bases) == 1:
+                    genoytpe_results[genotype]['match'][pos] = found_base
+
+                else:
+                    genoytpe_results[genotype]['mismatch'][pos] = found_base
+
+
 
         for genotype in genoytpe_results:
             matches = len(genoytpe_results[genotype]['match'])
             mismatches = len(genoytpe_results[genotype]['mismatch'])
             total = matches + mismatches
             if total > 0:
                 dists[genotype] = 1 - matches /total
 
 
         result[sample_id]['genoytpe_dists'] =  {k: v for k, v in sorted(dists.items(), key=lambda item: item[1])}
         pdist = 1
         for genotype in result[sample_id]['genoytpe_dists']:
             dist =  result[sample_id]['genoytpe_dists'][genotype]
+
             if dist <= pdist and dist <= max_dist:
                 result[sample_id]['predicted_genotype(s)'].append(genotype)
                 result[sample_id]['predicted_genotype_dist'] = dist
                 pdist = dist
 
         num_geno = len(result[sample_id]['predicted_genotype(s)'])
         if num_geno > 1:
@@ -172,14 +205,15 @@
                 for k in range(i+1,num_geno):
                     if "{}.".format(result[sample_id]['predicted_genotype(s)'][i]) in result[sample_id]['predicted_genotype(s)'][k]:
                         is_substring = True
                 if not is_substring:
                     filt.append(result[sample_id]['predicted_genotype(s)'][i])
             result[sample_id]['predicted_genotype(s)'] = filt
         del result[sample_id]['genoytpe_dists']
+
         #del result[sample_id]['genoytpe_results']
         #print("{}\t{}".format(sample_id,time.time() - stime))
     return result
 
 def run():
     cmd_args = parse_args()
     scheme_file = cmd_args.in_scheme
@@ -202,14 +236,17 @@
 
     logging.info("Reading metadata file {}".format(metadata_file))
     metadata = parse_metadata(metadata_file)
 
 
     logging.info("Reading scheme file {}".format(scheme_file))
     genotype_rules = parse_scheme_genotypes(scheme_file)
+    for genotype in genotype_rules:
+        if len(genotype_rules[genotype]['positive']) == 0:
+            logging.warn("Genotype {} has no required kmers".format(genotype))
     rule_id = ray.put(genotype_rules)
     num_genotypes = len(genotype_rules)
 
 
     valid_positions = []
     for genotype in genotype_rules:
         for state in genotype_rules[genotype]:
@@ -294,12 +331,12 @@
         for i in range(0,num_samples):
             sample_id = samples[i]
             if sample_id in group_samples[genotype]['truth']:
                 truth[i] = 1
             if sample_id in group_samples[genotype]['pred']:
                 pred[i] = 1
         geno_f1 = f1_score(truth, pred)
-        fh.write("{}\t{}\t{}\t{}\n".format(genotype,num_true,num_samples,geno_f1))
+        fh.write("{}\t{}\t{}\t{}\n".format(genotype,num_true,sum(pred),geno_f1))
     fh.close()
 
     logging.info("Analysis complete")
```

### Comparing `cladeomatic-0.0.1/cladeomatic/utils/jellyfish.py` & `cladeomatic-0.1.0/cladeomatic/utils/jellyfish.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import pandas as pd
 from cladeomatic.utils import run_command
 import pandas as pd
+from deprecated import deprecated
 
 from cladeomatic.utils import run_command
 
-
+@deprecated
 def run_jellyfish_count(seq_file,out_file,mem='10M',k=21,n_threads=1,jf_out=False):
     if jf_out:
         cmd = "jellyfish count -t {} -m {} -s {} -C -o {} {}".format(n_threads, k, mem, out_file, seq_file)
     else:
         cmd = "jellyfish count --text -t {} -m {} -s {} -C -o {} {}".format(n_threads,k,mem,out_file,seq_file)
 
     (stdout,stderr) = run_command(cmd)
     print(stdout)
     print(stderr)
     return (stdout,stderr)
-
+@deprecated()
 def run_jellyfish_query(seq_file,jellyfish_mers,out_file):
     cmd = "jellyfish query -o {} {} {}".format(out_file, seq_file, jellyfish_mers)
     (stdout,stderr) = run_command(cmd)
     return (stdout,stderr)
 
 
-
+@deprecated()
 def parse_jellyfish_counts(file):
     return pd.read_csv(file,skiprows=1, header=None,names=['kmer','count'],sep=' ')
```

### Comparing `cladeomatic-0.0.1/cladeomatic/utils/phylo_tree.py` & `cladeomatic-0.1.0/cladeomatic/utils/phylo_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 import os
 
 import dendropy
 from ete3 import Tree, NodeStyle, TreeStyle, TextFace, RectFace
+from deprecated import deprecated
 
 
 if not 'DISPLAY' in os.environ:
     os.environ['QT_QPA_PLATFORM']='offscreen'
 
+@deprecated()
 def tree_to_distance_matrix(tree_file,out_file):
-    '''
-
-    Parameters
-    ----------
-    tree_file
-    out_file
-
-    Returns
-    -------
-
-    '''
+    """
+    This method converts a dendropy tree object to a distance
+    matrix and writes this matrix to a csv file
+    :param tree_file: String - the path to the tree file (newick format only)
+    :param out_file: String - the path to the CSV output file for the distance
+    matrix
+    """
     tree = dendropy.Tree.get(path=tree_file, schema='newick')
     pdm = tree.phylogenetic_distance_matrix()
     pdm.write_csv(out_file)
 
+@deprecated()
 def get_pairwise_distances_from_matrix(matrix_file):
-    '''
-
-    Parameters
-    ----------
-    matrix_file: str path to file
-
-    Returns list of distances
-    -------
-
-    '''
+    """
+    This method gets the pairwise distances from the passed matrix file
+    and adds them to a list
+    :param matrix_file:
+    :return: list - the list of the pairwise distances
+    """
     dists = []
     with open(matrix_file,'r') as fh:
         line = next(fh)
         for line in fh:
             row = line.split(',')
             dists += [float(x) for x in row[1:]]
         fh.close()
     return dists
 
-
-
 def remove_unsupported_clades(ete_tree_obj, valid_clades):
     """
     Remove non-leaf nodes from the tree while maintaining children
-    :param ete_tree_obj: [ETE obj] Phylogenetic tree
-    :param valid_clades: [list] Valid node names to maintain
-    :return: ete_tree_obj: [ETE obj] Phylogenetic tree with only nodes in the valid list
+    :param ete_tree_obj: ETE3 obj - Phylogenetic tree
+    :param valid_clades: list - Valid node names to maintain
+    :return: ete_tree_obj: ETE3 obj - Phylogenetic tree with only nodes in the valid list
     """
     tree = ete_tree_obj.copy()
 
     for node in tree.traverse("preorder"):
         if node.is_root() or node.is_leaf():
             continue
 
         node_id = node.name
         remove_node = True
         if node_id in valid_clades:
             remove_node = False
         if remove_node:
             node.delete()
-
     return tree
 
+@deprecated()
 def prune_tree(ete_tree_obj,valid_nodes):
     """
-    :param ete_tree_obj: [ETE obj] Tree object
-    :param valid_nodes: [List] Node names which are valide
-    :return: [ETE Tree ] With only valid nodes
+    This method removes nodes from the ETE3 tree object
+    that are not part of the list of valid node names
+    :param ete_tree_obj: ETE3 obj - Tree object for pruning
+    :param valid_nodes: List - Node names which are valid
+    :return: list - A list of both the ETE3 tree object and the list
+    of only valid nodes
     """
     invalid_nodes = []
+    #traverse the tree to make a list of invalid nodes
     for node in ete_tree_obj.traverse("postorder"):
         node_id = node.name
         if node.is_leaf() or node_id not in valid_nodes:
             continue
         node_ancestors = node.get_ancestors()
 
         for n in node_ancestors:
@@ -109,19 +106,15 @@
     ete_format [int] : Refer to documentation http://etetoolkit.org/docs/latest/reference/reference_tree.html
     set_root [Bool] : Set root for the tree
     resolve_polytomy [Bool]: Force bifurcations of the tree on polytomies
     ladderize [Bool] : Sort the branches of a given tree (swapping children nodes) according to the size
     method [str]: Method to root tree, either midpoint or outgroup
     outgroup [str] : Name of taxon to root tree on
 
-    Returns
-    -------
-
-    ETE tree obj
-
+    Returns ETE tree obj
     """
 
     logging.info("Attempting to parse tree file {}".format(tree_file))
 
     if not os.path.isfile(tree_file):
         logging.error("Specified tree file {} is not found, please check that it exists".format(tree_file))
         return dict()
@@ -199,18 +192,19 @@
         logging.error("Error the tree is unrooted, you must either specify the root using an outgroup or midpoint rooting")
 
     return t
 
 
 def get_internal_clades(ete_tree_obj):
     """
-    Identify internal nodes in the ETE3 tree and return a dict of the samples associated with that clade
+    Identify internal nodes in the ETE3 tree and return a dict of the samples
+    associated with that clade
     Parameters
     ----------
-    ete_tree_obj [ETE tree obj] :
+    ete_tree_obj [ETE tree obj] :the ETE3 otree object for parsing
 
     Returns
     -------
     clade_dict [dict]: Dictionary of tree nodes which are not leaves
 
     """
     cache = ete_tree_obj.get_cached_content()
@@ -219,30 +213,53 @@
         clade_id = clade.name
         children = clade.get_leaf_names()
         if len(children) == 1:
             continue
         clade_dict[clade_id] = children
     return clade_dict
 
+@deprecated()
 def init_clade_info(ete_tree_obj):
+    """
+    This method initializes the clade dictionary for the tree passed.
+    It parses the tree to find the internal clade memberships and
+    sets these to a dictionary
+    :param ete_tree_obj: ete3 tree object - the tree to parse for clade
+    memberships
+    :return: the initializd clade memberhsip dictionary for the tree passed
+    """
     clade_info = {}
     memberships = get_internal_clades(ete_tree_obj)
 
     for clade_id in memberships:
         clade_info[clade_id] = {'num_members':len(memberships[clade_id]),'membership':set(memberships[clade_id]),'canSNPs':{},'canSNP_count':0}
 
     return clade_info
 
 
+@deprecated()
 def get_tree_node_distances(ete_tree_obj):
+    """
+    This method creates a dictionary of tree distances for the
+    ETE3 tree object passed
+    :param ete_tree_obj: ETE3 object - the tree to determine distances for
+    :return: dictionary - the dictionary of the node name and the distance calculated
+    """
     distances = {}
     for node in ete_tree_obj.iter_descendants("preorder"):
         distances[node.name] = node.dist
     return distances
 
+@deprecated()
 def get_tree_node_bootstrap(ete_tree_obj):
+    """
+    A method to determine the branch support for the branches in the
+    ETE3 tree object passes
+    :param ete_tree_obj: ETE3 tree object - the tree to parse
+    :return: dictionary - the dictionary of node names and their support value
+    """
     support = {}
     for node in ete_tree_obj.iter_descendants("preorder"):
         support[node.name] = node.support
 
     return support
```

### Comparing `cladeomatic-0.0.1/cladeomatic.egg-info/PKG-INFO` & `cladeomatic-0.1.0/cladeomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cladeomatic
-Version: 0.0.1
+Version: 0.1.0
 Summary: Clade-O-Matic: Automatic recognition of population structures based on canonical SNPs
 Home-page: https://github.com/phac-nml/cladeomaticc
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Keywords: Genotyping,population structure,kmer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cladeomatic-0.0.1/cladeomatic.egg-info/SOURCES.txt` & `cladeomatic-0.1.0/cladeomatic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 cladeomatic/__init__.py
 cladeomatic/benchmark.py
+cladeomatic/clades.py
 cladeomatic/constants.py
 cladeomatic/create.py
+cladeomatic/genotype.py
+cladeomatic/kmers.py
 cladeomatic/main.py
-cladeomatic/simulate_genomes.py
+cladeomatic/namer.py
+cladeomatic/snps.py
 cladeomatic/test.py
 cladeomatic/version.py
+cladeomatic/visualize.py
+cladeomatic/writers.py
 cladeomatic.egg-info/PKG-INFO
 cladeomatic.egg-info/SOURCES.txt
 cladeomatic.egg-info/dependency_links.txt
 cladeomatic.egg-info/entry_points.txt
 cladeomatic.egg-info/requires.txt
 cladeomatic.egg-info/top_level.txt
 cladeomatic/utils/__init__.py
 cladeomatic/utils/jellyfish.py
 cladeomatic/utils/kmerSearch.py
 cladeomatic/utils/phylo_tree.py
 cladeomatic/utils/seqdata.py
+cladeomatic/utils/snpdists.py
 cladeomatic/utils/vcfhelper.py
 cladeomatic/utils/visualization.py
```

### Comparing `cladeomatic-0.0.1/setup.py` & `cladeomatic-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import os
 from distutils.core import setup
 from setuptools import find_packages
-
+from cladeomatic.version import __version__
 author = 'James Robertson'
 
 classifiers = """
 Development Status :: 3 - Alpha
 Environment :: Console
 License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 
 
 exec(open('cladeomatic/version.py').read())
 
 setup(
     name='cladeomatic',
     include_package_data=True,
-    version='0.0.1',
+    version=__version__,
     python_requires='>=3.8.0,<4',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     packages=find_packages(exclude=['tests']),
     url='https://github.com/phac-nml/cladeomaticc',
     license='GPLv3',
     author='James Robertson',
@@ -44,29 +44,32 @@
     classifiers=classifiers,
     package_dir={'cladeomatic': 'cladeomatic'},
     package_data={
         "": ["*.txt", "*.fasta","*.html","*.gb"],
     },
 
     install_requires=[
-        'numpy',
-        'pandas',
-        'biopython',
-        'scipy',
-        'six',
-        'matplotlib',
-        'argparse',
-        'statistics',
-        'plotly',
-        'ete3',
-        'jellyfish',
-        'DendroPy',
-        'pyahocorasick',
-        'PyQt5',
-        'ray'
+        'numpy==1.23.0',
+        'pandas==2.0.1',
+        'biopython==1.81',
+        'six==1.16.0',
+        'matplotlib==3.7.1',
+        'argparse==1.4.0',
+        'statistics==1.0.3.5',
+        'plotly==5.14.1',
+        'ete3==3.1.2',
+        'jellyfish==0.9.0',
+        'DendroPy==4.5.2',
+        'PyQt5==5.15.9',
+        'ray==2.3.1',
+        'deprecated==1.2.13',
+        'psutil==5.9.1',
+        'scikit-learn==1.1.1',
+        'scipy==1.10.1',
+        'pyahocorasick==1.4.4',
 
     ],
 
     entry_points={
         'console_scripts': [
             'cladeomatic=cladeomatic.main:main',
         ],
```


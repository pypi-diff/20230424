# Comparing `tmp/genotations-0.1.5.tar.gz` & `tmp/genotations-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genotations-0.1.5.tar", last modified: Fri Mar 17 16:15:38 2023, max compression
+gzip compressed data, was "genotations-0.1.6.tar", last modified: Mon Apr 24 01:33:31 2023, max compression
```

## Comparing `genotations-0.1.5.tar` & `genotations-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-17 16:15:38.719301 genotations-0.1.5/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3255 2023-03-17 16:15:38.719301 genotations-0.1.5/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2602 2023-03-02 13:56:49.000000 genotations-0.1.5/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-17 16:15:38.719301 genotations-0.1.5/examples/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-02 13:40:07.000000 genotations-0.1.5/examples/__init__.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-17 16:15:38.719301 genotations-0.1.5/genotations/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       21 2023-03-02 13:40:07.000000 genotations-0.1.5/genotations/__init__.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    25871 2023-03-17 15:49:59.000000 genotations-0.1.5/genotations/ensembl.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    21909 2023-03-02 13:40:07.000000 genotations-0.1.5/genotations/genomes.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3557 2023-03-02 13:40:07.000000 genotations-0.1.5/genotations/intersections.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    15203 2023-03-02 13:40:07.000000 genotations-0.1.5/genotations/primers.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4837 2023-03-05 01:13:02.000000 genotations-0.1.5/genotations/quantification.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-17 16:15:38.719301 genotations-0.1.5/genotations.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3255 2023-03-17 16:15:38.000000 genotations-0.1.5/genotations.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      365 2023-03-17 16:15:38.000000 genotations-0.1.5/genotations.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-03-17 16:15:38.000000 genotations-0.1.5/genotations.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       79 2023-03-17 16:15:38.000000 genotations-0.1.5/genotations.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       21 2023-03-17 16:15:38.000000 genotations-0.1.5/genotations.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-03-17 16:15:38.719301 genotations-0.1.5/setup.cfg
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1284 2023-03-17 16:15:03.000000 genotations-0.1.5/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-04-24 01:33:31.951071 genotations-0.1.6/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3752 2023-04-24 01:33:31.951071 genotations-0.1.6/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3099 2023-03-19 00:13:13.000000 genotations-0.1.6/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-04-24 01:33:31.947071 genotations-0.1.6/examples/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-03-02 13:40:07.000000 genotations-0.1.6/examples/__init__.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-04-24 01:33:31.947071 genotations-0.1.6/genotations/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       21 2023-03-02 13:40:07.000000 genotations-0.1.6/genotations/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    25871 2023-03-17 15:49:59.000000 genotations-0.1.6/genotations/ensembl.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    21845 2023-04-24 01:31:40.000000 genotations-0.1.6/genotations/genomes.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3560 2023-04-24 01:32:20.000000 genotations-0.1.6/genotations/intersections.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    15203 2023-03-02 13:40:07.000000 genotations-0.1.6/genotations/primers.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4830 2023-04-24 01:32:44.000000 genotations-0.1.6/genotations/quantification.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-04-24 01:33:31.951071 genotations-0.1.6/genotations.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3752 2023-04-24 01:33:31.000000 genotations-0.1.6/genotations.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      365 2023-04-24 01:33:31.000000 genotations-0.1.6/genotations.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-04-24 01:33:31.000000 genotations-0.1.6/genotations.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       79 2023-04-24 01:33:31.000000 genotations-0.1.6/genotations.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       21 2023-04-24 01:33:31.000000 genotations-0.1.6/genotations.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-04-24 01:33:31.951071 genotations-0.1.6/setup.cfg
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1284 2023-04-24 01:32:02.000000 genotations-0.1.6/setup.py
```

### Comparing `genotations-0.1.5/PKG-INFO` & `genotations-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genotations
-Version: 0.1.5
+Version: 0.1.6
 Summary: Genotations - python library to work with genomes and primers
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
@@ -33,14 +33,34 @@
 Usage
 =====
 
 Install with pip:
 ```bash
 pip install genotations
 ```
+In some cases you may also need to install ucsc annotation tools, you can add them to your micromamba/conda environment as they are installed from bioconda channel.
+Here how it may look in your environment file:
+```yaml
+name: genotations
+channels:
+  - conda-forge
+  - BjornFJohansson
+  - bioconda
+  - defaults
+dependencies:
+  - python=3.10
+  - ucsc-bedtogenepred
+  - ucsc-genepredtobed
+  - ucsc-genepredtogtf
+  - ucsc-gff3togenepred
+  - ucsc-gtftogenepred
+  - pip
+  - pip:
+      - genotations
+```
 
 Now you can start using it, for example:
 ```python
 from genotations import ensembl
 human = ensembl.human # getting human genome
 mouse = ensembl.mouse # getting mosue genome
 mouse.annotations.exons().annotations_df # getting exons as DataFrame
```

### Comparing `genotations-0.1.5/README.md` & `genotations-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,34 @@
 Usage
 =====
 
 Install with pip:
 ```bash
 pip install genotations
 ```
+In some cases you may also need to install ucsc annotation tools, you can add them to your micromamba/conda environment as they are installed from bioconda channel.
+Here how it may look in your environment file:
+```yaml
+name: genotations
+channels:
+  - conda-forge
+  - BjornFJohansson
+  - bioconda
+  - defaults
+dependencies:
+  - python=3.10
+  - ucsc-bedtogenepred
+  - ucsc-genepredtobed
+  - ucsc-genepredtogtf
+  - ucsc-gff3togenepred
+  - ucsc-gtftogenepred
+  - pip
+  - pip:
+      - genotations
+```
 
 Now you can start using it, for example:
 ```python
 from genotations import ensembl
 human = ensembl.human # getting human genome
 mouse = ensembl.mouse # getting mosue genome
 mouse.annotations.exons().annotations_df # getting exons as DataFrame
```

### Comparing `genotations-0.1.5/genotations/ensembl.py` & `genotations-0.1.6/genotations/ensembl.py`

 * *Files identical despite different names*

### Comparing `genotations-0.1.5/genotations/genomes.py` & `genotations-0.1.6/genotations/genomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,31 +126,32 @@
                              dtypes={
                                  #sometimes polars makes mistakes in automatic type derivation with some fields
                                  "seqname": pl.Utf8, #pl.Categorical,
                                  "start": pl.UInt64, "end": pl.UInt64,
                                  "strand": pl.Categorical
                              }
                              )
-        transcript_exon_compute = (self.transcript_name_col+pl.lit("_")+pl.col("exon_number")).alias("transcript_exon")
+        transcript_exon_compute = (self.transcript_name_col+pl.lit("_")+pl.col("exon_number").cast(pl.Utf8)).alias("transcript_exon")
         # does some preprocessing, mostly extracting attributes (which are multiple per cell in GTF files) to separate columns with regular expressions
-        result = loaded \
-                 .with_column(att.str.extract("gene_id \"[a-zA-Z0-9_.-]*", 0).str.replace("gene_id \"", "").alias("gene")) \
-                 .with_column(att.str.extract("gene_name \"[a-zA-Z0-9_.-]*", 0).str.replace("gene_name \"", "").alias("gene_name")) \
-                 .with_column(att.str.extract("gene_biotype \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_biotype \"", "").alias("transcript_biotype")) \
-                 .with_column(att.str.extract("transcript_id \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_id \"", "").alias("transcript")) \
-                 .with_column(att.str.extract("transcript_name \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_name \"", "").alias("transcript_name")) \
-                 .with_column(att.str.extract("transcript_biotype \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_biotype \"", "").alias("transcript_biotype")) \
-                 .with_column(att.str.extract("exon_id \"[a-zA-Z0-9_.-]*", 0).str.replace("exon_id \"", "").cast(pl.Utf8).alias("exon")) \
-                 .with_column(att.str.extract("exon_number \"[0-9_.-]*", 0).str.replace("exon_number \"", "").cast(pl.UInt64).alias("exon_number")) \
-                 .with_column(transcript_exon_compute)
+        cols = [
+            att.str.extract("gene_id \"[a-zA-Z0-9_.-]*", 0).str.replace("gene_id \"", "").alias("gene") ,
+            att.str.extract("gene_name \"[a-zA-Z0-9_.-]*", 0).str.replace("gene_name \"", "").alias("gene_name"),
+            att.str.extract("gene_biotype \"[a-zA-Z0-9_.-]*", 0).str.replace("gene_biotype \"", "").alias("gene_biotype"),
+            att.str.extract("transcript_id \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_id \"", "").alias("transcript"),
+            att.str.extract("transcript_name \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_name \"", "").alias("transcript_name"),
+            att.str.extract("transcript_biotype \"[a-zA-Z0-9_.-]*", 0).str.replace("transcript_biotype \"", "").alias("transcript_biotype"),
+            att.str.extract("exon_id \"[a-zA-Z0-9_.-]*", 0).str.replace("exon_id \"", "").cast(pl.Utf8).alias("exon"),
+            att.str.extract("exon_number \"[0-9_.-]*", 0).str.replace("exon_number \"", "").cast(pl.UInt64).alias("exon_number"),
+        ]
+        result = loaded.with_columns(cols).with_columns([transcript_exon_compute])
         return result
 
 
     def with_coordinates_column(self) -> 'Annotations':
-        return self if "coordinates" in self.annotations_df.columns else Annotations(self.annotations_df.with_column(self.coordinates_compute_col))
+        return self if "coordinates" in self.annotations_df.columns else Annotations(self.annotations_df.with_columns([self.coordinates_compute_col]))
 
     def has_sequence(self) -> bool:
         return "sequence" in self.annotations_df.columns
 
     def _optional_sequence(self, selection: list[pl.col]) -> list[pl.col]:
         return selection + [self.sequence_col] if self.has_sequence() else selection
 
@@ -303,19 +304,22 @@
         return seq(strings).fold_left( ((0, 0),), lambda acc, el: acc + ((acc[-1][0]+acc[-1][1], len(el)),) ).to_list()[1:]
 
     def get_transcript_sequences(self, genome: genomepy.genome = None, strand: Strand = Strand.Undefined) -> pl.DataFrame:
         assert genome is not None or self.has_sequence(), "there should be either sequence or genome available!"
         if not self.has_sequence():
             return self.with_sequences(genome, strand).get_transcript_sequences()
         else:
+            extra_cols = [
+                pl.col("sequence").apply(self._strings_to_spans).alias("spans"),
+                pl.col("sequence").apply(lambda r: seq(r).reduce(lambda a,b : a+b)).alias("mRNA")
+            ]
             return self.annotations_df.sort([self.transcript_name_col, self.exon_number_col])\
                 .groupby(self.transcript_name_col, maintain_order=True)\
                 .agg([self.sequence_col])\
-                .with_column(pl.col("sequence").apply(self._strings_to_spans).alias("spans"))\
-                .with_column(pl.col("sequence").apply(lambda r: seq(r).reduce(lambda a,b : a+b)).alias("mRNA"))
+                .with_columns(extra_cols)
 
     @cached_property
     def transcript_gene_names_df(self) -> pl.DataFrame:
         """
         Getting just  Ensembl Transcript id -> Transcript name and Ensembl gene id -> gene name correspondence is a common task as we often want to join such dataframe with others
         :return: NOTE: returns dataframe and not self, _df suffix means dataframe
         """
@@ -450,17 +454,17 @@
         if "sequence" in self.annotations_df.columns:
             print("sequence column already exists, no work needed!")
             return self
         else:
             if self.annotations_df.shape[0] > 100:
                 print(f"There are {self.annotations_df.shape} annotations, loading sequences can take quite a while!")
             extract_sequence = functools.partial(_get_sequence_from_series, genome=genome, strand=strand)
-            with_sequences = self.with_coordinates_column().annotations_df.with_column(self.coordinates_col.apply(extract_sequence).alias("sequence"))
+            with_sequences = self.with_coordinates_column().annotations_df.with_columns([self.coordinates_col.apply(extract_sequence).alias("sequence")])
             return Annotations(with_sequences)
 
     def get_intervals_with_set(self):
         """
         gets interval sets, used for primers selection and other purposes
         :return:
         """
-        return self.annotations_df.with_column(self.coordinates_col) \
+        return self.annotations_df.with_columns([self.coordinates_col]) \
             .select([pl.col("seqname"), pl.col("start"), pl.col("end")]).distinct().apply(lambda r: (set(r[0]), r[1], r[2])).rows()
```

### Comparing `genotations-0.1.5/genotations/intersections.py` & `genotations-0.1.6/genotations/intersections.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class TranscriptIntersection:
     @staticmethod
     def extract_intervals(annotations: genotations.genomes.Annotations):
         """
         gets transcript interval, used for primers selection and other purposes
         :return:
         """
-        return seq(annotations.annotations_df.with_column(annotations.coordinates_col).sort(pl.col("start"))\
+        return seq(annotations.annotations_df.with_columns([annotations.coordinates_col]).sort(pl.col("start"))\
                    .select([annotations.transcript_exon_col, pl.col("seqname"), pl.col("start"), pl.col("end")])\
                    .rows()).map(lambda row: TranscriptIntersection({row[0]}, row[1], row[2], row[3]))
 
 
     """
     TODO: move to primers module
     """
```

### Comparing `genotations-0.1.5/genotations/primers.py` & `genotations-0.1.6/genotations/primers.py`

 * *Files identical despite different names*

### Comparing `genotations-0.1.5/genotations/quantification.py` & `genotations-0.1.6/genotations/quantification.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :param path:
     :param transcripts:
     :return:
     """
     alias = "transcript" if transcripts else "gene"
     gene = pl.col("Name").str.split(".").apply(lambda s: s[0]).alias(alias)
     dtypes={"TPM": pl.datatypes.Float64, "EffectiveLength": pl.datatypes.Float64, "NumReads": pl.datatypes.Float64}
-    return pl.read_csv(path, sep="\t", dtypes = dtypes).with_column(gene).select([gene, pl.col("TPM"), pl.col("EffectiveLength"), pl.col("NumReads")])
+    return pl.read_csv(path, sep="\t", dtypes = dtypes).with_columns([gene]).select([gene, pl.col("TPM"), pl.col("EffectiveLength"), pl.col("NumReads")])
 
 
 def quant_from_run(run: Path, name_part: str = "quant.sf", dir_part: str = "quant_") -> Optional[pl.DataFrame]:
     transcripts = "gene" not in dir_part and "gene" not in name_part
     qq = dirs(run).filter(lambda f: dir_part in f.name)
     if qq.len() < 1:
         print(f"could not find quantification data for {run}")
@@ -104,15 +104,15 @@
                                ) -> pl.DataFrame:
     """
     :param df:
     :return:
     """
     sums = pl.sum(tpm_columns).alias("sum_TPM")
     avg = (sums / df.select(tpm_columns).shape[1]).alias("avg_TPM")
-    df = df.with_column(sums).with_column(avg).sort(avg, True)
+    df = df.with_column([sums, avg]).sort(avg, True)
     return df if min_avg_value <= 0.0 else df.filter(pl.col("avg_TPM") >= min_avg_value)
 
 
 def summarized_expressions_from_bioproject(project: Path, transcripts: bool = True,
                                            tpm_columns: Union[pl.Expr, list[pl.Expr], "str", list[str]] = pl.col("^SRR[a-zA-Z0-9]+$")):
     expressions = expressions_from_bioproject(project, transcripts)
     return with_expressions_summaries(expressions, tpm_columns)
```

### Comparing `genotations-0.1.5/genotations.egg-info/PKG-INFO` & `genotations-0.1.6/genotations.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genotations
-Version: 0.1.5
+Version: 0.1.6
 Summary: Genotations - python library to work with genomes and primers
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
@@ -33,14 +33,34 @@
 Usage
 =====
 
 Install with pip:
 ```bash
 pip install genotations
 ```
+In some cases you may also need to install ucsc annotation tools, you can add them to your micromamba/conda environment as they are installed from bioconda channel.
+Here how it may look in your environment file:
+```yaml
+name: genotations
+channels:
+  - conda-forge
+  - BjornFJohansson
+  - bioconda
+  - defaults
+dependencies:
+  - python=3.10
+  - ucsc-bedtogenepred
+  - ucsc-genepredtobed
+  - ucsc-genepredtogtf
+  - ucsc-gff3togenepred
+  - ucsc-gtftogenepred
+  - pip
+  - pip:
+      - genotations
+```
 
 Now you can start using it, for example:
 ```python
 from genotations import ensembl
 human = ensembl.human # getting human genome
 mouse = ensembl.mouse # getting mosue genome
 mouse.annotations.exons().annotations_df # getting exons as DataFrame
```

### Comparing `genotations-0.1.5/setup.py` & `genotations-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Genotations - python library to work with genomes and primers'
 LONG_DESCRIPTION = 'Genotations - python library to work with genomes and primers'
 
 # Setting up
 setup(
     name="genotations",
     version=VERSION,
```


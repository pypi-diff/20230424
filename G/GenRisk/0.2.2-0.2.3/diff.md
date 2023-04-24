# Comparing `tmp/GenRisk-0.2.2.tar.gz` & `tmp/GenRisk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenRisk-0.2.2.tar", last modified: Wed Mar 22 13:29:16 2023, max compression
+gzip compressed data, was "GenRisk-0.2.3.tar", last modified: Mon Apr 24 13:19:34 2023, max compression
```

## Comparing `GenRisk-0.2.2.tar` & `GenRisk-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-03-22 13:29:16.033590 GenRisk-0.2.2/
--rw-r--r--   0 raldisi    (501) staff       (20)     1068 2021-07-21 16:39:45.000000 GenRisk-0.2.2/LICENSE
--rw-r--r--   0 raldisi    (501) staff       (20)     4390 2023-03-22 13:29:16.033777 GenRisk-0.2.2/PKG-INFO
--rw-r--r--   0 raldisi    (501) staff       (20)     3155 2023-03-15 14:48:24.000000 GenRisk-0.2.2/README.md
--rw-r--r--   0 raldisi    (501) staff       (20)      103 2021-10-18 09:34:04.000000 GenRisk-0.2.2/pyproject.toml
--rw-r--r--   0 raldisi    (501) staff       (20)     1081 2023-03-22 13:29:16.034407 GenRisk-0.2.2/setup.cfg
--rw-r--r--   0 raldisi    (501) staff       (20)      115 2021-07-21 16:39:45.000000 GenRisk-0.2.2/setup.py
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-03-22 13:29:16.018733 GenRisk-0.2.2/src/
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-03-22 13:29:16.025071 GenRisk-0.2.2/src/GenRisk.egg-info/
--rw-r--r--   0 raldisi    (501) staff       (20)     4390 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/PKG-INFO
--rw-r--r--   0 raldisi    (501) staff       (20)      556 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/SOURCES.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        1 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/dependency_links.txt
--rw-r--r--   0 raldisi    (501) staff       (20)       46 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/entry_points.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        1 2021-10-18 14:25:34.000000 GenRisk-0.2.2/src/GenRisk.egg-info/not-zip-safe
--rw-r--r--   0 raldisi    (501) staff       (20)      203 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/requires.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        8 2023-03-22 13:29:15.000000 GenRisk-0.2.2/src/GenRisk.egg-info/top_level.txt
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-03-22 13:29:16.033002 GenRisk-0.2.2/src/genrisk/
--rw-r--r--   0 raldisi    (501) staff       (20)       32 2021-07-21 16:39:45.000000 GenRisk-0.2.2/src/genrisk/__init__.py
--rw-r--r--   0 raldisi    (501) staff       (20)      154 2021-10-12 12:05:52.000000 GenRisk-0.2.2/src/genrisk/__main__.py
--rw-r--r--   0 raldisi    (501) staff       (20)     6933 2022-03-01 12:52:55.000000 GenRisk-0.2.2/src/genrisk/association_analysis.py
--rw-r--r--   0 raldisi    (501) staff       (20)    30612 2023-03-22 10:19:03.000000 GenRisk-0.2.2/src/genrisk/cli.py
--rw-r--r--   0 raldisi    (501) staff       (20)     9588 2023-03-09 14:28:42.000000 GenRisk-0.2.2/src/genrisk/gene_scoring.py
--rw-r--r--   0 raldisi    (501) staff       (20)     3374 2022-08-20 08:52:58.000000 GenRisk-0.2.2/src/genrisk/helpers.py
--rw-r--r--   0 raldisi    (501) staff       (20)    15513 2023-03-22 13:21:54.000000 GenRisk-0.2.2/src/genrisk/pipeline.py
--rw-r--r--   0 raldisi    (501) staff       (20)     7939 2022-08-17 08:46:38.000000 GenRisk-0.2.2/src/genrisk/prediction_models.py
--rw-r--r--   0 raldisi    (501) staff       (20)     2838 2022-02-04 09:26:13.000000 GenRisk-0.2.2/src/genrisk/prs_scoring.py
--rw-r--r--   0 raldisi    (501) staff       (20)     5572 2022-08-22 10:23:10.000000 GenRisk-0.2.2/src/genrisk/utils.py
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 13:19:34.094955 GenRisk-0.2.3/
+-rw-r--r--   0 raldisi    (501) staff       (20)     1068 2021-07-21 16:39:45.000000 GenRisk-0.2.3/LICENSE
+-rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-24 13:19:34.095125 GenRisk-0.2.3/PKG-INFO
+-rw-r--r--   0 raldisi    (501) staff       (20)     3155 2023-03-15 14:48:24.000000 GenRisk-0.2.3/README.md
+-rw-r--r--   0 raldisi    (501) staff       (20)      103 2021-10-18 09:34:04.000000 GenRisk-0.2.3/pyproject.toml
+-rw-r--r--   0 raldisi    (501) staff       (20)     1193 2023-04-24 13:19:34.095791 GenRisk-0.2.3/setup.cfg
+-rw-r--r--   0 raldisi    (501) staff       (20)      115 2021-07-21 16:39:45.000000 GenRisk-0.2.3/setup.py
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 13:19:34.083477 GenRisk-0.2.3/src/
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 13:19:34.088132 GenRisk-0.2.3/src/GenRisk.egg-info/
+-rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/PKG-INFO
+-rw-r--r--   0 raldisi    (501) staff       (20)      556 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/SOURCES.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        1 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/dependency_links.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)       46 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/entry_points.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        1 2021-10-18 14:25:34.000000 GenRisk-0.2.3/src/GenRisk.egg-info/not-zip-safe
+-rw-r--r--   0 raldisi    (501) staff       (20)      309 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/requires.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        8 2023-04-24 13:19:33.000000 GenRisk-0.2.3/src/GenRisk.egg-info/top_level.txt
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 13:19:34.094390 GenRisk-0.2.3/src/genrisk/
+-rw-r--r--   0 raldisi    (501) staff       (20)       32 2021-07-21 16:39:45.000000 GenRisk-0.2.3/src/genrisk/__init__.py
+-rw-r--r--   0 raldisi    (501) staff       (20)      154 2021-10-12 12:05:52.000000 GenRisk-0.2.3/src/genrisk/__main__.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     6945 2023-04-04 12:13:50.000000 GenRisk-0.2.3/src/genrisk/association_analysis.py
+-rw-r--r--   0 raldisi    (501) staff       (20)    30612 2023-04-03 19:36:08.000000 GenRisk-0.2.3/src/genrisk/cli.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     9589 2023-04-24 11:43:57.000000 GenRisk-0.2.3/src/genrisk/gene_scoring.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     3374 2022-08-20 08:52:58.000000 GenRisk-0.2.3/src/genrisk/helpers.py
+-rw-r--r--   0 raldisi    (501) staff       (20)    15514 2023-04-24 13:17:29.000000 GenRisk-0.2.3/src/genrisk/pipeline.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     7913 2023-04-03 19:34:00.000000 GenRisk-0.2.3/src/genrisk/prediction_models.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     2838 2022-02-04 09:26:13.000000 GenRisk-0.2.3/src/genrisk/prs_scoring.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     5615 2023-03-22 14:17:27.000000 GenRisk-0.2.3/src/genrisk/utils.py
```

### Comparing `GenRisk-0.2.2/LICENSE` & `GenRisk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/PKG-INFO` & `GenRisk-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenRisk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Comprehensive genetic risk assessment
 Home-page: https://github.com/AldisiRana/genrisk
 Author: Rana Aldisi
 Author-email: aldisi.rana@gmail.com
 License: MIT
 Description: # GenRisk
         
@@ -86,10 +86,10 @@
 Keywords: genetics,scoring,risk,comprehensive
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3
+Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `GenRisk-0.2.2/README.md` & `GenRisk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/setup.cfg` & `GenRisk-0.2.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GenRisk
-version = 0.2.2
+version = 0.2.3
 description = Comprehensive genetic risk assessment
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AldisiRana/genrisk
 author = Rana Aldisi
 author_email = aldisi.rana@gmail.com
 license = MIT
@@ -19,29 +19,31 @@
 	genetics
 	scoring
 	risk
 	comprehensive
 
 [options]
 install_requires = 
-	pandas
-	numpy
-	click
-	statsmodels
+	pandas==1.5.3
+	numpy==1.20.3
+	click==7.1.2
+	statsmodels==0.13.5
 	scikit-learn==0.23.2
-	scipy
-	tqdm
-	pycaret
-	qmplot
-	matplotlib
-	seaborn
+	scipy==1.5.4
+	tqdm==4.64.1
+	pycaret==3.0.0
+	qmplot==0.3.2
+	matplotlib==3.6.3
+	seaborn==0.12.2
+	setuptools==1.2.0
+	joblib==1.0.1
 	adjustText
 	pybiomart
 zip_safe = false
-python_requires = >= 3
+python_requires = >= 3.7.5
 packages = find:
 package_dir = 
 	= src
 
 [options.extras_require]
 docs = 
 	sphinx
```

### Comparing `GenRisk-0.2.2/src/GenRisk.egg-info/PKG-INFO` & `GenRisk-0.2.3/src/GenRisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenRisk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Comprehensive genetic risk assessment
 Home-page: https://github.com/AldisiRana/genrisk
 Author: Rana Aldisi
 Author-email: aldisi.rana@gmail.com
 License: MIT
 Description: # GenRisk
         
@@ -86,10 +86,10 @@
 Keywords: genetics,scoring,risk,comprehensive
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3
+Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `GenRisk-0.2.2/src/GenRisk.egg-info/SOURCES.txt` & `GenRisk-0.2.3/src/GenRisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/src/genrisk/association_analysis.py` & `GenRisk-0.2.3/src/genrisk/association_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
          a list with gene name, pvalues, coefs and std err.
 
     """
     try:
         x_set[gene_col[0]] = gene_col[1]
         x_set = sm.add_constant(x_set)
         logit_model = sm.Logit(y_set, x_set)
-        result = logit_model.fit()
+        result = logit_model.fit_regularized()
         pval = list(result.pvalues)
         std_err = result.bse[-1]
         coef = result.params[-1]
     except:
         return
     return [gene_col[0]] + pval + [coef, std_err]
```

### Comparing `GenRisk-0.2.2/src/genrisk/cli.py` & `GenRisk-0.2.3/src/genrisk/cli.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/src/genrisk/gene_scoring.py` & `GenRisk-0.2.3/src/genrisk/gene_scoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     #     info[col] = info[col].str.split(pat='=', expand=True).drop(columns=0)
     #     info.rename(columns={col: val[0]}, inplace=True)
     # df = pd.concat([df, info], axis=1)
     df[af_col].replace('.', 3.98e-6, inplace=True) # 1 allele out 125,748 indiv in gnomADexome (251496 alleles)
     df[af_col].replace('nan', 3.98e-6, inplace=True) # 1 allele out 125,748 indiv in gnomADexome (251496 alleles)
     df[del_col].replace('.', 0, inplace=True)
     df[del_col].replace('nan', 0, inplace=True)
-    df = df[df[af_col].values.astype(float) < maf_threshold]
+    df = df[df[af_col].values.astype(float) <= maf_threshold]
     if weight_func == 'beta':
         df[weight_func] = beta.pdf(df[af_col].values.astype(float), beta_param[0], beta_param[1])
     elif weight_func == 'log10':
         df[weight_func] = -np.log10(df[af_col].values.astype(float))
         df[weight_func].replace([np.inf, -np.inf, np.nan], 0.0, inplace=True)
     df['score'] = df[weight_func].values.astype(float) * df[del_col].values.astype(float)
     genes = list(set(df[genes_col]))
```

### Comparing `GenRisk-0.2.2/src/genrisk/helpers.py` & `GenRisk-0.2.3/src/genrisk/helpers.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/src/genrisk/pipeline.py` & `GenRisk-0.2.3/src/genrisk/pipeline.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -461,8 +461,8 @@
                 continue
             scores_df[col] = (scores_df[col] - scores_df[col].median()) / (scores_df[col].quantile(0.75) - scores_df[col].quantile(0.25))
     else:
         raise Exception(
             'This function does not support the normalization method you selected. Methods: [zscore, gene_length, minmax, maxabs, robust]'
         )
     scores_df.replace([np.inf, -np.inf], 0, inplace=True)
-    return scores_df
+    return scores_df
```

### Comparing `GenRisk-0.2.2/src/genrisk/prediction_models.py` & `GenRisk-0.2.3/src/genrisk/prediction_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     -------
     Final regression model
 
     """
     if not metric:
         metric = 'RMSE'
     setup = pyreg.setup(target=y_col, data=training_set, normalize=normalize, normalize_method=normalize_method,
-                        test_data=testing_set, fold=folds, silent=True, session_id=seed,
+                        test_data=testing_set, fold=folds, session_id=seed,
                         feature_selection=feature_selection)
     best_model = pyreg.compare_models(sort=metric, include=include_models)
     pyreg.pull().to_csv(model_name + '_compare_models.tsv', sep='\t', index=False)
     reg_model = pyreg.create_model(best_model)
     reg_tuned_model = pyreg.tune_model(reg_model, optimize=metric)
     pyreg.pull().to_csv(model_name + '_tuned_model.tsv', sep='\t', index=False)
     final_model = pyreg.finalize_model(reg_tuned_model)
@@ -133,15 +133,15 @@
         metric = 'AUC'
     if len(training_set.groupby(y_col).groups) == 2:
         training_set[y_col] = np.interp(
             training_set[y_col], (training_set[y_col].min(), training_set[y_col].max()), (0, 1))
         testing_set[y_col] = np.interp(
             testing_set[y_col], (testing_set[y_col].min(), testing_set[y_col].max()), (0, 1))
     setup = pycl.setup(target=y_col, fix_imbalance=imbalanced, normalize=normalize, normalize_method=normalize_method,
-                    data=training_set, test_data=testing_set, silent=True, fold=folds, session_id=seed,
+                    data=training_set, test_data=testing_set, fold=folds, session_id=seed,
                     feature_selection=feature_selection)
     best_model = pycl.compare_models(sort=metric, include=include_models)
     pycl.pull().to_csv(model_name + '_compare_models.tsv', sep='\t', index=False)
     cl_model = pycl.create_model(best_model)
     cl_tuned_model = pycl.tune_model(cl_model, optimize=metric)
     pycl.pull().to_csv(model_name + '_tuned_model.tsv', sep='\t', index=False)
     final_model = pycl.finalize_model(cl_tuned_model)
```

### Comparing `GenRisk-0.2.2/src/genrisk/prs_scoring.py` & `GenRisk-0.2.3/src/genrisk/prs_scoring.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.2/src/genrisk/utils.py` & `GenRisk-0.2.3/src/genrisk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from adjustText import adjust_text
 from qmplot import qqplot
 from tqdm import tqdm
 from pybiomart import Dataset
+from textwrap import wrap
+
 
 
 def gene_length_normalize(*, genes_info, genes_col='HGNC symbol', length_col='gene_length', scores_df, samples_col):
     """
     Normalize dataset by gene length. if gene lengths file is not provided, info will be retrieved from ensembl.
 
     Parameters
@@ -126,22 +128,22 @@
     Returns
     -------
     QQPlot
 
     """
     pvals.dropna(inplace=True)
     f, ax = plt.subplots(figsize=(6, 6), facecolor="w", edgecolor="k")
+    title = "\n".join(wrap(qq_output.split('.')[0], 50))
     qqplot(data=pvals,
+           title=title,
            marker="o",
-           title=qq_output.split('.')[0],
            xlabel=r"Expected $-log_{10}{(P)}$",
            ylabel=r"Observed $-log_{10}{(P)}$",
-           dpi=300,
-           figname=qq_output,
            ax=ax)
+    plt.savefig(qq_output)
     return ax
 
 
 def merge_files(*, files_lst, sep, by, cols=None):
     """
     Merge a list of files with the same format into one dataframe.
```


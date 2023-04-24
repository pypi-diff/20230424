# Comparing `tmp/pheno-utils-0.1.5.tar.gz` & `tmp/pheno-utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.5.tar", last modified: Sun Apr 23 11:10:52 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.6.tar", last modified: Mon Apr 24 07:18:35 2023, max compression
```

## Comparing `pheno-utils-0.1.5.tar` & `pheno-utils-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.387734 pheno-utils-0.1.5/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.5/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.5/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-23 11:10:52.387368 pheno-utils-0.1.5/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.5/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.381982 pheno-utils-0.1.5/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)      328 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3441 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16321 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-23 11:10:17.000000 pheno-utils-0.1.5/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-23 11:10:52.386768 pheno-utils-0.1.5/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.5/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-23 11:10:52.000000 pheno-utils-0.1.5/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-23 11:08:21.000000 pheno-utils-0.1.5/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-23 11:10:52.387885 pheno-utils-0.1.5/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.5/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.397408 pheno-utils-0.1.6/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.6/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.6/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 07:18:35.397005 pheno-utils-0.1.6/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.6/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.391991 pheno-utils-0.1.6/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)      328 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    17037 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.396354 pheno-utils-0.1.6/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.6/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-24 07:03:30.000000 pheno-utils-0.1.6/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-24 07:18:35.397578 pheno-utils-0.1.6/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.6/setup.py
```

### Comparing `pheno-utils-0.1.5/LICENSE` & `pheno-utils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/PKG-INFO` & `pheno-utils-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.5/pheno_utils/_modidx.py` & `pheno-utils-0.1.6/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.6/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.6/pheno_utils/basic_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,16 +84,18 @@
     Assign the nearest research stage to each record in a dataset.
     
     Args:
         dataset (pd.DataFrame): The dataset containing records to be assigned research stages.
         population (pd.DataFrame): The population data with participant_id, cohort, research_stage, and research_stage_date.
         max_days (int, optional): The maximum number of days allowed between the collection date and research stage date. Defaults to 60.
         stages (List[str], optional): The list of types of research stages to consider. Defaults to ['visit'].
-        agg (Union[str, None], optional): The aggregation function to be used when grouping data. 
-                                          Can be 'first', 'last', 'mean', 'min', 'max', or None. Defaults to 'first'.
+        agg (Union[str, None], optional): The aggregation function to be used when (optionally) aggregating multiple rows
+                                          from the same research stage. The rows are already sorted by distance from the
+                                          date of the research stage. Can be 'first' (closest), 'last' (farthest), 'mean',
+                                          'min', 'max', or None. Defaults to 'first'.
 
     Returns:
         pd.DataFrame: The dataset with the nearest research stage assigned to each record.
     """
     data_wo_stage = dataset.sort_values('collection_date').reset_index()\
         .drop(columns=['research_stage'], errors='ignore')
     population = population.loc[
@@ -116,9 +118,9 @@
         # return data_wo_stage, data_w_stage
         return data_wo_stage.merge(
             data_w_stage[['participant_id', 'cohort', 'collection_date', 'research_stage']].drop_duplicates(),
             how='left')\
             .set_index(dataset.index.names)
 
     return data_w_stage.groupby(['participant_id', 'cohort', 'research_stage']).agg(agg)\
-        .drop(columns=['array_index']).rename(columns={'collection_date': 'closest_collection_date'})
+        .drop(columns=['array_index'], errors='ignore')
```

### Comparing `pheno-utils-0.1.5/pheno_utils/basic_plots.py` & `pheno-utils-0.1.6/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.6/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.6/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/config.py` & `pheno-utils-0.1.6/pheno_utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_config.ipynb.
 
 # %% auto 0
 __all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH', 'COHORT',
-           'POPULATION_DATASET', 'CONFIG_FILES', 'generate_synthetic_data', 'generate_synthetic_data_like']
+           'POPULATION_DATASET', 'ERROR_ACTION', 'CONFIG_FILES', 'generate_synthetic_data',
+           'generate_synthetic_data_like']
 
 # %% ../nbs/00_config.ipynb 3
 import os
 
 import numpy as np
 import pandas as pd
 
@@ -18,14 +19,15 @@
 
 GLUC_COLOR = "C0"
 FOOD_COLOR = "C1"
 
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
 COHORT = '10k'
 POPULATION_DATASET = 'population'
+ERROR_ACTION = 'raise'
 CONFIG_FILES = ['.pheno/config', '~/.pheno/config', '/efs/.pheno/config']
 
 for cf in CONFIG_FILES:
     cf = os.path.expanduser(cf)
     if not os.path.isfile(cf):
         continue
     with open(cf, 'r') as f:
@@ -34,14 +36,16 @@
                 DATASETS_PATH = line.split('=')[1].strip()
             elif line.startswith('POPULATION_DATASET'):
                 POPULATION_DATASET = line.split('=')[1].strip()
             elif line.startswith('COHORT'):
                 COHORT = line.split('=')[1].strip()
                 if (len(COHORT) == 0) or (COHORT == 'None'):
                     COHORT = None
+            elif line.startswith('ERROR_ACTION'):
+                ERROR_ACTION = line.split('=')[1].strip()
     break
 
 
 # %% ../nbs/00_config.ipynb 5
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
```

### Comparing `pheno-utils-0.1.5/pheno_utils/data_loader.py` & `pheno-utils-0.1.6/pheno_utils/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to POPULATION_DATASET.
         skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
         flexible_field_search (bool, optional): Whether to allow regex field search. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
-            Possible values are 'raise' and 'warn'. Defaults to 'raise'.
+            Possible values are 'raise', 'warn' and 'ignore'. Defaults to 'raise'.
 
     Attributes:
     
         dict (pd.DataFrame): The data dictionary for the dataset, containing information about each field.
         dfs (dict): A dictionary of dataframes, one for each table in the dataset.
         fields (list): A list of all fields in the dataset.
         dataset (str): The name of the dataset being used.
@@ -63,15 +63,15 @@
         cohort: str = COHORT,
         age_sex_dataset: str = POPULATION_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         flexible_field_search: bool = False,
-        errors: str = 'raise'
+        errors: str = ERROR_ACTION,
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.dataset_path = self.__get_dataset_path__(self.dataset)
         if self.dataset != age_sex_dataset:
             self.age_sex_dataset = age_sex_dataset
@@ -244,49 +244,67 @@
             return df1
         return df1.join(df2, how='outer')
 
     def __load_age_sex__(self) -> None:
         """
         Add sex and compute age from birth date.
         """
-        age_path = os.path.join(self.__get_dataset_path__('population'), 'events.parquet')
+        age_path = os.path.join(self.__get_dataset_path__(self.age_sex_dataset), 'events.parquet')
         align_df = self.dfs[list(self.dfs)[0]]
 
         if ('research_stage' in align_df.columns) or ('research_stage' in align_df.index.names):
-            age_df = pd.read_parquet(age_path)
-            self.dfs['age_sex'] = align_df.join(
-                age_df[['age_at_research_stage', 'sex']].droplevel('array_index'))\
-                .rename(columns={'age_at_research_stage': 'age'})[['age', 'sex']]
+            try:
+                age_df = pd.read_parquet(age_path)
+                self.dfs['age_sex'] = align_df.join(
+                    age_df[['age_at_research_stage', 'sex']].droplevel('array_index'))\
+                    .rename(columns={'age_at_research_stage': 'age'})[['age', 'sex']]
+
+            except Exception as e:
+                if self.errors == 'raise':
+                    raise(e)
+                elif self.errors == 'warn':
+                    warnings.warn(f'Error joining research_stage: {e}')
+                self.dfs['age_sex'] = pd.DataFrame(index=align_df.index).assign(age=np.nan, sex=np.nan)
+
         else:
             # init an empty df
             self.dfs['age_sex'] = pd.DataFrame(index=align_df.index).assign(age=np.nan, sex=np.nan)
 
         self.fields += ['age', 'sex']
         ind = self.dfs['age_sex'].isnull().any(axis=1)
         if not ind.any():  # no missing values
             return
 
         # fill in missing values by computing age from birth date
-        date_cols = np.array(['collection_timestamp', 'collection_date', 'sequencing_date'])
+        date_cols = np.array(['collection_date', 'collection_timestamp', 'sequencing_date'])
         date = date_cols[np.isin(date_cols, align_df.columns)][0]  # prefer first match
 
         ind &= align_df[date].notnull()
         if not ind.any():
             return
 
         age_df = pd.read_parquet(age_path.replace('events', 'population'))
-        age_df['birth_date'] = pd.to_datetime(
-            age_df['year_of_birth'].astype(str) + '-' + age_df['month_of_birth'].astype(str))
 
         # trying a workaround for a pandas deprecation warning
         age_sex = self.dfs['age_sex']
-        missing_age_sex = align_df.loc[ind, [date]].join(age_df[['sex', 'birth_date']])\
-            .assign(age=lambda x: ((x[date].dt.date - x['birth_date'].dt.date).dt.days / 365.25).round(1))\
-            [['age', 'sex']]
-        age_sex = age_sex.join(missing_age_sex, rsuffix='_miss')
+        try:
+            age_df['birth_date'] = pd.to_datetime(
+                age_df['year_of_birth'].astype(str) + '-' + age_df['month_of_birth'].astype(str))
+            missing_age_sex = align_df.loc[ind, [date]].join(age_df[['sex', 'birth_date']])\
+                .assign(age=lambda x: ((x[date].dt.date - x['birth_date'].dt.date).dt.days / 365.25).round(1))\
+                [['age', 'sex']]
+            age_sex = age_sex.join(missing_age_sex, rsuffix='_miss')
+
+        except Exception as e:
+            if self.errors == 'raise':
+                raise(e)
+            elif self.errors == 'warn':
+                warnings.warn(f'Error joining on {date}: {e}')
+            age_sex = age_sex.join(age_df[['sex']], rsuffix='_miss').assign(age_miss=np.nan)
+
         age_sex['age'] = age_sex['age'].fillna(age_sex['age_miss'])
         age_sex['sex'] = age_sex['sex'].fillna(age_sex['sex_miss'])
         self.dfs['age_sex'] = age_sex[['age', 'sex']]
 
     def __load_dataframes__(self) -> None:
         """
         Load all tables in the dataset dictionary.
```

### Comparing `pheno-utils-0.1.5/pheno_utils/dates_plots.py` & `pheno-utils-0.1.6/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.6/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.6/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.6/pheno_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.5/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.6/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.5/settings.ini` & `pheno-utils-0.1.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.5
+version = 0.1.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.5/setup.py` & `pheno-utils-0.1.6/setup.py`

 * *Files identical despite different names*


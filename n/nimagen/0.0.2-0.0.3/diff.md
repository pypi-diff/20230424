# Comparing `tmp/nimagen-0.0.2.tar.gz` & `tmp/nimagen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimagen-0.0.2.tar", last modified: Mon Mar 20 09:14:44 2023, max compression
+gzip compressed data, was "nimagen-0.0.3.tar", last modified: Mon Apr 24 10:13:23 2023, max compression
```

## Comparing `nimagen-0.0.2.tar` & `nimagen-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-03-20 09:14:44.132465 nimagen-0.0.2/
--rw-r--r--   0 hai        (501) staff       (20)     1073 2023-01-02 14:13:22.000000 nimagen-0.0.2/LICENSE
--rw-r--r--   0 hai        (501) staff       (20)      669 2023-03-20 09:14:44.132170 nimagen-0.0.2/PKG-INFO
--rw-r--r--   0 hai        (501) staff       (20)      202 2023-01-12 23:22:01.000000 nimagen-0.0.2/README.md
--rw-r--r--   0 hai        (501) staff       (20)      549 2023-03-20 09:13:21.000000 nimagen-0.0.2/pyproject.toml
--rw-r--r--   0 hai        (501) staff       (20)       38 2023-03-20 09:14:44.132570 nimagen-0.0.2/setup.cfg
-drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-03-20 09:14:44.119120 nimagen-0.0.2/src/
-drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-03-20 09:14:44.127110 nimagen-0.0.2/src/nimagen/
--rw-r--r--   0 hai        (501) staff       (20)        0 2023-01-02 13:16:46.000000 nimagen-0.0.2/src/nimagen/__init__.py
--rw-r--r--   0 hai        (501) staff       (20)    13764 2023-01-02 14:10:50.000000 nimagen-0.0.2/src/nimagen/genes.py
--rw-r--r--   0 hai        (501) staff       (20)    22569 2023-01-02 14:10:42.000000 nimagen-0.0.2/src/nimagen/graph.py
--rw-r--r--   0 hai        (501) staff       (20)    60291 2023-03-04 05:48:43.000000 nimagen-0.0.2/src/nimagen/stats.py
--rw-r--r--   0 hai        (501) staff       (20)    93297 2023-02-27 14:56:14.000000 nimagen-0.0.2/src/nimagen/visualisation.py
-drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-03-20 09:14:44.131760 nimagen-0.0.2/src/nimagen.egg-info/
--rw-r--r--   0 hai        (501) staff       (20)      669 2023-03-20 09:14:44.000000 nimagen-0.0.2/src/nimagen.egg-info/PKG-INFO
--rw-r--r--   0 hai        (501) staff       (20)      288 2023-03-20 09:14:44.000000 nimagen-0.0.2/src/nimagen.egg-info/SOURCES.txt
--rw-r--r--   0 hai        (501) staff       (20)        1 2023-03-20 09:14:44.000000 nimagen-0.0.2/src/nimagen.egg-info/dependency_links.txt
--rw-r--r--   0 hai        (501) staff       (20)        8 2023-03-20 09:14:44.000000 nimagen-0.0.2/src/nimagen.egg-info/top_level.txt
+drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-04-24 10:13:23.867925 nimagen-0.0.3/
+-rw-r--r--   0 hai        (501) staff       (20)     1073 2023-01-02 14:13:22.000000 nimagen-0.0.3/LICENSE
+-rw-r--r--   0 hai        (501) staff       (20)     2139 2023-04-24 10:13:23.867418 nimagen-0.0.3/PKG-INFO
+-rw-r--r--   0 hai        (501) staff       (20)     1671 2023-04-24 09:47:50.000000 nimagen-0.0.3/README.md
+-rw-r--r--   0 hai        (501) staff       (20)      549 2023-04-24 10:12:43.000000 nimagen-0.0.3/pyproject.toml
+-rw-r--r--   0 hai        (501) staff       (20)       38 2023-04-24 10:13:23.868095 nimagen-0.0.3/setup.cfg
+drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-04-24 10:13:23.853155 nimagen-0.0.3/src/
+drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-04-24 10:13:23.861167 nimagen-0.0.3/src/nimagen/
+-rw-r--r--   0 hai        (501) staff       (20)        0 2023-01-02 13:16:46.000000 nimagen-0.0.3/src/nimagen/__init__.py
+-rw-r--r--   0 hai        (501) staff       (20)    18095 2023-04-15 16:32:06.000000 nimagen-0.0.3/src/nimagen/genes.py
+-rw-r--r--   0 hai        (501) staff       (20)    22569 2023-01-02 14:10:42.000000 nimagen-0.0.3/src/nimagen/graph.py
+-rw-r--r--   0 hai        (501) staff       (20)    64301 2023-04-23 15:49:08.000000 nimagen-0.0.3/src/nimagen/stats.py
+-rw-r--r--   0 hai        (501) staff       (20)    98606 2023-04-24 01:29:17.000000 nimagen-0.0.3/src/nimagen/visualisation.py
+drwxr-xr-x   0 hai        (501) staff       (20)        0 2023-04-24 10:13:23.866708 nimagen-0.0.3/src/nimagen.egg-info/
+-rw-r--r--   0 hai        (501) staff       (20)     2139 2023-04-24 10:13:23.000000 nimagen-0.0.3/src/nimagen.egg-info/PKG-INFO
+-rw-r--r--   0 hai        (501) staff       (20)      288 2023-04-24 10:13:23.000000 nimagen-0.0.3/src/nimagen.egg-info/SOURCES.txt
+-rw-r--r--   0 hai        (501) staff       (20)        1 2023-04-24 10:13:23.000000 nimagen-0.0.3/src/nimagen.egg-info/dependency_links.txt
+-rw-r--r--   0 hai        (501) staff       (20)        8 2023-04-24 10:13:23.000000 nimagen-0.0.3/src/nimagen.egg-info/top_level.txt
```

### Comparing `nimagen-0.0.2/LICENSE` & `nimagen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nimagen-0.0.2/pyproject.toml` & `nimagen-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nimagen"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hai Le", email="l.haimcl@gmail.com" },
 ]
 description = "Simple statistical and visualisation tool for neuroimaging genetics studies"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `nimagen-0.0.2/src/nimagen/graph.py` & `nimagen-0.0.3/src/nimagen/graph.py`

 * *Files identical despite different names*

### Comparing `nimagen-0.0.2/src/nimagen/stats.py` & `nimagen-0.0.3/src/nimagen/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Uses to perform mass univariate and everything related to it
 """
 from typing import List, Union, Optional
 from collections import defaultdict
 from itertools import combinations
 import statsmodels.api as sm
 import statsmodels.formula.api as sfm
+from statsmodels.stats.multitest import fdrcorrection
 from scipy.stats import ttest_ind, zscore, f
 import pandas as pd
 import numpy as np
 
 from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import StandardScaler, LabelBinarizer
 from sklearn.model_selection import train_test_split
@@ -445,18 +446,19 @@
             DESCRIPTION.
         see MassUnivariate.mass_univariate for full variable descriptions
         Returns
         -------
         new_df : TYPE
             DESCRIPTION.
         """
+        disable_tqdm = kwargs.get('disable_tqdm',False)
         new_df = pd.DataFrame()
         if cont_independentVar_cols is None:
             cont_independentVar_cols = []
-        for threshold in tqdm.tqdm(thresholds):
+        for threshold in tqdm.tqdm(thresholds,disable=disable_tqdm):
             try:
                 temp_model, temp_model_summary = cls.mass_univariate(
                     df,
                     cat_independentVar_cols=cat_independentVar_cols,
                     cont_independentVar_cols=cont_independentVar_cols + [threshold],
                     dependentVar_cols=dependentVar_cols,**kwargs)
                 temp_model_summary.reset_index(drop=False, inplace=True)
@@ -565,27 +567,27 @@
     
     @classmethod
     def check_all_predictors_combo_linear_Reg(cls,df: Optional[pd.DataFrame] = None,
                                             cat_independentVar_cols: Optional[List[str]] = None,
                                             cont_independentVar_cols: Optional[List[str]] = None,
                                             check_cols:Optional[List[str]]=None,
                                             check_plan:Optional[str]=None,
-                                            dependentVar_cols: Optional[List[str]] = None):
+                                            dependentVar_cols: Optional[List[str]] = None,**kwargs):
         """[Perform univariate test on all combinations of predictors]
 
         Args:
             df (Optional[pd.DataFrame]): [description]
             cat_independentVar_cols (Optional[List[str]], optional): [categorical variable]. Defaults to None.
             cont_independentVar_cols (Optional[List[str]], optional): [Continuous variables]. Defaults to None.
             dependentVar_cols (Optional[List[str]], optional): [description]. Defaults to None.
         Returns:
             [type]: [description]
         """
         all_models = defaultdict(list)
-
+        disable_tqdm = kwargs.get('disable_tqdm',False)
         def print_model_results(model: sm.regression.linear_model.RegressionResultsWrapper,
                                 model_name: str,
                                 dictionary: dict = all_models) -> None:
             #convenience function to print the model results from the sm.regression model
             
             variables = model.params.index.to_list()
             len_variables = len(variables)-1
@@ -612,15 +614,15 @@
         check_all=False
         if not check_cols:
             check_all=True
             check_cols = total_predictors
         
         if check_plan=='sequential':
             k_combo = (check_cols[0:n] for n in range(1,len(check_cols)+1))
-            for idx,model_combo in tqdm.tqdm(enumerate(k_combo)):
+            for idx,model_combo in tqdm.tqdm(enumerate(k_combo),disable=disable_tqdm):
                 cat_independentVar_cols_temp = [i for i in cat_independentVar_cols if i not in check_cols]
                 cont_independentVar_cols_temp = [i for i in cont_independentVar_cols if i not in check_cols]
                 for _, covar in enumerate(model_combo):
 
                     if covar in cat_independentVar_cols:
                         cat_independentVar_cols_temp.append(covar)
                     elif covar in cont_independentVar_cols:
@@ -635,15 +637,15 @@
                                                 cont_independentVar_cols=cont_independentVar_cols_temp,
                                                 dependentVar_cols=dependentVar_cols)
 
                 model_name_temp = str(len(model_combo))+'_'+str(idx)
                 print_model_results(model_temp, model_name_temp)
         # for k in range(1,len(total_predictors)+1):
         else:
-            for k in tqdm.tqdm(range(1, len(check_cols)+1)):
+            for k in tqdm.tqdm(range(1, len(check_cols)+1),disable=disable_tqdm):
                 k_combo = combinations(check_cols, k)
                 for idx, model_combo in enumerate(k_combo):
                     cat_independentVar_cols_temp = []
                     cont_independentVar_cols_temp = []
                     if not check_all:
                         cat_independentVar_cols_temp = [i for i in cat_independentVar_cols if i not in check_cols]
                         cont_independentVar_cols_temp = [i for i in cont_independentVar_cols if i not in check_cols]
@@ -715,29 +717,32 @@
 
     @classmethod
     def print_summary_table(cls,
                             df:pd.DataFrame,
                             thresholds:List[str]=None,
                             cat_independentVar_cols:List[str]=None,
                             cont_independentVar_cols:List[str]=None,
-                            dependentVar_cols:List[str]=None)->pd.DataFrame:
+                            dependentVar_cols:List[str]=None,
+                            **kwargs)->pd.DataFrame:
         """
         
 
         Parameters
         ----------
         see data_exploration.MassUnivariate.mass_univariate for full description of the variables
         Returns
         -------
         summary_table : pd.DataFrame
             The summary table containing R, Beta value, P-value for each dependent variable at each PRS threshold.
 
         """
+        disable_tqdm = kwargs.get('disable_tqdm',False)
+
         Result_dict=defaultdict(dict)
-        for dependent_variable in tqdm.tqdm(dependentVar_cols):
+        for dependent_variable in tqdm.tqdm(dependentVar_cols,disable=disable_tqdm):
             Result_dict[dependent_variable] = defaultdict(dict)
             for threshold in thresholds:
                 Result_dict[dependent_variable][threshold] = defaultdict(dict)
                 Result_dict[dependent_variable][threshold]['R2'] = defaultdict(dict)
                 temp_model, _ = cls.mass_univariate(
                     df=df,
                     cat_independentVar_cols=cat_independentVar_cols,
@@ -757,57 +762,80 @@
         summary_table = pd.DataFrame.from_dict({(i,j,k): Result_dict[i][j][k] 
                                                 for i in Result_dict.keys() 
                                                 for j in Result_dict[i].keys() 
                                                 for k in Result_dict[i][j].keys()},
                        orient='index')
         
         return summary_table
+
+class MultipleCorrection:
+    @staticmethod
+    def fdr(df:pd.DataFrame=None,
+            p_val:Union[np.ndarray,str]=None,
+            alpha:float=0.05,
+            return_adj:bool=True):
+        if isinstance(df,pd.DataFrame):
+            if not isinstance(p_val,str):
+                return TypeError('Must give the column name if providing dataframe')
+            p_val = df[p_val].values
+        elif isinstance(p_val,np.ndarray):
+            if p_val.ndim != 1:
+                p_val = p_val.reshape(-1)
+        survived,adjusted_pval = fdrcorrection(p_val)
+        if isinstance(df,pd.DataFrame):
+            if return_adj:
+                df['adjP'] = adjusted_pval
+            return df[survived]
+        else:
+            return survived,adjusted_pval
+            
+            
+
+    @staticmethod
+    def matSpDLite(correlation_matrix:np.ndarray,alpha:str = 0.05):
+        """
+        Adapted from Nyholt DR R script.
+        Please cite
+        Nyholt DR (2004) A simple correction for multiple testing for SNPs in linkage disequilibrium with each other. Am J Hum Genet 74(4):765-769.
+        and 
+        http://gump.qimr.edu.au/general/daleN/matSpDlite/
+        and
+        Li and Ji 2005. 
         
+        Parameters
+        ----------
+        correlation_matrix : np.ndarray
+            The correlation matrix. It must be symmetric.
+        alpha : str, optional
+            DESCRIPTION. The default is 0.05.
 
-def matSpDLite(correlation_matrix:np.ndarray,alpha:str = 0.05):
-    """
-    Adapted from Nyholt DR R script.
-    Please cite
-    Nyholt DR (2004) A simple correction for multiple testing for SNPs in linkage disequilibrium with each other. Am J Hum Genet 74(4):765-769.
-    and 
-    http://gump.qimr.edu.au/general/daleN/matSpDlite/
-    and
-    Li and Ji 2005. 
-    
-    Parameters
-    ----------
-    correlation_matrix : np.ndarray
-        The correlation matrix. It must be symmetric.
-    alpha : str, optional
-        DESCRIPTION. The default is 0.05.
-
-    """
-    evals,_ = np.linalg.eigh(correlation_matrix.T)
-    evals = np.sort(evals)[::-1]
-    
-    oldV = np.var(evals,ddof=1)
-    M = len(evals)
-    L = M-1
-    Meffold = (L*(1- oldV/M)) + 1
-    
-    print(f'Effective Number of Independent Variables [Veff] is {Meffold}')
-    newevals = np.where(evals<0,0,evals) # negative eigenvalues are set to 0
-    
-    IntLinewevals = np.where(newevals>=1,1,0) #the integral part "represents identical tests that should be counted as one in Meff"
-    NonIntLinewevals = newevals - np.floor(newevals) # the non integral part should represent the partially correlated test that should be counted as a fractional number between 0 and 1
-    MeffLi = np.sum(IntLinewevals + NonIntLinewevals)
-    
-    print(f'Effective Number of Independent Variables [VeffLi] (Using equation 5 of Li and Ji 2005) is {np.round(MeffLi)}')
-    
-    if MeffLi < Meffold:
-        adjusted_p_val = alpha/MeffLi
-    else:
-        adjusted_p_val = alpha/Meffold
-    print(f'The adjusted multiple testing correction p-val is alpha/lower(Meff) = {adjusted_p_val}')
-    return MeffLi
+        """
+        evals,_ = np.linalg.eigh(correlation_matrix.T)
+        evals = np.sort(evals)[::-1]
+        
+        oldV = np.var(evals,ddof=1)
+        M = len(evals)
+        L = M-1
+        Meffold = (L*(1- oldV/M)) + 1
+        
+        print(f'Effective Number of Independent Variables [Veff] is {Meffold}')
+        newevals = np.where(evals<0,0,evals) # negative eigenvalues are set to 0
+        
+        IntLinewevals = np.where(newevals>=1,1,0) #the integral part "represents identical tests that should be counted as one in Meff"
+        NonIntLinewevals = newevals - np.floor(newevals) # the non integral part should represent the partially correlated test that should be counted as a fractional number between 0 and 1
+        MeffLi = np.sum(IntLinewevals + NonIntLinewevals)
+        
+        print(f'Effective Number of Independent Variables [VeffLi] (Using equation 5 of Li and Ji 2005) is {np.round(MeffLi)}')
+        
+        if MeffLi < Meffold:
+            adjusted_p_val = alpha/MeffLi
+        else:
+            adjusted_p_val = alpha/Meffold
+        print(f'The adjusted multiple testing correction p-val is alpha/lower(Meff) = {adjusted_p_val}')
+        return MeffLi
 
 
 # def save_dict_with_pickle(dictionary: Optional[dict],
 #                           file_path: Optional[str]) -> None:
 #     a_file = open(file_path, 'wb')
 #     pickle.dump(dictionary, a_file)
 #     a_file.close()
@@ -834,15 +862,15 @@
                                   test_size: float = 0.5, random_state: int = 42) -> tuple:
         """[splitting the data based on several stratification]
     
         Args:
             df (Union[pd.DataFrame, np.ndarray], optional): [the data/ dataframe to be split]. Defaults to None.
             bins (int, optional): [the bins used to separate the continuous data,
                                         if it is too high, then due to small dataset, there might be error due to not enough data in each class]. Defaults to 4.
-            This works by concatenate multiple stratification criteria together, and then attempt train test split. This is done at each level of stratification. If the stratificatio is not successful, we reduce the bins number, and try again.
+            This works by concatenate multiple stratification criteria together, and then attempt train test split. This is done at each level of stratification. If the stratification is not successful, we reduce the bins number, and try again.
             This is done in succession, so depending on what you want to stratify by, you put it earlier in the list. so GA_vol, PMA_vol will stratify first by GA, and then PMA.
         Returns:
             tuple : train and test set.
         """
         def attempting_train_test_split(df, stratify_by, idx, test_size,random_state):
             try:
                 train, test = train_test_split(df, stratify=stratify_by, test_size=test_size, random_state=random_state)
@@ -871,14 +899,72 @@
                 if train_test:
                     break
                 else:
                     bins -= 1
 
         return train_test
     
+    @staticmethod
+    def split_group(df:Union[pd.DataFrame, np.ndarray],
+                    stratify_by_args:Union[str,np.array]=None,
+                    n=2,
+                    fraction:Union[List[float],float]=None,
+                    bins:int=4):
+        """Splitting dataframe or array into groups
+
+        Args:
+            df (Union[pd.DataFrame, np.ndarray]): DataFrame or Array
+            stratify_by_args (Union[str,np.array], optional): list of string or columns names that need to be stratified. Defaults to None.
+            n (int, optional): number of groups. Defaults to 2.
+            bins (int, optional): bins to stratify the continuous variables. Defaults to 4.
+
+        Returns:
+            List[pd.DataFrame]: list of dataframe corresponding for each group
+        """
+        if isinstance(df,np.ndarray):
+            temp_df = pd.DataFrame(df)
+        elif isinstance(df,pd.DataFrame):
+            temp_df = df.copy()
+        
+        
+        stratification_list = []
+        if stratify_by_args is not None:
+            for idx, stratification in enumerate(stratify_by_args):
+                if isinstance(stratification, str):
+                    strat = df.loc[:, stratification].values
+                    if isinstance(strat[0], float):
+                        strat = pd.cut(strat, bins=bins, labels=False)
+                elif isinstance(stratification, np.ndarray):
+                    strat = stratification
+                    if isinstance(stratification[0], float):
+                        strat = pd.cut(strat, bins=bins, labels=False)
+                stratification_list.append(strat)
+                stratify_by = [''.join(map(lambda x: str(x), i))
+                                for i in zip(*stratification_list)]
+                
+            temp_df['stratify_by'] = stratify_by
+            unique_stratified_group = np.unique(stratify_by)
+            if isinstance(fraction,float):
+                return df.iloc[temp_df.groupby('stratify_by',group_keys=False).apply(lambda x: x.sample(frac=fraction)).index]
+            all_group = pd.concat([
+                temp_df[temp_df['stratify_by']==unique_group].apply(
+                    lambda x: np.random.choice([
+                        i for i in range(n)],1)[0],axis=1) for unique_group in unique_stratified_group
+                ])
+        else:
+            if isinstance(fraction,float):
+                return df.iloc[temp_df.sample(frac=fraction).index]
+            all_group = temp_df.apply(
+                lambda x: np.random.choice([i for i in range(n)],1)[0],axis=1)
+            
+        return [temp_df.iloc[all_group[all_group==i].index] for i in range(n)]
+        
+        
+    
+    
     # @staticmethod
     # def generate_stratified_fold(df: Union[pd.DataFrame, np.ndarray] = None,
     #                               *stratify_by_args, 
     #                               bins : int =4,
     #                               n_splits=3,
     #                               random_state: int = 42):
     #     stratified_split = StratifiedKFold(n_splits=n_splits)
```

### Comparing `nimagen-0.0.2/src/nimagen/visualisation.py` & `nimagen-0.0.3/src/nimagen/visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 import statsmodels.api as sm
 from typing import List, Union, Optional
 import nibabel as nib # used to do visualise brain maps
 import copy
 from matplotlib.collections import LineCollection
 import matplotlib.patches as mpatches
 import matplotlib as mpl
-from matplotlib.colors import ListedColormap
+from matplotlib.colors import ListedColormap, to_rgb, rgb2hex, CSS4_COLORS
+
 from collections import defaultdict
 from itertools import product, chain
 
 from functools import reduce  # forward compatibility for Python 3
 import operator
 
 class SimplePlots:
@@ -382,15 +383,14 @@
         """
         x,xlabel,_ = SimplePlots.return_array(x,data=data,must_be='str')
         y,ylabel,_ = SimplePlots.return_array(y,data=data)
         y2,y2label,_ = SimplePlots.return_array(y2,data=data)
         colorby,colorbar_label,_ = SimplePlots.return_array(colorby,data=data)
         separateby,plot_label,_ = SimplePlots.return_array(separateby,data=data,must_be='str')
         hue,legend_label,_ = SimplePlots.return_array(hue,data = data,must_be='str')
-        
         if (hue is not None) and (colorby is not None):
             #if both hue and colorby is present, show only hue
             colorby = None
             colorbar_label = None
         if separateby is None:
             separateby = [None for i in range(len(x))]
         if colorby is None:
@@ -431,18 +431,30 @@
         if order is not None:
             if 'order_reversed' not in figkwargs:
                 figkwargs['order_reversed'] = False
             if isinstance(order,dict):
                 all_bars_vals = SimplePlots.sort_array(all_bars_vals,
                                                         specific_order=order)
             else:
-                all_bars_vals = SimplePlots.sort_array(all_bars_vals,
-                                                       order=order,
-                                                       ascending=figkwargs['order_reversed'])
-        
+                try:
+                    all_bars_vals = SimplePlots.sort_array(all_bars_vals,
+                                                        order=order,
+                                                        ascending=figkwargs['order_reversed'])
+                except TypeError:
+                #this happens when the continuous values has equal values, e.g, 0.000 in multiple places, the code will then try to sort the rows by the first axis. If that first axis is None, then it will throw bad error.
+                    try:
+                        assert all(v is None for v in all_bars_vals['separateby']) #make sure that all of the values in all_bar_vals separateby is None.
+                    except AssertionError:
+                        raise TypeError('The separateby value is not None, there is something wrong with sorting process')
+                    all_bars_vals['separateby'] = 0
+                    all_bars_vals = SimplePlots.sort_array(all_bars_vals,
+                                                        order=order,
+                                                        ascending=figkwargs['order_reversed'])
+                    all_bars_vals['separateby'] = None
+                    
         separateby = all_bars_vals['separateby']
         if all(item is None for item in separateby):
             separateby = None
         x = all_bars_vals['x']
         hue = all_bars_vals['hue']
         if all(item is None for item in hue):
             hue = None
@@ -1069,18 +1081,18 @@
         box_plots_kwargs['notch']=figkwargs.get('notch',False)
         box_plots_kwargs['medianprops'] = figkwargs.get('medianprops',dict(color='grey'))
         box_plots_kwargs['vert'] = figkwargs.get('vert',True)
         box_plots_kwargs['whis'] = figkwargs.get('whis',1.5)
         box_plots_kwargs['bootstrap'] = figkwargs.get('bootstrap',None)
         box_plots_kwargs['usermedians'] = figkwargs.get('usermedians',None)
         box_plots_kwargs['conf_intervals'] = figkwargs.get('conf_intervals',None)
-        
         legend_label = dict()
         legend_label['loc'] =  figkwargs.get('legend_loc','upper right')
-        
+        rotation_x = figkwargs.get('rotation_x',0)
+
         ######### figkwargs:end ##############
         
         if not all(item is None for item in to_plot_dictionary.keys()): # the first level is separateby
             uniq_separateby = list(to_plot_dictionary.keys())
             if len(uniq_separateby)>3:
                 row = int(np.ceil(len(uniq_separateby)/3))
                 column = 3
@@ -1133,15 +1145,15 @@
                             whiskerprops=dict(color=c),
                             flierprops=dict(color=c, markeredgecolor=c),                       
                             **box_plots_kwargs
                             )
                 hue_legends.append(boxes['boxes'][0])
             ax.legend(hue_legends,[i for i in to_plot.keys()],**legend_label)
             ax.set_xticks(xlocations)
-            ax.set_xticklabels(label_list,rotation=0)
+            ax.set_xticklabels(label_list,rotation=rotation_x)
         
         for idx, ax in enumerate(axes):
             if not all(item is None for item in separateby):
                 for separate_key in to_plot_dictionary.keys():    
                     if not all(item is None for item in hue):
                         unique_hues = np.unique(hue)
                         to_plot = {h: {x_:to_plot_dictionary[separate_key][x_][h]['y'] for x_ in unique_x } for h in unique_hues}
@@ -1311,17 +1323,18 @@
                          map_view:List=['all'],
                          atlas_slice:Union[int,list,dict]=None,
                          regions_to_hide:list=None,
                          plot_values:dict=None,
                          plot_values_threshold:float=None,
                          mask:dict=None,
                          fig:mpl.figure.Figure=None,
-                         axes:Union[np.ndarray,List]=None,
+                         axes:Union[np.ndarray,List,plt.Axes]=None,
                          colorbar:bool=False,
                          label_legend:dict=None,
+                         label_legend_colours:dict=None,
                          legends:bool=True,
                          atlas_file:Union[str,nib.nifti1.Nifti1Image]=None,
                          cmap:str='Spectral',plot_orientation:bool=True,**figkwargs):
         """
         Plot the brain segmentation
         
         Note:
@@ -1354,14 +1367,18 @@
         colorbar : bool, optional
             If plot_values is specified, then can choose if to plot the colorbar. The default is False.
         label_legend : dict, optional
             If not using the plot_values, but you want to show the segmentation.
             Each color patch in the legend will correspond to the color in the plot
             Must provide a dictionary, where the key is interger denoting the label.
             And value is the string abbreviation. The default is None.
+        label_legend_colours: dict, optional
+            If providing label_legend, and if you are performing multiple subplots. It may be good idea, to use this to have consistent colours.
+            Must provide a dictionary, where the key is interger denoting the label, and value is the colour.
+            
         legend: bool, optional
             Whether to plot the brain legend.
             The default is True
         atlas_file : Union[str,nib.nifti1.Nifti1Image], optional
             The path to the nifti file, or the nib.load(Nifti file). The default is None.
         cmap : str, optional
             The color scheme. The default is 'Spectral'.
@@ -1414,14 +1431,26 @@
             for key,value in atlas_slice.items():
                 atlas_slice_dict[key] = value                
         
         #original atlases are used to delineate the outline
         original_axial_atlas = brain_map.atlas[:,:,atlas_slice_dict['axial']].copy()
         original_coronal_atlas = brain_map.atlas[:,atlas_slice_dict['coronal'],:].copy()
         original_sagittal_atlas = brain_map.atlas[atlas_slice_dict['sagittal'],:,:].copy()
+        
+        # the following regions need to be hidden (but outline will still be shown)
+        if regions_to_hide is not None:
+            for region in regions_to_hide:
+                brain_map.atlas[brain_map.atlas == region] = np.nan
+                if 'outline_regions_to_hide' not in figkwargs:
+                    figkwargs['outline_regions_to_hide'] = True
+                if not figkwargs['outline_regions_to_hide']:
+                    original_axial_atlas = brain_map.atlas[:,:,atlas_slice_dict['axial']].copy()
+                    original_coronal_atlas = brain_map.atlas[:,atlas_slice_dict['coronal'],:].copy()
+                    original_sagittal_atlas = brain_map.atlas[atlas_slice_dict['sagittal'],:,:].copy()
+            
 
         if label_legend is not None:# if legend dictionary is provided
             unique_regions = np.unique(brain_map.atlas[~np.isnan(brain_map.atlas)]) #not labelling the np.nan values
             for region in unique_regions:
                 if region not in label_legend:
                     brain_map.atlas[brain_map.atlas==region] = np.nan #regions that are not provided in the legend they are removed from colouring.
             
@@ -1431,32 +1460,56 @@
             legend_label = {uniq_leg:[k for k in label_legend.keys() if label_legend[k] == uniq_leg] for uniq_leg in unique_legends}
             for legend,label in legend_label.items():
                 if len(label)>1:
                     for region in label:
                         #if more than one key show the same value, then change it to the same key.
                         brain_map.atlas[brain_map.atlas==region] = label[0]
             
+            ####setting vmin vmax - this is needed to get common colours across multiple plots
+            # the colours are not in sequential order. For example, number 5 and 79 denotes the same structures.
+            
+            #####ploting label legends####
+            def find_closest_name(col):
+                #taken from here
+                #https://stackoverflow.com/questions/71756150/getting-the-names-of-colors-from-matplotlib-colormap-object
+                #This function is used to get the name from to_rgb function
+                rv, gv, bv = to_rgb(col)
+                min_colors = {}
+                for col in CSS4_COLORS:
+                    rc, gc, bc = to_rgb(col)
+                    min_colors[(rc - rv) ** 2 + (gc - gv) ** 2 + (bc - bv) ** 2] = col
+                closest = min(min_colors.keys())
+                return min_colors[closest], np.sqrt(closest)
+            
+            if label_legend_colours is None:
+
+                label_val = list(set(label_legend.values()))
+                n_colors = len(label_val)
+                vals = np.linspace(0, 1, n_colors)
+                label_legend_colours_inversed = {k:find_closest_name(brain_map.cmap(val))[0] for k,val in zip(label_val,vals)} # {'temporal':[0,0,0],'parietal':[0.1,0.2,0.3],...}
+                label_legend_colours = {k:label_legend_colours_inversed[v] for k,v in label_legend.items()} #{5:[0.1,0.2,0.3],6:[1,2,3],...}
+                # brain_map.cmap = LinearSegmentedColormap.from_list('from_list',
+                #                                  [(val, col) for val, col in zip(vals, label_legend_colours.values())])
+
+            if not isinstance(label_legend_colours,dict):
+                raise TypeError('label_legend_colours need to be dictionary')
+            
+            if all(isinstance(v,str) for v in label_legend_colours.values()):
+                label_legend_colours = {k:np.array(to_rgb(v)) for k,v in label_legend_colours.items()}
+            
+            if not all(isinstance(v,np.ndarray) for v in label_legend_colours.values()):
+                raise TypeError('the colours must be defined as either string or np.ndarray. Use matplotlib.colors.to_rgb')
+                
+            
             if 'outline_label_legends' not in figkwargs: # whether to outline only the keys in the legend
                 figkwargs['outline_label_legends'] = True
             if figkwargs['outline_label_legends']:
                 original_axial_atlas = brain_map.atlas[:,:,atlas_slice_dict['axial']].copy()
                 original_coronal_atlas = brain_map.atlas[:,atlas_slice_dict['coronal'],:].copy()
                 original_sagittal_atlas = brain_map.atlas[atlas_slice_dict['sagittal'],:,:].copy()
-        
-        # the following regions need to be hide (but outline will still be shown)
-        if regions_to_hide is not None:
-            for region in regions_to_hide:
-                brain_map.atlas[brain_map.atlas == region] = np.nan
-                if 'outline_regions_to_hide' not in figkwargs:
-                    figkwargs['outline_regions_to_hide'] = True
-                if not figkwargs['outline_regions_to_hide']:
-                    original_axial_atlas = brain_map.atlas[:,:,atlas_slice_dict['axial']].copy()
-                    original_coronal_atlas = brain_map.atlas[:,atlas_slice_dict['coronal'],:].copy()
-                    original_sagittal_atlas = brain_map.atlas[atlas_slice_dict['sagittal'],:,:].copy()
-            
                 
                 
         if plot_values is not None:
             if not isinstance(plot_values,dict):
                 raise TypeError('plot_values needs to be a dictionary, where keys are the label, and values are the plot values')
             else:
                 unique_regions = np.unique(brain_map.atlas[~np.isnan(brain_map.atlas)])
@@ -1490,15 +1543,16 @@
                 if len(axes) != 3:
                     raise ValueError('need 3 axes')
             else:
                 if len(map_view) != len(axes):
                     raise ValueError('number of map_view does not match number of axes provided')
             if (fig is None) and (plot_values is not None) and (colorbar is not None):
                 raise AttributeError('Need fig element to plot the colorbar')
-        
+        elif isinstance(axes,plt.Axes) and len(map_view)==1 and map_view != 'all':
+            axes=[axes]
         #
         axial_atlas = brain_map.atlas[:,:,atlas_slice_dict['axial']].copy()
         coronal_atlas = brain_map.atlas[:,atlas_slice_dict['coronal'],:].copy()
         sagittal_atlas = brain_map.atlas[atlas_slice_dict['sagittal'],:,:].copy()
 
         map_view_dict = defaultdict(dict)
         if 'all' in map_view:
@@ -1512,20 +1566,33 @@
                 map_view_dict[view]['atlas'] = coronal_atlas
                 map_view_dict[view]['original_atlas'] = original_coronal_atlas
             elif view == 'sagittal':
                 map_view_dict[view]['atlas'] = sagittal_atlas
                 map_view_dict[view]['original_atlas'] = original_sagittal_atlas
         
         #plot the images
+        
         vmin = np.min([map_view_dict[view]['atlas'][~np.isnan(map_view_dict[view]['atlas'])].min() for view in map_view_dict.keys()])
         vmax = np.max([map_view_dict[view]['atlas'][~np.isnan(map_view_dict[view]['atlas'])].max() for view in map_view_dict.keys()])
-
+        
         for view,ax in map_view_dict.items():
-            map_view_dict[view]['im'] = map_view_dict[view]['ax'].imshow(np.rot90(map_view_dict[view]['atlas']),vmin=vmin,vmax=vmax,cmap=brain_map.cmap)
-    
+            
+            if isinstance(label_legend_colours,dict):
+                #if legend with colour is provided. We need to map the colours to the value in the atlas.
+                value_to_colour = np.ndarray(shape=(map_view_dict[view]['atlas'].shape[0],map_view_dict[view]['atlas'].shape[1],3))
+                for i in range(0, map_view_dict[view]['atlas'].shape[0]):
+                    for j in range(0, map_view_dict[view]['atlas'].shape[1]):
+                        try:
+                            value_to_colour[i][j] = label_legend_colours[map_view_dict[view]['atlas'][i][j]] 
+                        except KeyError:
+                            value_to_colour[i][j] = 1
+                map_view_dict[view]['im'] = map_view_dict[view]['ax'].imshow(np.rot90(value_to_colour))
+            else:
+                map_view_dict[view]['im'] = map_view_dict[view]['ax'].imshow(np.rot90(map_view_dict[view]['atlas']),vmin=vmin,vmax=vmax,cmap=brain_map.cmap)
+        
             #plot the outlines
             temp_original_atlas = map_view_dict[view]['original_atlas']
             for unique_label in np.unique(temp_original_atlas[~np.isnan(temp_original_atlas)]):
                 #if it is that label, draw the outline
                 temp_outline_atlas = temp_original_atlas.copy()
                 temp_outline_atlas[temp_outline_atlas != unique_label] = 0 # if it is not that label, set the pixel to 0
                 temp_outline_atlas[temp_outline_atlas == unique_label] = 1 # basically draw the border where there is pixel value 1
@@ -1553,22 +1620,18 @@
         if 'label_legend_loc' not in figkwargs:
             figkwargs['label_legend_loc'] = 'lower left'
         if 'label_legend_fontsize' not in figkwargs:
             figkwargs['label_legend_fontsize'] = 'medium'
         if label_legend is not None:
             #to plot legends?
             if legends:
-                #get the unique labels
-                values = np.unique(np.concatenate([map_view_dict[view]['atlas'].ravel() for view in map_view]))
-                values = values[~np.isnan(values)] #not labelling the np.nan values
-                # get the colors of the values, according to the 
-                # colormap used by imshow
-                temp_im = map_view_dict[list(map_view_dict)[0]]['im']
-                colors = [temp_im.cmap(temp_im.norm(value)) for value in values]
-                patches = [mpatches.Patch(color=colors[idx], label=label_legend[int(i)]) for idx, i in enumerate(values) if i in label_legend]
+                
+                to_legend = {v1:find_closest_name(v2)[0] for v1,v2 in zip(label_legend.values(),label_legend_colours.values())}
+                
+                patches = [mpatches.Patch(color=v, label=k) for k, v in to_legend.items()]
                 plt.legend(handles=patches, 
                            bbox_to_anchor=figkwargs['label_legend_bbox_to_anchor'], 
                            loc=figkwargs['label_legend_loc'],
                            ncol=figkwargs['label_legend_ncol'],
                            fontsize = figkwargs['label_legend_fontsize'],
                            frameon=False)
 
@@ -1632,23 +1695,23 @@
 
     @staticmethod
     def create_heatmap(gene_set_table:pd.DataFrame,
                        genes_set_column:str = 'GeneSet',
                        genes_list_column:str = 'genes',
                        gene_table:pd.DataFrame = None,
                        top:int = 20,
-                       ordered_by:str='P_Frontal_lobe_WM',
+                       ordered_by:str=None,
                        gene_table_gene_name:str='Genes_Name') -> List[np.array]:
         """
         Create a heatmap of gene set analysis, where the x-axis is the list of genes, and y-axis is the gene set list.
         Args:
             gene_set_table (pd.DataFrame): enrichment result in table format
-            |Geneset|P-value for phenotype 1| P-value for phenotype 2|List of genes| etc.
-            genes_set_column (str, optional): _description_. Defaults to 'GeneSet'.
-            genes_list_column (str, optional): _description_. Defaults to 'genes'.
+            |Geneset|P-value for phenotype 1| P-value for phenotype 2|List of genes| etc. (this is the FUMA table result)
+            genes_set_column (str, optional): the gene set column name. Defaults to 'GeneSet'.
+            genes_list_column (str, optional): the gene list column name. Defaults to 'genes'.
             gene_table (pd.DataFrame, optional): table containing rows of genes (or SNPs) and columns of P-value associated with 1 or 2 phenotypes (usually 1 for variable of interest and 1 taken directly from GWAS schizophrenia). Defaults to None.
         Note:
         The following genes name in the FUMA Gene-sets do not correspond with genes name in gene-table
         ['ADGRV1' if gene == 'GPR98' else 'ADGRB3' if gene == 'BAI3' else gene for gene in FUMA_gene_sets]
         
         Returns:
             heatmap: binary np.array, the x axis = list of genes, y axis = gene sets, 1 where there is a presence of the gene in gene set.
@@ -1715,63 +1778,83 @@
     @staticmethod
     def visualise_enrichment_p_value(gene_set_table:pd.DataFrame,
                                      x:str='adjP',
                                      y:str = 'GeneSet',
                                      colour_by:str = 'Proportion',
                                      xlabel:str = None,
                                      ylabel:str = None,
-                                     ax:np.array=None,
-                                     cbar_ax:np.array=None):
+                                     ax:np.array=None):
+        """Visualise the enrichment p-value from the gene-set table
+
+        Args:
+            gene_set_table (pd.DataFrame): the gene set table. (FUMA table output)
+            x (str, optional): to be plotted on the x axis. Defaults to 'adjP'.
+            y (str, optional): to be plotted on the y axis. Defaults to 'GeneSet'.
+            colour_by (str, optional): color the bar. Defaults to 'Proportion'.
+            xlabel (str, optional): x label. Defaults to None.
+            ylabel (str, optional): y label. Defaults to None.
+            ax (np.array, optional): _description_. Defaults to None.
+
+        Returns:
+            plt.plot
+        """
         norm = plt.Normalize(gene_set_table[colour_by].min(),
                              gene_set_table[colour_by].max())
         sm = plt.cm.ScalarMappable(cmap='Reds',norm = norm)
         sm.set_array([])
         
         g = sns.barplot(x=-np.log10(gene_set_table[x]), y=y, hue=colour_by, data=gene_set_table,palette='Reds', 
                         dodge=False,ax=ax)
         ax.set_ylabel(ylabel)
         ax.set_xlabel(xlabel)
         ax.legend_.remove()
         cbar = ax.figure.colorbar(sm,ax = ax)
         cbar.set_label(colour_by,fontsize=15)
         ax.set_yticks([])        
         return ax
+    
     @staticmethod    
     def visualise_heatmap(heatmap:np.array,
                           all_genes:List[str],
                           gene_sets:List[str],
                           ax:np.array,**figkwargs)->None:
         """Visualise the gene-set heatmap
 
         Args:
             heatmap (np.array): the heatmap generated by GeneSet.create_heatmap
             all_genes (List[str]): the list of genes generated by GeneSet.create_heatmap
             ax (np.array): the plt.Ax to plot on.
         """
-        ax.imshow(heatmap,vmin=0, vmax=1,aspect='equal',cmap='Blues')
+        aspect=figkwargs.get('aspect','equal')
+        x_tickrotation=figkwargs.get('x_tickrotation',45)
+        y_tickrotation=figkwargs.get('y_tickrotation',45)
+        x_tickfontsize=figkwargs.get('x_tickfontsize',15)
+        y_tickfontsize=figkwargs.get('y_tickfontsize',15)
+        ax.imshow(heatmap,vmin=0, vmax=1,aspect=aspect,cmap='Blues')
         ax.set_xticks(np.arange(0,len(all_genes),1))
         ax.set_yticks(np.arange(0,len(gene_sets),1))
         
         ax.set_xticks(np.arange(-.5, len(all_genes), 1), minor=True)
         ax.set_yticks(np.arange(-.5, len(gene_sets), 1), minor=True)
         
-        ax.set_xticklabels(all_genes,rotation=45,fontsize=15)
-        ax.set_yticklabels(gene_sets,rotation=45,fontsize=15)
+        ax.set_xticklabels(all_genes,rotation=x_tickrotation,fontsize=x_tickfontsize)
+        ax.set_yticklabels(gene_sets,rotation=y_tickrotation,fontsize=y_tickfontsize)
         ax.grid(which='minor', color='w', linestyle='-', linewidth=2)
         return ax
+    
     @staticmethod
     def visualise_gene_p_value(gene_table:pd.DataFrame,
                                all_genes:List[str],
                                gene_table_gene_name:str='Genes_Name',
-                               ordered_by:str='P_Frontal_lobe_WM',
-                               coloured_by:str='P_schizo',
+                               ordered_by:str=None,
+                               coloured_by:str=None,
                                bar_number:str='N_SNP',
                                p_threshold:float=5e-08,
                                ax:np.array=None,
-                               cbar_ax=None)->None:
+                               cbar_ax=None,**kwargs)->None:
         """Visualise the p-value of the genes in genes list.
 
         Args:
             gene_table (pd.DataFrame): _description_
             all_genes (List[str]): _description_
             ordered_by (str,optional): the p-value column name to order by
             coloured_by (str, optional): the p-value column name to colour the bar. Defaults to P_schizo.
@@ -1787,15 +1870,16 @@
         gene_table = gene_table.sort_values(by=gene_table_gene_name).reset_index(drop=True)
         bar_plot_y_axis = -np.log10(gene_table[ordered_by].tolist())
         
         g = sns.barplot(x=gene_table_gene_name,
                         y=bar_plot_y_axis,
                         data=gene_table,
                         ax=ax)
-        
+        cbar_label=kwargs.get('cbar_label','disease')
+        ylabel=kwargs.get('ylabel','phenotype')
         if coloured_by is not None:
             bar_plot_colour_by = -np.log10(gene_table[coloured_by].tolist())
             if p_threshold is not None:
                 bar_clrs = ['grey' if x < -np.log10(p_threshold) else 'red' for x in bar_plot_colour_by]
                 for patch,bar_clr in zip(g.patches,bar_clrs):
                     patch.set_color(bar_clr)
                     
@@ -1808,27 +1892,28 @@
                 sm = plt.cm.ScalarMappable(cmap=my_cmap,norm=norm)
                 sm.set_array([])
                 palette = np.array(pal)
                 for patch,bar_clr in zip(g.patches,palette[rank[index]]):
                     patch.set_color(bar_clr)
                 if cbar_ax is not None:
                     cbar = g.figure.colorbar(sm,cax = cbar_ax)
-                    cbar.set_label('$-log_{10}(SNP p-value) SCZ $',fontsize=15)
+                    if cbar_label is not None:
+                        cbar.set_label('$-log_{10}(SNP p-value)%s$'%cbar_label,fontsize=15)
 
         if bar_number is not None:                   
             for patch,label in zip(g.patches,gene_table.loc[:,bar_number].tolist()):
                 if label > 1:
                     ax.annotate(label,
                                 (patch.get_x()*1.005,
                                 patch.get_height()*1.005),fontsize = 15)
         
         ax.set_xticks([])
         ax.set_xlabel('') 
         
-        ax.set_ylabel('$-log_{10}(SNP p-value) FL_{WM}.R$',fontsize=15)
+        ax.set_ylabel('$-log_{10}(SNP p-value) %s$'%ylabel,fontsize=15)
         return ax
         
         
         
         
     
 def visualise_heatmap(df,
```


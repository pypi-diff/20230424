# Comparing `tmp/speechtotext-python-0.3.5.tar.gz` & `tmp/speechtotext-python-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.5.tar", last modified: Tue Apr 18 08:11:47 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.6.tar", last modified: Mon Apr 24 09:28:16 2023, max compression
```

## Comparing `speechtotext-python-0.3.5.tar` & `speechtotext-python-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3458 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6399 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 08:11:47.000000 speechtotext-python-0.3.5/speechtotext_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:11:47.803644 speechtotext-python-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 08:10:25.000000 speechtotext-python-0.3.5/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.371530 speechtotext-python-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:28:16.371530 speechtotext-python-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4109 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3603 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/tests/test_imports.py
```

### Comparing `speechtotext-python-0.3.5/LICENSE` & `speechtotext-python-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.5/PKG-INFO` & `speechtotext-python-0.3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.5/setup.py` & `speechtotext-python-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 EMAIL = 'jarneamerlinck@gmail.com'
 AUTHOR = 'Jarne Amerlinck'
 REQUIRES_PYTHON = '>=3.9.2,<3.11'
 VERSION = '' # Version is defined in __version__.py in the package
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-	'jiwer', 'pandas', 'numpy', 'torch', 
+	'jiwer', 'pandas<2.0.0', 'numpy', 'torch>=2.0.0', 
 	'openai-whisper', 'openai', 'python-dotenv',
 	'matplotlib', 'ipywidgets', 'seaborn',
 	'dtale', 'boto3', 'google-cloud-speech',
 	'deepgram-sdk', 'azure-cognitiveservices-speech', 
-	'speechmatics-python==1.6.4', 'pydub'
+	'speechmatics-python==1.6.4', 'pydub', 'docstring_parser'
 ]
 
 # What packages are optional?
 EXTRAS = {
 	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
 			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'pytest']
 }
```

### Comparing `speechtotext-python-0.3.5/speechtotext/datasets.py` & `speechtotext-python-0.3.6/speechtotext/datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,22 +35,24 @@
 	# Get n trandom samples
 	dataset_n_random: SampleDataset = dataset.get_n_samples(number_of_samples)
 """
 
 from os.path import exists
 import pandas as pd
 
+from speechtotext.functions import get_file_name_without_extention
+
 class DatasetBare():
 	"""Bare dataset class.
 	"""    
 	def __init__(self, path_to_dir:str, name: str, file_ext:str=".wav"):
 		"""Creates dataset object.
 		There needs to be an transcripts.txt directly in the dir.
 		Args:
-			path_to_dir (str): path to dir ending with "/".
+			path_to_dir (str): Path to dir ending with "/".
 			name (str): Name of dataset.
 			file_ext (str): Extention of files.
 		"""     
 		self.name = name
 		self.path_to_dir = path_to_dir
 		self.file_ext = file_ext
 
@@ -62,18 +64,18 @@
 		"""     
 		return self.dataset.shape[0]
   
 	def get_path_of_fragment(self, id:str)-> str:
 		"""Gets path of fragment.
 
 		Args:
-			id (str): id of file.
+			id (str): Id of file.
 
 		Raises:
-			FileNotFoundError: if id doesn't exist.
+			FileNotFoundError: If id doesn't exist.
 
 		Returns:
 			str: Path to fragment.
 		"""     
 		path = f"{self.path_to_dir}/{id}{self.file_ext}"
 
 		if exists(path):
@@ -81,18 +83,18 @@
 		else:
 			raise FileNotFoundError()
 		 
 	def get_text_of_id(self, id:str) -> str:
 		"""Get text of fragment id.
 
 		Args:
-			id (str): id of fragment.
+			id (str): Id of fragment.
 
 		Returns:
-			str: string of spoken text.
+			str: String of spoken text.
 		"""     
 		row = self.dataset[self.dataset["id"] == id]
 		try:
 			return row.values[0][1]
 		except:
 			return None
 
@@ -114,24 +116,25 @@
 		"""Loads transcript.
 		"""     
 		file_path = f"{self.path_to_dir}/transcripts.txt"
 
 		df= pd.read_csv(file_path, sep="|", header=None)
 		df = df.iloc[:, 0:2] 
 		df.columns = ["id", "text"]
+		df['id'] = df['id'].apply(lambda id :get_file_name_without_extention(id) )
 		self.dataset = df
 
 	def get_n_samples(self, number_of_samples:int) -> SampleDataset:
 		"""Get n random samples.
 
 		Args:
 			number_of_samples (int): Number of random samples.
 
 		Returns:
-			SampleDataset: dataset with the samples.
+			SampleDataset: Dataset with the samples.
 		"""     
 		if number_of_samples > self.number_of_samples():
 			print("number larger then samples in dataset. Using full dataset")
 			number_of_samples = self.dataset.number_of_samples()
 		df = self.dataset.sample(n=number_of_samples)
 
 		return SampleDataset(df, self.path_to_dir, self.name, self.file_ext)
```

### Comparing `speechtotext-python-0.3.5/speechtotext/functions.py` & `speechtotext-python-0.3.6/speechtotext/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,62 +8,64 @@
  	from speechtotext.functions import *
 	
 	# Force torch use for cuda
 	force_cudnn_initialization()
 	
 	# Clean string
 	string_cleaning("this has.//./8 to be cleaned::@")
-
-Attributes:
-	REGEX_STRING_PARSE (str): Regex string parce used to clean up transcripts that are used to validate the speechtotext models.
 """
 
 from functools import wraps
 from time import time
 import os
 import re
 import torch
 import functools
 import pandas as pd
 from datetime import datetime
 from abc import ABC, abstractmethod
 from dotenv import load_dotenv
 
-REGEX_STRING_PARSE = '[^A-Za-z0-9 ]+'
-
-DEFAULT_DATATIME_FORMAT = datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
-DEFAULT_REPORTS_FOLDER = "reports"
-DEFAULT_CSV_NAME = f"{DEFAULT_REPORTS_FOLDER}/Benchmark_results_{DEFAULT_DATATIME_FORMAT}.csv"
-DEFAULT_HTML_NAME = f"{DEFAULT_REPORTS_FOLDER}/Benchmark_results_{DEFAULT_DATATIME_FORMAT}.html"
-DEFAULT_HTML_TITLE = f"{DEFAULT_REPORTS_FOLDER}/Benchmark results of {DEFAULT_DATATIME_FORMAT}"
-
+REGEX_STRING_PARSE:str = '[^A-Za-z0-9 ]+'
+"""str: Regex used to clean the transcripts.
+"""
+DEFAULT_DATETIME_FORMAT:str = datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
+"""str: Default datetime format. (Uses string format for datetime)
+"""
+DEFAULT_REPORTS_FOLDER:str = "reports"
+"""str: Default folder to save the reports.
+"""
+DEFAULT_CSV_NAME:str = f"{DEFAULT_REPORTS_FOLDER}/Benchmark_results_{DEFAULT_DATETIME_FORMAT}.csv"
+"""str: Default path to save Benchmark results.
+"""
 
 def force_cudnn_initialization():
-	"""Force torch use for cuda.
+	"""Force torch use for cuda if available.
 	"""    
-	s = 32
-	dev = torch.device('cuda')
-	torch.nn.functional.conv2d(torch.zeros(s, s, s, s, device=dev), torch.zeros(s, s, s, s, device=dev))
+	if torch.cuda.is_available():
+		s = 32
+		dev = torch.device('cuda')
+		torch.nn.functional.conv2d(torch.zeros(s, s, s, s, device=dev), torch.zeros(s, s, s, s, device=dev))
 
 def string_cleaning(text:str)-> str:
 	"""Cleaning of string for STT.
 
 	Args:
-		text (str): uncleaned string.
+		text (str): Uncleaned string.
 
 	Returns:
-		str: cleaned string.
+		str: Cleaned string.
 	"""    
 	return re.sub(REGEX_STRING_PARSE, '', text)
 
 def join_benchmark_results(results: list[pd.core.frame.DataFrame], set_index=True) -> pd.core.frame.DataFrame:
 	"""Join Benchmark results.
 
 	Args:
-			results (list[pd.core.frame.DataFrame]): results of benchmarks.
+			results (list[pd.core.frame.DataFrame]): Results of benchmarks.
 			set_index (bool, optional): Set True if ["model_name", "audio_ID"] can be set as index. Defaults to True.
 
 	Returns:
 			pd.core.frame.DataFrame: Dataframe with results of all benchmarks.
 	"""
 	df = pd.concat(results)
 	if set_index:
@@ -73,15 +75,15 @@
 def separate_benchmark_results_by_model(dataframe: pd.core.frame.DataFrame) -> dict[str, pd.core.frame.DataFrame]:
 	"""Seperate benchmark results for each model.
 
 	Args:
 			dataframe pd.core.frame.DataFrame: Dataframe with results of all benchmarks.
 
 	Returns:
-			(list[pd.core.frame.DataFrame]): results of benchmarks. 
+			(list[pd.core.frame.DataFrame]): Results of benchmarks. 
 	"""
 	
 	model_names = dataframe["model_name"].unique()
 
 	DataFrameDict = {elem : pd.DataFrame() for elem in model_names}
 
 	for key in DataFrameDict.keys():
@@ -93,56 +95,59 @@
 	return DataFrameDict
 
 def benchmark_results_to_csv(results: list[pd.core.frame.DataFrame], save_name:str=DEFAULT_CSV_NAME):
 	"""Creates csv from benchmark results.
 	
 	Args:
 		results (list[pd.core.frame.DataFrame]): List of results from benchmarks.
-		save_name (str, optional): filename of output. Defaults to DEFAULT_CSV_NAME.
+		save_name (str, optional): Filename of output. Defaults to DEFAULT_CSV_NAME.
 	"""  
 	df = pd.concat(results)
 	df.to_csv(save_name, index=False)
  
 def save_sub_folder_name(folder_path:str, subfolder_name:str) -> str:
 	"""Creates subfolder path.
 
 	Args:
-		folder_path (str): path of parent folder.
-		subfolder_name (str): subfolder name.
+		folder_path (str): Path of parent folder.
+		subfolder_name (str): Subfolder name.
 
 	Returns:
-		str: path to save folder.
+		str: Path to save folder.
 	"""    
 	folder_name =  f"{folder_path}/{subfolder_name}"
 	if not os.path.isdir(folder_name):
 		os.makedirs(folder_name)
 	return folder_name
 
 def save_folder_name(report_name:str, folder_name:str = DEFAULT_REPORTS_FOLDER) -> str:
 	"""Makes folder path.
 
 	Args:
-		report_name (str): name of report.
+		report_name (str): Name of report.
 		folder_name (str, optional): Name of folder. Defaults to DEFAULT_REPORT_FOLDER.
 
 	Returns:
 		str: path to save folder.
 	"""    
-	folder_name =  f"{folder_name}/{report_name}_{DEFAULT_DATATIME_FORMAT}"
+	folder_name =  f"{folder_name}/{report_name}_{DEFAULT_DATETIME_FORMAT}"
 	if not os.path.isdir(folder_name):
 		os.makedirs(folder_name)
 	return folder_name
 
 class BaseResult(ABC):
+	"""Parent class for results. 
+ 	Child class should be made and added to Plotting.CUSTOM_RESULTS, Plotting.CUSTOM_ERRORS, Plotting.CUSTOM_PLOTS or Plotting.CUSTOM_ERROR_PLOTS
+	"""   
 	def __init__(self, df:pd.core.frame.DataFrame, report_folder:str, file_name:str):
 		"""Creates object of BaseResult. Child class should be added to Plotting.CUSTOM_RESULTS.
 
 		Args:
-			df (pd.core.frame.DataFrame): dataframe that needs to be plotted.
-			report_folder (str): path to report folder.
+			df (pd.core.frame.DataFrame): Dataframe that needs to be plotted.
+			report_folder (str): Path to report folder.
 			file_name (str): Name of saved File.
 		"""     
 		self.report_folder = report_folder
 		self.file_name = file_name
 		self.df = df
 		self.save_file_name = f"{self.report_folder}/{self.file_name}{self.ext}"
 
@@ -172,14 +177,25 @@
 
 	Returns:
 		str: Extention of tile name.
 	"""    
 	file_name, _ = os.path.splitext(file_name)
 	return file_name
 
+def uppercase_for_first_character_in_string(string:str) -> str:
+	"""Return string where first character is uppercase.
+
+	Args:
+		string (str): String to process.
+
+	Returns:
+		str: String where first character is uppercase.
+	"""    
+	return  string[0].upper() + string[1:]
+
 def multidispatch(*types):
 	"""Allow for Method overloading for classes.
 	"""    
 	def register(function):
 		name = function.__name__
 		mm = multidispatch.registry.get(name)
 		if mm is None:
@@ -212,15 +228,15 @@
 	Args:
 		env_name (str): .env key.
 
 	Raises:
 		RequiredEnvVariablesMissing: Prints the variable name if its missing.
 
 	Returns:
-		str: value of the .env key.
+		str: Value of the .env key.
 	"""    
 	load_dotenv()
 	if env_name not in os.environ:
 		raise RequiredEnvVariablesMissing(env_name)
 	return os.getenv(env_name)
```

### Comparing `speechtotext-python-0.3.5/speechtotext_python.egg-info/PKG-INFO` & `speechtotext-python-0.3.6/speechtotext_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.5/tests/test_imports.py` & `speechtotext-python-0.3.6/tests/test_imports.py`

 * *Files identical despite different names*


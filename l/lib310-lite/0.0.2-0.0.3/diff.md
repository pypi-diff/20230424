# Comparing `tmp/lib310_lite-0.0.2.tar.gz` & `tmp/lib310_lite-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.2.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.3.tar", max compression
```

## Comparing `lib310_lite-0.0.2.tar` & `lib310_lite-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      249 2023-03-13 17:23:54.978361 lib310_lite-0.0.2/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     8274 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      769 2023-03-13 17:23:54.982361 lib310_lite-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 lib310_lite-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.3/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.3/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-03-08 14:56:22.918017 lib310_lite-0.0.3/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.3/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.3/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9326 2023-04-24 18:40:54.149010 lib310_lite-0.0.3/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      769 2023-04-24 17:55:46.127215 lib310_lite-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 lib310_lite-0.0.3/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 lib310_lite-0.0.3/PKG-INFO
```

### Comparing `lib310_lite-0.0.2/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.3/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.2/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.3/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.2/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.3/lib310_lite/mldl/mldl.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,157 +8,165 @@
 import concurrent.futures
 from bounded_pool_executor import BoundedThreadPoolExecutor
 import dask.dataframe as dd
 from ..bigquery.client import Client as BigQueryClient
 from ..bigquery.constants import FileFormat
 
 
-TRAIN = 'TRAIN'
-TEST = 'TEST'
-MAIN = 'MAIN'
-INTERACTION = 'INTERACTION'
+class MLDL:
 
+    __TRAIN = 'TRAIN'
+    __TEST = 'TEST'
+    __MAIN = 'MAIN'
+    __INTERACTION = 'INTERACTION'
+    __DB_NAME = 'A310'
+    __TOKEN_NAMES = 'token_names'
+    __PARTS = {__INTERACTION: 1, __TOKEN_NAMES: 1}
 
-class MLDL:
-    def __init__(self, mongo_url: str, cache_size: int = 50, num_threads: int = 10):
-        random.seed(time.time())
+    def __init__(self, mongo_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
+        random.seed(random_seed)
         self.client = MongoClient(mongo_url)
         self.bq_client = BigQueryClient()
-        self.db = self.client['A310']
+        self.db = self.client[MLDL.__DB_NAME]
+
         self.collections = {
-            TRAIN: {
-                MAIN: self.db['seq_lang5_train'],
-                INTERACTION: self.db['interactions_lang5_train'],
+            MLDL.__TRAIN: {
+                MLDL.__MAIN: self.db['seq_lang5'],
+                MLDL.__INTERACTION: self.db['interactions_lang5_train'],
             },
-            TEST: {
-                MAIN: self.db['seq_lang5_test'],
-                INTERACTION: self.db['interactions_lang5_test'],
+            MLDL.__TEST: {
+                MLDL.__MAIN: self.db['seq_lang5'],
+                MLDL.__INTERACTION: self.db['interactions_lang5_test'],
             }
         }
 
-        self.cache = {TRAIN: {}, TEST: {}}
+        # this is the pool of samples row_id
         self.sample_cache = []
+        # this is the maximum number of requests we fetch sooner from the database
         self.max_queue_size = cache_size
+        # this is the number of threads we use to fetch data from the database
         self.num_threads = num_threads
+        # this is the key that we know MLDL requests are same or not if it changes we need to fetch new data
         self.queue_key = None
+        # this is the key shows that pool is still valid or not
         self.pool_key = None
+        # this is the queue that we use to cache requests and put it in the queue
         self.queue = Queue(self.max_queue_size)
+        # this is the thread that we use to fill the queue
         self.filler_thread = None
+        # this is the event that we use to kill the filler thread
         self.kill_event = Event()
+        # this is the number of retries we have
         self.retry = 0
 
-
-        # Cache the data with regard to length of sequence
-        tmp = self.db['length_freq_lang5_train'].find().sort('len', ASCENDING)
-        for item in tmp:
-            self.cache[TRAIN][item['len']] = {'freq': item['freq'], 'maxi': item['maxi'], 'mini': item['mini']}
-        tmp = self.db['length_freq_lang5_test'].find().sort('len', ASCENDING)
-        for item in tmp:
-            self.cache[TEST][item['len']] = {'freq': item['freq'], 'maxi': item['maxi'], 'mini': item['mini']}
-
-    def get_batch(self, num: int, max_length: int, min_num_feature: int = 0, stage: str = TRAIN):
+    def get_batch(self, num: int, max_length: int, min_num_feature: int = 0, stage: str = __TRAIN, parts: dict = None):
         """
         Get a batch of data from the database with regard to the length of the sequence and the number of features
         It also start the background thread to fill the caches and queue
         :param num: number of samples
         :param max_length: maximum length of the sequence
         :param min_num_feature: minimum number of features
         :param stage: TRAIN or TEST
+        :param parts: the parts of the data that we want to fetch
         :return: a pandas dataframe
         """
         stage = stage.upper()
-        if stage == TRAIN:
-            col = self.collections[TRAIN]
-        elif stage == TEST:
-            col = self.collections[TEST]
+        if stage == MLDL.__TRAIN:
+            col = self.collections[MLDL.__TRAIN]
+        elif stage == MLDL.__TEST:
+            col = self.collections[MLDL.__TEST]
         else:
             raise ValueError('Stage must be either TRAIN or TEST')
 
-        if max_length not in self.cache[stage.upper()].keys():
-            arr = [i for i in self.cache[stage.upper()].keys() if i <= max_length]
-            if len(arr) == 0:
-                return pd.DataFrame()
-            max_length = max(arr)
+        if parts is None:
+            parts = MLDL.__PARTS
 
         hit = self.queue_key == f'{num}_{max_length}_{min_num_feature}_{stage}'
         if hit:
             # HIT
             return pd.DataFrame(self.queue.get())
 
         # MISS
-        maxi = self.cache[stage.upper()][max_length]['maxi']
-        if min_num_feature > 11:
-            table = '1_uniprot.mongo_lang5_train'
-            if stage == TEST:
-                table = '1_uniprot.mongo_lang5_test'
-            if len(self.sample_cache) == 0 or not self.pool_key or self.pool_key != f'{max_length}_{min_num_feature}_{stage}':
-                self.pool_key = f'{max_length}_{min_num_feature}_{stage}'
-                res = self.bq_client.cache_query(
-                    query=f"SELECT row_id FROM `{table}` WHERE len <= {max_length} and token_size >= {min_num_feature}",
-                    name=f'{max_length}_{min_num_feature}_{stage}',
-                    destination_format=FileFormat.CSV,
-                )
-                ddf = dd.read_csv(res['uri'])
-                df = ddf.compute()
-                self.sample_cache = df['row_id'].tolist()
-        else:
-            self.sample_cache = range(1, maxi)
+        table = '1_uniprot.mongo_lang5'
+        
+        if len(self.sample_cache) == 0 or not self.pool_key or self.pool_key != f'{max_length}_{min_num_feature}_{stage}':
+            self.pool_key = f'{max_length}_{min_num_feature}_{stage}'
+            res = self.bq_client.cache_query(
+                query=f"SELECT row_id FROM `{table}` WHERE len <= {max_length} and token_size >= {min_num_feature} and stage = '{stage}'",
+                name=f'{max_length}_{min_num_feature}_{stage}',
+                destination_format=FileFormat.CSV,
+            )
+            ddf = dd.read_csv(res['uri'])
+            df = ddf.compute()
+            self.sample_cache = df['row_id'].tolist()
 
+        # killing the previous thread
         if self.filler_thread is not None:
             self.kill_event.set()
             self.queue.get()
             self.filler_thread.join()
             self.kill_event.clear()
             self.queue = Queue(self.max_queue_size)
 
+        # generate new key
         self.queue_key = f'{num}_{max_length}_{min_num_feature}_{stage}'
 
-        self.filler_thread = Thread(target=self.filler, args=(num, col))
+        # start new thread
+        self.filler_thread = Thread(target=self.filler, args=(num, col, stage, parts))
         self.filler_thread.start()
         time.sleep(3)
-        return self.fetch_sample(num, col)
+        return self.fetch_sample(num, col, stage, parts)
 
-    def filler(self, num: int, col):
+    def filler(self, num: int, col, stage: str, parts: dict = None):
         """
         This function is used to fill the queue with data then get batch read data from the queue
         :param num: number of samples
         :param col: collections of the data
+        :param stage: TRAIN or TEST
+        :param parts: the parts of the data that we want to fetch
         """
+        if parts is None:
+            parts = MLDL.__PARTS
         with BoundedThreadPoolExecutor(max_workers=self.num_threads) as executor:
             while not self.kill_event.is_set():
-                # print(f'filler thread started {self.kill_event.is_set()}')
-                executor.submit(self.filler_worker, num, col)
-            # print(f'filler thread ended {self.kill_event.is_set()}')
+                executor.submit(self.filler_worker, num, col, stage, parts)
             while not self.queue.empty():
                 self.queue.get()
-            # print('queue emptied')
             executor.shutdown(wait=True)
-            # print('executor shutdown')
 
-    def filler_worker(self, num: int, col):
-        df = self.fetch_sample(num, col)
+    def filler_worker(self, num: int, col, stage: str, parts: dict = None):
+        if parts is None:
+            parts = MLDL.__PARTS
+        df = self.fetch_sample(num, col, stage, parts)
         self.queue.put(df)
         return
 
-    def fetch_sample(self, num: int, collections):
+    def fetch_sample(self, num: int, collections, stage: str, parts: dict = None):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
         :param collections: collections of the data
+        :param stage: TRAIN or TEST
+        :param parts: the parts of the data that we want to fetch
         :return: dataframe of the data
         """
+        if parts is None:
+            parts = MLDL.__PARTS
         try:
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, collections[MAIN])
-                interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, collections[INTERACTION])
+                main_thread = executor.submit(self.fetch_sample_main, index_list, collections[MLDL.__MAIN], stage, parts)
+                if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, collections[MLDL.__INTERACTION])
 
                 main_df = main_thread.result()
-                interaction_df = interaction_thread.result()
+                interaction_df = pd.DataFrame()
+                if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
+                    interaction_df = interaction_thread.result()
 
                 if len(interaction_df) == 0:
                     main_df['interactions'] = np.nan
                     self.retry = 0
                     return main_df
                 df = pd.merge(main_df, interaction_df, on='row_id', how='left')
                 self.retry = 0
@@ -169,24 +177,32 @@
                 time.sleep(1)
             else:
                 time.sleep(self.retry * 10)
             self.retry += 1
             print(f'Cannot fetch data from database, retry number {self.retry} times')
             if self.retry > 7:
                 raise Exception('Cannot fetch data from database')
-            return self.fetch_sample(num, collections)
+            return self.fetch_sample(num, collections, stage, parts)
 
-    def fetch_sample_main(self, index_list: list, col):
+    def fetch_sample_main(self, index_list: list, col, stage: str, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
         :param col: main collection
+        :param stage: stage of the data
+        :param parts: parts of the data
         :return: dataframe of main data
         """
-        cursor = col.find({'row_id': {'$in': index_list}}, {'_id': 0, 'row_id': 1, 'sequence': 1, 'token_ids': 1})
+        if parts is None:
+            parts = MLDL.__PARTS
+        token_names = 0
+        if parts[MLDL.__TOKEN_NAMES] and parts[MLDL.__TOKEN_NAMES] == 1:
+            token_names = 1
+        cursor = col.pofind({'row_id': {'$in': index_list}, 'stage': stage}, {'_id': 0, 'row_id': 1, 'sequence': 1,
+                                                                            'token_ids': 1, 'token_names': token_names})
         return pd.DataFrame(list(cursor))
 
     def fetch_sample_interaction(self, index_list: list, col):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
         :param col: interaction collection
```

### Comparing `lib310_lite-0.0.2/pyproject.toml` & `lib310_lite-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.2"
+version = "0.0.3"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.2/PKG-INFO` & `lib310_lite-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.2
+Version: 0.0.3
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bounded_pool_executor (>=0.0.0)
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: dask-sql (>=2022.11.0)
 Requires-Dist: db-dtypes (>=1.0.0)
 Requires-Dist: distributed (>=2022.11.0)
 Requires-Dist: gcsfs (>=2022.11.0)
 Requires-Dist: google-cloud (>=0.34.0)
```


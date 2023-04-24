# Comparing `tmp/etl_csm_pet-0.0.5.tar.gz` & `tmp/etl_csm_pet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm_pet-0.0.5.tar", last modified: Wed Apr 19 20:29:34 2023, max compression
+gzip compressed data, was "etl_csm_pet-0.0.6.tar", last modified: Mon Apr 24 15:04:01 2023, max compression
```

## Comparing `etl_csm_pet-0.0.5.tar` & `etl_csm_pet-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.975407 etl_csm_pet-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.971408 etl_csm_pet-0.0.5/Etl/
--rw-rw-rw-   0        0        0     3381 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Execute.py
--rw-rw-rw-   0        0        0     1577 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Extrator.py
--rw-rw-rw-   0        0        0     2812 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Helper.py
--rw-rw-rw-   0        0        0     2023 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Loader.py
--rw-rw-rw-   0        0        0     4918 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.5/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.5/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.5/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      552 2023-04-19 20:29:34.975407 etl_csm_pet-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.974407 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/
--rw-rw-rw-   0        0        0      552 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:29:34.976407 etl_csm_pet-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-19 20:29:04.000000 etl_csm_pet-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:04:01.830376 etl_csm_pet-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:04:01.825379 etl_csm_pet-0.0.6/Etl/
+-rw-rw-rw-   0        0        0     3389 2023-04-24 15:00:15.000000 etl_csm_pet-0.0.6/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1577 2023-04-24 15:00:15.000000 etl_csm_pet-0.0.6/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     2812 2023-04-24 15:00:15.000000 etl_csm_pet-0.0.6/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1980 2023-04-24 15:02:57.000000 etl_csm_pet-0.0.6/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4918 2023-04-24 15:00:15.000000 etl_csm_pet-0.0.6/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.6/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.6/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.6/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      552 2023-04-24 15:04:01.829376 etl_csm_pet-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:04:01.828377 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-04-24 15:04:01.000000 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-24 15:04:01.000000 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:04:01.000000 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-24 15:04:01.000000 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-24 15:04:01.000000 etl_csm_pet-0.0.6/etl_csm_pet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:04:01.830376 etl_csm_pet-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-24 15:03:36.000000 etl_csm_pet-0.0.6/setup.py
```

### Comparing `etl_csm_pet-0.0.5/Etl/Execute.py` & `etl_csm_pet-0.0.6/Etl/Execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     def etl_extras_df_pme(self,df:Type) -> Type:
         extras_df = form_df_extras(df) #1
         extras_df = patternizing_columns(extras_df) #2
         # extras_df = ensure_nan_extras(extras_df) #3 Deixar para avaliacao
         # extras_df = fill_na_extras(extras_df) #4 Deixar para avaliacao
         # extras_df = dtype_extras(extras_df) #5 Deixar para avaliacao
         return extras_df
+    
+
 
     def run(self) -> None:
         if self.bot == 'residential':
             df = self.etl_df()
             extras_df = self.etl_extras_df(df)
             df = concat([df,extras_df],axis = 1)
             load_cloud(df,self.bot)
```

### Comparing `etl_csm_pet-0.0.5/Etl/Extrator.py` & `etl_csm_pet-0.0.6/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/Etl/Helper.py` & `etl_csm_pet-0.0.6/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/Etl/Loader.py` & `etl_csm_pet-0.0.6/Etl/Loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,19 @@
     Ira fazer o processo de carregamento para o RDS depois de processado.
     Ira estipular os datatype para sqlalchemy
     Em seu excption acrescentar nova coluna de acordo com o datatype que ela precisa
     ARGS
     df = pd.DataFrame
     """
     engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PET_PASSWORD']}@pet-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
-    sql_dic = sqlcol(df) 
     tries = 5
 
     for _ in range(tries):
         try:
-            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,dtype = sql_dic ,method = psql_insert_copy,if_exists='append',index = False,chunksize = 10000)
+            df.to_sql(f'{bot}_tracking_treated',engine_alchemy, method = psql_insert_copy,if_exists='append',index = False,chunksize = 10000)
         except  (Exception,psycopg2.Error) as error:
             warning("Tivemos um erro", error)
             warning("Vou executar um handler para ver se consigo resolver!")         
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
                 password = environ['SQL_PRD_PASSWORD'],
```

### Comparing `etl_csm_pet-0.0.5/Etl/Treatment_extras.py` & `etl_csm_pet-0.0.6/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/Etl/Treatment_tracking.py` & `etl_csm_pet-0.0.6/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/Etl/Treatment_tracking_pme.py` & `etl_csm_pet-0.0.6/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/Etl/__init__.py` & `etl_csm_pet-0.0.6/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/LICENSE` & `etl_csm_pet-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/PKG-INFO` & `etl_csm_pet-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm_pet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.5/README.md` & `etl_csm_pet-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.5/etl_csm_pet.egg-info/PKG-INFO` & `etl_csm_pet-0.0.6/etl_csm_pet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm-pet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.5/setup.py` & `etl_csm_pet-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm_pet",
     version = VERSION,
     author = "ingloriamori",
```


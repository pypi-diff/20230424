# Comparing `tmp/NikeCA-0.1.82.tar.gz` & `tmp/NikeCA-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.82.tar", last modified: Mon Apr 24 07:06:20 2023, max compression
+gzip compressed data, was "NikeCA-0.1.83.tar", last modified: Mon Apr 24 07:25:00 2023, max compression
```

## Comparing `NikeCA-0.1.82.tar` & `NikeCA-0.1.83.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.971609 NikeCA-0.1.82/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.82/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:06:20.971327 NikeCA-0.1.82/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.82/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 07:06:20.971693 NikeCA-0.1.82/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 07:05:44.000000 NikeCA-0.1.82/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.966243 NikeCA-0.1.82/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.967122 NikeCA-0.1.82/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.967912 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.969169 NikeCA-0.1.82/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6622 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.970905 NikeCA-0.1.82/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      332 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.369698 NikeCA-0.1.83/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.83/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:25:00.369149 NikeCA-0.1.83/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.83/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 07:25:00.369865 NikeCA-0.1.83/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 07:24:54.000000 NikeCA-0.1.83/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.360946 NikeCA-0.1.83/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.362946 NikeCA-0.1.83/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.364030 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.365292 NikeCA-0.1.83/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6117 2023-04-24 07:19:42.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.368386 NikeCA-0.1.83/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      332 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/__init__.py
```

### Comparing `NikeCA-0.1.82/LICENSE` & `NikeCA-0.1.83/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/PKG-INFO` & `NikeCA-0.1.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.82
+Version: 0.1.83
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.82/README.md` & `NikeCA-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/setup.py` & `NikeCA-0.1.83/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.82',
+	version='0.1.83',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.82/src/Dashboards/Dashboards.py` & `NikeCA-0.1.83/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.83/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.83/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.83/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,184 +1,186 @@
 
+from mdpr.src.Dashboards.Telemetry.ProductUsage import ProductUsage
 
-class Telemetry:
 
-    class ProductUsage:
-        def product_viewed(self
-                           , username: str
-                           , warehouse: str
-                           , database: str
-                           , role: str
-                           , filters: list | None = None
-                           , order_by: list | None = None
-                           , polars: bool = False
-                           , start_date: str = '1900-01-01'
-                           , end_date: str = '9999-12-31'
-                           ):
-
-            from NikeCA import Snowflake
-            import polars as pl
-            import configparser
-
-            config = configparser.ConfigParser()
-            config.read('pip.ini')
-
-            b = config['telemetry_product_usage'].get('col_b')
-
-            # Ensure filters is a list
-            if not (isinstance(filters, list) or filters is None):
-                raise TypeError("filters must be a list")
-
-            # Ensure order_by is a list
-            if not (isinstance(order_by, list) or order_by is None):
-                raise TypeError("order_by must be a list")
-
-            if order_by is None:
-                order_by = config['telemetry_product_usage'].get('order_by')
-            else:
-                order_by = ', '.join(order_by)
-
-            query = f"""
-                    /*
-                    The query calculates the daily usage of different data products on different platforms, groups the data by platform and product, and sorts the result in descending order based on the total usage
-                    */
-                    SELECT 
-                        {b}
-                        , PRODUCT_NAME
-                        , SUM(DAILY_USAGE) AS TOTAL_USAGE
-                    FROM (
-    
-                    {self.get_base_query(start_date=start_date, end_date=end_date)}
-    
-                    )
-    
-                    GROUP BY 
-                        {b}
-                        , PRODUCT_NAME
-    
-                    HAVING 
-                        TOTAL_USAGE > 0
-    
-                    ORDER BY
-                        {order_by}
-    
-                    ;
-                """
-
-            df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
-                                        role=role).snowflake_pull(query=query, polars=polars))
-
-            print(query)
-
-            return df
-
-        def get_base_query(self
-                           , filters: list | None = None
-                           , start_date: str = '1900-01-01'
-                           , end_date: str = '9999-12-31'
-                           ):
-
-            import configparser
-
-            config = configparser.ConfigParser()
-            config.read('pip.ini')
-
-            table = config['telemetry_product_usage'].get('table')
-            a = config['telemetry_product_usage'].get('col_a')
-            b = config['telemetry_product_usage'].get('col_b')
-            c = config['telemetry_product_usage'].get('col_c')
-            d = config['telemetry_product_usage'].get('col_d')
-            e = config['telemetry_product_usage'].get('col_e')
-            f = config['telemetry_product_usage'].get('col_f')
-            g = config['telemetry_product_usage'].get('col_g')
-            date_column = config['telemetry_product_usage'].get('date_column')
-            filter_a = config['telemetry_product_usage'].get('filter_a')
-            filter_b = config['telemetry_product_usage'].get('filter_b')
-            filter_c = config['telemetry_product_usage'].get('filter_c')
-
-            # Ensure filters is a list
-            if not (isinstance(filters, list) or filters is None):
-                raise TypeError("filters must be a list")
-
-            if filters is None:
-                filters = []
-                filters_str = f'WHERE {date_column} BETWEEN {start_date} AND {end_date}'
-
-            # Join column filters into comma-separated string, if any
-            if len(filters) > 0:
-                filters_str = 'AND '.join(filters)
-                filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}' AND {filters_str}"
-            else:
-                filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}'"
-
-            base_query = f"""
-                    SELECT
-                        DISTINCT 
-                        {a}
-                        , {b}
-                        , CASE 
-                            WHEN {b} = '{filter_a}' THEN {c}
-                            WHEN {b} = '{filter_b}' THEN {d}
-                            WHEN {b} = '{filter_c}' THEN {e}
-                            else null 
-                        END AS PRODUCT_NAME
-                        , COUNT(DISTINCT {f})
-                        , (SUM({g})/NULLIF(COUNT(DISTINCT {f}),0 )) AS DAILY_USAGE
-                    FROM 
-                        {table}
-    
-                    {filters_str}
-    
-                    GROUP BY
-                        {a}
-                        , {b}
-                        , PRODUCT_NAME
+class Telemetry(ProductUsage):
+
+    ProductUsage = ProductUsage
+
+    def product_viewed(self
+                       , username: str
+                       , warehouse: str
+                       , database: str
+                       , role: str
+                       , filters: list | None = None
+                       , order_by: list | None = None
+                       , polars: bool = False
+                       , start_date: str = '1900-01-01'
+                       , end_date: str = '9999-12-31'
+                       ):
+
+        from NikeCA import Snowflake
+        import polars as pl
+        import configparser
+
+        config = configparser.ConfigParser()
+        config.read('pip.ini')
+
+        b = config['telemetry_product_usage'].get('col_b')
+
+        # Ensure filters is a list
+        if not (isinstance(filters, list) or filters is None):
+            raise TypeError("filters must be a list")
+
+        # Ensure order_by is a list
+        if not (isinstance(order_by, list) or order_by is None):
+            raise TypeError("order_by must be a list")
+
+        if order_by is None:
+            order_by = config['telemetry_product_usage'].get('order_by')
+        else:
+            order_by = ', '.join(order_by)
+
+        query = f"""
+                /*
+                The query calculates the daily usage of different data products on different platforms, groups the data by platform and product, and sorts the result in descending order based on the total usage
+                */
+                SELECT 
+                    {b}
+                    , PRODUCT_NAME
+                    , SUM(DAILY_USAGE) AS TOTAL_USAGE
+                FROM (
+
+                {self.get_base_query(start_date=start_date, end_date=end_date)}
+
+                )
+
+                GROUP BY 
+                    {b}
+                    , PRODUCT_NAME
+
+                HAVING 
+                    TOTAL_USAGE > 0
+
+                ORDER BY
+                    {order_by}
+
+                ;
             """
-            return base_query
 
+        df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
+                                    role=role).snowflake_pull(query=query, polars=polars))
+
+        print(query)
+
+        return df
 
-        def summary(self
-                    , username: str
-                    , warehouse: str
-                    , database: str
-                    , role: str
-                    , filters: list | None = None
-                    , order_by: list | None = None
-                    , polars: bool = False
-                    , start_date: str = '1900-01-01'
-                    , end_date: str = '9999-12-31'
-                    ):
-            import configparser
-
-            config = configparser.ConfigParser()
-            config.read('pip.ini')
-            b = config['telemetry_product_usage'].get('col_b')
-
-            if order_by is None:
-                order_by = config['telemetry_product_usage'].get('order_by')
-            else:
-                order_by = ', '.join(order_by)
-
-            query = f"""
-            SELECT 
-                DISTINCT
-                {b}
-                , SUM(DAILY_USAGE) OVER (PARTITION BY {b}) AS TOTAL_USAGE
-            FROM (
-                {self.get_base_query(start_date=start_date, end_date=end_date, filters=filters)}   
-            )
-            ORDER BY
-                {order_by}
+    def get_base_query(self
+                       , filters: list | None = None
+                       , start_date: str = '1900-01-01'
+                       , end_date: str = '9999-12-31'
+                       ):
+
+        import configparser
+
+        config = configparser.ConfigParser()
+        config.read('pip.ini')
+
+        table = config['telemetry_product_usage'].get('table')
+        a = config['telemetry_product_usage'].get('col_a')
+        b = config['telemetry_product_usage'].get('col_b')
+        c = config['telemetry_product_usage'].get('col_c')
+        d = config['telemetry_product_usage'].get('col_d')
+        e = config['telemetry_product_usage'].get('col_e')
+        f = config['telemetry_product_usage'].get('col_f')
+        g = config['telemetry_product_usage'].get('col_g')
+        date_column = config['telemetry_product_usage'].get('date_column')
+        filter_a = config['telemetry_product_usage'].get('filter_a')
+        filter_b = config['telemetry_product_usage'].get('filter_b')
+        filter_c = config['telemetry_product_usage'].get('filter_c')
+
+        # Ensure filters is a list
+        if not (isinstance(filters, list) or filters is None):
+            raise TypeError("filters must be a list")
+
+        if filters is None:
+            filters = []
+            filters_str = f'WHERE {date_column} BETWEEN {start_date} AND {end_date}'
+
+        # Join column filters into comma-separated string, if any
+        if len(filters) > 0:
+            filters_str = 'AND '.join(filters)
+            filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}' AND {filters_str}"
+        else:
+            filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}'"
+
+        base_query = f"""
+                SELECT
+                    DISTINCT 
+                    {a}
+                    , {b}
+                    , CASE 
+                        WHEN {b} = '{filter_a}' THEN {c}
+                        WHEN {b} = '{filter_b}' THEN {d}
+                        WHEN {b} = '{filter_c}' THEN {e}
+                        else null 
+                    END AS PRODUCT_NAME
+                    , COUNT(DISTINCT {f})
+                    , (SUM({g})/NULLIF(COUNT(DISTINCT {f}),0 )) AS DAILY_USAGE
+                FROM 
+                    {table}
+
+                {filters_str}
+
+                GROUP BY
+                    {a}
+                    , {b}
+                    , PRODUCT_NAME
         """
+        return base_query
 
-            from NikeCA import Snowflake
-            import polars as pl
+    def summary(self
+                , username: str
+                , warehouse: str
+                , database: str
+                , role: str
+                , filters: list | None = None
+                , order_by: list | None = None
+                , polars: bool = False
+                , start_date: str = '1900-01-01'
+                , end_date: str = '9999-12-31'
+                ):
+        import configparser
+
+        config = configparser.ConfigParser()
+        config.read('pip.ini')
+        b = config['telemetry_product_usage'].get('col_b')
+
+        if order_by is None:
+            order_by = config['telemetry_product_usage'].get('order_by')
+        else:
+            order_by = ', '.join(order_by)
+
+        query = f"""
+        SELECT 
+            DISTINCT
+            {b}
+            , SUM(DAILY_USAGE) OVER (PARTITION BY {b}) AS TOTAL_USAGE
+        FROM (
+            {self.get_base_query(start_date=start_date, end_date=end_date, filters=filters)}   
+        )
+        ORDER BY
+            {order_by}
+    """
+
+        from NikeCA import Snowflake
+        import polars as pl
 
-            df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
-                                        role=role).snowflake_pull(query=query, polars=polars))
+        df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
+                                    role=role).snowflake_pull(query=query, polars=polars))
 
-            print(query)
+        print(query)
 
-            return df
+        return df
```

### Comparing `NikeCA-0.1.82/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.83/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.82
+Version: 0.1.83
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.82/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.83/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.83/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/NikeQA.py` & `NikeCA-0.1.83/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/NikeSF.py` & `NikeCA-0.1.83/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_BuildSearchQuery.py` & `NikeCA-0.1.83/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_GitHub.py` & `NikeCA-0.1.83/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_QA.py` & `NikeCA-0.1.83/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_SearchFiles.py` & `NikeCA-0.1.83/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_SnowflakeData.py` & `NikeCA-0.1.83/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_SnowflakeDependencies.py` & `NikeCA-0.1.83/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.82/src/_SnowflakePull.py` & `NikeCA-0.1.83/src/_SnowflakePull.py`

 * *Files identical despite different names*


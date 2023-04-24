# Comparing `tmp/hkfdb-2.6.tar.gz` & `tmp/hkfdb-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.6.tar", last modified: Sun Apr 16 06:42:34 2023, max compression
+gzip compressed data, was "hkfdb-2.7.tar", last modified: Mon Apr 24 10:23:06 2023, max compression
```

## Comparing `hkfdb-2.6.tar` & `hkfdb-2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.531413 hkfdb-2.6/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-2.6/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-04-16 06:42:34.531223 hkfdb-2.6/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-2.6/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.530286 hkfdb-2.6/hkfdb/
--rw-r--r--   0 cmw        (501) staff       (20)    90392 2023-04-16 06:32:33.000000 hkfdb-2.6/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-2.6/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.531017 hkfdb-2.6/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-16 06:42:34.531465 hkfdb-2.6/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-04-16 06:42:27.000000 hkfdb-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.642122 hkfdb-2.7/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.7/LICENSE
+-rw-rw-rw-   0        0        0     1651 2023-04-24 10:23:06.642122 hkfdb-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.631468 hkfdb-2.7/hkfdb/
+-rw-rw-rw-   0        0        0    90787 2023-04-24 10:19:26.000000 hkfdb-2.7/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.7/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.641111 hkfdb-2.7/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1651 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:23:06.642122 hkfdb-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-04-24 10:20:36.000000 hkfdb-2.7/setup.py
```

### Comparing `hkfdb-2.6/LICENSE` & `hkfdb-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.6/PKG-INFO` & `hkfdb-2.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,70 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 2.6
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
-
-
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 2.7
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
```

### Comparing `hkfdb-2.6/README.md` & `hkfdb-2.7/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.6/hkfdb/Database.py` & `hkfdb-2.7/hkfdb/Database.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             freq_str = 'freq=' + freq
             price_adj_str = 'price_adj=0' if price_adj == False else 'price_adj=1'
             vol_adj_str = 'vol_adj=0' if vol_adj == False else 'vol_adj=1'
             link_str = link_url + code_str + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + \
                        end_date_str + '&' + freq_str + '&' + price_adj_str + '&' + vol_adj_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 if price_adj == False:
                     json1 = json.loads(response.content).replace("'", "\"").replace('False','0').replace('True','1').replace('nan','NaN')
                     ohlc_result = json.loads(json1)
@@ -93,15 +93,15 @@
 
                     last_date = str(max([int(qfq_df.loc[qfq_df.index[-1], 'date']), int(df.loc[df.index[-1], 'date'])]))
 
                     if '-' in qfq_df.at[0, 'date']:
                         qfq_df['date'] = pd.to_datetime(qfq_df['date'], format='%Y-%m-%d')
                     else:
                         qfq_df['date'] = pd.to_datetime(qfq_df['date'], format='%Y%m%d')
-                        
+
                     qfq_df = qfq_df.set_index(keys='date')
                     t_index = pd.DatetimeIndex(pd.date_range(start=first_date, end=last_date, freq='1D'))
 
                     qfq_df = qfq_df.reindex(t_index)
                     qfq_df = qfq_df.fillna(method='bfill')
                     qfq_df = qfq_df.fillna(method='ffill')
                     qfq_df = qfq_df.reset_index()
@@ -150,15 +150,15 @@
                     df['time'] = df['time'].astype(int)
                 else:
                     df['time'] = 0
 
                 df = df[['date', 'time', 'open', 'high', 'low', 'close', 'volume']]
 
                 return df
-    
+
     def get_us_stock_ohlc(self, code, start_date, end_date):
 
         check_bool_dict = self.check_us_stock_ohlc_args(code, start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
@@ -304,15 +304,14 @@
                         back_year_month = str(date_list[-1])[2:6]
                         front_expiry_date = int(expiry_date_dict[front_year_month].strftime('%Y%m%d'))
                         back_expiry_date = int(expiry_date_dict[back_year_month].strftime('%Y%m%d'))
                         for i in range(len(date_list)):
                             date_item = date_list[i]
 
                             if i + rolling_day <= len(date_list) - 1:
-                                print(i, date_list[i + rolling_day], front_expiry_date)
                                 if date_list[i + rolling_day] == front_expiry_date:
                                     front_cut_off_date = date_item
                                 elif date_list[i + rolling_day] == back_expiry_date:
                                     back_cut_off_date = date_item
                                     break
                             else:
                                 back_cut_off_date = max(date_list)
@@ -407,15 +406,15 @@
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
     def get_hk_market_cap_hist_by_date(self, start_date, end_date):
-        
+
         check_bool_dict = self.check_start_end_date(start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_market_cap_hist_by_date'
             start_date_str = 'start_date=' + str(start_date)
@@ -438,36 +437,41 @@
                     if len(df) > 0:
                         df['date'] = str(date_int)
                         df_list.append(df)
                 df = pd.concat(df_list)
 
                 df = df.sort_values(['date', 'market_cap_mil'], ascending=[True, False])
                 df = df.reset_index(drop=True)
-                df['date'] = pd.to_datetime(df['date'],format='%Y-%m-%d')
+
+                if '-' in df.at[0, 'date']:
+                    df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
+                else:
+                    df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
+
                 df = df[['date','code','issued_share_mil','market_cap_mil','cumulative_market_cap_mil']]
                 return df
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
     def get_hk_market_cap_hist_by_code(self, code):
-        
+
         check_bool_dict = self.check_hk_code_args(code)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_market_cap_hist_by_code'
             code_str = 'code=' + str(code)
             link_str = link_url + '&' + token_str + '&' + database_str + '&' + code_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 json_content = json.loads(response.content)
                 json_content = json_content.replace(' nan', '\" nan\"')
                 result = json.loads(json_content.replace("'", "\""))
@@ -479,15 +483,18 @@
                     if len(df) > 0:
                         df['date'] = str(date_int)
                         df_list.append(df)
                 df = pd.concat(df_list)
 
                 df = df.sort_values(by='date')
                 df = df.reset_index(drop=True)
-                df['date'] = pd.to_datetime(df['date'],format='%Y-%m-%d')
+                if '-' in df.at[0, 'date']:
+                    df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
+                else:
+                    df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
                 df = df[['date','code','issued_share_mil','market_cap_mil','cumulative_market_cap_mil']]
                 df = df.set_index('date')
                 df = df[~df.index.duplicated(keep='first')]
 
                 return df
 
         else:
@@ -500,15 +507,15 @@
     def get_hk_buyback_by_code(self, code, agg_value = False):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'hk_buyback_by_code'
         code_str = 'code=' + code
         link_str = link_url + code_str + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
         if response_ok == True:
 
             result = json.loads(json.loads(response.content).replace("'", "\""))
 
             df = pd.DataFrame(result)
@@ -530,15 +537,15 @@
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_buyback_by_date'
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 json_content = json.loads(response.content)
                 json_content = json_content.replace(' nan', '\" nan\"')
 
@@ -661,15 +668,15 @@
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_earning_calendar_by_date'
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = ast.literal_eval(json.loads(response.content))
 
                 df_list = []
@@ -698,40 +705,40 @@
     def get_us_earning_calendar_by_code(self, code):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'us_earning_calendar_by_code'
         code_str = 'code=' + code
         link_str = link_url + code_str + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
         if response_ok == True:
 
             result = ast.literal_eval(json.loads(response.content))
 
             temp_list = list(result)
             date_list = []
             for date in temp_list:
                 date_list.append(datetime.datetime.strptime(date,'%Y-%m-%d').date())
 
             return date_list
 
     def get_us_earning_calendar_by_date(self, start_date, end_date):
-        
+
         check_bool_dict = self.check_start_end_date(start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'us_earning_calendar_by_date'
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df_list = []
@@ -765,15 +772,15 @@
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'ccass_by_code'
             code_str = 'code=' + code
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + code_str + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df_list = []
@@ -798,15 +805,15 @@
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
-            
+
     def get_ccass_holding_rank(self, code, start_date, end_date):
 
         check_bool_dict = self.check_ccass_holding_rank_args(code, start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
@@ -1029,80 +1036,92 @@
 
             for i in range(len(df)):
                 end_date = df.loc[i,'end_date']
                 if end_date == mode:
                     df.at[i,'end_date'] = datetime.datetime.now().strftime('%Y-%m-%d')
             for col in df.columns:
                 if col == 'start_date' or col == 'end_date':
-                    df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                    if '-' in df.at[0, col]:
+                        df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                    else:
+                        df[col] = pd.to_datetime(df[col], format='%Y%m%d')
+
 
         return df
-    
+
     def get_hk_index_const(self, index_name, sort_mkt_cap = False):
-        
+
         if len(index_name) > 0:
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_index_const'
             index_name_str = 'index_name=' + index_name
             link_str = link_url + index_name_str + '&' + token_str + '&' + database_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
 
             if response_ok == True:
 
                 result = ast.literal_eval(json.loads(response.content))
 
                 df = pd.DataFrame(result)
                 df['code'] = df['code'].str.zfill(5)
 
                 for col in df.columns:
                     if col == 'start_date' or col == 'end_date':
-                        df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                        if '-' in df.at[0, col]:
+                            df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                        else:
+                            df[col] = pd.to_datetime(df[col], format='%Y%m%d')
 
                 if index_name == 'hsi_const_hist':
 
                     df['is_alive'] = df['is_alive'].astype(bool)
                     df = df.rename(columns={'is_alive':'is_active'})
 
                     for i in range(len(df)):
                         end_date = df.loc[i, 'end_date']
                         is_active = df.loc[i, 'is_active']
                         if is_active == True:
+
                             df.at[i, 'end_date'] = datetime.datetime.now().strftime('%Y-%m-%d')
 
                     for col in df.columns:
                         if col == 'start_date' or col == 'end_date':
-                            df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                            if '-' in df.at[0, col]:
+                                df[col] = pd.to_datetime(df[col], format='%Y-%m-%d')
+                            else:
+                                df[col] = pd.to_datetime(df[col], format='%Y%m%d')
+
                     df = df[['code','name','start_date','end_date','is_active']]
 
                 if sort_mkt_cap:
                     info = self.get_basic_hk_stock_info()
                     info = info[['code','market_capital']]
                     df = pd.merge(df, info, on='code', how='inner')
                     df = df.sort_values(by='market_capital', ascending=False)
 
                 return df
 
         else:
             err_msg =  'index_name missing'
             print(err_msg)
-            
+
     def get_hk_stock_plate_const(self, plate_name):
-        
+
         if len(plate_name) > 0:
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'hk_stock_plate_const'
             plate_name_str = 'plate_name=' + plate_name
             link_str = link_url + plate_name_str + '&' + token_str + '&' + database_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df = pd.DataFrame(result)
@@ -1110,23 +1129,23 @@
                 df['code'] = df['code'].str.zfill(5)
 
                 return df
 
         else:
             err_msg =  'index_name missing'
             print(err_msg)
-            
-        
+
+
     def get_all_hk_index_name(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'all_hk_index_name'
         link_str = link_url + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
         if response_ok == True:
 
             result = ast.literal_eval(json.loads(response.content))
 
             name_list = list(result)
@@ -1137,15 +1156,15 @@
 
     def get_all_hk_stock_plate_name(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'all_hk_stock_plate_name'
         link_str = link_url + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
 
         if response_ok == True:
 
             result = ast.literal_eval(json.loads(response.content))
 
@@ -1155,15 +1174,15 @@
 
     def get_basic_hk_stock_info(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'basic_hk_stock_info'
         link_str = link_url + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
         if response_ok == True:
 
             r_content = response.content
             json1 = json.loads(r_content).replace("'", "\"")
             json1 = json1.replace('nan','NaN')
@@ -1174,15 +1193,18 @@
             json1 = json1.replace('\"\"True\"\"','\"True\"')
             json1 = json1.replace('\"\"False\"\"','\"False\"')
 
             result = json.loads(json1)
 
             df = pd.DataFrame(result)
 
-            df['ipo_date'] = pd.to_datetime(df['ipo_date'],format='%Y-%m-%d')
+            if '-' in df.at[0, 'ipo_date']:
+                df['ipo_date'] = pd.to_datetime(df['ipo_date'], format='%Y-%m-%d')
+            else:
+                df['ipo_date'] = pd.to_datetime(df['ipo_date'], format='%Y%m%d')
 
             df['share_issued'] = df['share_issued'].astype(str)
             df['share_issued'] = df['share_issued'].str.replace('-','', regex=False)
             df['share_issued'] = df['share_issued'].astype('int64')
 
             df['volume'] = df['volume'].str.replace('.0','', regex=False)
             df['turnover'] = df['turnover'].str.replace('.0','', regex=False)
@@ -1211,15 +1233,15 @@
 
     def get_hk_ipo_hist(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'hk_ipo_hist'
         link_str = link_url + '&' + token_str + '&' + database_str
-        
+
         response = requests.get(link_str)
         response_ok = response_check(response)
         if response_ok == True:
 
             json_content = json.loads(response.content)
             json_content = json_content.replace(' nan', '\" nan\"')
             json_content = json_content.replace('N/A\\n\\n', '0')
@@ -1244,29 +1266,29 @@
 
             df['prospectus_date'] = pd.to_datetime(df['prospectus_date'], format='%d/%m/%Y')
             df['listing_date'] = pd.to_datetime(df['listing_date'], format='%d/%m/%Y')
 
             return df
 
     def get_market_highlight(self, start_date, end_date):
-        
+
         market = 'hk_main_board'
-        
+
         check_bool_dict = self.check_market_highlight_args(market, start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'market_highlight'
             market_str = 'market=' + market
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + market_str + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + \
                        end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df_list = []
@@ -1302,15 +1324,15 @@
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
             database_str = 'database=' + 'north_water'
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + '&' + token_str + '&' + database_str + '&' + start_date_str + '&' + \
                        end_date_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 json_content = json.loads(response.content)
                 if 'nan' in json_content:
                     result = json.loads(json_content.replace("'", "\"").replace("nan", "0"))
@@ -1354,22 +1376,23 @@
             exp_str = 'exp=' + exp
             database_str = 'database=' + 'hk_deri_daily_market_report'
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             link_str = link_url + '&' + token_str + '&' + database_str \
                        + '&' + start_date_str + '&' + end_date_str\
                        + '&' + deri_str  + '&' + code_str  + '&' + exp_str
-            
+
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df_list = []
+
                 for item in result:
                     date_int = item['_id']
                     df = pd.DataFrame(item['content'])
                     if len(df) > 0:
                         df['date'] = str(date_int)
                         df_list.append(df)
                 df = pd.concat(df_list)
@@ -1449,27 +1472,27 @@
                         if type(content) is list:
                             df = pd.DataFrame(content, columns=columns)
                             df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
                             df['listing_date'] = pd.to_datetime(df['listing_date'], format='%Y%m%d')
                             df_list.append(df)
 
                 df = pd.concat(df_list)
-                df = df.sort_values('unique_id')
+                df = df.sort_values('date')
                 df = df.set_index('unique_id')
                 # df = df.drop('index', axis=1)
 
                 return df
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
-            
+
     #########################################################################################
 
     def check_hk_stock_ohlc_args(self, code, start_date, end_date, freq):
         freq_list = ['1T', '5T', '15T', '30T', '1D','1DW']
         freq_valid = True if freq in freq_list else False
 
         try:
@@ -1509,26 +1532,26 @@
         #     end_date_future = False
 
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),'%Y%m%d').date() >= \
                                    datetime.datetime.strptime(str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
+
         check_bool_dict = {'freq_valid': freq_valid,
                            'code_isdigit': code_isdigit,
                            'code_length': code_length,
                            'start_date_length': start_date_length,
                            'start_date_is_int': start_date_is_int,
                            'start_date_future': start_date_future,
                            'end_date_is_int': end_date_is_int,
                            'end_date_length': end_date_length,
                            #'end_date_future': end_date_future,
                            'end_after_start_date': end_after_start_date}
-        
+
         return check_bool_dict
     def check_us_stock_ohlc_args(self, code, start_date, end_date):
 
         try:
             code_length = len(code) > 0
         except:
             code_length = False
@@ -1561,25 +1584,25 @@
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),
                                                               '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
-        
+
+
         check_bool_dict = {'code_length': code_length,
                            'start_date_length': start_date_length,
                            'start_date_is_int': start_date_is_int,
                            'start_date_future': start_date_future,
                            'end_date_is_int': end_date_is_int,
                            'end_date_length': end_date_length,
                            #'end_date_future': end_date_future,
                            'end_after_start_date': end_after_start_date}
-        
+
         return check_bool_dict
 
     def check_hk_fut_ohlc_args(self, index, freq, start_date, end_date, rolling_day, rolling_time):
 
         freq_list = ['1T', '5T', '15T', '1D']
         freq_valid = True if freq in freq_list else False
 
@@ -1725,24 +1748,24 @@
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),
                                                               '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
+
         check_bool_dict = {
             'start_date_length': start_date_length,
             'start_date_is_int': start_date_is_int,
             'start_date_future': start_date_future,
             'end_date_is_int': end_date_is_int,
             'end_date_length': end_date_length,
             #'end_date_future': end_date_future,
             'end_after_start_date': end_after_start_date}
-        
+
         return check_bool_dict
 
     def check_ccass_by_id_args(self, ccass_id, start_date, end_date):
         if len(ccass_id) > 0:
             ccass_id_len = True
         else:
             ccass_id_len = False
@@ -1772,26 +1795,26 @@
         # except:
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date), '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
-        
+
+
         check_bool_dict = {'ccass_id_len' : ccass_id_len,
                            'start_date_length': start_date_length,
                            'start_date_is_int': start_date_is_int,
                            'start_date_future': start_date_future,
                            'end_date_is_int': end_date_is_int,
                            'end_date_length': end_date_length,
                            #'end_date_future': end_date_future,
                            'end_after_start_date': end_after_start_date}
         return check_bool_dict
-    
+
     def check_ccass_by_code_args(self, code, start_date, end_date):
 
         try:
             code_length = len(code) == 5
         except:
             code_length = False
         try:
@@ -1826,27 +1849,27 @@
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),
                                                               '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
-        
+
+
         check_bool_dict = {
             'code_isdigit': code_isdigit,
             'code_length': code_length,
             'start_date_length': start_date_length,
             'start_date_is_int': start_date_is_int,
             'start_date_future': start_date_future,
             'end_date_is_int': end_date_is_int,
             'end_date_length': end_date_length,
             #'end_date_future': end_date_future,
             'end_after_start_date': end_after_start_date}
-        
+
         return check_bool_dict
     def check_ccass_holding_rank_args(self, code, start_date, end_date):
 
         try:
             code_length = len(code) == 5
         except:
             code_length = False
@@ -1883,15 +1906,15 @@
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),
                                                               '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
+
 
         check_bool_dict = {
             'code_isdigit': code_isdigit,
             'code_length': code_length,
             'start_date_length': start_date_length,
             'start_date_is_int': start_date_is_int,
             'start_date_future': start_date_future,
@@ -1950,16 +1973,16 @@
         #     end_date_future = False
         try:
             end_after_start_date = datetime.datetime.strptime(str(end_date),
                                                               '%Y%m%d').date() >= datetime.datetime.strptime(
                 str(start_date), '%Y%m%d').date()
         except:
             end_after_start_date = False
-        
-        
+
+
         check_bool_dict = {'code_length': code_length,
                            'start_date_length': start_date_length,
                            'start_date_is_int': start_date_is_int,
                            'start_date_future': start_date_future,
                            'end_date_is_int': end_date_is_int,
                            'end_date_length': end_date_length,
                            #'end_date_future': end_date_future,
```

### Comparing `hkfdb-2.6/hkfdb.egg-info/PKG-INFO` & `hkfdb-2.7/hkfdb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,70 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 2.6
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
-
-
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 2.7
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
```

### Comparing `hkfdb-2.6/setup.py` & `hkfdb-2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.6",
+    version="2.7",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```


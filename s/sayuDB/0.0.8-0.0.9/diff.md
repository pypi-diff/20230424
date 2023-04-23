# Comparing `tmp/sayuDB-0.0.8.tar.gz` & `tmp/sayuDB-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-0.0.8.tar", last modified: Mon Apr 17 20:49:10 2023, max compression
+gzip compressed data, was "sayuDB-0.0.9.tar", last modified: Sun Apr 23 22:39:44 2023, max compression
```

## Comparing `sayuDB-0.0.8.tar` & `sayuDB-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.823084 sayuDB-0.0.8/
--rw-rw-rw-   0        0        0     1064 2023-04-08 21:51:28.000000 sayuDB-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     6072 2023-04-17 20:49:10.821672 sayuDB-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5767 2023-04-08 21:51:28.000000 sayuDB-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.815647 sayuDB-0.0.8/sayuDB/
--rw-rw-rw-   0        0        0      635 2023-04-08 21:51:28.000000 sayuDB-0.0.8/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-04-17 20:47:46.000000 sayuDB-0.0.8/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    20386 2023-04-17 20:45:24.000000 sayuDB-0.0.8/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2042 2023-04-08 21:52:33.000000 sayuDB-0.0.8/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3252 2023-04-08 21:52:17.000000 sayuDB-0.0.8/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.821672 sayuDB-0.0.8/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     6072 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 20:49:10.823084 sayuDB-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     6275 2023-04-17 20:47:37.000000 sayuDB-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.354617 sayuDB-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9981 2023-04-23 22:39:44.354617 sayuDB-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9672 2023-04-23 22:35:49.000000 sayuDB-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.325718 sayuDB-0.0.9/sayuDB/
+-rw-rw-rw-   0        0        0      635 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-04-23 22:36:18.000000 sayuDB-0.0.9/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    21632 2023-04-23 06:25:51.000000 sayuDB-0.0.9/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-04-23 05:32:47.000000 sayuDB-0.0.9/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:44.353614 sayuDB-0.0.9/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 22:39:44.000000 sayuDB-0.0.9/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 22:39:44.354617 sayuDB-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0    10184 2023-04-23 22:37:07.000000 sayuDB-0.0.9/setup.py
```

### Comparing `sayuDB-0.0.8/LICENSE` & `sayuDB-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Arsybai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Arsybai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sayuDB-0.0.8/sayuDB/__init__.py` & `sayuDB-0.0.9/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.8/sayuDB/__main__.py` & `sayuDB-0.0.9/sayuDB/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except:
     print("Read the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""Invalid commad. get help by
 --h""")
     exit()
 
 if sys.argv[1] == "help" or sys.argv[1] == '--h':
-    print("sayuDB v0.0.8\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
+    print("sayuDB v0.0.9\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""
 [ USERS ]
 Show Users  \t\t: show users
 Create user \t\t: create user <username> <password>
 Remove user \t\t: remove user <username>
 
 [ DATABASE ]
```

### Comparing `sayuDB-0.0.8/sayuDB/processor.py` & `sayuDB-0.0.9/sayuDB/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,18 @@
                 print("Import error")
     else:
         print("File or directory not found")
         
 
 class sayuDB:
     
-    def __init__(self, database, username:str=None, password:str=None, host:str=None):
+    def __init__(self, database, username:str=None, password:str=None, host:str=None, as_json=None):
         self.database = database
         self.is_remote = False
+        self.as_json = as_json
         if username != None and host != None:
             self.is_remote = True
             self.remote = remote.remote(username, password, host)
             self.remote.database_exsistence(database)
         return None
     
     def save_table(self, name: str, content: object):
@@ -270,14 +271,16 @@
         Args:
             table (str): The table name
             col (_type_): The column what you want to show. use * for all column
             where (_type_, optional): where the column contain some value. Defaults to None.
             order_by (_type_, optional): short data by column asc or desc. Defaults to None.
             as_json (bool, optional): return as json or table. Defaults to False.
         """
+        if self.as_json != None:
+            as_json = self.as_json
         db_ = self.openDB()
         datas_ = db_[table]['datas']
         if col == '*':
             datas_ = datas_
         else:
             col = col.split(',')
             idx = 0
@@ -475,14 +478,37 @@
                     temp_.append(i)
         elif ' contain ' in where:
             col_ = where.split(' contain ')[0]
             val_ = where.split(' contain ')[1]
             for i in db_[table]['datas']:
                 if str(val_) not in str(i[col_]):
                     temp_.append(i)
+        elif 'row between ' in where:
+            temp_ = []
+            to_del_ = []
+            pp_ = where.replace("row between ","").split("-")
+            if int(pp_[0]) > len(db_[table]["datas"]) or int(pp_[1]) > len(db_[table]["datas"]):
+                raise Exception("Row number out of range")
+            if int(pp_[0]) > int(pp_[1]):
+                raise Exception("The number between x-y. the x can not bigger or same with the y")
+            for i in range(int(pp_[0])-1, int(pp_[1])-1):
+                to_del_.append(db_[table]["datas"][i])
+            for i in db_[table]["datas"]:
+                if i not in to_del_:
+                    temp_.append(i)
+        elif 'row ' in where and 'between' not in where:
+            temp_ = []
+            to_del_ = []
+            pp_ = where.replace("row ","")
+            if int(pp_) > len(db_[table]["datas"]):
+                raise Exception("Row number out of range")
+            to_del_.append(db_[table]["datas"][int(pp_)-1])
+            for i in db_[table]["datas"]:
+                if i not in to_del_:
+                    temp_.append(i)
         db_[table]["datas"] = temp_
         self.save_table(table, db_)
 
     def alter_table_rename_column(self,table:str, col:str, to_:str):
         db = self.openDB()
         db[table]["column"][to_] = db[table]["column"][col]
         del db[table]["column"][col]
```

### Comparing `sayuDB-0.0.8/sayuDB/remote.py` & `sayuDB-0.0.9/sayuDB/remote.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.8/sayuDB/server.py` & `sayuDB-0.0.9/sayuDB/server.py`

 * *Files identical despite different names*


# Comparing `tmp/dorsa_logging-1.0.3.tar.gz` & `tmp/dorsa_logging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorsa_logging-1.0.3.tar", last modified: Thu Apr 13 11:17:53 2023, max compression
+gzip compressed data, was "dorsa_logging-1.1.0.tar", last modified: Mon Apr 24 03:06:19 2023, max compression
```

## Comparing `dorsa_logging-1.0.3.tar` & `dorsa_logging-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.0.3/LICENSE.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1084 2023-04-13 08:42:14.000000 dorsa_logging-1.0.3/README.md
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/dorsa_logging/
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)       39 2023-04-13 11:16:22.000000 dorsa_logging-1.0.3/dorsa_logging/__init__.py
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7223 2023-04-13 08:43:26.000000 dorsa_logging-1.0.3/dorsa_logging/logging_funcs.py
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/dorsa_logging.egg-info/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/requires.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/top_level.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/setup.cfg
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1723 2023-04-13 11:17:30.000000 dorsa_logging-1.0.3/setup.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-24 03:06:19.480275 dorsa_logging-1.1.0/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.1.0/LICENSE.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1929 2023-04-24 03:06:19.480275 dorsa_logging-1.1.0/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1085 2023-04-24 03:02:02.000000 dorsa_logging-1.1.0/README.md
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-24 03:06:19.476276 dorsa_logging-1.1.0/dorsa_logging/
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)       39 2023-04-13 11:16:22.000000 dorsa_logging-1.1.0/dorsa_logging/__init__.py
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7341 2023-04-24 03:01:39.000000 dorsa_logging-1.1.0/dorsa_logging/logging_funcs.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-24 03:06:19.480275 dorsa_logging-1.1.0/dorsa_logging.egg-info/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1929 2023-04-24 03:06:19.000000 dorsa_logging-1.1.0/dorsa_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-24 03:06:19.000000 dorsa_logging-1.1.0/dorsa_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-24 03:06:19.000000 dorsa_logging-1.1.0/dorsa_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-24 03:06:19.000000 dorsa_logging-1.1.0/dorsa_logging.egg-info/requires.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-24 03:06:19.000000 dorsa_logging-1.1.0/dorsa_logging.egg-info/top_level.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-24 03:06:19.480275 dorsa_logging-1.1.0/setup.cfg
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1723 2023-04-24 03:02:33.000000 dorsa_logging-1.1.0/setup.py
```

### Comparing `dorsa_logging-1.0.3/LICENSE.txt` & `dorsa_logging-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.3/PKG-INFO` & `dorsa_logging-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa_logging
-Version: 1.0.3
+Version: 1.1.0
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
@@ -38,12 +38,12 @@
 
 logger.set_current_user(current_username='DORSA')
 logger.create_new_log(message='This is a debug message', level=0)
 logger.create_new_log(message='This is a info message', level=1)
 logger.create_new_log(message='This is a warning message', level=2)
 logger.create_new_log(message='This is a error message', level=3)
 logger.create_new_log(message='This is a critical error message', level=4)
-logger.create_new_log(message='This is a excepion error message', level=5)
+logger.create_new_log(message='This is a exception error message', level=5)
 ```
 ## License
 [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/)
```

### Comparing `dorsa_logging-1.0.3/README.md` & `dorsa_logging-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
 logger.set_current_user(current_username='DORSA')
 logger.create_new_log(message='This is a debug message', level=0)
 logger.create_new_log(message='This is a info message', level=1)
 logger.create_new_log(message='This is a warning message', level=2)
 logger.create_new_log(message='This is a error message', level=3)
 logger.create_new_log(message='This is a critical error message', level=4)
-logger.create_new_log(message='This is a excepion error message', level=5)
+logger.create_new_log(message='This is a exception error message', level=5)
 ```
 ## License
 [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/)
```

### Comparing `dorsa_logging-1.0.3/dorsa_logging/logging_funcs.py` & `dorsa_logging-1.1.0/dorsa_logging/logging_funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 
 import dorsa_datetime
 
 
 class app_logger():
-    def __init__(self, name='app_logger', log_mainfolderpath='./app_logs', console_log=True):
+    def __init__(self, name='app_logger', log_mainfolderpath='./app_logs', console_log=True, persian=True):
         """This class initializes a logger object that will be used for logging all things happening in the application. The logs are written in a log file, and can be shown
         in the console too. The logs are saved day by day, and on every app start/close.
 
         :param name: Logger object name, defaults to 'app_logger'
         :type name: str, optional
         :param log_mainfolderpath: Main folder path to create logs, defaults to './app_logs'
         :type log_mainfolderpath: str, optional
@@ -17,19 +17,22 @@
         :type console_log: bool, optional
         """
 
         # Create a custom logger
         self.logger_name = name
         self.logger = logging.getLogger(name)
 
+        # set language
+        self.persian = persian
+
         # create log folders and files
         self.console_log = console_log
         self.main_folderpath = log_mainfolderpath
-        self.daily_folderpath = dorsa_datetime.get_date(persian=True, folder_path=True)
-        self.current_filepath = os.path.join(self.main_folderpath, self.daily_folderpath, dorsa_datetime.get_datetime(persian=True, folder_path=True)+'.log')
+        self.daily_folderpath = dorsa_datetime.get_date(persian=self.persian, folder_path=True)
+        self.current_filepath = os.path.join(self.main_folderpath, self.daily_folderpath, dorsa_datetime.get_datetime(persian=self.persian, folder_path=True)+'.log')
         self.__create_mainfolder()
         self.__create_dailyfolder()
 
         # set log levels to write logs
         self.logger_level = logging.DEBUG
         self.console_level = logging.DEBUG
         self.file_level = logging.DEBUG
@@ -85,16 +88,16 @@
             os.mkdir(os.path.join(self.main_folderpath, self.daily_folderpath))
  
 
     def __change_path_on_date_change(self):
         """This function is used to change log file path on date change (end of the day).
         """
 
-        self.daily_folderpath = dorsa_datetime.get_date(persian=True, folder_path=True)
-        self.current_filepath = os.path.join(self.main_folderpath, self.daily_folderpath, dorsa_datetime.get_datetime(persian=True, folder_path=True)+'.log')
+        self.daily_folderpath = dorsa_datetime.get_date(persian=self.persian, folder_path=True)
+        self.current_filepath = os.path.join(self.main_folderpath, self.daily_folderpath, dorsa_datetime.get_datetime(persian=self.persian, folder_path=True)+'.log')
         self.__create_dailyfolder()
 
         # file handler
         self.file_handler = logging.FileHandler(filename=self.current_filepath, mode='w')
         self.file_handler.setLevel(self.file_level)
 
         # file formatter
@@ -124,18 +127,18 @@
                     4: critical error
                     5: excepion error
                     , defaults to 1
         :type level: int, optional
         """
         
         # get date and tme
-        datetime = dorsa_datetime.get_datetime(persian=True, folder_path=False)
+        datetime = dorsa_datetime.get_datetime(persian=self.persian, folder_path=False)
 
         # change log path on date change
-        if self.daily_folderpath != dorsa_datetime.get_date(persian=True, folder_path=True):
+        if self.daily_folderpath != dorsa_datetime.get_date(persian=self.persian, folder_path=True):
             self.__change_path_on_date_change()
 
 
         # do log by levels
         # debug
         if level == 0:
             self.logger.debug(msg='%s - %s : %s\n------------------------------------------------------------------------------' % (datetime, self.current_username, message))
@@ -165,7 +168,8 @@
         """This function sets the input username as the current user.
 
         :param current_username: Current username that logged in the app
         :type current_username: str, optional
         """
         
         self.current_username = current_username if current_username!=None else 'root'
+
```

### Comparing `dorsa_logging-1.0.3/dorsa_logging.egg-info/PKG-INFO` & `dorsa_logging-1.1.0/dorsa_logging.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa-logging
-Version: 1.0.3
+Version: 1.1.0
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
@@ -38,12 +38,12 @@
 
 logger.set_current_user(current_username='DORSA')
 logger.create_new_log(message='This is a debug message', level=0)
 logger.create_new_log(message='This is a info message', level=1)
 logger.create_new_log(message='This is a warning message', level=2)
 logger.create_new_log(message='This is a error message', level=3)
 logger.create_new_log(message='This is a critical error message', level=4)
-logger.create_new_log(message='This is a excepion error message', level=5)
+logger.create_new_log(message='This is a exception error message', level=5)
 ```
 ## License
 [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/)
```

### Comparing `dorsa_logging-1.0.3/setup.py` & `dorsa_logging-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dorsa_logging',                           # should match the package folder
     packages=['dorsa_logging'],                     # should match the package folder
-    version='1.0.3',                                # important for updates
+    version='1.1.0',                                # important for updates
     license='Apache License 2.0',                                  # should match your chosen license
     description='Log application happenings',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Dorsa-co',
     author_email='info@dorsa-co.ir',
     url='https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging',
```


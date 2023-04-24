# Comparing `tmp/quik_config-1.7.0.tar.gz` & `tmp/quik_config-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik_config-1.7.0.tar", last modified: Wed Nov  2 00:31:13 2022, max compression
+gzip compressed data, was "quik_config-1.7.1.tar", last modified: Mon Apr 24 15:40:29 2023, max compression
```

## Comparing `quik_config-1.7.0.tar` & `quik_config-1.7.1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-02 00:31:13.319000 quik_config-1.7.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5776 2022-11-02 00:31:13.318868 quik_config-1.7.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-02 00:31:13.317443 quik_config-1.7.0/quik_config/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       30 2022-11-01 23:59:12.000000 quik_config-1.7.0/quik_config/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    32684 2022-11-02 00:03:07.000000 quik_config-1.7.0/quik_config/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-02 00:31:13.318694 quik_config-1.7.0/quik_config.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5776 2022-11-02 00:31:13.000000 quik_config-1.7.0/quik_config.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      226 2022-11-02 00:31:13.000000 quik_config-1.7.0/quik_config.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-02 00:31:13.000000 quik_config-1.7.0/quik_config.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2022-11-02 00:31:13.000000 quik_config-1.7.0/quik_config.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       12 2022-11-02 00:31:13.000000 quik_config-1.7.0/quik_config.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-02 00:31:13.319038 quik_config-1.7.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1389 2022-11-01 23:59:12.000000 quik_config-1.7.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.298634 quik_config-1.7.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 15:40:29.298454 quik_config-1.7.1/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.297783 quik_config-1.7.1/quik_config/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    33411 2023-04-24 15:37:27.000000 quik_config-1.7.1/quik_config/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.298276 quik_config-1.7.1/quik_config.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 15:40:28.000000 quik_config-1.7.1/quik_config.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      172 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       12 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 15:40:29.298680 quik_config-1.7.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2023-04-20 16:40:30.000000 quik_config-1.7.1/setup.py
```

### Comparing `quik_config-1.7.0/quik_config/main.py` & `quik_config-1.7.1/quik_config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 from collections import namedtuple
 import json
+import re
 
-from super_map import Map, LazyDict
-from walk_up import walk_up_until
-import ez_yaml
-import ruamel.yaml
-import regex as re
+from .__dependencies__.walk_up import walk_up_until
+from .__dependencies__.super_map import Map, LazyDict
+from .__dependencies__ import ez_yaml
 
 def find_and_load(file_name, *, fully_parse_args=False, parse_args=False, args=None, defaults_for_local_data=[], cd_to_filepath=True, show_help_for_no_args=False):
     """
         Example Python:
             # basic call
             config, path_to, *_ = find_and_load("info.yaml", defaults_for_local_data=["DEV"])
             # full call
@@ -166,29 +165,36 @@
                 local_data = { "(selected_profiles)" : selected_profiles }
         selected_profiles = reversed(selected_profiles) # this makes first===highest priority 
         config = available_profiles.get("(default)", {})
     
     # 
     # parse cli arguments
     #
-    if True: 
+    if True:
+        import sys
+        direct_args = args != None
+        looking_for_double_dash = parse_args and not direct_args
+        
+        command_prefix = f'python {sys.argv[0]} '
+        if looking_for_double_dash:
+            command_prefix += "-- "
+        
         if parse_args and args is None:
-            import sys
             args = list(sys.argv)
             args.pop(0) # remove the path of the python file
         
         if args is None:
             args = []
         
         # 
         # remove up to the first "--" argument and only until the next "--" argument
         # 
         unused_args = []
         remaining_args = list(args)
-        if not fully_parse_args:
+        if looking_for_double_dash:
             while len(remaining_args) > 0:
                 if remaining_args[0] == '--':
                     remaining_args.pop(0)
                     break
                 unused_args.append(remaining_args.pop(0))
         resume_unused = False
         second_half_unused = list(remaining_args)
@@ -222,29 +228,25 @@
                 QUIK CONFIG HELP
                 ---------------------------------------------------------------------------------
                 
                 open the file below and look for "(profiles)" for more information:
                     {path}
                 
                 examples:
-                    python3 ./ur_file.py   --  --help --profiles
-                    python3 ./ur_file.py   --  --help key1
-                    python3 ./ur_file.py   --  --help key1:subKey
-                    python3 ./ur_file.py   --  --help key1:subKey key2
-                    python3 ./ur_file.py   --  --profiles='[YOUR_PROFILE, YOUR_OTHER_PROFILE]'
-                    python3 ./ur_file.py   --  thing1:"Im a new value"          part2:"10000"
-                    python3 ./ur_file.py   --  thing1:"I : cause errors"        part2:10000
-                    python3 ./ur_file.py   --  'thing1:"I : dont cause errors"  part2:10000
-                    python3 ./ur_file.py   --  'thing1:["Im in a list"]'
-                    python3 ./ur_file.py   --  'thing1:part_A:"Im nested"'
-                    python3 ./ur_file.py "I get sent to ./ur_file.py" --  part2:"new value"
-                    python3 ./ur_file.py "I get ignored" "me too"  --  part2:10000
+                    {command_prefix} --help --profiles
+                    {command_prefix} --help key1
+                    {command_prefix} --help key1:sub_key
+                    {command_prefix} --help key1:sub_key key2
+                    {command_prefix} thing1:"Im a new value"          part2:"10000"
+                    {command_prefix} thing1:"I : cause errors"        part2:10000
+                    {command_prefix} 'thing1:"I : dont cause errors"  part2:10000
+                    {command_prefix} 'thing1:["Im in a list"]'
+                    {command_prefix} 'thing1:part_a:"Im nested"'
                 
                 how it works:
-                    - the "--" is a required argument, quik config only looks after the --
                     - given "thing1:10", "thing1" is the key, "10" is the value
                     - All values are parsed as json/yaml
                         - "true" is boolean true
                         - "10" is a number
                         - '"10"' is a string (JSON escaping)
                         - '"10\\n"' is a string with a newline
                         - '[10,11,hello]' is a list with two numbers and an unquoted string
@@ -277,24 +279,34 @@
             # 
             # check for user-provided help
             # 
             if len(args_after_help) > 0:
                 if args_after_help[0] == "--profiles":
                     args_after_help.pop(0) # remove the "--profiles" arg
                     
+                    available_profile_names = list(available_profiles.keys())
+                    available_profile_names = [ each for each in available_profile_names if each != '(default)']
                     # if that was the only arg
                     if len(args_after_help) == 0:
-                        print("\navailable profiles:")
-                        for each in available_profiles:
-                            if each != '(default)':
+                        if len(available_profiles) == 0:
+                            print(f"I don't see any available profiles")
+                            print(f"If that is strange, open up {path} and look for (profiles):")
+                            print(f"See https://github.com/jeff-hykin/quik_config_python for a complete explanation")
+                        else:
+                            print("\navailable profiles:")
+                            for each in available_profiles:
                                 print(f"    - {each}")
-                        print("\nas cli argument:")
-                        for each in available_profiles:
-                            if each != '(default)':
-                                print(f"   -- --profiles='{json.dumps([each])}'")
+                            print("\nexample usage:")
+                            if all(each.isidentifier() for each in available_profile_names):
+                                print(command_prefix+f" @{available_profile_names[0]}")
+                                if len(available_profile_names) > 1:
+                                    print(command_prefix+f" @{available_profile_names[0]} @{available_profile_names[1]}")
+                            else:
+                                for each in available_profile_names:
+                                    print(command_prefix + f"--profiles='{json.dumps([each])}'")
                     else:
                         print("")
                         print(f"here are the values for: {args_after_help}")
                         for each_profile_name in args_after_help:
                             print("")
                             print(f"    {each_profile_name}:")
                             if each_profile_name in available_profiles:
```

### Comparing `quik_config-1.7.0/setup.py` & `quik_config-1.7.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,19 +22,14 @@
     description=package_info["description"],
     url=package_info["url"],
     author=package_info["author"],
     author_email=package_info["author_email"],
     license=package_info["license"],
     packages=[package_info["name"]],
     install_requires=[
-        'dict-recursive-update == 1.0.1',
-        'super-map >= 1.1.1',
-        'walk-up >= 0.1.0',
-        'ez-yaml >= 1.2.0',
-        'regex >= 2022.3.2',
         # examples:
         # 'aiohttp >= 3.7.4',
         # 'python-socketio >= 5.3.0',
         # 'requests == 2.26.0',
     ],
     classifiers=[
         # examples:
```


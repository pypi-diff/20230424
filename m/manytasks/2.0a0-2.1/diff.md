# Comparing `tmp/manytasks-2.0a0.tar.gz` & `tmp/manytasks-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manytasks-2.0a0.tar", last modified: Tue Jul 12 12:45:13 2022, max compression
+gzip compressed data, was "manytasks-2.1.tar", last modified: Mon Apr 24 10:18:52 2023, max compression
```

## Comparing `manytasks-2.0a0.tar` & `manytasks-2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-07-12 12:45:13.000000 manytasks-2.0a0/
--rw-r--r--   0 admin      (502) staff       (20)      279 2022-07-12 12:45:13.000000 manytasks-2.0a0/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)     4137 2022-07-12 12:41:21.000000 manytasks-2.0a0/README.md
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks/
--rw-r--r--   0 admin      (502) staff       (20)        0 2021-10-01 08:51:25.000000 manytasks-2.0a0/manytasks/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      550 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/cuda_manager.py
--rw-r--r--   0 admin      (502) staff       (20)     4575 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/defs.py
--rw-r--r--   0 admin      (502) staff       (20)     8267 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/entry.py
--rw-r--r--   0 admin      (502) staff       (20)     3897 2022-05-09 13:45:49.000000 manytasks-2.0a0/manytasks/log_extractor.py
--rw-r--r--   0 admin      (502) staff       (20)     5042 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/task_runner.py
--rw-r--r--   0 admin      (502) staff       (20)     7322 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/taskpool_loader.py
--rw-r--r--   0 admin      (502) staff       (20)     3506 2022-07-12 12:41:21.000000 manytasks-2.0a0/manytasks/util.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)      279 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      434 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)       51 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/entry_points.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2022-07-03 02:41:06.000000 manytasks-2.0a0/manytasks.egg-info/not-zip-safe
--rw-r--r--   0 admin      (502) staff       (20)       39 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/requires.txt
--rw-r--r--   0 admin      (502) staff       (20)       10 2022-07-12 12:45:13.000000 manytasks-2.0a0/manytasks.egg-info/top_level.txt
--rw-r--r--   0 admin      (502) staff       (20)       38 2022-07-12 12:45:13.000000 manytasks-2.0a0/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)      665 2022-07-12 12:41:21.000000 manytasks-2.0a0/setup.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.343328 manytasks-2.1/
+-rw-r--r--   0 admin      (502) staff       (20)     4716 2023-04-24 10:18:52.342670 manytasks-2.1/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)     4406 2023-04-24 10:18:06.000000 manytasks-2.1/README.md
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.333900 manytasks-2.1/manytasks/
+-rw-r--r--   0 admin      (502) staff       (20)        0 2021-10-01 08:51:25.000000 manytasks-2.1/manytasks/__init__.py
+-rw-r--r--   0 admin      (502) staff       (20)      550 2022-07-12 12:41:21.000000 manytasks-2.1/manytasks/cuda_manager.py
+-rw-r--r--   0 admin      (502) staff       (20)     4914 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/defs.py
+-rw-r--r--   0 admin      (502) staff       (20)     8321 2022-12-21 16:04:37.000000 manytasks-2.1/manytasks/entry.py
+-rw-r--r--   0 admin      (502) staff       (20)     3897 2022-05-09 13:45:49.000000 manytasks-2.1/manytasks/log_extractor.py
+-rw-r--r--   0 admin      (502) staff       (20)     5249 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/task_runner.py
+-rw-r--r--   0 admin      (502) staff       (20)     7448 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/taskpool_loader.py
+-rw-r--r--   0 admin      (502) staff       (20)     3668 2023-04-24 10:18:06.000000 manytasks-2.1/manytasks/util.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-04-24 10:18:52.340008 manytasks-2.1/manytasks.egg-info/
+-rw-r--r--   0 admin      (502) staff       (20)     4716 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      434 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (502) staff       (20)       51 2023-04-24 10:18:51.000000 manytasks-2.1/manytasks.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2022-07-03 02:41:06.000000 manytasks-2.1/manytasks.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (502) staff       (20)       39 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/requires.txt
+-rw-r--r--   0 admin      (502) staff       (20)       10 2023-04-24 10:18:52.000000 manytasks-2.1/manytasks.egg-info/top_level.txt
+-rw-r--r--   0 admin      (502) staff       (20)       38 2023-04-24 10:18:52.343678 manytasks-2.1/setup.cfg
+-rw-r--r--   0 admin      (502) staff       (20)      844 2023-04-24 10:18:06.000000 manytasks-2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `manytasks-2.0a0/manytasks/cuda_manager.py` & `manytasks-2.1/manytasks/cuda_manager.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.0a0/manytasks/defs.py` & `manytasks-2.1/manytasks/defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+import re
 from typing import List
 
 
 # Definition
 class Arg:
     def __init__(self, key, value) -> None:
         self.key: str = key
@@ -28,16 +29,27 @@
     @property
     def values(self):
         ret = []
         for arg in self.args:
             ret.append(arg.value)
         return ret
 
+    def smart_key(self, key):
+        if re.match(r"\d+", key):
+            return f"__{key}"
+        if re.match(r"\d+\.\d+", key):
+            return f"__{key}"
+        if f"-{key}" in self.keys:
+            return f"-{key}"
+        if f"--{key}" in self.keys:
+            return f"--{key}"
+        return None
+
     def __contains__(self, key):
-        return key in self.keys
+        return self.smart_key(key) is not None
 
     def __setitem__(self, key, value):
         self.args[self.keys.index(key)].value = value
 
     def __getitem__(self, key):
         return self.args[self.keys.index(key)].value
```

### Comparing `manytasks-2.0a0/manytasks/entry.py` & `manytasks-2.1/manytasks/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,39 +24,39 @@
     #     "\t3. Run `manytasks show -h` to see how to extract the results of tasks"
 
     parser = ArgumentParser()
     subparsers = parser.add_subparsers(dest="mode")
 
     # create a config/rule file
     init_mode = subparsers.add_parser("init")
-    init_mode.add_argument(              dest="template",    action="store", default="",   type=str,   choices=["config", "rule"],
+    init_mode.add_argument(                    dest="template",    action="store", default="",   type=str,   choices=["config", "rule"],
                             help="Generate a template file, `config` for running tasks and `rule` for log extraction.")
 
     # run a config file
     run_mode = subparsers.add_parser("run")
-    run_mode.add_argument(               dest="config_path", action="store", default="",   type=str,   
+    run_mode.add_argument(                     dest="config_path", action="store", default="",   type=str,   
                             help="Specify the config path such as 'config_name.json', " 
                                 + "where the suffix '.json' can be omitted in case that it is in the current directory.")
-    run_mode.add_argument("--log-path",  dest="log_path",    action="store", default="",   type=str,   
+    run_mode.add_argument("--log-path",  "-p", dest="log_path",    action="store", default="",   type=str,   
                             help="Specify the log path. " 
                                 + "The path will be 'config_name.logs' in case that it is not specified.")
-    run_mode.add_argument("--override",  dest="override",    action="store_true",                      
+    run_mode.add_argument("--override",  "-o", dest="override",    action="store_true",                      
                             help="Whether to force override existing logs. ")
-    run_mode.add_argument("--resume",    dest="resume",      action="store_true",                      
+    run_mode.add_argument("--resume",    "-r", dest="resume",      action="store_true",                      
                             help="Whether to resume from existing logs. "
                                 + "Only tasks that are failed will be runned again.")
-    run_mode.add_argument("--random-exe",dest="random_exe",  action="store_true",                      
+    run_mode.add_argument("--random-exe","-e", dest="random_exe",  action="store_true",                      
                             help="Whether tasks are executed randomly. ")
-    run_mode.add_argument("--dry",       dest="dry",         action="store_true",                      
+    run_mode.add_argument("--dry",       "-d", dest="dry",         action="store_true",                      
                             help="Just print all tasks to run instead of running them. ")
-    run_mode.add_argument("--latency",   dest="latency",     action="store", default=1,    type=int,   
+    run_mode.add_argument("--latency",   "-l", dest="latency",     action="store", default=1,    type=int,   
                             help="Time (seconds) between execution of two tasks ." 
                                 + "This can be useful if executing tasks too frequently will cause some errors, \n"
                                 + "such as downloading many files from a server too frequently.")
-    run_mode.add_argument("--timeout",   dest="timeout",     action="store", default=None, type=str,   
+    run_mode.add_argument("--timeout",   "-t", dest="timeout",     action="store", default=None, type=str,   
                             help="Timeout of a task (9S, 5m, 3H, 4d, etc.). "
                                + "This can be useful if a task is not expected to run for too long time. "
                                + "The 'early stop' strategy can help you explore more settings. "
                                + "Note that the upper case (1S, 1M, 1H, 1D) denotes that a timeout is considered as SUCESS, "
                                + "while the lower case (1s, 1m, 1h, 1d) denotes that it is considered as FAILED. ")
 
     # show the result
```

### Comparing `manytasks-2.0a0/manytasks/log_extractor.py` & `manytasks-2.1/manytasks/log_extractor.py`

 * *Files identical despite different names*

### Comparing `manytasks-2.0a0/manytasks/task_runner.py` & `manytasks-2.1/manytasks/task_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,48 @@
 import time
 from collections import defaultdict
 from concurrent.futures.thread import ThreadPoolExecutor
 from pathlib import Path
 
 from manytasks import cuda_manager
 from manytasks.defs import Mode, Status, TaskPool
-from manytasks.util import (current_time, draw_logo, log, log_config,
+from manytasks.util import (current_time, human_readable_time_delta, draw_logo, log, log_config,
                             show_task_list)
 
 
 def run_task(opt, taskpool: TaskPool, task_idx):
     if opt.latency:
         time.sleep(opt.latency)
     task = taskpool[task_idx]
 
     with open("{}/task-{}.txt".format(opt.log_path, task_idx), 'w') as output:
         env = os.environ.copy()
         if opt.cuda == -1:
             cuda_str = "-1"
+            env["CUDA_VISIBLE_DEVICES"] = cuda_str
         elif len(opt.cuda) == 0:
             cuda_str = ""
         else:
             cuda_idxs = cuda_manager.acquire_cuda(opt.cuda_per_task)
             cuda_str = ",".join(list(map(str, cuda_idxs)))
+            env["CUDA_VISIBLE_DEVICES"] = cuda_str
 
-        env["CUDA_VISIBLE_DEVICES"] = cuda_str
         callee = task.executor + task.to_callable_args()
 
         width = int(math.log10(len(taskpool))) + 1
         task_info = "TASK {:>{width}}/{:>{width}}".format(taskpool.index(task),
                                                           len(taskpool),
                                                           width=width)
 
         # process starting...
         p = subprocess.Popen(callee, stdout=output, stderr=output, env=env)
         cuda_status = "| CUDA {}".format(cuda_str) if cuda_str != "" else ""
         pid_status = "| PID {:<8}".format(p.pid)
         status = " START {} {} {}".format(task_info, cuda_status, pid_status)
+        start_time = time.time()
         log("{} [{}] {} : {}".format("👉", current_time(), status,
                                      task.to_finalized_cmd()))
 
         # process ending...
         if opt.timeout is None:
             ret = p.wait()
         else:
@@ -53,17 +55,18 @@
             try:
                 ret = p.wait(timeout=timeout_num)
             except subprocess.TimeoutExpired:
                 if timeout_as_success:
                     ret = 0
                 else:
                     ret = -1926
-        cuda_status = "| CUDA {}".format(cuda_str) if cuda_str != "" else ""
-        ret_status = "| RET {:<8}".format(ret)
-        status = "FINISH {} {} {}".format(task_info, cuda_status, ret_status)
+        # cuda_status = "| CUDA {}".format(cuda_str) if cuda_str != "" else ""
+        ret_status = "| RET {:<2}".format(ret)
+        cost_time = "| COST {}".format(human_readable_time_delta(time.time() - start_time))
+        status = "FINISH {} {} {}".format(task_info, cost_time, ret_status)
         log("{} [{}] {} : {}".format(
             defaultdict(lambda: "❌", {
                 0: "✅",
                 -1926: "🐸"
             })[ret], current_time(), status, task.to_finalized_cmd()))
 
         if cuda_str not in ("-1", ""):
```

### Comparing `manytasks-2.0a0/manytasks/taskpool_loader.py` & `manytasks-2.1/manytasks/taskpool_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def parse_config(cfg_name, config: list) -> List[Tuple[str, List]]:
     """
         Input:  parse_config(None, [
                     "data",
                     "--multigpu",
-                    "--fp16", ["$_ON_", "$_OFF_"],
+                    "--fp16", "$<?>",
                     "--a", [1, 2],
                     "-b", "$<1:4>"
                 ])
         Return: [
                     ("__1", ["data"]),
                     ("--multigpu", ["$_ON_"]),
                     ("--fp16", ["$_ON_", "$_OFF_"]),
@@ -59,15 +59,15 @@
             # convert int/float to str, and pass it to the next `if` statement
             if isinstance(ele, int) or isinstance(ele, float):
                 ele = str(ele)
             # key-value or non-key value?
             if isinstance(ele, list):
                 values = ele
             if isinstance(ele, str):
-                values = parse_string(ele) 
+                values = parse_string(ele)
             if pending_key:
                 ret.append((pending_key, values))
                 pending_key = None
             else:
                 ret.append((next(nonekey), values))
     if pending_key is not None:
         ret.append((pending_key, [Reserved.ON]))
@@ -78,29 +78,35 @@
     """
         Test Case:
 
             print(parse_string("$<1:6:2;2>"))
             print(parse_string("$<1:4>"))
             print(parse_string("$<a|b|c>"))
             print(parse_string("$<a|b|c>.$<1:4>"))
-            print(parse_string("$<[f'{i:03}' for i in range(1, 10, 2)]>"))
-            print(parse_string("$<os.listdir()>"))
+            print(parse_string("$<?>"))
     """
     enum_lists = []
     enum_idx = 0
     # Step 1. analyze the string to find all possible cases to enumerate
     while True:
         found = re.search(r"\$\<[^>]*\>", string)
         if not found:
             break
         
         enum_repr = found.group()
+        enum_start, enum_end = found.start(), found.end()
 
         while "SWITCH":
             # Case I
+            #   $<?>
+            if enum_repr.strip() == "$<?>":
+                enum_list = [Reserved.ON, Reserved.OFF]
+                break
+
+            # Case II
             #   $<start:end:[step]:[zfill]>
             found = re.search(r"^(-?\d+)(:-?\d+)(:-?\d+)?(;\d+)?$", enum_repr[2:-1])
             if found:
                 start = int(found.group(1))
                 end = int(found.group(2)[1:])
                 step = int(found.group(3)[1:]) if found.group(3) else None
                 zero_num = int(found.group(4)[1:]) if found.group(4) else None
@@ -110,47 +116,39 @@
                     r = range(start, end)
                 if zero_num:
                     enum_list = list(str(i).zfill(zero_num) for i in r)
                 else:
                     enum_list = list(str(i) for i in r)
                 break
 
-            # Case II
+            # Case III
             #   $<a|b|c|d>
             found = re.search(r"^([^|]+\|)+[^|]+$", enum_repr[2:-1])
             if found:
                 enum_list = enum_repr[2:-1].split("|")
                 break
 
-            # Case Fallback
-            #   $<python-script>
-            try:
-                enum_list = list(eval(enum_repr[2:-1]))
-            except Exception:
-                print("Error occurs when parsing {}: {}!".format(string, enum_repr))
-                exit(1)
-
             break
 
-        string = string.replace(enum_repr, f'🔢<{enum_idx}>')
+        string = string[:enum_start] + f"#ENUM<{enum_idx}>" + string[enum_end:]
         enum_lists.append(enum_list)
         enum_idx += 1
         
     # Step 2. expand the string to list
     if enum_idx == 0:
         ret = [string]
     else:
         enum_product = list(itertools.product(*enum_lists))
         ret = []
         for i in range(len(enum_product)):
             tmp = string
             for eid in range(enum_idx):
-                tmp = tmp.replace(f'🔢<{eid}>', str(enum_product[i][eid]))
-            ret.append(tmp)   
-        
+                tmp = tmp.replace(f'#ENUM<{eid}>', str(enum_product[i][eid]))
+            ret.append(tmp)
+
     return ret
 
 
 def config_to_tasks(executor, configs):
     ret = []
     # [(k1, [v1, v2]), (k2, [v1])] -> [[(k1, v1), (k1, v2])], [(k2, v1)]]
     expand_configs = []
@@ -164,55 +162,60 @@
     return ret
 
 
 def apply_arg_reference(tasks: List[Task]):
     for task in tasks:
         for arg in task:
             key, val = arg.key, arg.value
+            # print("processing", key, val)
             while True:
                 found = re.search(r"\$\{[^}]+\}", val)
                 if not found:
                     break
                 arg_ref = found.group()
 
                 while "SWITCH":
-                    # Case I: ${--key[start_idx:end_idx]}
+                    # Case I: ${key[start_idx:end_idx]}
                     found = re.search(r"^([^\[]+)\[(\d*):(-?\d*)\]$", arg_ref[2:-1])
                     if found:
                         refered_key = found.group(1)
+                        refered_key = task.smart_key(refered_key)
                         start_idx = int(found.group(2)) if found.group(2) else 0
                         end_idx = int(found.group(3)) if found.group(3) else None
                         new_val = task[refered_key][start_idx:end_idx]
                         break
                     
-                    # Case II: ${--key[pattern1:val1,pattern2:val2,_:default]}
+                    # Case II: ${key[pattern1:val1,pattern2:val2,_:default]}
                     found = re.search(r"^([^\[]+)\[((([^:]+):([^,]+))+)\]$", arg_ref[2:-1])
                     if found:
                         refered_key, pairs = found.group(1), found.group(2)
+                        refered_key = task.smart_key(refered_key)
                         refered_val = task[refered_key]
                         pairs = dict(re.findall(r"([^:]+):([^,]+),?", pairs))
                         if "_" in pairs:
                             pairs = defaultdict(lambda: pairs["_"], pairs)
                         new_val = pairs[refered_val]
                         break
                     
-                    # arg_ref ~ key
-                    new_val = task[arg_ref[2:-1]]
+                    # Case III: ${key}
+                    refered_key = arg_ref[2:-1]
+                    refered_key = task.smart_key(refered_key)
+                    new_val = task[refered_key]
                     break
                 val = val.replace(arg_ref, new_val)
             task[key] = val
 
 
 def load_taskpool(path):
     config = jstyleson.load(fp=open(path))
     executor = config["executor"].split(" ")
     base_conf = parse_config(None, config["configs"]["==base=="])
     more_confs = []
     for mid, more_conf in enumerate(config["configs"]["==more=="]):
-        more_confs.append(parse_config("m{}".format(mid), more_conf))
+        more_confs.append(parse_config(mid, more_conf))
     if len(more_confs) == 0:
         more_confs = [[]]
     tasks = []
     for more_conf in more_confs:
         tasks.extend(config_to_tasks(executor, base_conf + more_conf))
     apply_arg_reference(tasks)
     taskpool = TaskPool()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `manytasks-2.0a0/manytasks/util.py` & `manytasks-2.1/manytasks/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,23 @@
     globals()["__logger__"] = logger
 
 
 def current_time():
     return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
 
 
+def human_readable_time_delta(x):
+    x = int(x)
+    h = x // (60 * 60)
+    x = x % (60 * 60)
+    m = x // 60
+    s = x % 60
+    return f"{h:02}:{m:02}:{s:02}"
+
+
 def draw_logo():
     log("""
     =================================================================
                                       _____              _         
           /\/\    __ _  _ __   _   _ /__   \  __ _  ___ | | __ ___ 
          /    \  / _` || '_ \ | | | |  / /\/ / _` |/ __|| |/ // __| 
         / /\/\ \| (_| || | | || |_| | / /   | (_| |\__ \|   < \__ \ 
@@ -91,15 +100,15 @@
 
 
 def init_config():
     path = read_from_console("Input the config name", "config")
     jstyleson.dump(
         {
             "executor": "python main.py",
-            "cuda": -1,
+            "cuda": [],
             "concurrency": 1,
             "cuda_per_task": 1,
             "configs": {
                 "==base==": [],
                 "==more==": []
             }
         },
```

### Comparing `manytasks-2.0a0/setup.py` & `manytasks-2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="manytasks",
-    version="2.0.alpha",
+    version="2.1",
     keywords=["manytasks", ],
-    description="eds sdk",
-    long_description="A tool for deploying many tasks automatically.",
+    description="A tool for deploying many tasks automatically.",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     license="WTFPL Licence",
 
     url="https://github.com/dugu9sword/manytasks",
     author="dugu9sword",
     author_email="dugu9sword@163.com",
 
     packages=find_packages(),
```


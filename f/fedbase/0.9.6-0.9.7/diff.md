# Comparing `tmp/fedbase-0.9.6.tar.gz` & `tmp/fedbase-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedbase-0.9.6.tar", last modified: Sun Apr 23 01:07:45 2023, max compression
+gzip compressed data, was "fedbase-0.9.7.tar", last modified: Mon Apr 24 01:33:35 2023, max compression
```

## Comparing `fedbase-0.9.6.tar` & `fedbase-0.9.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.807165 fedbase-0.9.6/
--rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.6/LICENSE
--rw-rw-rw-   0        0        0     2297 2023-04-23 01:07:45.806164 fedbase-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.716947 fedbase-0.9.6/fedbase/
--rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.6/fedbase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.792164 fedbase-0.9.6/fedbase/baselines/
--rw-rw-rw-   0        0        0     1191 2023-02-03 00:08:19.000000 fedbase-0.9.6/fedbase/baselines/Central.py
--rw-rw-rw-   0        0        0     2442 2023-04-04 07:24:24.000000 fedbase-0.9.6/fedbase/baselines/Ditto.py
--rw-rw-rw-   0        0        0     2504 2023-04-04 07:25:03.000000 fedbase-0.9.6/fedbase/baselines/Fedavg.py
--rw-rw-rw-   0        0        0     2721 2023-04-04 07:25:55.000000 fedbase-0.9.6/fedbase/baselines/Fedavg_finetune.py
--rw-rw-rw-   0        0        0     2147 2023-02-04 11:27:20.000000 fedbase-0.9.6/fedbase/baselines/Local.py
--rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.6/fedbase/baselines/__init__.py
--rw-rw-rw-   0        0        0     2970 2023-04-04 07:26:42.000000 fedbase-0.9.6/fedbase/baselines/fedavg_ensemble.py
--rw-rw-rw-   0        0        0     2561 2023-04-04 07:25:15.000000 fedbase-0.9.6/fedbase/baselines/fedprox.py
--rw-rw-rw-   0        0        0     3083 2023-04-04 07:23:54.000000 fedbase-0.9.6/fedbase/baselines/fedprox_ensemble.py
--rw-rw-rw-   0        0        0     3142 2023-02-03 00:15:00.000000 fedbase-0.9.6/fedbase/baselines/fesem.py
--rw-rw-rw-   0        0        0     5123 2023-04-04 07:41:10.000000 fedbase-0.9.6/fedbase/baselines/fesem_con.py
--rw-rw-rw-   0        0        0     3774 2023-02-17 00:15:09.000000 fedbase-0.9.6/fedbase/baselines/ifca.py
--rw-rw-rw-   0        0        0     4378 2023-03-06 06:23:47.000000 fedbase-0.9.6/fedbase/baselines/ifca_con.py
--rw-rw-rw-   0        0        0     4701 2023-04-04 05:17:58.000000 fedbase-0.9.6/fedbase/baselines/ifca_res.py
--rw-rw-rw-   0        0        0     4330 2023-02-18 08:23:21.000000 fedbase-0.9.6/fedbase/baselines/wecfl.py
--rw-rw-rw-   0        0        0     4852 2023-04-23 01:04:22.000000 fedbase-0.9.6/fedbase/baselines/wecfl_con.py
--rw-rw-rw-   0        0        0     4413 2023-02-18 08:56:27.000000 fedbase-0.9.6/fedbase/baselines/wecfl_res.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.795165 fedbase-0.9.6/fedbase/model/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.6/fedbase/model/__init__.py
--rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.6/fedbase/model/model.py
--rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.6/fedbase/model/resnet.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.798165 fedbase-0.9.6/fedbase/nodes/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.6/fedbase/nodes/__init__.py
--rw-rw-rw-   0        0        0    14825 2023-04-23 01:06:53.000000 fedbase-0.9.6/fedbase/nodes/node.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.800165 fedbase-0.9.6/fedbase/server/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.6/fedbase/server/__init__.py
--rw-rw-rw-   0        0        0     5838 2023-04-04 05:15:22.000000 fedbase-0.9.6/fedbase/server/server.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.805162 fedbase-0.9.6/fedbase/utils/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.6/fedbase/utils/__init__.py
--rw-rw-rw-   0        0        0    14531 2023-04-23 01:05:04.000000 fedbase-0.9.6/fedbase/utils/data_loader.py
--rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.6/fedbase/utils/femnist.py
--rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.6/fedbase/utils/model_utils.py
--rw-rw-rw-   0        0        0     1694 2023-04-23 01:03:36.000000 fedbase-0.9.6/fedbase/utils/tools.py
--rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.6/fedbase/utils/visualize.py
-drwxrwxrwx   0        0        0        0 2023-04-23 01:07:45.735947 fedbase-0.9.6/fedbase.egg-info/
--rw-rw-rw-   0        0        0     2297 2023-04-23 01:07:45.000000 fedbase-0.9.6/fedbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-04-23 01:07:45.000000 fedbase-0.9.6/fedbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 01:07:45.000000 fedbase-0.9.6/fedbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 01:07:45.000000 fedbase-0.9.6/fedbase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 01:07:45.807165 fedbase-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-04-23 01:07:35.000000 fedbase-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.327235 fedbase-0.9.7/
+-rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0     2297 2023-04-24 01:33:35.326234 fedbase-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.266685 fedbase-0.9.7/fedbase/
+-rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.7/fedbase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.311235 fedbase-0.9.7/fedbase/baselines/
+-rw-rw-rw-   0        0        0     1224 2023-04-24 00:48:42.000000 fedbase-0.9.7/fedbase/baselines/Central.py
+-rw-rw-rw-   0        0        0     2475 2023-04-24 00:49:07.000000 fedbase-0.9.7/fedbase/baselines/Ditto.py
+-rw-rw-rw-   0        0        0     2503 2023-04-24 00:47:54.000000 fedbase-0.9.7/fedbase/baselines/Fedavg.py
+-rw-rw-rw-   0        0        0     2759 2023-04-24 00:48:16.000000 fedbase-0.9.7/fedbase/baselines/Fedavg_finetune.py
+-rw-rw-rw-   0        0        0     2148 2023-04-24 00:42:15.000000 fedbase-0.9.7/fedbase/baselines/Local.py
+-rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.7/fedbase/baselines/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-24 00:50:07.000000 fedbase-0.9.7/fedbase/baselines/fedavg_ensemble.py
+-rw-rw-rw-   0        0        0     2594 2023-04-24 00:45:57.000000 fedbase-0.9.7/fedbase/baselines/fedprox.py
+-rw-rw-rw-   0        0        0     3015 2023-04-24 00:47:24.000000 fedbase-0.9.7/fedbase/baselines/fedprox_ensemble.py
+-rw-rw-rw-   0        0        0     3047 2023-04-24 01:14:00.000000 fedbase-0.9.7/fedbase/baselines/fesem.py
+-rw-rw-rw-   0        0        0     5188 2023-04-24 01:17:55.000000 fedbase-0.9.7/fedbase/baselines/fesem_con.py
+-rw-rw-rw-   0        0        0     3841 2023-04-24 01:28:41.000000 fedbase-0.9.7/fedbase/baselines/ifca.py
+-rw-rw-rw-   0        0        0     4604 2023-04-24 01:18:19.000000 fedbase-0.9.7/fedbase/baselines/ifca_con.py
+-rw-rw-rw-   0        0        0     4606 2023-04-24 00:40:35.000000 fedbase-0.9.7/fedbase/baselines/ifca_res.py
+-rw-rw-rw-   0        0        0     4230 2023-04-24 00:45:04.000000 fedbase-0.9.7/fedbase/baselines/wecfl.py
+-rw-rw-rw-   0        0        0     5166 2023-04-23 01:25:03.000000 fedbase-0.9.7/fedbase/baselines/wecfl_con.py
+-rw-rw-rw-   0        0        0     4313 2023-04-24 00:39:51.000000 fedbase-0.9.7/fedbase/baselines/wecfl_res.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.314237 fedbase-0.9.7/fedbase/model/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/model/__init__.py
+-rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.7/fedbase/model/model.py
+-rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.7/fedbase/model/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.317235 fedbase-0.9.7/fedbase/nodes/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/nodes/__init__.py
+-rw-rw-rw-   0        0        0    14825 2023-04-23 01:06:53.000000 fedbase-0.9.7/fedbase/nodes/node.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.319237 fedbase-0.9.7/fedbase/server/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/server/__init__.py
+-rw-rw-rw-   0        0        0     5838 2023-04-23 01:25:17.000000 fedbase-0.9.7/fedbase/server/server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.325235 fedbase-0.9.7/fedbase/utils/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/utils/__init__.py
+-rw-rw-rw-   0        0        0    14531 2023-04-23 01:05:04.000000 fedbase-0.9.7/fedbase/utils/data_loader.py
+-rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.7/fedbase/utils/femnist.py
+-rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.7/fedbase/utils/model_utils.py
+-rw-rw-rw-   0        0        0     1694 2023-04-23 01:03:36.000000 fedbase-0.9.7/fedbase/utils/tools.py
+-rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.7/fedbase/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.281685 fedbase-0.9.7/fedbase.egg-info/
+-rw-rw-rw-   0        0        0     2297 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:33:35.327235 fedbase-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-04-24 01:33:25.000000 fedbase-0.9.7/setup.py
```

### Comparing `fedbase-0.9.6/LICENSE` & `fedbase-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/PKG-INFO` & `fedbase-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.6
+Version: 0.9.7
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.6/README.md` & `fedbase-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/baselines/Central.py` & `fedbase-0.9.7/fedbase/baselines/Central.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 
 
@@ -23,10 +24,10 @@
 
     print('-------------------start-------------------')
     for i in range(global_rounds):
         nodes0.local_update_epochs(1)
         nodes0.local_test()
 
     # log
-    log(os.path.basename(__file__)[:-3]+ '_' + str(dt.dataset_name), [nodes0], server={})
+    log(os.path.basename(__file__)[:-3]+ add_(dt.dataset_name), [nodes0], server={})
 
     return nodes0.model
```

### Comparing `fedbase-0.9.6/fedbase/baselines/Ditto.py` & `fedbase-0.9.7/fedbase/baselines/Fedavg_finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, finetune_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
 
     server = server_class(device)
     server.assign_model(model())
 
@@ -32,24 +34,32 @@
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
     weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
     server.distribute([nodes[i].model for i in range(num_nodes)])
-    
+
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
-            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
-            nodes[j].local_test()
-        # server aggregation
+            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
+        # server aggregation and distribution
         server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        server.distribute([nodes[i].model for i in range(num_nodes)])
         # test accuracy
+        for j in range(num_nodes):
+            nodes[j].local_test()
         server.acc(nodes, weight_list)
 
+    # fine tune
+    for j in range(num_nodes):
+        nodes[j].local_update_steps(finetune_steps, partial(nodes[j].train_single_step))
+        nodes[j].local_test()
+    server.acc(nodes, weight_list)
+
     # log
-    log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(split_para), nodes, server)
 
     return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.6/fedbase/baselines/Fedavg.py` & `fedbase-0.9.7/fedbase/baselines/Local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu'), log_file = True):
+
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
 
     server = server_class(device)
     server.assign_model(model())
 
@@ -26,33 +28,27 @@
         nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
         # model
         nodes[i].assign_model(model())
         # objective
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
-
+    
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute([nodes[i].model for i in range(num_nodes)])
-    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
-    
+    server.distribute(nodes, list(range(num_nodes)))
+
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
             nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
-        # server aggregation and distribution
-        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
-        server.distribute([nodes[i].model for i in range(num_nodes)])
-        # test accuracy
-        for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, weight_list)
+        # test accuracy
+        server.acc(nodes, list(range(num_nodes)))
 
     # log
-    if log_file:
-        log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(split_para), nodes, server)
 
-    return server.model
+    return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.6/fedbase/baselines/Fedavg_finetune.py` & `fedbase-0.9.7/fedbase/baselines/fedprox_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, finetune_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, n_ensemble, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
+    print('data splited')
 
-    server = server_class(device)
-    server.assign_model(model())
+    models = []
+    for _ in range(n_ensemble):
+        server = server_class(device)
+        server.assign_model(model())
+
+        nodes = [node(i, device) for i in range(num_nodes)]
+        # local_models = [model() for i in range(num_nodes)]
+        # local_loss = [objective() for i in range(num_nodes)]
+
+        for i in range(num_nodes):
+            # data
+            # print(len(train_splited[i]), len(test_splited[i]))
+            nodes[i].assign_train(DataLoader(train_splited[i], batch_size=batch_size, shuffle=True))
+            nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
+            # model
+            nodes[i].assign_model(model())
+            # objective
+            nodes[i].assign_objective(objective())
+            # optim
+            nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
 
-    nodes = [node(i, device) for i in range(num_nodes)]
-    # local_models = [model() for i in range(num_nodes)]
-    # local_loss = [objective() for i in range(num_nodes)]
-
-    for i in range(num_nodes):
-        # data
-        # print(len(train_splited[i]), len(test_splited[i]))
-        nodes[i].assign_train(DataLoader(train_splited[i], batch_size=batch_size, shuffle=True))
-        nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
-        # model
-        nodes[i].assign_model(model())
-        # objective
-        nodes[i].assign_objective(objective())
-        # optim
-        nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
-    
-    del train_splited, test_splited
-
-    # initialize parameters to nodes
-    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
-    server.distribute([nodes[i].model for i in range(num_nodes)])
-
-    # train!
-    for i in range(global_rounds):
-        print('-------------------Global round %d start-------------------' % (i))
-        # single-processing!
-        for j in range(num_nodes):
-            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
-        # server aggregation and distribution
-        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        # initialize parameters to nodes
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
         server.distribute([nodes[i].model for i in range(num_nodes)])
-        # test accuracy
-        for j in range(num_nodes):
-            nodes[j].local_test()
-        server.acc(nodes, weight_list)
 
-    # fine tune
+        # train!
+        for i in range(global_rounds):
+            print('-------------------Global round %d start-------------------' % (i))
+            # single-processing!
+            for j in range(num_nodes):
+                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
+            # server aggregation and distribution
+            server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+            server.distribute([nodes[i].model for i in range(num_nodes)])
+            # test accuracy
+            for j in range(num_nodes):
+                nodes[j].local_test()
+            server.acc(nodes, weight_list)
+        
+        # ensemble
+        models.append(server.model)
+
+    # test ensemble
+    print('test ensemble\n')
     for j in range(num_nodes):
-        nodes[j].local_update_steps(finetune_steps, partial(nodes[j].train_single_step))
-        nodes[j].local_test()
-    server.acc(nodes, weight_list)
+        nodes[j].local_ensemble_test(models, voting = 'soft')
+    server.acc(nodes, list(range(num_nodes)))
 
     # log
-    log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(n_ensemble) + add_(reg) + add_(split_para), nodes, server)
 
-    return [nodes[i].model for i in range(num_nodes)]
+    return models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/Local.py` & `fedbase-0.9.7/fedbase/baselines/Fedavg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
-
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu'), log_file=True):
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
 
     server = server_class(device)
     server.assign_model(model())
 
@@ -27,28 +27,32 @@
         nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
         # model
         nodes[i].assign_model(model())
         # objective
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
-    
+
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
-
+    server.distribute([nodes[i].model for i in range(num_nodes)])
+    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
         # single-processing!
         for j in range(num_nodes):
             nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
-            nodes[j].local_test()
+        # server aggregation and distribution
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        server.distribute([nodes[i].model for i in range(num_nodes)])
         # test accuracy
-        server.acc(nodes, list(range(num_nodes)))
+        for j in range(num_nodes):
+            nodes[j].local_test()
+        server.acc(nodes, weight_list)
 
     # log
-    if log_file:
-        log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(split_para), nodes, server)
 
-    return [nodes[i].model for i in range(num_nodes)]
+    return server.model
```

### Comparing `fedbase-0.9.6/fedbase/baselines/fedavg_ensemble.py` & `fedbase-0.9.7/fedbase/baselines/fedavg_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
@@ -57,13 +58,12 @@
     # test ensemble
     print('test ensemble\n')
     for j in range(num_nodes):
         nodes[j].local_ensemble_test(models, voting = 'soft')
     server.acc(nodes, list(range(num_nodes)))
 
     # log
-    # log(os.path.basename(__file__)[:-3] + '_' + split_para, nodes, server)
-    log(os.path.basename(__file__)[:-3] + '_' + str(n_ensemble) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(n_ensemble) + add_(split_para), nodes, server)
 
     return models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/fedprox.py` & `fedbase-0.9.7/fedbase/baselines/fedprox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 import os
 from functools import partial
 
@@ -48,10 +49,10 @@
         server.distribute([nodes[i].model for i in range(num_nodes)])
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, weight_list)
 
     # log
-    log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(reg) + add_(split_para) , nodes, server)
 
     return server.model
```

### Comparing `fedbase-0.9.6/fedbase/baselines/fedprox_ensemble.py` & `fedbase-0.9.7/fedbase/baselines/fesem.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
+from fedbase.model.model import CNNCifar, CNNMnist
 import os
+import sys
+import inspect
 from functools import partial
 
-def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, n_ensemble, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+def run(dataset_splited, batch_size, K, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg = None, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
-    print('data splited')
-
-    models = []
-    for _ in range(n_ensemble):
-        server = server_class(device)
-        server.assign_model(model())
-
-        nodes = [node(i, device) for i in range(num_nodes)]
-        # local_models = [model() for i in range(num_nodes)]
-        # local_loss = [objective() for i in range(num_nodes)]
-
-        for i in range(num_nodes):
-            # data
-            # print(len(train_splited[i]), len(test_splited[i]))
-            nodes[i].assign_train(DataLoader(train_splited[i], batch_size=batch_size, shuffle=True))
-            nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
-            # model
-            nodes[i].assign_model(model())
-            # objective
-            nodes[i].assign_objective(objective())
-            # optim
-            nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
-
-        # initialize parameters to nodes
-        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
-        server.distribute([nodes[i].model for i in range(num_nodes)])
-
-        # train!
-        for i in range(global_rounds):
-            print('-------------------Global round %d start-------------------' % (i))
-            # single-processing!
-            for j in range(num_nodes):
-                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
-            # server aggregation and distribution
-            server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
-            server.distribute([nodes[i].model for i in range(num_nodes)])
-            # test accuracy
-            for j in range(num_nodes):
-                nodes[j].local_test()
-            server.acc(nodes, weight_list)
-        
-        # ensemble
-        models.append(server.model)
-
-    # test ensemble
-    print('test ensemble\n')
-    for j in range(num_nodes):
-        nodes[j].local_ensemble_test(models, voting = 'soft')
-    server.acc(nodes, list(range(num_nodes)))
+    server = server_class(device)
+    server.assign_model(model())
 
+    nodes = [node(i, device) for i in range(num_nodes)]
+    # local_models = [model() for i in range(num_nodes)]
+    # local_loss = [objective() for i in range(num_nodes)]
+
+    for i in range(num_nodes):
+        # data
+        # print(len(train_splited[i]), len(test_splited[i]))
+        nodes[i].assign_train(DataLoader(train_splited[i], batch_size=batch_size, shuffle=True))
+        nodes[i].assign_test(DataLoader(test_splited[i], batch_size=batch_size, shuffle=False))
+        # model
+        nodes[i].assign_model(model())
+        # objective
+        nodes[i].assign_objective(objective())
+        # optim
+        nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
+    
+    del train_splited, test_splited
+
+    # initialize parameters to nodes
+    server.distribute(nodes, list(range(num_nodes)))
+
+    # initialize K cluster model
+    cluster_models = [model() for i in range(K)]
+
+    # train!
+    for i in range(global_rounds):
+        print('-------------------Global round %d start-------------------' % (i))
+        # local update
+        for j in range(num_nodes):
+            if not reg:
+                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
+            else:
+                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.aggregate(nodes, list(range(num_nodes))), lam= reg))
+        # server clustering
+        server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
+        # server aggregation and distribution by cluster
+        for i in range(K):
+            server.aggregate(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
+            server.distribute(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
+            cluster_models[k].load_state_dict(server.model.state_dict())
+        # test accuracy
+        for j in range(num_nodes):
+            nodes[j].local_test()
+        server.acc(nodes, list(range(num_nodes)))
+    
     # log
-    # log(os.path.basename(__file__)[:-3] + '_' + str(reg) + '_' + split_para , nodes, server)
-    log(os.path.basename(__file__)[:-3] + '_' + str(n_ensemble) + '_' + str(reg) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
-    return models
+    return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/fesem.py` & `fedbase-0.9.7/fedbase/baselines/Ditto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from fedbase.utils.data_loader import data_process, log
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
-from fedbase.model.model import CNNCifar, CNNMnist
 import os
-import sys
-import inspect
 from functools import partial
 
-def run(dataset_splited, batch_size, K, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg = None, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+def run(dataset_splited, batch_size, num_nodes, model, objective, optimizer, global_rounds, local_steps, reg, device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     # dt = data_process(dataset)
     # train_splited, test_splited = dt.split_dataset(num_nodes, split['split_para'], split['split_method'])
     train_splited, test_splited, split_para = dataset_splited
+
     server = server_class(device)
     server.assign_model(model())
 
     nodes = [node(i, device) for i in range(num_nodes)]
     # local_models = [model() for i in range(num_nodes)]
     # local_loss = [objective() for i in range(num_nodes)]
 
@@ -32,40 +31,26 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
-
-    # initialize K cluster model
-    cluster_models = [model() for i in range(K)]
-
+    weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+    server.distribute([nodes[i].model for i in range(num_nodes)])
+    
     # train!
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
-        # local update
-        for j in range(num_nodes):
-            if not reg:
-                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
-            else:
-                nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.aggregate(nodes, list(range(num_nodes))), lam= reg))
-        # server clustering
-        server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
-        # server aggregation and distribution by cluster
-        for i in range(K):
-            server.aggregate(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
-            server.distribute(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
-            cluster_models[k].load_state_dict(server.model.state_dict())
-        # test accuracy
+        # single-processing!
         for j in range(num_nodes):
+            nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.model, lam= reg))
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
-    
+        # server aggregation
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
+        # test accuracy
+        server.acc(nodes, weight_list)
+
     # log
-    if reg:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg) + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(reg) + add_(split_para) , nodes, server)
 
-    return cluster_models
+    return [nodes[i].model for i in range(num_nodes)]
```

### Comparing `fedbase-0.9.6/fedbase/baselines/fesem_con.py` & `fedbase-0.9.7/fedbase/baselines/wecfl_con.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.utils.visualize import dimension_reduction
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
@@ -46,25 +47,27 @@
     # train!
     # b_list = []
     # uu_list = []
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
 
         # local update
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
         for j in range(num_nodes):
             if i == 0:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             elif i < warmup_rounds:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = None\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = base\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
                 
         # # tsne or pca plot
         # # if i == global_rounds-1:
         # if i == i :
         #     cluster_data = torch.nn.utils.parameters_to_vector(nodes[0].model.parameters()).cpu().detach().numpy()[-1000:]
         #     for i in range(1, num_nodes):
         #         cluster_data = np.concatenate((cluster_data, torch.nn.utils.parameters_to_vector(nodes[i].model.parameters()).cpu().detach().numpy()[-1000:]), axis = 0)
@@ -78,30 +81,27 @@
         # b_list.append(max(B_list))
         # uu_list.append(max(u_list))
         # print(b_list, uu_list)
         # for k in range(num_nodes):
         #     nodes[k].grads = []
         
         # server clustering
-        server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
+        server.weighted_clustering(nodes, list(range(num_nodes)), K)
 
         # server aggregation and distribution by cluster
         for j in range(K):
-            id_list = [i for i in list(range(num_nodes)) if nodes[i].label==j]
-            server.modelload_state_dict(server.aggregate([nodes[i] for i in id_list], \
-                [nodes[i].data_size/sum([nodes[i].data_size for i in id_list]) for i in id_list]))
-            server.distribute([nodes[i].model for i in id_list])
+            assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
+            server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls])
             cluster_models[j].load_state_dict(server.model.state_dict())
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
     
     # log
-    if not reg_lam:
-        log(os.path.basename(__file__)[:-3] + '_' + base + '_'+ str(K)  + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + base + '_'+ str(K) + '_' + str(reg_lam) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(base) + add_(tmp) + add_(mu) + add_(reg_lam) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/ifca.py` & `fedbase-0.9.7/fedbase/baselines/ifca.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
 import sys
@@ -66,23 +67,22 @@
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.aggregate(nodes, list(range(num_nodes))), lam= reg))
 
         # server aggregation and distribution by cluster
         for k in range(K):
             if len(assignment[k])>0:
-                server.aggregate(nodes, assignment[k])
-                server.distribute(nodes, assignment[k])
+                weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assignment[k]]) for i in assignment[k]]
+                server.aggregate([nodes[i].model for i in assignment[k]], weight_ls)
+                server.distribute([nodes[i].model for i in assignment[k]])
                 cluster_models[k].load_state_dict(server.model.state_dict())
 
         # test accuracy
         for i in range(num_nodes):
             nodes[i].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
 
     # log
-    if reg:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg) + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
+
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/ifca_con.py` & `fedbase-0.9.7/fedbase/baselines/ifca_con.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
 import sys
@@ -58,38 +59,38 @@
             nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
         # print(server.clustering)
         server.clustering['label'].append(assignment)
         print(assignment)
         print([len(assignment[i]) for i in range(len(assignment))])
 
         # local update
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
         for j in range(num_nodes):
             if i == 0:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             elif i < warmup_rounds:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = None\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = base\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
 
         # server aggregation and distribution by cluster
         for k in range(K):
             if len(assignment[k])>0:
-                server.aggregate(nodes, assignment[k])
-                server.distribute(nodes, assignment[k])
+                weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assignment[k]]) for i in assignment[k]]
+                server.aggregate([nodes[i].model for i in assignment[k]], weight_ls)
+                server.distribute([nodes[i].model for i in assignment[k]])
                 cluster_models[k].load_state_dict(server.model.state_dict())
 
         # test accuracy
         for i in range(num_nodes):
             nodes[i].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
 
     # log
-    if reg_lam:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg_lam) + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg_lam) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/ifca_res.py` & `fedbase-0.9.7/fedbase/baselines/ifca_res.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.nodes.node import node
+from fedbase.utils.tools import add_
 from fedbase.server.server import server_class
 from fedbase.baselines import fedavg
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
@@ -87,13 +88,10 @@
  
         # test accuracy
         for i in range(num_nodes):
             nodes[i].local_test(model_res = server.model)
         server.acc(nodes, weight_list)
 
     # log
-    if reg:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg) + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/wecfl.py` & `fedbase-0.9.7/fedbase/baselines/wecfl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.utils.visualize import dimension_reduction
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
@@ -84,14 +85,11 @@
         
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, list(range(num_nodes)))
     
     # log
-    if not reg:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K)  + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/wecfl_con.py` & `fedbase-0.9.7/fedbase/baselines/fesem_con.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
-from fedbase.utils.visualize import dimension_reduction
 from fedbase.utils.tools import add_
+from fedbase.utils.visualize import dimension_reduction
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
 import os
@@ -35,37 +35,39 @@
         nodes[i].assign_objective(objective())
         # optim
         nodes[i].assign_optim(optimizer(nodes[i].model.parameters()))
     
     del train_splited, test_splited
 
     # initialize parameters to nodes
-    server.distribute(nodes, list(range(num_nodes)))
+    server.distribute([nodes[i].model for i in range(num_nodes)])
 
     # initialize K cluster model
     cluster_models = [model().to(device) for i in range(K)]
 
     # train!
     # b_list = []
     # uu_list = []
     for i in range(global_rounds):
         print('-------------------Global round %d start-------------------' % (i))
 
         # local update
+        weight_list = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.model.load_state_dict(server.aggregate([nodes[i].model for i in range(num_nodes)], weight_list))
         for j in range(num_nodes):
             if i == 0:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             elif i < warmup_rounds:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = None\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_con, \
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = base\
-                        , reg_lam = reg_lam, reg_model = server.aggregate(nodes, list(range(num_nodes)))))
+                        , reg_lam = reg_lam, reg_model = server.model))
                 
         # # tsne or pca plot
         # # if i == global_rounds-1:
         # if i == i :
         #     cluster_data = torch.nn.utils.parameters_to_vector(nodes[0].model.parameters()).cpu().detach().numpy()[-1000:]
         #     for i in range(1, num_nodes):
         #         cluster_data = np.concatenate((cluster_data, torch.nn.utils.parameters_to_vector(nodes[i].model.parameters()).cpu().detach().numpy()[-1000:]), axis = 0)
@@ -79,25 +81,27 @@
         # b_list.append(max(B_list))
         # uu_list.append(max(u_list))
         # print(b_list, uu_list)
         # for k in range(num_nodes):
         #     nodes[k].grads = []
         
         # server clustering
-        server.weighted_clustering(nodes, list(range(num_nodes)), K)
+        server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
 
         # server aggregation and distribution by cluster
         for j in range(K):
-            server.aggregate(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
-            server.distribute(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
+            assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
+            server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls])
             cluster_models[j].load_state_dict(server.model.state_dict())
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
     
     # log
     log(os.path.basename(__file__)[:-3] + add_(K) + add_(base) + add_(tmp) + add_(mu) + add_(reg_lam) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/baselines/wecfl_res.py` & `fedbase-0.9.7/fedbase/baselines/wecfl_res.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fedbase.utils.data_loader import data_process, log
 from fedbase.utils.visualize import dimension_reduction
+from fedbase.utils.tools import add_
 from fedbase.nodes.node import node
 from fedbase.server.server import server_class
 from fedbase.baselines import local
 import torch
 from torch.utils.data import DataLoader
 import torch.optim as optim
 from fedbase.model.model import CNNCifar, CNNMnist
@@ -82,14 +83,11 @@
         
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, list(range(num_nodes)))
     
     # log
-    if not reg:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K)  + '_' + split_para, nodes, server)
-    else:
-        log(os.path.basename(__file__)[:-3] + '_' + str(K) + '_' + str(reg) + '_' + split_para, nodes, server)
+    log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.6/fedbase/model/model.py` & `fedbase-0.9.7/fedbase/model/model.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/model/resnet.py` & `fedbase-0.9.7/fedbase/model/resnet.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/nodes/node.py` & `fedbase-0.9.7/fedbase/nodes/node.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/server/server.py` & `fedbase-0.9.7/fedbase/server/server.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/utils/data_loader.py` & `fedbase-0.9.7/fedbase/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/utils/femnist.py` & `fedbase-0.9.7/fedbase/utils/femnist.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/utils/model_utils.py` & `fedbase-0.9.7/fedbase/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/utils/tools.py` & `fedbase-0.9.7/fedbase/utils/tools.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase/utils/visualize.py` & `fedbase-0.9.7/fedbase/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/fedbase.egg-info/PKG-INFO` & `fedbase-0.9.7/fedbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.6
+Version: 0.9.7
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.6/fedbase.egg-info/SOURCES.txt` & `fedbase-0.9.7/fedbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.6/setup.py` & `fedbase-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fedbase",
-    version="0.9.6",
+    version="0.9.7",
     author="Jie MA",
     # author_email="ustcmj@gmail.com, jie.ma-5@student.uts.edu.au",
     author_email="ustcmj@gmail.com",
     description="An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jie-ma-ai/FedBase",
```


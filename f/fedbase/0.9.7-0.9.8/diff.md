# Comparing `tmp/fedbase-0.9.7.tar.gz` & `tmp/fedbase-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedbase-0.9.7.tar", last modified: Mon Apr 24 01:33:35 2023, max compression
+gzip compressed data, was "fedbase-0.9.8.tar", last modified: Mon Apr 24 01:53:48 2023, max compression
```

## Comparing `fedbase-0.9.7.tar` & `fedbase-0.9.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.327235 fedbase-0.9.7/
--rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.7/LICENSE
--rw-rw-rw-   0        0        0     2297 2023-04-24 01:33:35.326234 fedbase-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.266685 fedbase-0.9.7/fedbase/
--rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.7/fedbase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.311235 fedbase-0.9.7/fedbase/baselines/
--rw-rw-rw-   0        0        0     1224 2023-04-24 00:48:42.000000 fedbase-0.9.7/fedbase/baselines/Central.py
--rw-rw-rw-   0        0        0     2475 2023-04-24 00:49:07.000000 fedbase-0.9.7/fedbase/baselines/Ditto.py
--rw-rw-rw-   0        0        0     2503 2023-04-24 00:47:54.000000 fedbase-0.9.7/fedbase/baselines/Fedavg.py
--rw-rw-rw-   0        0        0     2759 2023-04-24 00:48:16.000000 fedbase-0.9.7/fedbase/baselines/Fedavg_finetune.py
--rw-rw-rw-   0        0        0     2148 2023-04-24 00:42:15.000000 fedbase-0.9.7/fedbase/baselines/Local.py
--rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.7/fedbase/baselines/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-04-24 00:50:07.000000 fedbase-0.9.7/fedbase/baselines/fedavg_ensemble.py
--rw-rw-rw-   0        0        0     2594 2023-04-24 00:45:57.000000 fedbase-0.9.7/fedbase/baselines/fedprox.py
--rw-rw-rw-   0        0        0     3015 2023-04-24 00:47:24.000000 fedbase-0.9.7/fedbase/baselines/fedprox_ensemble.py
--rw-rw-rw-   0        0        0     3047 2023-04-24 01:14:00.000000 fedbase-0.9.7/fedbase/baselines/fesem.py
--rw-rw-rw-   0        0        0     5188 2023-04-24 01:17:55.000000 fedbase-0.9.7/fedbase/baselines/fesem_con.py
--rw-rw-rw-   0        0        0     3841 2023-04-24 01:28:41.000000 fedbase-0.9.7/fedbase/baselines/ifca.py
--rw-rw-rw-   0        0        0     4604 2023-04-24 01:18:19.000000 fedbase-0.9.7/fedbase/baselines/ifca_con.py
--rw-rw-rw-   0        0        0     4606 2023-04-24 00:40:35.000000 fedbase-0.9.7/fedbase/baselines/ifca_res.py
--rw-rw-rw-   0        0        0     4230 2023-04-24 00:45:04.000000 fedbase-0.9.7/fedbase/baselines/wecfl.py
--rw-rw-rw-   0        0        0     5166 2023-04-23 01:25:03.000000 fedbase-0.9.7/fedbase/baselines/wecfl_con.py
--rw-rw-rw-   0        0        0     4313 2023-04-24 00:39:51.000000 fedbase-0.9.7/fedbase/baselines/wecfl_res.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.314237 fedbase-0.9.7/fedbase/model/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/model/__init__.py
--rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.7/fedbase/model/model.py
--rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.7/fedbase/model/resnet.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.317235 fedbase-0.9.7/fedbase/nodes/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/nodes/__init__.py
--rw-rw-rw-   0        0        0    14825 2023-04-23 01:06:53.000000 fedbase-0.9.7/fedbase/nodes/node.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.319237 fedbase-0.9.7/fedbase/server/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/server/__init__.py
--rw-rw-rw-   0        0        0     5838 2023-04-23 01:25:17.000000 fedbase-0.9.7/fedbase/server/server.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.325235 fedbase-0.9.7/fedbase/utils/
--rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.7/fedbase/utils/__init__.py
--rw-rw-rw-   0        0        0    14531 2023-04-23 01:05:04.000000 fedbase-0.9.7/fedbase/utils/data_loader.py
--rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.7/fedbase/utils/femnist.py
--rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.7/fedbase/utils/model_utils.py
--rw-rw-rw-   0        0        0     1694 2023-04-23 01:03:36.000000 fedbase-0.9.7/fedbase/utils/tools.py
--rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.7/fedbase/utils/visualize.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:33:35.281685 fedbase-0.9.7/fedbase.egg-info/
--rw-rw-rw-   0        0        0     2297 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 01:33:35.000000 fedbase-0.9.7/fedbase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 01:33:35.327235 fedbase-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-04-24 01:33:25.000000 fedbase-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.435715 fedbase-0.9.8/
+-rw-rw-rw-   0        0        0     1083 2021-11-25 09:10:20.000000 fedbase-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0     2297 2023-04-24 01:53:48.434716 fedbase-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2022-04-16 12:00:00.000000 fedbase-0.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.375598 fedbase-0.9.8/fedbase/
+-rw-rw-rw-   0        0        0       16 2021-11-25 09:27:32.000000 fedbase-0.9.8/fedbase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.419722 fedbase-0.9.8/fedbase/baselines/
+-rw-rw-rw-   0        0        0     1224 2023-04-24 00:48:42.000000 fedbase-0.9.8/fedbase/baselines/Central.py
+-rw-rw-rw-   0        0        0     2475 2023-04-24 00:49:07.000000 fedbase-0.9.8/fedbase/baselines/Ditto.py
+-rw-rw-rw-   0        0        0     2503 2023-04-24 00:47:54.000000 fedbase-0.9.8/fedbase/baselines/Fedavg.py
+-rw-rw-rw-   0        0        0     2759 2023-04-24 00:48:16.000000 fedbase-0.9.8/fedbase/baselines/Fedavg_finetune.py
+-rw-rw-rw-   0        0        0     2148 2023-04-24 00:42:15.000000 fedbase-0.9.8/fedbase/baselines/Local.py
+-rw-rw-rw-   0        0        0      213 2023-02-07 09:23:33.000000 fedbase-0.9.8/fedbase/baselines/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-24 00:50:07.000000 fedbase-0.9.8/fedbase/baselines/fedavg_ensemble.py
+-rw-rw-rw-   0        0        0     2594 2023-04-24 00:45:57.000000 fedbase-0.9.8/fedbase/baselines/fedprox.py
+-rw-rw-rw-   0        0        0     3015 2023-04-24 00:47:24.000000 fedbase-0.9.8/fedbase/baselines/fedprox_ensemble.py
+-rw-rw-rw-   0        0        0     3188 2023-04-24 01:51:43.000000 fedbase-0.9.8/fedbase/baselines/fesem.py
+-rw-rw-rw-   0        0        0     5189 2023-04-24 01:49:45.000000 fedbase-0.9.8/fedbase/baselines/fesem_con.py
+-rw-rw-rw-   0        0        0     3838 2023-04-24 01:51:26.000000 fedbase-0.9.8/fedbase/baselines/ifca.py
+-rw-rw-rw-   0        0        0     4601 2023-04-24 01:49:06.000000 fedbase-0.9.8/fedbase/baselines/ifca_con.py
+-rw-rw-rw-   0        0        0     4606 2023-04-24 00:40:35.000000 fedbase-0.9.8/fedbase/baselines/ifca_res.py
+-rw-rw-rw-   0        0        0     4359 2023-04-24 01:50:57.000000 fedbase-0.9.8/fedbase/baselines/wecfl.py
+-rw-rw-rw-   0        0        0     5167 2023-04-24 01:50:15.000000 fedbase-0.9.8/fedbase/baselines/wecfl_con.py
+-rw-rw-rw-   0        0        0     4543 2023-04-24 01:43:34.000000 fedbase-0.9.8/fedbase/baselines/wecfl_res.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.423720 fedbase-0.9.8/fedbase/model/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.8/fedbase/model/__init__.py
+-rw-rw-rw-   0        0        0     7655 2023-02-18 03:01:07.000000 fedbase-0.9.8/fedbase/model/model.py
+-rw-rw-rw-   0        0        0     9298 2021-11-25 11:00:44.000000 fedbase-0.9.8/fedbase/model/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.425737 fedbase-0.9.8/fedbase/nodes/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.8/fedbase/nodes/__init__.py
+-rw-rw-rw-   0        0        0    14825 2023-04-23 01:06:53.000000 fedbase-0.9.8/fedbase/nodes/node.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.427715 fedbase-0.9.8/fedbase/server/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.8/fedbase/server/__init__.py
+-rw-rw-rw-   0        0        0     5838 2023-04-23 01:25:17.000000 fedbase-0.9.8/fedbase/server/server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.433713 fedbase-0.9.8/fedbase/utils/
+-rw-rw-rw-   0        0        0        0 2021-11-25 11:37:24.000000 fedbase-0.9.8/fedbase/utils/__init__.py
+-rw-rw-rw-   0        0        0    14531 2023-04-23 01:05:04.000000 fedbase-0.9.8/fedbase/utils/data_loader.py
+-rw-rw-rw-   0        0        0     6168 2021-11-25 11:00:44.000000 fedbase-0.9.8/fedbase/utils/femnist.py
+-rw-rw-rw-   0        0        0      944 2021-12-15 01:18:16.000000 fedbase-0.9.8/fedbase/utils/model_utils.py
+-rw-rw-rw-   0        0        0     1694 2023-04-23 01:03:36.000000 fedbase-0.9.8/fedbase/utils/tools.py
+-rw-rw-rw-   0        0        0     1125 2022-12-08 06:10:12.000000 fedbase-0.9.8/fedbase/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:53:48.390723 fedbase-0.9.8/fedbase.egg-info/
+-rw-rw-rw-   0        0        0     2297 2023-04-24 01:53:48.000000 fedbase-0.9.8/fedbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-04-24 01:53:48.000000 fedbase-0.9.8/fedbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:53:48.000000 fedbase-0.9.8/fedbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 01:53:48.000000 fedbase-0.9.8/fedbase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:53:48.435715 fedbase-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-04-24 01:53:35.000000 fedbase-0.9.8/setup.py
```

### Comparing `fedbase-0.9.7/LICENSE` & `fedbase-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/PKG-INFO` & `fedbase-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.7
+Version: 0.9.8
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.7/README.md` & `fedbase-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/Central.py` & `fedbase-0.9.8/fedbase/baselines/Central.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/Ditto.py` & `fedbase-0.9.8/fedbase/baselines/Ditto.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/Fedavg.py` & `fedbase-0.9.8/fedbase/baselines/Fedavg.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/Fedavg_finetune.py` & `fedbase-0.9.8/fedbase/baselines/Fedavg_finetune.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/Local.py` & `fedbase-0.9.8/fedbase/baselines/Local.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/fedavg_ensemble.py` & `fedbase-0.9.8/fedbase/baselines/fedavg_ensemble.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/fedprox.py` & `fedbase-0.9.8/fedbase/baselines/fedprox.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/fedprox_ensemble.py` & `fedbase-0.9.8/fedbase/baselines/fedprox_ensemble.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/fesem.py` & `fedbase-0.9.8/fedbase/baselines/fesem.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,21 +49,25 @@
         for j in range(num_nodes):
             if not reg:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step))
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.aggregate(nodes, list(range(num_nodes))), lam= reg))
         # server clustering
         server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
+
         # server aggregation and distribution by cluster
-        for i in range(K):
-            server.aggregate(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
-            server.distribute(nodes, [j for j in list(range(num_nodes)) if nodes[j].label==i])
-            cluster_models[k].load_state_dict(server.model.state_dict())
+        for j in range(K):
+            assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
+            model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls], model_k)
+            cluster_models[j].load_state_dict(model_k)
+
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
     
     # log
     log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.7/fedbase/baselines/fesem_con.py` & `fedbase-0.9.8/fedbase/baselines/fesem_con.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,17 @@
         # server clustering
         server.weighted_clustering(nodes, list(range(num_nodes)), K, weight_type= 'equal')
 
         # server aggregation and distribution by cluster
         for j in range(K):
             assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
             weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
-            server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
-            server.distribute([nodes[i].model for i in assign_ls])
-            cluster_models[j].load_state_dict(server.model.state_dict())
+            model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls], model_k)
+            cluster_models[j].load_state_dict(model_k)
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, weight_list)
     
     # log
```

### Comparing `fedbase-0.9.7/fedbase/baselines/ifca.py` & `fedbase-0.9.8/fedbase/baselines/ifca.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,17 +68,17 @@
             else:
                 nodes[j].local_update_steps(local_steps, partial(nodes[j].train_single_step_fedprox, reg_model = server.aggregate(nodes, list(range(num_nodes))), lam= reg))
 
         # server aggregation and distribution by cluster
         for k in range(K):
             if len(assignment[k])>0:
                 weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assignment[k]]) for i in assignment[k]]
-                server.aggregate([nodes[i].model for i in assignment[k]], weight_ls)
-                server.distribute([nodes[i].model for i in assignment[k]])
-                cluster_models[k].load_state_dict(server.model.state_dict())
+                model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+                server.distribute([nodes[i].model for i in assignment[k]], model_k)
+                cluster_models[k].load_state_dict(model_k)
 
         # test accuracy
         for i in range(num_nodes):
             nodes[i].local_test()
         server.acc(nodes, weight_list)
 
     # log
```

### Comparing `fedbase-0.9.7/fedbase/baselines/ifca_con.py` & `fedbase-0.9.8/fedbase/baselines/ifca_con.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
                     model_sim = cluster_models[nodes[j].label], model_all = cluster_models, tmp = tmp, mu = mu, base = base\
                         , reg_lam = reg_lam, reg_model = server.model))
 
         # server aggregation and distribution by cluster
         for k in range(K):
             if len(assignment[k])>0:
                 weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assignment[k]]) for i in assignment[k]]
-                server.aggregate([nodes[i].model for i in assignment[k]], weight_ls)
-                server.distribute([nodes[i].model for i in assignment[k]])
-                cluster_models[k].load_state_dict(server.model.state_dict())
+                model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+                server.distribute([nodes[i].model for i in assignment[k]], model_k)
+                cluster_models[k].load_state_dict(model_k)
 
         # test accuracy
         for i in range(num_nodes):
             nodes[i].local_test()
         server.acc(nodes, weight_list)
 
     # log
```

### Comparing `fedbase-0.9.7/fedbase/baselines/ifca_res.py` & `fedbase-0.9.8/fedbase/baselines/ifca_res.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/baselines/wecfl.py` & `fedbase-0.9.8/fedbase/baselines/wecfl.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,21 +75,23 @@
         # uu_list.append(max(u_list))
         # print(b_list, uu_list)
         # for k in range(num_nodes):
         #     nodes[k].grads = []
         # print(a)
         # server aggregation and distribution by cluster
         for j in range(K):
-            server.aggregate(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
-            server.distribute(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
-            cluster_models[j].load_state_dict(server.model.state_dict())
-        
+            assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
+            model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls], model_k)
+            cluster_models[j].load_state_dict(model_k)
+
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
     
     # log
     log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.7/fedbase/baselines/wecfl_con.py` & `fedbase-0.9.8/fedbase/baselines/wecfl_con.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,17 @@
         # server clustering
         server.weighted_clustering(nodes, list(range(num_nodes)), K)
 
         # server aggregation and distribution by cluster
         for j in range(K):
             assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
             weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls]
-            server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
-            server.distribute([nodes[i].model for i in assign_ls])
-            cluster_models[j].load_state_dict(server.model.state_dict())
+            model_k = server.aggregate([nodes[i].model for i in assign_ls], weight_ls)
+            server.distribute([nodes[i].model for i in assign_ls], model_k)
+            cluster_models[j].load_state_dict(model_k)
 
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
         server.acc(nodes, weight_list)
     
     # log
```

### Comparing `fedbase-0.9.7/fedbase/baselines/wecfl_res.py` & `fedbase-0.9.8/fedbase/baselines/wecfl_res.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,25 +69,26 @@
                 model_opt = nodes[j].model, model_fix = nodes[j].model_g))
 
         # server clustering
         server.weighted_clustering(nodes, list(range(num_nodes)), K)
 
         # server aggregation and distribution by cluster
         for j in range(K):
-            server.aggregate(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
-            server.distribute(nodes, [i for i in list(range(num_nodes)) if nodes[i].label==j])
+            assign_ls = [i for i in list(range(num_nodes)) if nodes[i].label==j]
+            weight_ls = [nodes[i].data_size/sum([nodes[i].data_size for i in assign_ls]) for i in assign_ls] 
+            server.distribute([nodes[i].model for i in assign_ls], server.aggregate([nodes[i].model for i in assign_ls], weight_ls))
             cluster_models[j].load_state_dict(server.model.state_dict())
         
         # aggregate model_g
-        server.aggregate_model_g(nodes, list(range(num_nodes)))
-        server.distribute_model_g(nodes, list(range(num_nodes)))
+        weight_all = [nodes[i].data_size/sum([nodes[i].data_size for i in range(num_nodes)]) for i in range(num_nodes)]
+        server.model.load_state_dict(server.aggregate([nodes[i].model_1 for i in range(num_nodes)], weight_list))
         
         # test accuracy
         for j in range(num_nodes):
             nodes[j].local_test()
-        server.acc(nodes, list(range(num_nodes)))
+        server.acc(nodes, weight_list)
     
     # log
     log(os.path.basename(__file__)[:-3] + add_(K) + add_(reg) + add_(split_para), nodes, server)
 
     return cluster_models
```

### Comparing `fedbase-0.9.7/fedbase/model/model.py` & `fedbase-0.9.8/fedbase/model/model.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/model/resnet.py` & `fedbase-0.9.8/fedbase/model/resnet.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/nodes/node.py` & `fedbase-0.9.8/fedbase/nodes/node.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/server/server.py` & `fedbase-0.9.8/fedbase/server/server.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/utils/data_loader.py` & `fedbase-0.9.8/fedbase/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/utils/femnist.py` & `fedbase-0.9.8/fedbase/utils/femnist.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/utils/model_utils.py` & `fedbase-0.9.8/fedbase/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/utils/tools.py` & `fedbase-0.9.8/fedbase/utils/tools.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase/utils/visualize.py` & `fedbase-0.9.8/fedbase/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/fedbase.egg-info/PKG-INFO` & `fedbase-0.9.8/fedbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedbase
-Version: 0.9.7
+Version: 0.9.8
 Summary: An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.
 Home-page: https://github.com/jie-ma-ai/FedBase
 Author: Jie MA
 Author-email: ustcmj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedbase-0.9.7/fedbase.egg-info/SOURCES.txt` & `fedbase-0.9.8/fedbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedbase-0.9.7/setup.py` & `fedbase-0.9.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fedbase",
-    version="0.9.7",
+    version="0.9.8",
     author="Jie MA",
     # author_email="ustcmj@gmail.com, jie.ma-5@student.uts.edu.au",
     author_email="ustcmj@gmail.com",
     description="An easy, silly, DIY Federated Learning framework with many baselines for individual researchers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jie-ma-ai/FedBase",
```


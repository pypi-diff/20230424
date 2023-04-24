# Comparing `tmp/Slpapy-0.1.17.tar.gz` & `tmp/Slpapy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.17.tar", last modified: Wed Apr 19 06:20:25 2023, max compression
+gzip compressed data, was "Slpapy-0.2.1.tar", last modified: Mon Apr 24 01:56:38 2023, max compression
```

## Comparing `Slpapy-0.1.17.tar` & `Slpapy-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.862725 Slpapy-0.1.17/
--rw-rw-rw-   0        0        0      160 2023-04-19 06:20:25.861724 Slpapy-0.1.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.825710 Slpapy-0.1.17/Slpapy/
--rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.17/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.17/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.859725 Slpapy-0.1.17/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.1.17/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.1.17/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.1.17/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.1.17/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.1.17/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.1.17/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.1.17/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     4998 2023-04-18 10:22:59.000000 Slpapy-0.1.17/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:20:25.834711 Slpapy-0.1.17/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 06:20:25.000000 Slpapy-0.1.17/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 06:20:25.862725 Slpapy-0.1.17/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-19 06:20:03.000000 Slpapy-0.1.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.913779 Slpapy-0.2.1/
+-rw-rw-rw-   0        0        0      159 2023-04-24 01:56:38.912779 Slpapy-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.878780 Slpapy-0.2.1/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.2.1/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.1/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.910779 Slpapy-0.2.1/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.1/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.1/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.1/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.1/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.1/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5223 2023-04-24 01:55:15.000000 Slpapy-0.2.1/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.887780 Slpapy-0.2.1/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:56:38.913779 Slpapy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-04-24 01:55:15.000000 Slpapy-0.2.1/setup.py
```

### Comparing `Slpapy-0.1.17/Slpapy/Data_reconstruction.py` & `Slpapy-0.2.1/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/MZ_ppm_match.py` & `Slpapy-0.2.1/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/beats.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/logging.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.2.1/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.17/Slpapy/processing_analyze.py` & `Slpapy-0.2.1/Slpapy/processing_analyze.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
     # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
     adata.var['mt'] = adata.var_names.str.startswith('MT-')  # 将线粒体基因标记为 mt
     sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
                                log1p=False, inplace=True)
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
                  save='_total_counts.png')
+    adata = adata[adata.obs['total_counts'] != 0, :]
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     # 选择高变异基因
     if onlyhighly==True:
@@ -53,59 +54,62 @@
     #保存mz值
     mz=adata.var
     mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
-def se_analyze(adata):
+def se_analyze(adata, n_neighbors, n_pcs,resolution):
     # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
     #sc.pp.scale(adata, max_value=10)
     # 绘制 PCA 图降维
     sc.tl.pca(adata, svd_solver='arpack')  #
     # Neighborhood graph使用数据矩阵的 PCA 表示来计算细胞的邻域图
-    sc.pp.neighbors(adata, n_neighbors=20, n_pcs=30, )
-    # sc.pp.neighbors(adata, n_neighbors=20, n_pcs=30, )#YONG
+    sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, )
     sc.tl.umap(adata, min_dist=0.01, alpha=5, spread=2)  #
     # Leiden 图聚类
     # 计算
-    sc.tl.leiden(adata, resolution=0.3)
+    sc.tl.leiden(adata, resolution=resolution)
     return adata
 
 
 
 
 
 def Basic_processing_flow(
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
         orgknn: bool = False,
         onlyhighly: bool = False,
+        n_neighbors: int =20,
+        n_pcs: int =30,
+        resolution: int =0.3
+
 ) -> Optional[ad.AnnData]:
     adata = pp_analyze(adata,onlyhighly)
     if use_spacial == True:
         adata = XYadata(adata)
-        adata = se_analyze(adata)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
         sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
         sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_spacial_Wilcoxon.png')
         adata.obs['leidenXY'] = adata.obs['leiden']
         Spatial_map(adata, 'leidenXY')
     else:
-        adata = se_analyze(adata)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
         sc.pl.pca_variance_ratio(adata, log=True, save='_general.png')
         sc.pl.umap(adata, color=['leiden'], save='_general.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
         Spatial_map(adata, 'leiden')
 
     if orgknn == True:
-        adata = se_analyze(adata)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
         estimator = KMeans(n_clusters=adata.obs['leiden'].values.codes.max() + 1)  # 构造聚类器
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
         adata.obs['KNNlableXY'] = label_pred.T
         adata.obs['KNNlableXY'] = adata.obs['KNNlableXY'].astype('category')
         sc.tl.rank_genes_groups(adata, 'KNNlableXY', method='wilcoxon')
```

### Comparing `Slpapy-0.1.17/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.2.1/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


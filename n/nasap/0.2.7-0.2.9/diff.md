# Comparing `tmp/nasap-0.2.7.tar.gz` & `tmp/nasap-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nasap-0.2.7.tar", last modified: Wed Feb  1 15:40:55 2023, max compression
+gzip compressed data, was "dist/nasap-0.2.9.tar", last modified: Fri Feb 17 01:51:21 2023, max compression
```

## Comparing `nasap-0.2.7.tar` & `nasap-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap/
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      955 2022-05-25 17:58:29.000000 nasap-0.2.7/nasap/batch_nasap.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    30046 2023-01-31 17:16:32.000000 nasap-0.2.7/nasap/nasap.py
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap/scripts/
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    12850 2023-01-23 13:45:20.000000 nasap-0.2.7/nasap/scripts/extract_preprocess.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    14757 2023-01-24 03:06:05.000000 nasap-0.2.7/nasap/scripts/feature_attrs.py
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap/scripts/gencore/
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000) 10145424 2021-12-31 01:49:26.000000 nasap-0.2.7/nasap/scripts/gencore/gencore
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5250 2022-09-01 16:03:12.000000 nasap-0.2.7/nasap/scripts/genome_track_visualization.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     1325 2022-08-02 08:00:48.000000 nasap-0.2.7/nasap/scripts/map1.bash
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5708 2023-01-26 07:29:58.000000 nasap-0.2.7/nasap/scripts/map2.bash
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     3226 2023-01-26 07:27:51.000000 nasap-0.2.7/nasap/scripts/map_split.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    11662 2023-02-01 04:04:13.000000 nasap-0.2.7/nasap/scripts/network_analysis.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     3462 2022-07-08 04:56:12.000000 nasap-0.2.7/nasap/scripts/parse_gtf.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5540 2022-07-08 04:56:48.000000 nasap-0.2.7/nasap/scripts/pausing_sites.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5797 2022-10-26 06:10:26.000000 nasap-0.2.7/nasap/scripts/pausing_sites_low_memory.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    13572 2023-01-23 14:57:01.000000 nasap-0.2.7/nasap/scripts/plot.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    18382 2023-01-23 13:31:37.000000 nasap-0.2.7/nasap/scripts/preprocess.bash
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     4811 2022-12-08 13:31:52.000000 nasap-0.2.7/nasap/scripts/preprocess_fast.bash
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     6517 2022-10-11 10:10:47.000000 nasap-0.2.7/nasap/scripts/py_ext.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     9700 2022-10-26 09:48:41.000000 nasap-0.2.7/nasap/scripts/render_template.py
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap/scripts/templates/
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap/scripts/templates/static/
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    76316 2022-07-03 02:22:51.000000 nasap-0.2.7/nasap/scripts/templates/static/vue.min.js
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    21034 2023-01-22 15:40:58.000000 nasap-0.2.7/nasap/scripts/templates/template.html
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      791 2022-07-02 15:43:24.000000 nasap-0.2.7/nasap/scripts/templates/template_track.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    18276 2022-10-08 06:08:49.000000 nasap-0.2.7/nasap/scripts/tmp_plot.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      903 2022-08-28 17:42:26.000000 nasap-0.2.7/nasap/scripts/x.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      295 2022-10-06 02:47:17.000000 nasap-0.2.7/nasap/__init__.py
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)       15 2023-02-01 15:38:59.000000 nasap-0.2.7/nasap/__version__.py
-drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap.egg-info/
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        1 2023-02-01 15:40:54.000000 nasap-0.2.7/nasap.egg-info/dependency_links.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)       81 2023-02-01 15:40:54.000000 nasap-0.2.7/nasap.egg-info/entry_points.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      409 2023-02-01 15:40:54.000000 nasap-0.2.7/nasap.egg-info/PKG-INFO
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      121 2023-02-01 15:40:54.000000 nasap-0.2.7/nasap.egg-info/requires.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      931 2023-02-01 15:40:55.000000 nasap-0.2.7/nasap.egg-info/SOURCES.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        6 2023-02-01 15:40:54.000000 nasap-0.2.7/nasap.egg-info/top_level.txt
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      409 2023-02-01 15:40:55.000000 nasap-0.2.7/PKG-INFO
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      107 2023-02-01 15:40:55.000000 nasap-0.2.7/setup.cfg
--rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     2566 2023-01-31 15:42:02.000000 nasap-0.2.7/setup.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:22.000000 nasap-0.2.9/
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      955 2022-05-25 17:58:29.000000 nasap-0.2.9/nasap/batch_nasap.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    35646 2023-02-05 08:23:40.000000 nasap-0.2.9/nasap/nasap.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap/scripts/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    12850 2023-01-23 13:45:20.000000 nasap-0.2.9/nasap/scripts/extract_preprocess.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    17178 2023-02-15 09:45:04.000000 nasap-0.2.9/nasap/scripts/feature_attrs.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap/scripts/gencore/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000) 10145424 2021-12-31 01:49:26.000000 nasap-0.2.9/nasap/scripts/gencore/gencore
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5250 2022-09-01 16:03:12.000000 nasap-0.2.9/nasap/scripts/genome_track_visualization.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     1325 2022-08-02 08:00:48.000000 nasap-0.2.9/nasap/scripts/map1.bash
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5708 2023-01-26 07:29:58.000000 nasap-0.2.9/nasap/scripts/map2.bash
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     3226 2023-01-26 07:27:51.000000 nasap-0.2.9/nasap/scripts/map_split.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    12632 2023-02-05 14:31:49.000000 nasap-0.2.9/nasap/scripts/network_analysis.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     3462 2022-07-08 04:56:12.000000 nasap-0.2.9/nasap/scripts/parse_gtf.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5540 2022-07-08 04:56:48.000000 nasap-0.2.9/nasap/scripts/pausing_sites.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     5797 2022-10-26 06:10:26.000000 nasap-0.2.9/nasap/scripts/pausing_sites_low_memory.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    13572 2023-01-23 14:57:01.000000 nasap-0.2.9/nasap/scripts/plot.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    18382 2023-01-23 13:31:37.000000 nasap-0.2.9/nasap/scripts/preprocess.bash
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     4811 2022-12-08 13:31:52.000000 nasap-0.2.9/nasap/scripts/preprocess_fast.bash
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     6517 2022-10-11 10:10:47.000000 nasap-0.2.9/nasap/scripts/py_ext.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     9890 2023-02-14 09:06:56.000000 nasap-0.2.9/nasap/scripts/render_template.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:22.000000 nasap-0.2.9/nasap/scripts/templates/
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:22.000000 nasap-0.2.9/nasap/scripts/templates/static/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    76316 2022-07-03 02:22:51.000000 nasap-0.2.9/nasap/scripts/templates/static/vue.min.js
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    21357 2023-02-14 09:07:21.000000 nasap-0.2.9/nasap/scripts/templates/template.html
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      791 2022-07-02 15:43:24.000000 nasap-0.2.9/nasap/scripts/templates/template_track.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)    18276 2022-10-08 06:08:49.000000 nasap-0.2.9/nasap/scripts/tmp_plot.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:22.000000 nasap-0.2.9/nasap/scripts/ucsc/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)  9502408 2023-01-17 23:12:18.000000 nasap-0.2.9/nasap/scripts/ucsc/bedGraphToBigWig
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      903 2022-08-28 17:42:26.000000 nasap-0.2.9/nasap/scripts/x.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      295 2022-10-06 02:47:17.000000 nasap-0.2.9/nasap/__init__.py
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)       15 2023-02-17 01:35:47.000000 nasap-0.2.9/nasap/__version__.py
+drwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        0 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        1 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)       81 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/entry_points.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      409 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/PKG-INFO
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      121 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/requires.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      967 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)        6 2023-02-17 01:51:21.000000 nasap-0.2.9/nasap.egg-info/top_level.txt
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      409 2023-02-17 01:51:22.000000 nasap-0.2.9/PKG-INFO
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)      107 2023-02-17 01:51:22.000000 nasap-0.2.9/setup.cfg
+-rwxrwxrwx   0 biodancer  (1000) biodancer  (1000)     2655 2023-02-04 02:27:44.000000 nasap-0.2.9/setup.py
```

### Comparing `nasap-0.2.7/nasap/batch_nasap.py` & `nasap-0.2.9/nasap/batch_nasap.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/nasap.py` & `nasap-0.2.9/nasap/nasap.py`

 * *Files 12% similar despite different names*

```diff
@@ -107,15 +107,15 @@
   for sub_dir in output_subdir:
     if not output_root.endswith('/'): output_root = output_root + '/'
     sub_dir = output_root + sub_dir
     if not os.listdir(sub_dir):
       os.removedirs(sub_dir)
 
 
-def server(output_root='./test_output/', forward_bw=None, reverse_bw=None, gtf=None,  cores=1, tf_source=None, tf_filter_nodes=None, enhancer_source=None, enhancer_filter_nodes=None):
+def server(output_root='./test_output/', forward_bw=None, reverse_bw=None, gtf=None,  cores=1, tf_source=None, enhancer_source=None, select_nodes_file=None, express_file=None):
   global global_root
   global_root = output_root
   # logger.info('server--construct output dir')
   if not output_root.endswith('/'): output_root = output_root + '/'
   _create_project_dir(output_root)
   logger.info('server--check installed software')
   _check_soft( ['pandas', 'pyBigWig', 'numpy', 'scipy', 'networkx','community', 'hvplot'], isPython=True)
@@ -154,23 +154,24 @@
   if not (tf_source or enhancer_source):
     logger.error( 'Error, you have to provide at least one parameter for tf_source or enhancer_source')
     os.sys.exit(1)
 
   if tf_source:
     _check_para('--tf_source', tf_source, str, isFile=True, required=True, output_root=output_root)
     network_cmd_list.extend( ['--tf_source', tf_source])
-  if tf_filter_nodes:
-    _check_para('--tf_filter_nodes', tf_filter_nodes, str, isFile=True, required=True, output_root=output_root)
-    network_cmd_list.extend( ['--tf_filter_nodes', tf_filter_nodes])
+
   if enhancer_source:
     _check_para('--enhancer_source', enhancer_source, str, isFile=True, required=True, output_root=output_root)
     network_cmd_list.extend( ['--enhancer_source', enhancer_source])
-  if enhancer_filter_nodes:
-    _check_para('--enhancer_filter_nodes', enhancer_filter_nodes, str, isFile=True, required=True, output_root=output_root)
-    network_cmd_list.extend( ['--enhancer_filter_nodes', enhancer_filter_nodes])
+  if select_nodes_file:
+    _check_para('--select_nodes_file', select_nodes_file, str, isFile=True, required=True, output_root=output_root)
+    network_cmd_list.extend( ['--select_nodes_file', select_nodes_file])
+  if express_file:
+    _check_para('--express_file', express_file, str, isFile=True, required=True, output_root=output_root)
+    network_cmd_list.extend( ['--express_file', express_file])
 
   all_steps = [feature_assign_cmd_list, pausing_sites_cmd_list, network_cmd_list, render_cmd_list]
   steps_name = ['feature_assign', 'pausing_sites', 'network_analysis', 'render_output']
   for cmd_list, step in zip(all_steps, steps_name):
     try:
       logger.info(step + ' start')
       os.system( ' '.join(cmd_list) )
@@ -214,29 +215,29 @@
     except Exception as e:
       _write_err('gencore remove umi--Failed\n' + str(e) )
 
   if scale_factor:
     try:
       scale_factor = float(scale_factor)
     except Exception as e:
-      _write_err('--scale_factor parsed--Failed\n' + str(e) )
+      _write_err('--scale_factor parsed--Failed, scale-factor must be int or float number\n' + str(e) )
 
-  _tracks(output_root=output_root, bam=output_root + 'sam/uniquemapped_sort.bam', scale_factor=scale_factor)
+  _tracks(output_root=output_root, bam=output_root + 'sam/uniquemapped_sort.bam', cores=cores, scale_factor=scale_factor)
   _render_template(output_root=output_root, type='assessment', is_server='No')
 
-def all(output_root='./test_output/', read1=None, bowtie_index=None,  gtf=None,  cores=1, read2=None, adapter1=None, adapter2=None, umi_loc=None, umi_len=None, tf_source=None, tf_filter_nodes=None, enhancer_source=None, enhancer_filter_nodes=None):
+def all(output_root='./test_output/', read1=None, bowtie_index=None,  gtf=None,  cores=1, read2=None, adapter1=None, adapter2=None, umi_loc=None, umi_len=None, tf_source=None, select_nodes_file=None, enhancer_source=None, express_file=None):
   global global_root
   global_root = output_root
   logger.info('all--check installed software')
   if not output_root.endswith('/'): output_root = output_root + '/'
   _create_project_dir(output_root)
   _check_soft( ['fastp', 'bioawk', 'python', 'bowtie2', 'samtools', 'bedtools', 'deeptools'], isPython=False)
   _check_soft( ['pandas', 'pyBigWig', 'numpy', 'scipy', 'networkx','community', 'hvplot'], isPython=True)
   assessment(output_root=output_root, read1=read1,  cores=cores, read2=read2, adapter1=adapter1, adapter2=adapter2, umi_loc=umi_loc, umi_len=umi_len, bowtie_index=bowtie_index, gtf=gtf)
-  server(output_root=output_root, forward_bw=output_root + 'bw/forward.bw', reverse_bw=output_root + 'bw/reverse.bw', gtf=gtf, cores=cores, tf_source=tf_source, tf_filter_nodes=tf_filter_nodes, enhancer_source=enhancer_source, enhancer_filter_nodes=enhancer_filter_nodes )
+  server(output_root=output_root, forward_bw=output_root + 'bw/forward.bw', reverse_bw=output_root + 'bw/reverse.bw', gtf=gtf, cores=cores, tf_source=tf_source, select_nodes_file=select_nodes_file, enhancer_source=enhancer_source, express_file=express_file )
   _render_template(output_root=output_root, type='all', is_server='No')
 
 
 def _pp(output_root=os.getcwd()+'/tmp_output', read1=None,  cores=1, read2=None, adapter1=None, adapter2=None, umi_loc=None, umi_len=None, genome=None, scaleFactor=None):
   logger.info('preprocess--check installed software')
   _check_soft( ['fastp', 'bioawk', 'python'], isPython=False)
   if read2:
@@ -425,63 +426,171 @@
     os.system( ' '.join(cmd_list) )
   except Exception as e:
     _write_err('map_comutation--Failed\n' + str(e) )
 
   log_file.close()
   logger.success(_cur_time()+ 'alignment--Finished. Find the results in ' + output_root)
 
-def _tracks(bam=None, output_root=None, scale_factor=None):
+def _bamCov(bam=None, output_root=None, scale_factor=None, cores=None, five_end=None):
   logger.info('genome_tracks--check installed software')
   _check_soft( ['deeptools'], isPython=False)
 
   logger.info('genome_tracks--check parameter and input files')
   if not output_root.endswith('/'): output_root = output_root + '/'
   logger.info('genome_tracks--construct output dir')
   _create_project_dir(output_root)
   log_file = open(output_root + 'tmp.log', 'a+' )
 
   cmd_list = ['bamCoverage', '--binSize', '1']
   _check_para('--bam', bam, str, isFile=True, required=True, output_root=output_root)
   cmd_list.extend(['--bam', bam])
   log_file.write('bam--'+os.path.basename(bam) + '\n' )
-  log_file.write('bam_size--' + str(os.stat(bam).st_size / (1024 * 1024)) + 'Mb\n')
-  # 这里运行时间太长 cores直接写死 40，40是线程
-  # if cores:
-  #   cur_cores = _get_cores(cores)
-  #   cmd_list.extend(['-p', str(cur_cores)])
-  cmd_list.extend(['-p', str(40)])
+  bam_size = os.stat(bam).st_size / (1024 * 1024)
+  log_file.write('bam_size--' + str(bam_size) + 'Mb\n')
+  if cores:
+    cur_cores = _get_cores(cores)
+    cmd_list.extend(['-p', str(cur_cores)])
+  else:
+    # 这里运行时间太长 一开始cores直接写死 40，40是线程 后来发现小文件不合适
+    if bam_size < 100:
+      cmd_list.extend(['-p', str(4)])
+    elif bam_size < 500:
+      cmd_list.extend(['-p', str(8)])
+    elif bam_size < 1000:
+      cmd_list.extend(['-p', str(16)])
+    else:
+      cmd_list.extend(['-p', str(32)])
+
   if scale_factor:
     cmd_list.extend(['--scaleFactor', str(scale_factor)])
+
   cmd_list_forward, cmd_list_reverse = cmd_list.copy(), cmd_list.copy()
   cmd_list_forward.extend(['--filterRNAstrand', 'forward'])
   cmd_list_reverse.extend(['--filterRNAstrand', 'reverse'])
   cmd_list_forward.extend(['-o', output_root + 'bw/forward.bw'])
   cmd_list_reverse.extend(['-o', output_root + 'bw/reverse.bw'])
   log_file.write(_cur_time()+ ': generate forward genome track start\n')
   try:
     subprocess.run(' '.join(cmd_list_forward),  shell=True,  check=True)
-    cmd_list_forward[-1] = output_root + 'bw/forward_5_end.bw'
-    cmd_list_forward.extend(['--Offset', '1'])
-    subprocess.run(' '.join(cmd_list_forward),  shell=True,  check=True)
+    if five_end:
+      cmd_list_forward[-1] = output_root + 'bw/forward_5_end.bw'
+      cmd_list_forward.extend(['--Offset', '1'])
+      subprocess.run(' '.join(cmd_list_forward),  shell=True,  check=True)
   except Exception as e:
     _write_err('forward bamCoverage--Failed\n' + str(e) )
 
   log_file.write(_cur_time()+ ': generate reverse genome track start\n')
   try:
     subprocess.run(' '.join(cmd_list_reverse),  shell=True,  check=True)
-    cmd_list_reverse[-1] = output_root + 'bw/reverse_5_end.bw'
-    cmd_list_reverse.extend(['--Offset', '1'])
+    if five_end:
+      cmd_list_reverse[-1] = output_root + 'bw/reverse_5_end.bw'
+      cmd_list_reverse.extend(['--Offset', '1'])
+      subprocess.run(' '.join(cmd_list_reverse),  shell=True,  check=True)
+  except Exception as e:
+    _write_err('reverse bamCoverage--Failed\n' + str(e) )
+
+  log_file.close()
+  logger.success(_cur_time()+'genome_tracks--Finished. Find the results in ' + output_root)
+
+
+def _genomeCov(bam=None, output_root=None, scale_factor=None, cores=None, five_end=None):
+  # BAM -> BedGraph -> BigWig
+  # 1 software test
+  logger.info('genome_tracks--check installed software')
+  _check_soft(['bedtools'], isPython=False)
+  _check_soft(['samtools'], isPython=False)
+  try:
+    if os.system(self_src + 'ucsc/bedGraphToBigWig') != 0:
+      bg2bw_dir = self_src + 'ucsc/bedGraphToBigWig'
+    else:
+      if os.system('bedGraphToBigWig') != 0:
+        bg2bw_dir = 'bedGraphToBigWig'
+      else:
+        _write_err( 'import %s error.\nyou need to install %s first'%('bedGraphToBigWig', 'bedGraphToBigWig') )
+  except:
+    if os.system('bedGraphToBigWig') != 0:
+      bg2bw_dir = 'bedGraphToBigWig'
+    else:
+      _write_err( 'import %s error.\nyou need to install %s first'%('bedGraphToBigWig', 'bedGraphToBigWig') )
+
+  # 2 bedtools genomecov -ibam filename.bam -bg > filename.bedgraph
+  logger.info('genome_tracks--check parameter and input files')
+  if not output_root.endswith('/'): output_root = output_root + '/'
+  logger.info('genome_tracks--construct output dir')
+  _create_project_dir(output_root)
+  log_file = open(output_root + 'tmp.log', 'a+' )
+
+  cmd_list = ['bedtools', 'genomecov', '-bg']
+  _check_para('--bam', bam, str, isFile=True, required=True, output_root=output_root)
+  cmd_list.extend(['-ibam', bam])
+  log_file.write('bam--'+os.path.basename(bam) + '\n' )
+  bam_size = os.stat(bam).st_size / (1024 * 1024)
+  log_file.write('bam_size--' + str(bam_size) + 'Mb\n')
+  def generate_chr_size(bam):
+    os.system('samtools idxstats %s > %stmp_chr_size.txt'%(bam, output_root) )
+    with open( output_root + 'chr_size.txt', 'w') as f:
+      for ln in open(output_root + 'tmp_chr_size.txt'):
+        if '*' in ln: continue
+        seq_id, seq_len, _, _ = ln.split('\t')
+        f.write(seq_id + '\t' + seq_len + '\n')
+  generate_chr_size(bam)
+  if scale_factor:
+    cmd_list.extend(['-scale', str(scale_factor)])
+
+  cmd_list_forward, cmd_list_reverse = cmd_list.copy(), cmd_list.copy()
+  cmd_list_forward.extend(['-strand', '+'])
+  cmd_list_reverse.extend(['-strand', '-'])
+  forward_bg_file = output_root + 'tmp_forward.bedgraph'
+  reverse_bg_file = output_root + 'tmp_reverse.bedgraph'
+  cmd_list_forward.extend(['| sort -k1,1 -k2,2n', '>', forward_bg_file])
+  cmd_list_reverse.extend(['| sort -k1,1 -k2,2n', '>', reverse_bg_file])
+  log_file.write(_cur_time()+ ': generate forward genome track start\n')
+  # 3 bedGraphToBigWig filename.bedgraph $dm6 filename.bw
+  def bg2bw(bg_file, bw_file):
+    bg2bw_cmd_list =[bg2bw_dir, bg_file, output_root + 'chr_size.txt', output_root + 'bw/' + bw_file]
+    subprocess.run(' '.join(bg2bw_cmd_list),  shell=True,  check=True)
+
+  try:
+    subprocess.run(' '.join(cmd_list_forward),  shell=True,  check=True)
+    bg2bw(forward_bg_file, 'forward.bw')
+    if five_end:
+      forward_bg_file = output_root + 'tmp_forward_5_end.bedgraph'
+      cmd_list_forward[-1] = output_root + forward_bg_file
+      cmd_list_forward.extend(['-5'])
+      subprocess.run(' '.join(cmd_list_forward),  shell=True,  check=True)
+      bg2bw(forward_bg_file, 'forward_5_end.bw')
+  except Exception as e:
+    _write_err('forward bamCoverage--Failed\n' + str(e) )
+
+  log_file.write(_cur_time()+ ': generate reverse genome track start\n')
+  try:
     subprocess.run(' '.join(cmd_list_reverse),  shell=True,  check=True)
+    bg2bw(reverse_bg_file, 'reverse.bw')
+    if five_end:
+      reverse_bg_file = output_root + 'tmp_reverse_5_end.bedgraph'
+      cmd_list_reverse[-1] = output_root + reverse_bg_file
+      cmd_list_reverse.extend(['-5'])
+      subprocess.run(' '.join(cmd_list_reverse),  shell=True,  check=True)
+      bg2bw(reverse_bg_file, 'reverse_5_end.bw')
   except Exception as e:
     _write_err('reverse bamCoverage--Failed\n' + str(e) )
 
   log_file.close()
   logger.success(_cur_time()+'genome_tracks--Finished. Find the results in ' + output_root)
 
-def feature_assign(forward_bw=None, reverse_bw=None, gtf=None, output_root=None):
+
+def _tracks(bam=None, output_root=None, cores=None, scale_factor=None, five_end=None):
+  bam_size = float(os.path.getsize(bam)/1000000)
+  if bam_size < 50:
+    _genomeCov(bam=bam, output_root=output_root, scale_factor=scale_factor,  five_end=five_end)
+  else:
+    _bamCov(bam=bam, output_root=output_root, scale_factor=scale_factor, cores=cores,  five_end=five_end)
+
+
+def feature_assign(forward_bw=None, reverse_bw=None, gtf=None, output_root=None, tss_up=150, tss_down=150, gene_length=2000, rpkm_threshold=0.1):
   global global_root
   global_root = output_root
   if not output_root.endswith('/'): output_root = output_root + '/'
   # logger.info('feature_assign--construct output dir')
   _create_project_dir(output_root)
   logger.info('feature_assign--check installed software')
   _check_soft( ['pandas', 'pyBigWig', 'scipy'], isPython=True)
@@ -503,14 +612,37 @@
 
   _check_para('--gtf', gtf, str, isFile=True, required=True, output_root=output_root)
   cmd_list.extend(['--gtf', gtf])
 
   cmd_list.extend(['--output_root', output_root])
   log_file.write(_cur_time()+ 'feature assign start\n')
 
+
+  try:
+    tss_up = int(tss_up)
+    cmd_list.extend(['--tss_up', str(tss_up)])
+  except Exception as e:
+    _write_err('--tss_up parsed--Failed, tss_up must be int number\n' + str(e) )
+  try:
+    tss_down = int(tss_down)
+    cmd_list.extend(['--tss_down', str(tss_down)])
+  except Exception as e:
+    _write_err('--tss_down parsed--Failed, tss_down must be int number\n' + str(e) )
+
+  try:
+    gene_length = int(gene_length)
+    cmd_list.extend(['--gene_length', str(gene_length)])
+  except Exception as e:
+    _write_err('--gene_length parsed--Failed, gene_length must be int number\n' + str(e) )
+  try:
+    rpkm_threshold = float(rpkm_threshold)
+    cmd_list.extend(['--rpkm_threshold', str(rpkm_threshold)])
+  except Exception as e:
+    _write_err('--rpkm_threshold parsed--Failed, rpkm_threshold must be int number\n' + str(e) )
+
   try:
     os.system( ' '.join(cmd_list) )
     logger.success('feature_assign--Finished. Find the results in ' + output_root)
   except Exception as e:
     _write_err('feature_assign--Failed\n' + str(e) )
 
   log_file.write(_cur_time()+ 'feature assign finished\n')
@@ -552,15 +684,15 @@
     os.system( ' '.join(cmd_list) )
     logger.success('pausing_sites--Finished. Find the results in ' + output_root)
   except Exception as e:
     _write_err('pausing_sites--Failed\n' + str(e) )
 
   _render_template(output_root=output_root, type='pausing', is_server='No')
 
-def network_analysis(tf_source=None, tf_filter_nodes=None, enhancer_source=None, enhancer_filter_nodes=None, output_root=None ):
+def network_analysis(tf_source=None, enhancer_source=None, select_nodes_file=None, express_file=None, output_root=None ):
   global global_root
   global_root = output_root
   if not output_root.endswith('/'): output_root = output_root + '/'
   _create_project_dir(output_root)
   # logger.info('network_analysis--construct output dir')
   logger.info('network_analysis--check installed software')
   _check_soft(['networkx','community', 'hvplot', 'numpy'], isPython=True)
@@ -574,23 +706,23 @@
   if not(tf_source or enhancer_source):
     _write_err( 'network_analysis--Failed ' + 'no tf or enhancer source file')
     os.sys.exit(1)
 
   if tf_source:
     _check_para('--tf_source', tf_source, str, isFile=True, required=True, output_root=output_root)
     cmd_list.extend(['--tf_source', tf_source])
-  if tf_filter_nodes:
-    _check_para('--tf_filter_nodes', tf_filter_nodes, str, isFile=True, required=True, output_root=output_root)
-    cmd_list.extend(['--tf_filter_nodes', tf_filter_nodes])
+  if select_nodes_file:
+    _check_para('--select_nodes_file', select_nodes_file, str, isFile=True, required=True, output_root=output_root)
+    cmd_list.extend(['--select_nodes_file', select_nodes_file])
   if enhancer_source:
     _check_para('--enhancer_source', enhancer_source, str, isFile=True, required=True, output_root=output_root)
     cmd_list.extend(['--enhancer_source', enhancer_source])
-  if enhancer_filter_nodes:
-    _check_para('--enhancer_filter_nodes', enhancer_filter_nodes, str, isFile=True, required=True, output_root=output_root)
-    cmd_list.extend(['--enhancer_filter_nodes', enhancer_filter_nodes])
+  if express_file:
+    _check_para('--express_file', express_file, str, isFile=True, required=True, output_root=output_root)
+    cmd_list.extend(['--express_file', express_file])
 
   try:
     os.system( ' '.join(cmd_list) )
     logger.success('network analysis--Finished. Find the results in ' + output_root)
     _render_template(output_root=output_root, type='network', is_server='No')
   except Exception as e:
     _write_err('network analysis--Failed\n' + str(e) )
```

### Comparing `nasap-0.2.7/nasap/scripts/extract_preprocess.py` & `nasap-0.2.9/nasap/scripts/extract_preprocess.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/feature_attrs.py` & `nasap-0.2.9/nasap/scripts/feature_attrs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, fire, re, sys, pickle
+import os, fire, re, sys, math
 # sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))+ '/libs')
 script_dir = os.path.abspath(os.path.join(os.path.abspath(__file__), ".."))
 lib_dir = os.path.abspath(os.path.join(os.path.abspath(__file__), '../../libs') )
 sys.path.append(lib_dir)
 from collections import Counter
 
 import numpy as np
@@ -32,14 +32,40 @@
   max_index_list = np.argwhere(v_list == np.amax(v_list)).flatten().tolist()
   if strand == '+':
     max_index = max_index_list[0]
   else:
     max_index = max_index_list[-1]
   return left + max_index
 
+
+def search_truncated_region(arr):
+  window_size = 100
+  step_size = 25
+  read_threshold = 25
+  length_threshold = 800
+  new_shape = ((arr.size - window_size) // step_size + 1, window_size)
+  new_strides = (arr.strides[0] * step_size, arr.strides[0])
+  arr_strided = np.lib.stride_tricks.as_strided(arr, shape=new_shape, strides=new_strides)
+  arr_sum = arr_strided.sum(axis=1)
+  read_num_arr = arr_sum/window_size
+
+  # 获取大于threshold的元素的索引
+  index = np.nonzero(read_num_arr > read_threshold)[0]
+  # 计算索引的差值，找到连续索引的起点和长度
+  ranges = np.split(index, np.where(np.diff(index) != 1)[0]+1)
+  # print( ranges )
+  res = []
+  if ranges:
+    for r in ranges:
+        if len(r) > 0 and len(r) * step_size > length_threshold:
+          res.append( [r[0]*step_size, len(r) * step_size] )
+  return res
+
+
+
 def pausing_index( chr, start, end, strand,  bw, tss_up, tss_down ):
   # 获取 表达的蛋白， lincRNA
   if strand == '+':
     true_tss = find_true_tss(chr, start-tss_up, start + tss_down, bw, strand)
     pp = bw.stats( chr, true_tss-tss_up, true_tss + tss_down)[0]
     gb = bw.stats( chr, true_tss +tss_down, end)[0]
   else:
@@ -66,48 +92,73 @@
   if pp == 0:
     #
     prr = 'proximal promoter count zero'
   else:
     prr = gb/pp
   return prr
 
-def get_attrs(gene_range_dic, forward_bw, reverse_bw, total_bases, tss_up, tss_down):
+def get_attrs(gene_range_dic, forward_bw, reverse_bw, total_bases, tss_up=0, tss_down=150, gene_length=2000, rpkm_threshold=0.1):
   gene_rpkm_dic, gene_baseCount_dic, gene_rpm_dic =  {},{}, {}
   gene_pi_dic, gene_ei_dic = {}, {}
   gene_pp_count_dic, gene_gb_count_dic = {}, {}
+  trunc_gene_list = []
   for strand in ['+', '-']:
     strand_gene_range_dic = gene_range_dic[strand]
     bw = pyBigWig.open( {'+': forward_bw, '-': reverse_bw}[strand])
     for gene_name, gene_range in strand_gene_range_dic.items():
       c, s, e = gene_range[0], gene_range[1], gene_range[2]
       try:
         density = bw.stats(c, s, e)[0]
         rpkm = density2rpkm(density, total_bases)
         base_count = int( density * (e - s) )
         rpm = base_count * 1e6 /total_bases
-        if e - s < 2300:
-          pi, prr='gene too short', 'gene too short'
-          continue
+        if rpkm < rpkm_threshold:
+          pi, prr, pp_count, gb_count = 'gene not expressed', 'gene not expressed', 'gene not expressed', 'gene not expressed'
+
+        if e - s < gene_length:
+          pi, prr, pp_count, gb_count='gene too short', 'gene too short', 'gene too short', 'gene too short'
         else:
           pi, pp_count, gb_count = pausing_index(c,s, e, strand, bw, tss_up, tss_down)
-          prr = elongation_index(c,s, e, strand, bw)
-
+          # prr = elongation_index(c,s, e, strand, bw)
+          if pi == 0:
+            prr = 0
+          else:
+            prr = math.log2(1/pi)
       except:
         continue
       gene_rpkm_dic[gene_name] = rpkm
       gene_baseCount_dic[gene_name] = base_count
       gene_rpm_dic[gene_name] = rpm
       gene_pi_dic[gene_name] = pi
       gene_ei_dic[gene_name] = prr
       gene_pp_count_dic[gene_name] = pp_count
       gene_gb_count_dic[gene_name] = gb_count
+
+      try:
+        arr = bw.values(c, s, e)
+        region_list = search_truncated_region(arr)
+        if len(region_list) > 0:
+          for region in region_list:
+            if strand == '+':
+              trunc_gene_left = s+ region[0] -100
+              trunc_gene_right = s + region[0] + region[1]
+            else:
+              trunc_gene_left = s+ region[0]
+              trunc_gene_right = s+ region[0] + region[1] + 100
+
+            density = bw.stats(c, trunc_gene_left, trunc_gene_right)[0]
+            base_count = int( density * (trunc_gene_right - trunc_gene_left) )
+            trunc_gene_list.append([c, str(trunc_gene_left), str(trunc_gene_right), strand, str(base_count)])
+      except:
+        continue
+
     # dic2json(gene_rpkm_dic, rpkm_json_output)
   return gene_rpkm_dic, gene_baseCount_dic, gene_rpm_dic, \
   gene_pi_dic, gene_ei_dic, \
-  gene_pp_count_dic, gene_gb_count_dic
+  gene_pp_count_dic, gene_gb_count_dic, trunc_gene_list
 
 def coding_vs_linc(protein_data, linc_data, output_root):
   protein_num, linc_num = len(protein_data), len(linc_data)
   big_labels = [f'Coding\n({protein_num})', f'LncRNA\n({linc_num})']
   expressed_protein_num, expressed_linc_num = len(protein_data[protein_data>0]), len(linc_data[linc_data>0])
   expressed_protein_ratio = np.round( expressed_protein_num/protein_num, 2) * 100
   expressed_linc_ratio = np.round( expressed_linc_num/linc_num, 2) * 100
@@ -131,26 +182,34 @@
 
   expressed_dist_data = {'protein_data': protein_data, 'linc_data': linc_data }
   expressed_distribution(expressed_dist_data, output_root)
   # with open('expressed_dist_data.pickle', 'wb') as f:
   #   pickle.dump(expressed_dist_data, f)
 
 # count, RPKM, PI, EI, Exon/intron density
-def main(gtf, forward_bw, reverse_bw, output_root, tss_up=150, tss_down=150 ):
+def main(gtf, forward_bw, reverse_bw, output_root, tss_up=150, tss_down=150, gene_length=2000, rpkm_threshold=0.1):
   # 这里 多搞两个 参数用 tss_up, tss_down 去定义 pp区域，
   # tes的部分暂时不提，就用tss_right 到 tes 定义gb区域。
   total_bases = get_total_bases(forward_bw, reverse_bw)
   gene_df = get_gene_df( gtf )
   filter_gene_df = gene_df[ gene_df['genetype'].isin(['protein_coding', 'lincRNA', 'lncRNA']) ]
   gene_range_dic = gene_df2dic(filter_gene_df)
   # count, RPKM, promoter, geneBody count, PI, EI
 
   gene_rpkm_dic, gene_baseCount_dic, gene_rpm_dic, \
   gene_pi_dic, gene_ei_dic, \
-  gene_pp_count_dic, gene_gb_count_dic = get_attrs(gene_range_dic, forward_bw, reverse_bw, total_bases, tss_up, tss_down)
+  gene_pp_count_dic, gene_gb_count_dic, \
+  trunk_gene_list = get_attrs(gene_range_dic, forward_bw, reverse_bw, total_bases, tss_up, tss_down, gene_length, rpkm_threshold)
+  with open(output_root+'csv/trunc_genes_count.csv', 'w') as f:
+    f.write('\t'.join(['trunc_gene_name', 'chrom', 'start', 'end', 'strand', 'count']) + '\n' )
+    for x in trunk_gene_list:
+      gene_name = x[0] + ':' +  str(x[1]) + '-' + str(x[2])
+      x.insert(0, gene_name)
+      f.write( '\t'.join( x ) + '\n')
+
   # print( list(gene_rpkm_dic.items())[:5] )
 
   attr_list = ['baseCount', 'rpkm', 'rpm', 'pp_count', 'gb_count', 'pi', 'ei']
   filter_gene_type = set(filter_gene_df['genetype'])
   for gene_type in filter_gene_type:
     gene_list = filter_gene_df[filter_gene_df['genetype'] == gene_type]['gene_name']
     for attr in attr_list:
```

### Comparing `nasap-0.2.7/nasap/scripts/gencore/gencore` & `nasap-0.2.9/nasap/scripts/gencore/gencore`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/genome_track_visualization.py` & `nasap-0.2.9/nasap/scripts/genome_track_visualization.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/map1.bash` & `nasap-0.2.9/nasap/scripts/map1.bash`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/map2.bash` & `nasap-0.2.9/nasap/scripts/map2.bash`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/map_split.py` & `nasap-0.2.9/nasap/scripts/map_split.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/network_analysis.py` & `nasap-0.2.9/nasap/scripts/network_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     ls = ln.split(',')
     source, target =ls[0], ls[1].strip()
     source_set.add(source)
     target_set.add(target)
     source_target_edge_set.add( ( source, target ) )
 
   target_set = target_set - source_set
-  return  list( source_set ), list( target_set ), source_target_edge_set
+  return  list( source_set ), list( target_set ), list(source_target_edge_set)
 
 def generate_graph(tf_nodes, protein_nodes, edges):
   G = nx.DiGraph()
   G.add_nodes_from( tf_nodes, shape = 'D')
   G.add_nodes_from( protein_nodes, shape='o' )
   G.add_edges_from( edges )
   return G
@@ -88,28 +88,42 @@
     except:
       continue
     if float(attr) > over_condition:
       filter_nodes.append(node)
   sub_G = G.subgraph(filter_nodes)
   return sub_G
 
-def network_summary_info(G, output_root):
+def network_summary_info(G, output_root, tf_num, enhancer_num):
   graph_info = {}
   graph_info['nodes_num'] = nx.number_of_nodes(G)
   graph_info['edges_num'] = nx.number_of_edges(G)
+  graph_info['tf_num'] = tf_num
+  graph_info['enhancer_num'] = enhancer_num
   graph_info['mean_degree'] = 2* graph_info['edges_num']/graph_info['nodes_num']
-  graph_info['assortativity_coefficient'] = nx.degree_assortativity_coefficient(G) # 匹配系数
-  graph_info['correlation_coefficient'] = nx.degree_pearson_correlation_coefficient(G) # 相关性系数
+  try:
+    graph_info['assortativity_coefficient'] = nx.degree_assortativity_coefficient(G) # 匹配系数
+  except Exception as e:
+    print( e )
+  try:
+    graph_info['correlation_coefficient'] = nx.degree_pearson_correlation_coefficient(G) # 相关性系数
+  except Exception as e:
+    print( e )
   # graph_info['closeness_centrality'] = nx.closeness_centrality(G) # 节点距离中心系数
   # graph_info['betweenness_centrality'] = nx.betweenness_centrality(G) # 节点介数中心系数
-  graph_info['transitivity'] = nx.transitivity(G) # 图或网络的传递性。
+  try:
+    graph_info['transitivity'] = nx.transitivity(G) # 图或网络的传递性。
+  except Exception as e:
+    print( e )
   # graph_info['clustering'] = nx.clustering(G) # 图或网络中节点的聚类系数,用来度量连接的密度。
   # graph_info['average_clustering'] = nx.average_clustering(G) # nx.clustering(G) 的均值
   # graph_info['square_clustering'] = nx.square_clustering(G)
-  graph_info['density'] = nx.density(G)
+  try:
+    graph_info['density'] = nx.density(G)
+  except Exception as e:
+    print( e )
   dic2csv(graph_info, output_root + 'csv/graph_info.csv')
 
 
 def degree_analysis(G, output_root):
   def degree_histogram_directed(G, in_degree=False, out_degree=False):
     """Return a list of the frequency of each degree value.
 
@@ -178,14 +192,15 @@
 
   motif_dic = {'xAxis': xAxis, 'triad_count_list': triad_count_list}
   network_motif(motif_dic, output_root)
   with open('motif_dic.pickle', 'wb') as f:
     pickle.dump(motif_dic, f)
 
 
+
 def community_analysis( G, node_type_dic, output_root ):
   type_list = list( set( node_type_dic.values() ) )
   shape_list = 'od^ps>v<h8'
   if len(type_list) > len( shape_list):
     print('Error, node type is over', len(shape_list) )
   type_shape_dic = two_list_2_dict( type_list, shape_list[: len(type_list)] )
   partition = community_louvain.best_partition( nx.to_undirected( G ),resolution=1)
@@ -193,21 +208,21 @@
 
   community_dic = defaultdict( lambda: [])
   for n, c in partition.items():
     community_dic[c].append(n)
 
   dic2csv({'community_' + str(c): len(n_list) for c, n_list in community_dic.items()}, output_root + 'csv/community_node_num.csv')
   for c, n_list in community_dic.items():
-    g = G.subgraph( n_list )
-    keep_nodes = [n for n,d in g.degree if d >= 2 ]
-    g = g.subgraph( keep_nodes )
     with open( output_root + 'txt/community_%s.txt'%c, 'w' ) as f:
-      for n in g:
+      for n in n_list:
         f.write(n + '\n')
 
+    g = G.subgraph( n_list )
+    keep_nodes = [n for n,d in g.degree if d >= 2 ]
+    g = g.subgraph( keep_nodes )
     if len(g) <=10:
       print( 'community %s nodes less than 10'%str(c) )
       continue
     if len( g ) > 1000:
       print( 'community %s nodes more than 1000'%str(c) )
       continue
 
@@ -236,71 +251,82 @@
     hvnx.save( hv_final, output_root + 'html/community_' +str(c)+'.html')
 
     nx.draw_networkx_edges(g,pos)
     plt.legend(scatterpoints = 1)
     plt.savefig(output_root + "imgs/community_%s.png"%str(c), format="PNG")
     plt.close(fig)
 
+def main(tf_source=None, enhancer_source=None, select_nodes_file=None, express_file=None, output_root='./tmp_output/' ):
+  # 节点 + 边
+  total_source, total_target, total_edges =[], [], []
+  # 节点 属性
+  node_type_dic, node_express_dic = {}, {}
 
 
-def main(tf_source=None, tf_filter_nodes=None, enhancer_source=None, enhancer_filter_nodes=None, output_root='./tmp_output/' ):
-  filter_source, filter_target, edge_set =[], [], set()
-  node_type_dic = {}
-
-  # 1 使用source 构建网络
+  # 1 使用source file 获取 节点+边
+  tf_list, enhancer_list = [], []
   if tf_source:
-    tf_list, gene_list, tf_target_edge_set = get_source_target(tf_source)
+    tf_list, gene_list, tf_target_edge_list = get_source_target(tf_source)
     print( 'tf gene number is %s, target gene number is %s'%( str(len(tf_list) ), str(len(gene_list)) ))
-    if tf_filter_nodes:
-      filter_tf_nodes = [ln.strip() for ln in open(tf_filter_nodes)]
-      for tf in tf_list:
-        if tf in filter_tf_nodes:
-          filter_source.append( tf )
-
-      for gene in gene_list:
-        if gene in filter_tf_nodes:
-          filter_target.append( gene )
+    total_source.extend( list( set(tf_list) ) )
+    total_target.extend( list( set(gene_list) ) )
+    total_edges.extend( tf_target_edge_list )
 
-    else:
-      filter_source.extend(tf_list)
-      filter_target.extend(gene_list)
-    edge_set = tf_target_edge_set
+    # 节点属性
     for gene in gene_list:
       node_type_dic[gene] = 'gene'
     for tf in tf_list:
       node_type_dic[tf] = 'tf'
 
   if enhancer_source:
-    enhancer_list, gene_list, enhancer_gene_edge_set = get_source_target(enhancer_source)
+    enhancer_list, gene_list, enhancer_target_edge_list = get_source_target(enhancer_source)
     print( 'enhancer gene number is %s, target gene number is %s'%( str(len(enhancer_list) ), str(len(gene_list)) ))
-    if enhancer_filter_nodes:
-      filter_enhancer_nodes = [ln.strip() for ln in open(enhancer_filter_nodes)]
-      for enhancer in enhancer_list:
-        if enhancer in filter_enhancer_nodes:
-          filter_source.append( enhancer )
-      for gene in gene_list:
-        if gene in filter_enhancer_nodes:
-          filter_target.append( gene )
-    else:
-      filter_source.extend( enhancer_list  )
-      filter_target.extend( gene_list )
-
-    for edge in enhancer_gene_edge_set:
-      edge_set.add(edge)
+    total_source.extend( list( set(enhancer_list) ) )
+    total_target.extend( list( set(gene_list) ) )
+    total_edges.extend( enhancer_target_edge_list )
+    # 节点属性
     for gene in gene_list:
       if gene not in node_type_dic.keys():
         node_type_dic[gene] = 'gene'
     for enhancer in enhancer_list:
       node_type_dic[enhancer] = 'enhancer'
 
-  filter_source, filter_target = list(set(filter_source)), list(set(filter_target))
-  print( 'after filtering, source gene number is %s, target gene number is %s'%( str(len(filter_source) ), str(len(filter_target) )) )
 
-  G = generate_graph(filter_target, filter_source, edge_set)
-  network_summary_info(G, output_root)
+  # filter_nodes用于筛选的节点 包含了 tf, enhancer, gene。 最后的网络只在filter_nodes中
+  filtered_sources, filtered_targets = total_source, total_target
+  if select_nodes_file:
+    select_node_set = set([ln.strip() for ln in open(select_nodes_file)])
+    filtered_sources = list( select_node_set & set(filtered_sources) )
+    filtered_targets = list( select_node_set & set(filtered_targets) )
+
+  # print( len(filtered_targets), len(filtered_sources))
+  if express_file:
+    express_node_set = set()
+    for ln in open(express_file):
+      try:
+        gene, count = ln.strip().split(',')
+        if float(count) > 0:
+          express_node_set.add( gene )
+          node_express_dic[gene] = float(count)
+      except:
+        pass
+    # print( len(express_node_set) )
+    filtered_sources = list( set(filtered_sources) & express_node_set)
+    filtered_targets = list( set(filtered_targets) & express_node_set)
+
+  print( 'after filtering, source gene number is %s, target gene number is %s'%( str(len(filtered_sources) ), str(len(filtered_targets) )) )
+
+  filter_edges = []
+  for edge in total_edges:
+    s, t = edge[0], edge[1]
+    if s in filtered_sources and t in filtered_targets:
+      filter_edges.append(edge)
+
+  G = generate_graph(filtered_targets, filtered_sources, filter_edges)
+  network_summary_info(G, output_root, len( set(tf_list) & set(filtered_sources) ), len( set(enhancer_list) & set(filtered_sources) ) )
   # attr_dic = {ln.split(',')[0]: ln.split(',')[1] for ln in open(filter_nodes)}
   # print( len(protein_list), len(tf_list), len(tf_protein_edge_set))
   # G = generate_graph(protein_list, tf_list, tf_protein_edge_set)
   # filter_G = filter_nodes(G, attr_dic)
   # 2 degree 分析
   degree_analysis(G, output_root)
```

### Comparing `nasap-0.2.7/nasap/scripts/parse_gtf.py` & `nasap-0.2.9/nasap/scripts/parse_gtf.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/pausing_sites.py` & `nasap-0.2.9/nasap/scripts/pausing_sites.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/pausing_sites_low_memory.py` & `nasap-0.2.9/nasap/scripts/pausing_sites_low_memory.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/plot.py` & `nasap-0.2.9/nasap/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/preprocess.bash` & `nasap-0.2.9/nasap/scripts/preprocess.bash`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/preprocess_fast.bash` & `nasap-0.2.9/nasap/scripts/preprocess_fast.bash`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/py_ext.py` & `nasap-0.2.9/nasap/scripts/py_ext.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/render_template.py` & `nasap-0.2.9/nasap/scripts/render_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,21 @@
     'featureAssign': [
       # 2.1 Quantification & Normalization
       ('file', 'csv/all_feature_attrs.csv', 'all_feature_attrs_csv'),
       ('file', 'csv/lincRNA_baseCount.csv', 'lincRNA_baseCount_csv'),
       ('file', 'csv/lincRNA_gb_count.csv', 'lincRNA_gb_count_csv'),
       ('file', 'csv/lincRNA_pp_count.csv', 'lincRNA_pp_count_csv'),
       ('file', 'csv/lincRNA_rpkm.csv', 'lincRNA_rpkm_csv'),
+      ('file', 'csv/lincRNA_rpm.csv', 'lincRNA_rpm_csv'),
       ('file', 'csv/protein_coding_baseCount.csv', 'protein_coding_baseCount_csv'),
       ('file', 'csv/protein_coding_gb_count.csv', 'protein_coding_gb_count_csv'),
       ('file', 'csv/protein_coding_pp_count.csv', 'protein_coding_pp_count_csv'),
       ('file', 'csv/protein_coding_rpkm.csv', 'protein_coding_rpkm_csv'),
+      ('file', 'csv/protein_coding_rpkm.csv', 'protein_coding_rpm_csv'),
+      ('file', 'csv/erna_quant.csv', 'erna_quant_csv'),
       # 3.1 PI $EI
       ('file', 'csv/lincRNA_ei.csv', 'lincRNA_ei_csv'),
       ('file', 'csv/lincRNA_pi.csv', 'lincRNA_pi_csv'),
       ('file', 'csv/protein_coding_ei.csv', 'protein_coding_ei_csv'),
       ('file', 'csv/protein_coding_pi.csv', 'protein_coding_pi_csv'),
       # 1.5
       ('file', 'csv/exon_intron_ratio.csv', 'exon_intron_ratio_csv'),
```

### Comparing `nasap-0.2.7/nasap/scripts/templates/static/vue.min.js` & `nasap-0.2.9/nasap/scripts/templates/static/vue.min.js`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/templates/template.html` & `nasap-0.2.9/nasap/scripts/templates/template.html`

 * *Files 2% similar despite different names*

```diff
@@ -208,18 +208,21 @@
           <table border="1">
             <tr><th>File</th><th>Directory</th></tr>
             <tr v-if="all_feature_attrs_csv"><td>all feature attrs</td><td> {{ all_feature_attrs_csv }}</td></tr>
             <tr v-if="lincRNA_baseCount_csv"><td>lincRNA count</td><td> {{ lincRNA_baseCount_csv }}</td></tr>
             <tr v-if="lincRNA_gb_count_csv"><td>lincRNA gene body count</td><td> {{ lincRNA_gb_count_csv }}</td></tr>
             <tr v-if="lincRNA_pp_count_csv"><td>lincRNA proximal promoter count</td><td> {{ lincRNA_pp_count_csv }}</td></tr>
             <tr v-if="lincRNA_rpkm_csv"><td>lincRNA rpkm</td><td> {{ lincRNA_rpkm_csv }}</td></tr>
+            <tr v-if="lincRNA_rpm_csv"><td>lincRNA rpm</td><td> {{ lincRNA_rpm_csv }}</td></tr>
             <tr v-if="protein_coding_baseCount_csv"><td>protein coding count</td><td> {{ protein_coding_baseCount_csv }}</td></tr>
             <tr v-if="protein_coding_gb_count_csv"><td>protein coding gb count</td><td> {{ protein_coding_gb_count_csv }}</td></tr>
             <tr v-if="protein_coding_pp_count_csv"><td>protein coding pp count</td><td> {{ protein_coding_pp_count_csv }}</td></tr>
             <tr v-if="protein_coding_rpkm_csv"><td>protein coding rpkm</td><td> {{ protein_coding_rpkm_csv }}</td></tr>
+            <tr v-if="protein_coding_rpm_csv"><td>protein coding rpm</td><td> {{ protein_coding_rpm_csv }}</td></tr>
+            <tr v-if="erna_quant_csv"><td>enhancer RNA log density</td><td> {{ erna_quant_csv }}</td></tr>
           </table>
           <div class="title4 title">Quantitative analysis--2. Abundance estimate</div>
           <div class="card" v-if="img_expressed_genes">
             <img :src="img_expressed_genes" />
             <small>expressed genes pie plot</small>
             <p>The plot stats lincRNA and protein-coding RNA expressed genes.</p>
           </div>
```

#### html2text {}

```diff
@@ -106,18 +106,21 @@
  __________________________________________________________________
 |File___________________________|Directory_________________________|
 |all_feature_attrs______________|{{_all_feature_attrs_csv_}}_______|
 |lincRNA_count__________________|{{_lincRNA_baseCount_csv_}}_______|
 |lincRNA_gene_body_count________|{{_lincRNA_gb_count_csv_}}________|
 |lincRNA_proximal_promoter_count|{{_lincRNA_pp_count_csv_}}________|
 |lincRNA_rpkm___________________|{{_lincRNA_rpkm_csv_}}____________|
+|lincRNA_rpm____________________|{{_lincRNA_rpm_csv_}}_____________|
 |protein_coding_count___________|{{_protein_coding_baseCount_csv_}}|
 |protein_coding_gb_count________|{{_protein_coding_gb_count_csv_}}_|
 |protein_coding_pp_count________|{{_protein_coding_pp_count_csv_}}_|
 |protein_coding_rpkm____________|{{_protein_coding_rpkm_csv_}}_____|
+|protein_coding_rpm_____________|{{_protein_coding_rpm_csv_}}______|
+|enhancer_RNA_log_density_______|{{_erna_quant_csv_}}______________|
 Quantitative analysis--2. Abundance estimate
 src="img_expressed_genes" /> expressed genes pie plot
 The plot stats lincRNA and protein-coding RNA expressed genes.
 src="img_expression_distribution" /> expressed RNA distribution plot
 The relative abundance of different RNA molecules are evaluted in the plot
 Quantitative analysis--3.Gene expression on different chromosomes
 src="img_chr_rpkm" /> chromosomal distribution plot
```

### Comparing `nasap-0.2.7/nasap/scripts/templates/template_track.txt` & `nasap-0.2.9/nasap/scripts/templates/template_track.txt`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/tmp_plot.py` & `nasap-0.2.9/nasap/scripts/tmp_plot.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap/scripts/x.py` & `nasap-0.2.9/nasap/scripts/x.py`

 * *Files identical despite different names*

### Comparing `nasap-0.2.7/nasap.egg-info/SOURCES.txt` & `nasap-0.2.9/nasap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 nasap/scripts/py_ext.py
 nasap/scripts/render_template.py
 nasap/scripts/tmp_plot.py
 nasap/scripts/x.py
 nasap/scripts/gencore/gencore
 nasap/scripts/templates/template.html
 nasap/scripts/templates/template_track.txt
-nasap/scripts/templates/static/vue.min.js
+nasap/scripts/templates/static/vue.min.js
+nasap/scripts/ucsc/bedGraphToBigWig
```

### Comparing `nasap-0.2.7/setup.py` & `nasap-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 snap_directories = [f for f in glob(snapdir, recursive=True) if os.path.isdir( f )]
 # print( snap_directories )
 for directory in snap_directories:
   snap_files.append((directory, [os.path.join(directory, f) for f in os.listdir(directory) if not os.path.isdir(os.path.join(directory, f))]) )
 
 gencore_files = ['nasap/scripts/gencore/gencore']
+bg2bw_files = ['nasap/scripts/ucsc/bedGraphToBigWig']
 
 data_files = [('nasap/scripts/', glob('nasap/scripts/[!_]*.py', recursive=True) ),
   ('nasap/scripts/', glob('nasap/scripts/[!_]*.bash', recursive=True) ),
   ('nasap/scripts/templates/', ['nasap/scripts/templates/template.html', 'nasap/scripts/templates/template_track.txt']),
   ('nasap/scripts/templates/static/', ['nasap/scripts/templates/static/vue.min.js']),
 ]
 # print( snap_files )
 data_files.extend(snap_files)
 data_files.extend( gencore_files )
+data_files.extend( bg2bw_files )
 
 def get_version():
   with open( os.path.abspath(os.path.dirname(__file__) ) + '/nasap/__version__.py') as f:
     ver = f.read().split('version=')[1].replace('"', '').strip()
   return ver
 
 def main():
```


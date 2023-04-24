# Comparing `tmp/histcite-python-0.1.2.tar.gz` & `tmp/histcite-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.1.2.tar", last modified: Sun Apr 23 01:47:24 2023, max compression
+gzip compressed data, was "histcite-python-0.1.3.tar", last modified: Mon Apr 24 10:17:09 2023, max compression
```

## Comparing `histcite-python-0.1.2.tar` & `histcite-python-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-23 01:47:09.000000 histcite-python-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-23 01:47:24.339620 histcite-python-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-23 01:47:09.000000 histcite-python-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 01:47:24.339620 histcite-python-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 01:47:09.000000 histcite-python-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 10:16:58.000000 histcite-python-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:17:09.505904 histcite-python-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-24 10:16:58.000000 histcite-python-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/parse_citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/process_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:17:09.505904 histcite-python-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-24 10:16:58.000000 histcite-python-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_parse_citation.py
```

### Comparing `histcite-python-0.1.2/LICENSE` & `histcite-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.2/PKG-INFO` & `histcite-python-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -19,94 +19,104 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据[字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
 > 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
 
 ```console
-$ python3 -m pip install histcite-python
+# 需要 Python 3.8 或以上版本
+pip install histcite-python
 ```
 
 ## 使用方法
-1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-```console
-$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
-```
-参数说明：
+1、使用命令行工具，可用参数如下：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
-| -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+```console
+$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
+```
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图如下所示：
-<img src="examples/graph.svg">  
+生成的引文网络图：
+
+<img src="examples/graph.svg">
+
+对应的节点信息：
+| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+| :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
+|    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
+|    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
+|    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
+|    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
+|    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
+|    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path) # 读取并处理题录数据
-concated_table = process.concat_table() # 合并多个文件
-
-# 提取所有文献的参考文献
-reference_table = process.generate_reference_table(concated_table['CR']) 
+process = ProcessTable(folder_path)
+process.concat_table() # 合并多个文件
+process.process_citation() # 识别引文关系
+docs_table = process.docs_table
+reference_table = process.reference_table
 
-# 识别引文关系
-citation_table = process.process_citation(reference_table) 
-
-# 各分析单元的引文统计
-cm = ComputeMetrics(citation_table, reference_table)
+# 基本描述统计
+cm = ComputeMetrics(docs_table, reference_table)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(citation_table)
-doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph = Graphviz(docs_table)
+doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+
+# 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
 
-# 生成引文网络图节点文件
+# 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| - | - | - |
+| :-: | :-: | :-: |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
 | 是否开源 | 是 | 否 |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
```

### Comparing `histcite-python-0.1.2/README.md` & `histcite-python-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,99 @@
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据[字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
 > 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
 
 ```console
-$ python3 -m pip install histcite-python
+# 需要 Python 3.8 或以上版本
+pip install histcite-python
 ```
 
 ## 使用方法
-1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-```console
-$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
-```
-参数说明：
+1、使用命令行工具，可用参数如下：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
-| -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+```console
+$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
+```
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图如下所示：
-<img src="examples/graph.svg">  
+生成的引文网络图：
+
+<img src="examples/graph.svg">
+
+对应的节点信息：
+| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+| :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
+|    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
+|    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
+|    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
+|    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
+|    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
+|    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path) # 读取并处理题录数据
-concated_table = process.concat_table() # 合并多个文件
-
-# 提取所有文献的参考文献
-reference_table = process.generate_reference_table(concated_table['CR']) 
+process = ProcessTable(folder_path)
+process.concat_table() # 合并多个文件
+process.process_citation() # 识别引文关系
+docs_table = process.docs_table
+reference_table = process.reference_table
 
-# 识别引文关系
-citation_table = process.process_citation(reference_table) 
-
-# 各分析单元的引文统计
-cm = ComputeMetrics(citation_table, reference_table)
+# 基本描述统计
+cm = ComputeMetrics(docs_table, reference_table)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(citation_table)
-doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph = Graphviz(docs_table)
+doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+
+# 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
 
-# 生成引文网络图节点文件
+# 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| - | - | - |
+| :-: | :-: | :-: |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
 | 是否开源 | 是 | 否 |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
```

### Comparing `histcite-python-0.1.2/histcite/compute_metrics.py` & `histcite-python-0.1.3/histcite/compute_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import pandas as pd
 
 class ComputeMetrics:
     """生成统计结果"""
 
-    def __init__(self,citation_table,reference_table):
-        self.citation_table = citation_table
+    def __init__(self,docs_table,reference_table):
+        self.docs_table = docs_table
         self.reference_table = reference_table
 
     def __generate_table(self,use_cols:list,col:str,split_char=None)->pd.DataFrame:
         
-        df = self.citation_table[use_cols]
+        df = self.docs_table[use_cols]
         # 如果字段包含多个值，则进行拆分
         if split_char:
             try:
                 df = df.dropna(subset=[col])
                 df[col] = df[col].str.split(split_char)
             except NotImplementedError:
                 df = df.astype({col:'str'})
@@ -40,15 +40,15 @@
     def _generate_institution_table(self):
         use_cols = ['C3','LCS','TC']
         return self.__generate_table(use_cols,'C3','; ')
     
     def _generate_records_table(self):
         """生成文献简表"""
         use_cols = ['AU','TI','SO','LCS','TC','LCR','NR']
-        records_table = self.citation_table[use_cols]
+        records_table = self.docs_table[use_cols]
         records_table = records_table.rename(columns={'TC':'GCS','NR':'GCR'})
         return records_table
     
     def _generate_journal_table(self):
         use_cols = ['SO','LCS','TC']
         return self.__generate_table(use_cols,'SO')
 
@@ -63,15 +63,15 @@
     def _generate_reference_table(self):
         """生成参考文献表，按照引用次数降序排列，同时标记是否为本地文献"""
         check_cols = ['PY','J9','VL','BP']
         use_cols = self.reference_table.columns.tolist()[:-1]
         reference_table = self.reference_table.groupby(use_cols,as_index=False).size()
         reference_table = reference_table.sort_values(by='size',ascending=False)
         reference_table = reference_table.rename(columns={'size':'Recs'})
-        common_table = reference_table.reset_index().merge(self.citation_table[check_cols],on=check_cols)
+        common_table = reference_table.reset_index().merge(self.docs_table[check_cols],on=check_cols)
         reference_table['local'] = 0
         reference_table.loc[common_table['index'],'local'] = 1
         return reference_table
     
     def write2excel(self,save_path):
         """将统计结果写入excel"""
         save_folder_path = os.path.dirname(save_path)
```

### Comparing `histcite-python-0.1.2/histcite/network_graph.py` & `histcite-python-0.1.3/histcite/network_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 
 class GraphViz:
 
-    def __init__(self,citation_table):
-        self.citation_table = citation_table
-        self.year_empty_index = set(citation_table[citation_table['PY'].isna()].index)
+    def __init__(self,docs_table):
+        self.docs_table = docs_table
+        self.year_empty_index = set(docs_table[docs_table['PY'].isna()].index)
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
 
-        year_series = self.citation_table.loc[self.node_list,'PY']
+        year_series = self.docs_table.loc[self.node_list,'PY']
         groups = year_series.groupby(year_series)
         year_list = [i[0] for i in groups]
         grouped_doc_index = [i[1].index.tolist() for i in groups]
         self.year_list = year_list
         for idx,year in enumerate(year_list):
             grouped_doc_index[idx].insert(0,year)
         self.grouped_doc_index = grouped_doc_index
@@ -24,15 +24,15 @@
         related_doc_list = [int(i) for i in doc_relation.split(';') if int(i) not in self.year_empty_index]
         if relation_type=='reference':
             return {(doc_index,ref) for ref in related_doc_list}
         elif relation_type=='citation':
             return {(citation,doc_index) for citation in related_doc_list}
         
     def __generate_edge_list(self):
-        min_df = self.citation_table.loc[self.doc_indices,['reference','citation']]
+        min_df = self.docs_table.loc[self.doc_indices,['reference','citation']]
         edge_set = set()
         for idx in self.doc_indices:
             doc_index = idx
             doc_reference = min_df.loc[idx,'reference']
             doc_citation = min_df.loc[idx,'citation']
             if pd.notna(doc_citation):
                 edge_set.update(self.__generate_edge(doc_index, doc_citation, 'citation')) # type:ignore
@@ -62,15 +62,14 @@
         """
         self.doc_indices = [i for i in doc_indices if i not in self.year_empty_index]
         self.allow_external_node = allow_external_node
 
         raw_edge_list = self.__generate_edge_list()
         self.__obtain_groups()
         
-        # dot_edge_list = [f'\t{edge[0]} -> {edge[1]};\n' for edge in raw_edge_list]
         dot_edge_list = [f'\t{source} -> '+'{ '+' '.join([str(i) for i in raw_edge_list[source]])+' };\n' for source in raw_edge_list]
         dot_groups = [f'\t{{rank=same; {" ".join([str(i) for i in group_index])}}};\n' for group_index in self.grouped_doc_index]
         
         reverse_year_list = self.year_list[::-1]
         year_edge_list = [(year,reverse_year_list[idx+1]) for idx,year in enumerate(reverse_year_list) if idx < len(reverse_year_list)-1]
         dot_year_node_list = [f'\t{year} [ shape="plaintext" ];\n' for year in self.year_list]
         dot_year_edge_list = [f'\t{edge[0]} -> {edge[1]} [ style = invis ];\n' for edge in year_edge_list]
@@ -86,18 +85,15 @@
             dot_text += dot_year_edge
             
         for dot_edge in dot_edge_list:
             dot_text += dot_edge
         dot_text += '}'
         return dot_text
     
-    @staticmethod
-    def __extract_first_author(au_cell:str):
-        """提取一作"""
-        return au_cell.split(';',1)[0].replace(',','')
-    
     def generate_graph_node_file(self)->pd.DataFrame:
         use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
-        graph_node_table = self.citation_table.loc[self.node_list,use_cols]
-        graph_node_table['AU'] = graph_node_table['AU'].apply(self.__extract_first_author)
+        graph_node_table = self.docs_table.loc[self.node_list,use_cols]
         graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
-        return graph_node_table
+        return graph_node_table
+    
+    def _export_graph_node_file(self,file_path:str):
+        self.generate_graph_node_file().to_excel(file_path,index=False)
```

### Comparing `histcite-python-0.1.2/histcite/parse_citation.py` & `histcite-python-0.1.3/histcite/parse_citation.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 DI = DI.group(1)
                 if '[' in DI or ']' in DI:
                     DI = None
                                             
         finally:
             # AU strip
             if isinstance(AU,str):
-                cr_data['AU'] = AU.strip()
+                cr_data['AU'] = AU.strip(', ')
             else:
                 return None
         
             # check year
             if PY:
                 if re.match(r'^\d{4}$',PY):
                     PY = int(PY)
@@ -71,13 +71,8 @@
         parsed_cr_list = [self.__parse_one_cr(i) for i in self.cr_list]
         for single in parsed_cr_list:
             if single is not None:
                 for key in self.keys:
                     result[key].append(single[key])
         
         result['doc_index'] = self.doc_index
-        return result
-    
-    def export_citation_table(self):
-        parsed_result = self.parse_cr_cell()
-        if parsed_result:
-            return pd.DataFrame.from_dict(parsed_result)
+        return result
```

### Comparing `histcite-python-0.1.2/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.1.3/histcite_python.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -19,94 +19,104 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
 
 ## 术语说明
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
-- Web of science题录数据[字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
+- Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
 > 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
 
 ```console
-$ python3 -m pip install histcite-python
+# 需要 Python 3.8 或以上版本
+pip install histcite-python
 ```
 
 ## 使用方法
-1、使用命令行工具，输入 `histcite -h` 查看帮助信息
-```console
-$ 下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数为 100
-$ histcite -f /Users/.../downloads/dataset -n 100
-```
-参数说明：
+1、使用命令行工具，可用参数如下：
 | 简写参数 | 参数 | 说明 |
 | :-: | :-: | --- |
-| -f | --folder_path | 下载的题录数据存放的文件夹路径 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的50篇文献 |
+| -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
+| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+```console
+$ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
+$ histcite -f /Users/.../downloads/dataset -n 100
+```
 
-> 结果保存在 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot`, 三个文件，第一个是引文统计表，第二个是引文网络图文献节点表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。
+> 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图如下所示：
-<img src="examples/graph.svg">  
+生成的引文网络图：
+
+<img src="examples/graph.svg">
+
+对应的节点信息：
+| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+| :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
+|    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
+|    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
+|    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
+|    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
+|    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
+|    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
 from histcite.parse_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-process = ProcessTable(folder_path) # 读取并处理题录数据
-concated_table = process.concat_table() # 合并多个文件
-
-# 提取所有文献的参考文献
-reference_table = process.generate_reference_table(concated_table['CR']) 
+process = ProcessTable(folder_path)
+process.concat_table() # 合并多个文件
+process.process_citation() # 识别引文关系
+docs_table = process.docs_table
+reference_table = process.reference_table
 
-# 识别引文关系
-citation_table = process.process_citation(reference_table) 
-
-# 各分析单元的引文统计
-cm = ComputeMetrics(citation_table, reference_table)
+# 基本描述统计
+cm = ComputeMetrics(docs_table, reference_table)
 cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
 
 # 生成引文网络图文件
-graph = Graphviz(citation_table)
-doc_indices = citation_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
+graph = Graphviz(docs_table)
+doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
 graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
+
+# 保存引文网络图文件
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
 
-# 生成引文网络图节点文件
+# 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> `generate_dot_text` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的文献，`doc_indices` 一般为LCS比较高的文献，这些文献同样会参考低LCS的文献，或被低LCS的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认设置 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| - | - | - |
+| :-: | :-: | :-: |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
 | 是否开源 | 是 | 否 |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
 ## TODO
```

### Comparing `histcite-python-0.1.2/setup.py` & `histcite-python-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.2",
+    version="0.1.3",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.1.2/test/test_parse_citation.py` & `histcite-python-0.1.3/tests/test_parse_citation.py`

 * *Files identical despite different names*


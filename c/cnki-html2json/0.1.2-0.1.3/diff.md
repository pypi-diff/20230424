# Comparing `tmp/cnki_html2json-0.1.2.tar.gz` & `tmp/cnki_html2json-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.2.tar", last modified: Sun Apr 23 02:06:27 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.3.tar", last modified: Mon Apr 24 18:45:03 2023, max compression
```

## Comparing `cnki_html2json-0.1.2.tar` & `cnki_html2json-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.503498 cnki_html2json-0.1.3/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:45:03.000000 cnki_html2json-0.1.3/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:45:03.507498 cnki_html2json-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 18:44:48.000000 cnki_html2json-0.1.3/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.2/LICENSE` & `cnki_html2json-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.2/PKG-INFO` & `cnki_html2json-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,102 +22,98 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签
+- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本
-- 实现了一个基于selenium的爬虫，可以批量获取所需文献的结构化文本
-- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引
-  - 以上三种模式都包含参考文献文献，可以参考examples文件夹中给出的样例
-
-使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持
-- 对中文期刊论文进行引文分析
+核心功能：¥
+- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
+- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
+  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
+  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+
+<!-- 使用场景：
+- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
+- 对中文期刊论文进行引文分析； -->
 
 使用限制：
-- 确保你所在的网络环境能正常使用知网
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整
-- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
+- 确保你所在的网络环境能正常使用知网；
+- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
-$ python3 -m pip install cnki_html2json
+$ pip install cnki_html2json
 ```
 
 ## 使用方法
-
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
     html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| `export` | 是否导出，默认 `False` |
-| `export_path` | 保存结果的路径，默认为 `None` ，如果 `export` 设置为 `True`，该参数必须指定 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
-> 函数返回值说明：参考examples文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
-$ cnki-crawler -s 1 -e 100 -m structure -l false
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
-参数说明：
+命令行工具参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
+| -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
 ```
 
 ## json文件字段说明
-
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
 |  | authors |  |论文作者|
 |  | orgs |  |作者所属机构|
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
@@ -127,16 +123,9 @@
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
 |  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
-## 工具推荐
-
-| 工具  | 描述 |
-| --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
-
-## 责任声明
-
-- 使用者使用本工具造成的一切后果，由使用者自行承担
+## 开源协议
+本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.2/README.md` & `cnki_html2json-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,96 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签
+- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本
-- 实现了一个基于selenium的爬虫，可以批量获取所需文献的结构化文本
-- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引
-  - 以上三种模式都包含参考文献文献，可以参考examples文件夹中给出的样例
-
-使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持
-- 对中文期刊论文进行引文分析
+核心功能：¥
+- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
+- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
+  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
+  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+
+<!-- 使用场景：
+- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
+- 对中文期刊论文进行引文分析； -->
 
 使用限制：
-- 确保你所在的网络环境能正常使用知网
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整
-- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
+- 确保你所在的网络环境能正常使用知网；
+- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
-$ python3 -m pip install cnki_html2json
+$ pip install cnki_html2json
 ```
 
 ## 使用方法
-
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
     html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| `export` | 是否导出，默认 `False` |
-| `export_path` | 保存结果的路径，默认为 `None` ，如果 `export` 设置为 `True`，该参数必须指定 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
-> 函数返回值说明：参考examples文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
-$ cnki-crawler -s 1 -e 100 -m structure -l false
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
-参数说明：
+命令行工具参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
+| -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
 ```
 
 ## json文件字段说明
-
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
 |  | authors |  |论文作者|
 |  | orgs |  |作者所属机构|
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
@@ -104,16 +100,9 @@
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
 |  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
-## 工具推荐
-
-| 工具  | 描述 |
-| --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
-
-## 责任声明
-
-- 使用者使用本工具造成的一切后果，由使用者自行承担
+## 开源协议
+本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.2/cnki_html2json/cli.py` & `cnki_html2json-0.1.3/cnki_html2json/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='开始下载索引, 默认为1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='结束下载索引, 默认为None, 即下载到最后')
     parser.add_argument('-m','--mode',type=str,default='structure',help='模式: structure|plain|raw, 默认为structure')
     parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='浏览器类型: Chrome(default)|Firefox|Edge')
-    parser.add_argument('-l','--log',type=str,default='true',help='是否保存日志, true(default)|false')
     parser.add_argument('-save','--save_path',type=str,default='data',help='文件保存路径, 默认为当前目录的data文件夹')
     parser.add_argument('-wait','--wait_time',type=int,default=120,help='为检索预留的等待时间, 默认为120秒')
-    # parser.add_argument('--debug',action='store_false')
+    parser.add_argument('-l','--log',action='store_true',help="是否保存日志，指定该参数则保存日志，无需传值")
+    
     args = parser.parse_args()
     start_crawl(start_paper_index = args.start_paper_index,
                 end_paper_index = args.end_paper_index,
                 mode = args.mode,
                 save_path = args.save_path,
                 log = args.log,
                 wait_time = args.wait_time,
                 browser_type = args.browser_type,
-                )
-    
-if __name__ == '__main__':
-    main()
+                )
```

### Comparing `cnki_html2json-0.1.2/cnki_html2json/crawl.py` & `cnki_html2json-0.1.3/cnki_html2json/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,25 +104,25 @@
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
 
         
-def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',browser_type='Chrome',log='true',save_path='data',wait_time=120):
+def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',browser_type='Chrome',log=True,save_path='data',wait_time=120):
     """爬取cnki网站的论文
     start_paper_index: 开始爬取的论文索引，默认为1
     end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
     mode: 模式，structure|plain|raw，默认为structure
     save_path: 下载文件的保存路径，默认为当前目录的data文件夹
     log: 是否保存日志，默认为True
     wait_time: 为检索预留的等待时间，单位为秒
     browser_type: Chrome(默认)|Firefox|Edge|Safari
     """
-    if log=='true':
+    if log:
         if not os.path.exists(f'{save_path}/log'):
             os.makedirs(f'{save_path}/log')
             logger.info(f'已在{save_path}文件夹下创建log文件夹')
 
         current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
         logger.add(f"{save_path}/log/{current_time}.log",format="{time} {level} {message}",level="INFO",mode='w')
         logger.info('本次任务记录日志')
```

### Comparing `cnki_html2json-0.1.2/cnki_html2json/html2json.py` & `cnki_html2json-0.1.3/cnki_html2json/html2json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 # -*- coding: utf-8 -*-
-from lxml import html
 import re
 import json
+import os
+from lxml import html
 
-def extract_nodes(long_nodes_list:list,short_nodes_list:list):
+def _extract_nodes(long_nodes_list:list,short_nodes_list:list):
 	"""提取两个节点列表的差集"""
 	if short_nodes_list:
 		result = []
 		for node in long_nodes_list:
 			if node not in short_nodes_list:
 				result.append(node)
 			else:
 				return result
 	else:
 		return long_nodes_list
 
-def concat_nodes_value(nodes_list,task:str):
+def _concat_nodes_value(nodes_list,task:str):
 	"""合并节点列表的值"""
 
-	if nodes_list:
-		if task == 'citation':
+	if task == 'reference':
+		if nodes_list:
 			try:
 				result = sorted({int(i) for i in [node.text for node in nodes_list if node.text is not None]})
 			except ValueError:
 				result = sorted({int(i) for i in [eval(node.text)[0] for node in nodes_list if node.text is not None]})
 			return result
-		
 		else:
+			return []
+	
+	else:
+		if nodes_list:
 			result = ' '.join([node.text.strip() for node in nodes_list if node.text is not None])
 			return result.strip()
-	return None
+		else:
+			return ''
 
-def process_level_2_chapter(level_2_chapter:list):
-	"""处理第二级章节标题"""
+def _process_level_2_chapter(level_2_chapter:list):
+	"""处理二级章节标题"""
 	chapters = []
-	unnormal_chapters = {}
+	unusual_chapters = {}
 	for idx, chapter in enumerate(level_2_chapter):
 		if re.match(r'^\d{1}[\.．]{1}\d{1}\.?\d?\s*\w+',chapter):
 			chapters.append(chapter)
 		elif re.match(r'^\d{1}[\.．]{1}\d{1}\.?\d?\s*$',chapter):
 			chapters.append(level_2_chapter[idx+1])
-			unnormal_chapters[chapter] = level_2_chapter[idx+1]
-	return chapters, unnormal_chapters
+			unusual_chapters[chapter] = level_2_chapter[idx+1]
+	return chapters, unusual_chapters
 
-def process_level_1_chapter(level_1_chapter:list):
-	"""处理第一级章节标题"""
+def _process_level_1_chapter(level_1_chapter:list):
+	"""处理一级章节标题"""
 	chapters = []
-	unnormal_chapters = {}
+	unusual_chapters = {}
+	other_chapters = []
 	for idx, chapter in enumerate(level_1_chapter):
 		if re.match(r'^[0-9一二三四五六七八九][\s\.、．]*\D*[\u4e00-\u9fa5]+',chapter):
 			chapters.append(chapter)
 		elif re.match(r'^[0-9一二三四五六七八九][\s\.、．]*[^\u4e00-\u9fa5]*',chapter):
 			chapters.append(level_1_chapter[idx+1])
-			unnormal_chapters[chapter] = level_1_chapter[idx+1]
+			unusual_chapters[chapter] = level_1_chapter[idx+1]
 		elif re.match('作者贡献声明|利益冲突声明|参考文献|注释',chapter):
-			chapters.append(chapter)
+			other_chapters.append(chapter)
+	
 	# 去重
-	chapters_ = []
-	for i in chapters:
-		if i not in chapters_:
-			chapters_.append(i)
-	return chapters_, unnormal_chapters
+	# chapters_ = []
+	# for i in chapters:
+	# 	if i not in chapters_:
+	# 		chapters_.append(i)
+	return chapters, unusual_chapters, other_chapters
 
-class ExtractContent:
+class _ExtractContent:
 	"""提取文献内容"""
 
 	def __init__(self,resp_content:str,mode:str="structure") -> None:
 
 		"""
 		resp_content: html字符串
 		mode: structure:提取结构化文本(默认); plain:提取纯文本; raw:原生格式，会在正文中保留参考文献文献的索引
@@ -74,256 +81,257 @@
 		self.content = resp_content
 		# self.content = resp_content.replace('<!DOCTYPE html>','').strip()
 		self.html_general = html.fromstring(self.content)
 		
 		if mode != "raw":
 			self.html_text = html.fromstring(re.sub('<citation.*?</citation>|<sup>.*?</sup>|<i>.*?</i>','',self.content,flags=re.S))
 		
-		elif mode == "raw":
+		else:
 			# 匹配并替换
 			pattern = r'<citation.*?>.*?</citation>'
 			content_ = self.content
 
 			# 网页请求的源码
 			if content_.split('\n',1)[0] == '<!DOCTYPE html>': 
-				for match in re.findall(pattern, self.content,flags=re.S):
+				for match in re.findall(pattern, content_,flags=re.S):
 					match_result = '{}'.format([int(i) for i in re.findall(r'<a class="sup">(\d+)</a>',match)])
 					content_ = content_.replace(match, match_result)
 			
 			# 使用driver.page_source获取的源码
 			else: 
-				for match in re.findall(pattern, self.content,flags=re.S):
+				for match in re.findall(pattern, content_,flags=re.S):
 					match_result = '{}'.format([int(i) for i in re.findall(r'href="javascript:void\(0\);">(\d+)</a>',match,flags=re.S)])
 					content_ = content_.replace(match, match_result)
 				
 			self.html_text = html.fromstring(re.sub(r'<sup>.*?</sup>|<i>.*?</i>','',content_,flags=re.S))
 
 		self.error = False
-		self.annotation = False
+		# self.annotation = False
 		self.no_structure = False
 		self.prefix = False
 		self.mode = mode
 		
 		try:
-			level_1_chapter:list = self.html_general.xpath('//h3//text()')
-			self.level_1_chapter,self.unnormal_level_1_chapter = process_level_1_chapter(level_1_chapter)
-			if self.unnormal_level_1_chapter:
-				self.unnoraml_level_1_chapter_reverse = {v:k for k,v in self.unnormal_level_1_chapter.items()}
+			raw_level_1_chapter:list = self.html_general.xpath('//h3//text()')
+			self.main_level_1_chapter,self.unusual_level_1_chapter,self.other_level_1_chapter = _process_level_1_chapter(raw_level_1_chapter)
+			self.level_1_chapter = self.main_level_1_chapter+self.other_level_1_chapter
+			if self.unusual_level_1_chapter:
+				self.unusual_level_1_chapter_reverse = {v:k for k,v in self.unusual_level_1_chapter.items()}
 			
 		except AttributeError:
 			self.error = True
 		
 		else:
 			# 判断是否是正常文章
 			if "参考文献" not in self.level_1_chapter:
 				self.error = True
 			
 		if not self.error:
-
 			self.level_1_chapter_num = len(self.level_1_chapter)
-
-			original_level_2_chapter:list = self.html_general.xpath('//h4//text()')
-			self.level_2_chapter,self.unnormal_level_2_chapter = process_level_2_chapter(original_level_2_chapter)
+			raw_level_2_chapter:list = self.html_general.xpath('//h4//text()')
+			self.level_2_chapter,self.unusual_level_2_chapter = _process_level_2_chapter(raw_level_2_chapter)
 
 			self.text = {}
-			
 			# 判断是否存在没有章节标题的前言
 			if prefix := self.html_text.xpath('//h3[1]/preceding-sibling::div[@class="p1"]/p'):
-				prefix_text = concat_nodes_value(prefix,'text')
-				prefix_citaion_index = concat_nodes_value(
-					self.html_general.xpath('//h3[1]/preceding-sibling::div[@class="p1"]/p/citation/sup/a'),'citation')
-				self.text = {'0':{'citation':prefix_citaion_index,'text':prefix_text}}
+				prefix_text = _concat_nodes_value(prefix,'text')
+				prefix_citaion_index = _concat_nodes_value(
+					self.html_general.xpath('//h3[1]/preceding-sibling::div[@class="p1"]/p/reference/sup/a'),'reference')
+				self.text = {'0':{'reference':prefix_citaion_index,'text':prefix_text}}
 				self.prefix=True
 
 			# 处理没有篇章结构的文章
 			if self.level_1_chapter_num==0:
 				prefix_ = self.html_text.xpath('//div[@class="brief"][last()]/following-sibling::div[@class="p1"]/p')
 				if prefix_:
-					prefix_text = concat_nodes_value(prefix_,'text')
-					prefix_citaion_index = concat_nodes_value(
-						self.html_general.xpath('//div[@class="brief"][last()]/following-sibling::div[@class="p1"]/p/citation/sup/a'),'citation')
-					self.text = {'0':{'citation':prefix_citaion_index,'text':prefix_text}}
+					prefix_text = _concat_nodes_value(prefix_,'text')
+					prefix_citaion_index = _concat_nodes_value(
+						self.html_general.xpath('//div[@class="brief"][last()]/following-sibling::div[@class="p1"]/p/reference/sup/a'),'reference')
+					self.text = {'0':{'reference':prefix_citaion_index,'text':prefix_text}}
 					self.no_structure = True
 			
 			self.text |= {k:{} for k in self.level_1_chapter if k!='参考文献'}
-	
-	def generate_xpath(self,chapter_name:str,chapter_class:int,task:str,add_b_label = False,add_font_label=False):
+
+	def __generate_xpath(self,chapter_name:str,chapter_class:int,task:str,add_b_label = False,add_font_label=False)->str:
 		"""生成xpath
-		:param chapter_name: 章节名称
-		:param chapter_class: 章节等级,取1或2
+		param chapter_name: 章节名称
+		param chapter_class: 章节等级，取1或2
 		"""
 
 		if add_font_label==True:
 			xpath_ = f'//h{chapter_class+2}/font[text()="{chapter_name}"]/../following-sibling::div/p/font'
-			if task == 'citation':
+			if task == 'reference':
 				xpath_ += '/citation/sup/a'
 			return xpath_
 		
 		elif add_b_label==True:
 			xpath_ = f'//h{chapter_class+2}/b[text()="{chapter_name}"]/../following-sibling::div/p'
-			if task == 'citation':
+			if task == 'reference':
 				xpath_ += '/citation/sup/a'
 			return xpath_
 		
 		else:
 			xpath_ = f'//h{chapter_class+2}[text()="{chapter_name}"]/following-sibling::div/p'
-			if task == 'citation':
+			if task == 'reference':
 				xpath_ += '/citation/sup/a'
 			return xpath_
 		
-	def obtain_nodes_list(self,chapter_name:str,chapter_class:int,task:str):
+	def __obtain_nodes_list(self,chapter_name:str,chapter_class:int,task:str):
 		"""获取节点列表，依次尝试三种xpath表达式"""
 		
 		if task == 'text':
-			self.html = self.html_text
-		elif task == 'citation':
-			self.html = self.html_general
+			html = self.html_text
+		else:
+			html = self.html_general
 
-		xpath_expression = self.generate_xpath(chapter_name,chapter_class,task)
-		if result:=self.html.xpath(xpath_expression):
+		xpath_expression = self.__generate_xpath(chapter_name,chapter_class,task)
+		if result:= html.xpath(xpath_expression):
 			return result
 		
 		else:
-			xpath_expression = self.generate_xpath(chapter_name,chapter_class,task,add_b_label=True)
-			if result:=self.html.xpath(xpath_expression):
+			xpath_expression = self.__generate_xpath(chapter_name,chapter_class,task,add_b_label=True)
+			if result:=html.xpath(xpath_expression):
 				return result
 		
 			else:
-				xpath_expression = self.generate_xpath(chapter_name,chapter_class,task,add_font_label=True)
-				return self.html.xpath(xpath_expression)
+				xpath_expression = self.__generate_xpath(chapter_name,chapter_class,task,add_font_label=True)
+				return html.xpath(xpath_expression)
 	
 	def extract_plain_text(self):
-		
 		"""提取纯文本"""
+
 		if self.no_structure:
-			return self.text['0']['text'] # type: ignore
+			return self.text['0']['text'] # type:ignore
 		
 		else:
-			total_nodes_list = self.obtain_nodes_list(self.level_1_chapter[0],1,'text')
-			total_text = concat_nodes_value(total_nodes_list,'text')
+			total_nodes_list = self.__obtain_nodes_list(self.main_level_1_chapter[0],1,'text')
+			other_nodes_list = self.__obtain_nodes_list(self.other_level_1_chapter[0],1,'text')
+			valid_nodes_list = _extract_nodes(total_nodes_list,other_nodes_list)
+			total_text = _concat_nodes_value(valid_nodes_list,'text')
 			
 			if self.prefix:
 				return self.text['0']['text']+' '+total_text # type:ignore
 			else:
 				return total_text
 
 	def __extract(self,task:str)->None:
 		
 		if self.error:
 			self.text = None
 			return None
 		
 		offset = 1
-		if not self.annotation and "注释" in self.level_1_chapter:
+		# if not self.annotation and "注释" in self.level_1_chapter:
+		if "注释" in self.level_1_chapter:
 			offset = 2
 
+		end_idx = self.level_1_chapter_num-offset
+		if task == 'reference':
+			end_idx = self.level_1_chapter_num-len(self.other_level_1_chapter)
+		
 		idx = 0
-		while idx < self.level_1_chapter_num-offset:
-			first_nodes_list = self.obtain_nodes_list(self.level_1_chapter[idx],1,task)
-			second_nodes_list = self.obtain_nodes_list(self.level_1_chapter[idx+1],1,task)
+		while idx < end_idx:
+			first_nodes_list = self.__obtain_nodes_list(self.level_1_chapter[idx],1,task)
+			second_nodes_list = self.__obtain_nodes_list(self.level_1_chapter[idx+1],1,task)
 
 			# 筛选出二级章节
 			current_node_idx = self.level_1_chapter[idx].strip()[0]
 			
 			if current_node_idx in list('123456789'):
 				current_level_2_chapter_list = [i for i in self.level_2_chapter if i[0]==current_node_idx]
-				if self.unnormal_level_2_chapter:
-					current_level_2_chapter_list += [self.unnormal_level_2_chapter[i] for i in self.unnormal_level_2_chapter if i[0]==current_node_idx]
+				if self.unusual_level_2_chapter:
+					current_level_2_chapter_list += [self.unusual_level_2_chapter[i] for i in self.unusual_level_2_chapter if i[0]==current_node_idx]
 			else:
 				current_level_2_chapter_list = []
 			
 			if current_level_2_chapter_list:
 				
 				text_ = {}
 				current_level_2_chapter_num = len(current_level_2_chapter_list)
 				idx_ = 0
 				while idx_ < current_level_2_chapter_num:
-					first_nodes_list_ = self.obtain_nodes_list(current_level_2_chapter_list[idx_],2,task)
+					first_nodes_list_ = self.__obtain_nodes_list(current_level_2_chapter_list[idx_],2,task)
 		
 					if idx_ == current_level_2_chapter_num-1:
 						second_nodes_list_ = second_nodes_list
 
 					else:
-						second_nodes_list_ = self.obtain_nodes_list(current_level_2_chapter_list[idx_+1],2,task)
+						second_nodes_list_ = self.__obtain_nodes_list(current_level_2_chapter_list[idx_+1],2,task)
 			
 					if idx_ == 0:
-						following_node_ = extract_nodes(first_nodes_list,first_nodes_list_)
-						text_[current_node_idx+'.0'] = concat_nodes_value(following_node_,task)
+						following_node_ = _extract_nodes(first_nodes_list,first_nodes_list_)
+						text_[current_node_idx+'.0'] = _concat_nodes_value(following_node_,task)
 
-					current_node_ = extract_nodes(first_nodes_list_,second_nodes_list_)
+					current_node_ = _extract_nodes(first_nodes_list_,second_nodes_list_)
 
 					current_level_2_chapter = current_level_2_chapter_list[idx_]
-					unnoraml_level_2_chapter_reverse = {v:k for k,v in self.unnormal_level_2_chapter.items()}
+					unusual_level_2_chapter_reverse = {v:k for k,v in self.unusual_level_2_chapter.items()}
 
-					if current_level_2_chapter in unnoraml_level_2_chapter_reverse:
-						text_[unnoraml_level_2_chapter_reverse[current_level_2_chapter]+current_level_2_chapter] = concat_nodes_value(current_node_,task)
+					if current_level_2_chapter in unusual_level_2_chapter_reverse:
+						text_[unusual_level_2_chapter_reverse[current_level_2_chapter]+current_level_2_chapter] = _concat_nodes_value(current_node_,task)
 					else:
-						text_[current_level_2_chapter_list[idx_]] = concat_nodes_value(current_node_,task)
+						text_[current_level_2_chapter_list[idx_]] = _concat_nodes_value(current_node_,task)
 
 					idx_ += 1
 				self.text[self.level_1_chapter[idx]][task] = text_ # type: ignore
 
 			else:
-				current_node_ = extract_nodes(first_nodes_list,second_nodes_list)
+				current_node_ = _extract_nodes(first_nodes_list,second_nodes_list)
 				current_level_1_chapter = self.level_1_chapter[idx]
 
-				self.text[current_level_1_chapter][task] = concat_nodes_value(current_node_,task) # type: ignore
-		
+				self.text[current_level_1_chapter][task] = _concat_nodes_value(current_node_,task) # type: ignore
 			idx += 1
 
-	def extract_citation_index(self):
+	def extract_reference_index(self):
 		"""提取章节引用的文献索引"""
 
-		self.__extract(task='citation')
+		self.__extract(task='reference')
 		return self.text
 	
 	def extract_text(self):
 		"""提取正文"""
 		
 		self.__extract(task='text')
 		return self.text
 
-	def extract_citation(self):
+	def extract_reference(self):
 		"""提取参考文献"""
-		citation = [doc.strip() for doc in self.html_general.xpath('//div[@id="a_bibliography"]/p/a/text()') if doc.strip()!='']
-		citation_with_index = [f'[{idx}] '+re.sub(r'^[\.]+','',doc).strip() for idx,doc in enumerate(citation,1)]
-		return citation_with_index
+		reference = [doc.strip() for doc in self.html_general.xpath('//div[@id="a_bibliography"]/p/a/text()') if doc.strip()!='']
+		reference_with_index = [f'[{idx}] '+re.sub(r'^[\.]+','',doc).strip() for idx,doc in enumerate(reference,1)]
+		return reference_with_index
 
 	def extract_all(self)->dict:
 		"""提取全部"""
 		if self.error:
 			return {'body_text':None,'参考文献':None}
 		
 		result = {}
-		citing_docs = self.extract_citation()
+		citing_docs = self.extract_reference()
 		if self.mode != 'plain':
-			self.extract_citation_index()
+			self.extract_reference_index()
 			self.extract_text()
 			result = {'body_text':self.text}
 		
 		elif self.mode == 'plain':
 			result = {'body_text':self.extract_plain_text()}
 		
-		# result |= {'参考文献':citing_docs}
 		return {**result,**{'参考文献':citing_docs}}
-	
-# 设置公开的接口
-def export_json(text,json_path):
-    """导出json文件"""
-    with open(json_path,'w',encoding='utf-8') as f:
-        json.dump(text,f,ensure_ascii=False,indent=4)
-
-def extract(paper_html:str,mode:str='structure',export=False,export_path=None):
-    """将论文的html字符串转换为字典
-    paper_html: 论文的html字符串
-    mode: 模式，structure|plain|raw，默认为structure
-    export: 是否导出json文件，默认为False
-    export_path: 导出json文件的路径，默认为None，如果导出json文件，该参数必须指定
-    """
-    result = ExtractContent(paper_html,mode).extract_all()
-    if not export:
-        return result
-    else:
-        if export_path is None:
-            raise ValueError('请设置导出参数')
-        else:
-            export_json(result,export_path)
+
+def __export_json(text,json_path):
+	"""导出json文件"""
+	folder_path = os.path.dirname(json_path)
+	if not os.path.exists(folder_path):
+		os.makedirs(folder_path)
+	with open(json_path,'w',encoding='utf-8') as f:
+		json.dump(text,f,ensure_ascii=False,indent=4)
+
+def extract(paper_html:str,mode:str='structure',export_path=None):
+	"""将论文的html字符串转换为字典
+	paper_html: 论文的html字符串
+	mode: 模式，structure|plain|raw，默认为structure
+	export_path: 导出json文件的路径，默认为None，如果导出json文件，该参数必须指定
+	"""
+	result = _ExtractContent(paper_html,mode).extract_all()
+	if not export_path:
+		return result
+	else:
+		__export_json(result,export_path)
```

### Comparing `cnki_html2json-0.1.2/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.3/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.2/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.3/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.2/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.3/cnki_html2json.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,102 +22,98 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签
+- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
 
-核心功能：
-- 从文献的html字符串中解析出包含两级子章节标题的结构化文本
-- 实现了一个基于selenium的爬虫，可以批量获取所需文献的结构化文本
-- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本
-  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引
-  - 以上三种模式都包含参考文献文献，可以参考examples文件夹中给出的样例
-
-使用场景：
-- 对中文期刊论文进行全文获取和分析，为下游任务提供支持
-- 对中文期刊论文进行引文分析
+核心功能：¥
+- 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
+- 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
+- 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
+  - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
+  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+
+<!-- 使用场景：
+- 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
+- 对中文期刊论文进行引文分析； -->
 
 使用限制：
-- 确保你所在的网络环境能正常使用知网
-- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整
-- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取
+- 确保你所在的网络环境能正常使用知网；
+- 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
+- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
-
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
-$ python3 -m pip install cnki_html2json
+$ pip install cnki_html2json
 ```
 
 ## 使用方法
-
 1、调用 `html2json` 函数
 
 ```python
 from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
     html = f.read()
 print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
-| `export` | 是否导出，默认 `False` |
-| `export_path` | 保存结果的路径，默认为 `None` ，如果 `export` 设置为 `True`，该参数必须指定 |
+| `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
-> 函数返回值说明：参考examples文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
+> 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
 $ cnki-crawler
 ```
 ```console
-$ 设置论文提取的起始索引和终止索引，模式设置为structure，不记录日志
-$ cnki-crawler -s 1 -e 100 -m structure -l false
+$ 设置论文提取的起始索引和终止索引，模式设置为structure，记录日志
+$ cnki-crawler -s 1 -e 100 -m structure -l
 $ 或者是
-$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log false
+$ cnki-crawler --start_paper_index 1 --end_paper_index 100 -mode structure --log
 ```
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
-参数说明：
+命令行工具参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
-| s | `start_paper_index` | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
-| e | `end_paper_index` | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| m | `mode` | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| b | `browser` | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| l | `log` | 是否记录日志，默认为 `true`，日志将保存在 `save_path` 下的 `log` 文件夹中 |
-| save | `save_path` | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
-| wait | `wait_time` | 为检索预留的等待时间，默认 `120` 秒 |
+| -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
+| -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
+| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
+| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下;  
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log='false')
+start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
 ```
 
 ## json文件字段说明
-
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
 |  | authors |  |论文作者|
 |  | orgs |  |作者所属机构|
 |  | abstract |  |论文摘要|
 |  | keywords |  |论文关键词|
@@ -127,16 +123,9 @@
 |  | issue |  |发表刊号|
 | body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
 |  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |citation对应本章节的参考文献索引；text对应本章节的文本|
 |  | 2.xxx | 2.1xxx ||
 |  | ...| ... ||
 | 参考文献 |  |  |参考文献|
 
-## 工具推荐
-
-| 工具  | 描述 |
-| --- | --- |
-| [vermin](https://github.com/netromdk/vermin) | 从语法层面检测一个项目最低支持的 `Python` 版本 |
-
-## 责任声明
-
-- 使用者使用本工具造成的一切后果，由使用者自行承担
+## 开源协议
+本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.2/setup.py` & `cnki_html2json-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.2",
+    version="0.1.3",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.2/tests/test_html2json.py` & `cnki_html2json-0.1.3/tests/test_html2json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from cnki_html2json import html2json
 
 def test_html2json():
-    with open('test/fulltext.html','r') as f:
+    with open('tests/fulltext.html','r') as f:
         content = f.read()
 
-    text_structure = html2json.ExtractContent(content,'structure').extract_all()
-    assert text_structure['body_text']['1 引言']['text'][:3] == "近年来"
+    text_structure = html2json._ExtractContent(content,'structure').extract_all()
+    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT('
+    assert text_structure['body_text']['1 引言']['reference'][0]==1
 
-    text_plain = html2json.ExtractContent(content,'plain').extract_all()
-    assert text_plain['body_text'][:3] == "近年来"
+    text_plain = html2json._ExtractContent(content,'plain').extract_all()
+    assert text_plain['body_text'][:14] == '近年来，以Chat GPT('
 
-    text_raw = html2json.ExtractContent(content,'raw').extract_all()
+    text_raw = html2json._ExtractContent(content,'raw').extract_all()
     assert '[1]' in text_raw['body_text']['1 引言']['text']
```


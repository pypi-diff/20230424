# Comparing `tmp/damo-1.7.7.tar.gz` & `tmp/damo-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.7.7.tar", last modified: Mon Apr 17 21:31:34 2023, max compression
+gzip compressed data, was "damo-1.7.8.tar", last modified: Mon Apr 24 21:50:35 2023, max compression
```

## Comparing `damo-1.7.7.tar` & `damo-1.7.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.149330 damo-1.7.7/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-17 21:31:34.149330 damo-1.7.7/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5998 2023-04-17 21:31:29.000000 damo-1.7.7/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-17 21:31:29.000000 damo-1.7.7/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-17 21:31:34.149330 damo-1.7.7/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-17 21:31:29.000000 damo-1.7.7/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.133331 damo-1.7.7/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.145331 damo-1.7.7/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    33489 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9973 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8196 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17739 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17620 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19529 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1619 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1531 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3268 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      681 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      651 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-17 21:31:29.000000 damo-1.7.7/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-17 21:31:34.149330 damo-1.7.7/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-17 21:31:34.000000 damo-1.7.7/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.804108 damo-1.7.8/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6881 2023-04-24 21:50:35.804108 damo-1.7.8/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6360 2023-04-24 21:50:31.000000 damo-1.7.8/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-24 21:50:31.000000 damo-1.7.8/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-24 21:50:35.804108 damo-1.7.8/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-24 21:50:31.000000 damo-1.7.8/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.788109 damo-1.7.8/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.800108 damo-1.7.8/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    33096 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17917 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17878 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18889 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3289 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.800108 damo-1.7.8/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6881 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.7.7/PKG-INFO` & `damo-1.7.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: damo
-Version: 1.7.7
-Summary: DAMON user-space tool
-Home-page: https://github.com/awslabs/damo
-Author: SeongJae Park
-Author-email: sj@kernel.org
-Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
-Project-URL: DAMON, https://damonitor.github.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -42,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -102,14 +87,22 @@
 -----------------------------------------------------------------------------
 
 Because the DAMOS input you're using is no more supported.  Please report your
 usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
 depend on those.
 
 
+damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
+----------------------------------------------------------------------------------------
+
+Because the single line DAMOS scheme format is no more supported.  Please
+report your usecase to sj@kernel.org, damon@lists.linux.dev and
+linux-mm@kvack.org if you depend on those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
```

### Comparing `damo-1.7.7/README.md` & `damo-1.7.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 1.7.8
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -27,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,14 +102,22 @@
 -----------------------------------------------------------------------------
 
 Because the DAMOS input you're using is no more supported.  Please report your
 usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
 depend on those.
 
 
+damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
+----------------------------------------------------------------------------------------
+
+Because the single line DAMOS scheme format is no more supported.  Please
+report your usecase to sj@kernel.org, damon@lists.linux.dev and
+linux-mm@kvack.org if you depend on those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
```

### Comparing `damo-1.7.7/setup.py` & `damo-1.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.7.7",
+    version="1.7.8",
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.7.7/src/damo/_damo_dist.py` & `damo-1.7.8/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damo_fmt_str.py` & `damo-1.7.8/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damo_fs.py` & `damo-1.7.8/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damo_paddr_layout.py` & `damo-1.7.8/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damo_python2_support.py` & `damo-1.7.8/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damo_subcmds.py` & `damo-1.7.8/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/_damon.py` & `damo-1.7.8/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,21 +134,21 @@
     def to_kvpairs(self, raw=False):
         kvp = collections.OrderedDict()
         kvp['pid'] = self.pid
         kvp['regions'] = [r.to_kvpairs(raw) for r in self.regions]
         return kvp
 
 unit_percent = 'percent'
-unit_sample_intervals = 'sample_intervals'
+unit_samples = 'samples'
 unit_usec = 'usec'
 unit_aggr_intervals = 'aggr_intervals'
 
 class DamonIntervalsBasedValUnit:
     value = None
-    unit = None # percent, sample_intervals, usec, aggr_intervals
+    unit = None # percent, samples, usec, aggr_intervals
 
     def __init__(self, value, unit):
         self.value = value
         self.unit = unit
 
     def eq(self, other, intervals=None):
         if intervals == None:
@@ -158,30 +158,34 @@
 
     def __eq__(self, other):
         return self.eq(other, None)
 
     def value_for(self, new_unit, intervals):
         if self.unit == new_unit:
             return self.value
-        if self.unit == unit_sample_intervals and new_unit == unit_percent:
+        if self.unit == unit_samples and new_unit == unit_percent:
             max_val = intervals.aggr / intervals.sample
             return int(self.value * 100.0 / max_val)
-        elif self.unit == unit_percent and new_unit == unit_sample_intervals:
+        elif self.unit == unit_percent and new_unit == unit_samples:
             max_val = intervals.aggr / intervals.sample
             return int(self.value * max_val / 100)
         elif self.unit == unit_aggr_intervals and new_unit == unit_usec:
             return self.value * intervals.aggr
         elif self.unit == unit_usec and new_unit == unit_aggr_intervals:
             return int(self.value / intervals.aggr)
         raise Exception('unsupported unit change')
 
     def convert_unit(self, new_unit, intervals):
         self.value = self.value_for(new_unit, intervals)
         self.unit = new_unit
 
+    def converted_for_unit(self, new_unit, intervals):
+        return DamonIntervalsBasedValUnit(
+                self.value_for(new_unit, intervals), new_unit)
+
     def to_str(self, raw):
         unit = self.unit
 
         if unit == unit_usec:
             return _damo_fmt_str.format_time_us_exact(self.value, raw)
 
         if unit == unit_percent:
@@ -198,15 +202,15 @@
             nr_accesses=['min', 'max'], nr_accesses_unit=unit_percent,
             age=['min', 'max'], age_unit=unit_usec):
         self.sz_bytes = [_damo_fmt_str.text_to_bytes(sz_bytes[0]),
                 _damo_fmt_str.text_to_bytes(sz_bytes[1])]
 
         parsers_for_unit = {
                 unit_percent: _damo_fmt_str.text_to_percent,
-                unit_sample_intervals: _damo_fmt_str.text_to_nr,
+                unit_samples: _damo_fmt_str.text_to_nr,
                 unit_usec: _damo_fmt_str.text_to_us,
                 unit_aggr_intervals: _damo_fmt_str.text_to_nr}
 
         if not nr_accesses_unit in parsers_for_unit:
             raise Exception('invalid access pattern nr_accesses_unit \'%s\'' %
                     nr_accesses_unit)
         if not age_unit in parsers_for_unit:
@@ -302,17 +306,17 @@
         copied = copy.deepcopy(self)
         copied.convert_for_units(nr_accesses_unit, age_unit, intervals)
         return copied
 
     def effectively_equal(self, other, intervals):
         return (
                 self.converted_for_units(
-                    unit_sample_intervals, unit_aggr_intervals, intervals) ==
+                    unit_samples, unit_aggr_intervals, intervals) ==
                 other.converted_for_units(
-                    unit_sample_intervals, unit_aggr_intervals, intervals))
+                    unit_samples, unit_aggr_intervals, intervals))
 
 class DamosQuotas:
     time_ms = None
     sz_bytes = None
     reset_interval_ms = None
     weight_sz_permil = None
     weight_nr_accesses_permil = None
@@ -495,36 +499,34 @@
         return self.to_str(False)
 
 class DamosTriedRegion:
     start = None
     end = None
     nr_accesses = None
     age = None
-    age_unit = None
 
-    def __init__(self, start, end, nr_accesses, age, age_unit):
+    def __init__(self, start, end, nr_accesses, nr_accesses_unit,
+            age, age_unit):
         self.start = start
         self.end = end
-        self.nr_accesses = nr_accesses
-        self.age = age
-        self.age_unit = age_unit
+        self.nr_accesses = DamonIntervalsBasedValUnit(nr_accesses,
+                nr_accesses_unit)
+        self.age = DamonIntervalsBasedValUnit(age, age_unit)
 
     def to_str(self, raw, intervals=None):
-        age = self.age
         if raw == False and intervals != None:
-            max_nr_accesses = intervals.aggr / intervals.sample
-            nr_accesses = '%.2f%%' % (
-                    float(self.nr_accesses) * 100 / max_nr_accesses)
-            age = _damo_fmt_str.format_time_us(age * intervals.aggr, raw)
+            nr_accesses = self.nr_accesses.converted_for_unit(unit_percent,
+                    intervals)
+            age = self.age.converted_for_unit(unit_usec, intervals)
         else:
-            nr_accesses = '%s' % _damo_fmt_str.format_nr(self.nr_accesses, raw)
-            age = '%s %s' % (_damo_fmt_str.format_nr(age, raw), self.age_unit)
+            nr_accesses = self.nr_accesses
+            age = self.age
         return '%s: nr_accesses: %s, age: %s' % (
                 _damo_fmt_str.format_addr_range(self.start, self.end, raw),
-                nr_accesses, age)
+                nr_accesses.to_str(raw), age.to_str(raw))
 
     def __str__(self):
         return self.to_str(False)
 
 # TODO: check support of pageout and lru_(de)prio
 damos_actions = [
         'willneed',
@@ -639,17 +641,14 @@
         return (type(self) == type(other) and
                 self.access_pattern.effectively_equal(
                     other.access_pattern, intervals) and
                 self.action == other.action and self.quotas == other.quotas and
                 self.watermarks == other.watermarks and
                 self.filters == other.filters)
 
-def is_monitoring_scheme(scheme, intervals):
-    return Damos().effectively_equal(scheme, intervals)
-
 class DamonRecord:
     rfile_buf = None
     rfile_path = None
 
     def __init__(self, rfile_buf, rfile_path):
         self.rfile_buf = _damo_fmt_str.text_to_bytes(rfile_buf)
         self.rfile_path = rfile_path
@@ -800,15 +799,15 @@
             'schemes_prioritization',   # merged in v5.16 (38683e003153)
             'schemes_wmarks',           # merged in v5.16 (ee801b7dd782)
             'schemes_stat_succ',        # merged in v5.17 (0e92c2ee9f45)
             'schemes_stat_qt_exceed',   # merged in v5.17 (0e92c2ee9f45)
             'init_regions_target_idx',  # merged in v5.18 (144760f8e0c3)
             'fvaddr',       # merged in v5.19 (b82434471cd2)
             'schemes_tried_regions',    # merged in v6.2-rc1
-            'schemes_filters',          # merged in mm-unstable
+            'schemes_filters',          # merged in v6.3-rc1
             'schemes_tried_regions_sz', # developing
             ]
 
 _damon_fs = None
 
 pr_debug_log = False
 
@@ -859,93 +858,85 @@
         return 'sysfs'
     elif _damon_fs == _damon_dbgfs:
         return 'debugfs'
     raise Exception('_damo_fs is neither _damon_sysfs nor _damon_dbgfs')
 
 # DAMON status reading
 
-def is_kdamond_running(kdamond_name):
-    return _damon_fs.is_kdamond_running(kdamond_name)
+def is_kdamond_running(kdamond_idx):
+    return _damon_fs.is_kdamond_running(kdamond_idx)
 
 def current_kdamonds():
     return _damon_fs.current_kdamonds()
 
-def current_kdamond_names():
-    return _damon_fs.current_kdamond_names()
-
-def running_kdamonds():
-    return [k for k in current_kdamonds() if k.state == 'on']
+def nr_current_kdamonds():
+    return _damon_fs.nr_current_kdamonds()
 
-def running_kdamond_names():
-    return [name for name in current_kdamond_names()
-            if is_kdamond_running(name)]
+def running_kdamond_idxs():
+    return [idx for idx in range(nr_current_kdamonds())
+            if is_kdamond_running(idx)]
 
 def any_kdamond_running():
-    for kd_name in current_kdamond_names():
-        if is_kdamond_running(kd_name):
+    for idx in range(nr_current_kdamonds()):
+        if is_kdamond_running(idx):
             return True
     return False
 
-def every_kdamond_turned_off():
-    return not any_kdamond_running()
-
 def wait_current_kdamonds_turned_on():
-    for kd_name in current_kdamond_names():
-        while not is_kdamond_running(kd_name):
+    for idx in range(nr_current_kdamonds()):
+        while not is_kdamond_running(idx):
             time.sleep(1)
 
 def wait_current_kdamonds_turned_off():
-    for kd_name in current_kdamond_names():
-        while is_kdamond_running(kd_name):
+    for idx in range(nr_current_kdamonds()):
+        while is_kdamond_running(idx):
             time.sleep(1)
 
 # DAMON control
 
 def stage_kdamonds(kdamonds):
     return _damon_fs.stage_kdamonds(kdamonds)
 
-def commit_staged(kdamond_names):
+def commit_staged(kdamond_idxs):
     if _damon_fs == _damon_dbgfs:
         return 'debugfs interface unsupport commit_staged()'
-    return _damon_fs.commit_staged(kdamond_names)
+    return _damon_fs.commit_staged(kdamond_idxs)
 
 def commit(kdamonds):
     err = stage_kdamonds(kdamonds)
     if err:
         return 'staging updates failed (%s)' % err
     err = commit_staged(['%s' % idx for idx, k in enumerate(kdamonds)])
     if err:
         return 'commit staged updates filed (%s)' % err
     return None
 
-def update_schemes_stats(kdamond_names=None):
-    if kdamond_names == None:
-        kdamond_names = running_kdamond_names()
-    return _damon_fs.update_schemes_stats(kdamond_names)
-
-def update_schemes_tried_regions(kdamond_names=None):
-    if kdamond_names == None:
-        kdamond_names = running_kdamond_names()
-    if _damon_fs == _damon_dbgfs:
-        return 'DAMON debugfs doesn\'t support schemes tried regions'
-    return _damon_fs.update_schemes_tried_regions(kdamond_names)
+def update_schemes_stats(kdamond_idxs=None):
+    if kdamond_idxs == None:
+        kdamond_idxs = running_kdamond_idxs()
+    return _damon_fs.update_schemes_stats(kdamond_idxs)
+
+def update_schemes_tried_regions(kdamond_idxs=None):
+    if kdamond_idxs == None:
+        kdamond_idxs = running_kdamond_idxs()
+    return _damon_fs.update_schemes_tried_regions(kdamond_idxs)
 
 def update_schemes_status():
-    names = running_kdamond_names()
-    if len(names) == 0:
+    idxs = running_kdamond_idxs()
+    if len(idxs) == 0:
         return None
-    err = update_schemes_stats(names)
+    err = update_schemes_stats(idxs)
     if err != None:
         return err
-    return update_schemes_tried_regions(names)
+    return update_schemes_tried_regions(idxs)
 
-def turn_damon_on(kdamonds_names):
-    err = _damon_fs.turn_damon_on(kdamonds_names)
+def turn_damon_on(kdamonds_idxs):
+    err = _damon_fs.turn_damon_on(kdamonds_idxs)
     if err:
         return err
     wait_current_kdamonds_turned_on()
 
-def turn_damon_off(kdamonds_names):
-    err = _damon_fs.turn_damon_off(kdamonds_names)
+def turn_damon_off(kdamonds_idxs):
+    err = _damon_fs.turn_damon_off(kdamonds_idxs)
     if err:
         return err
     wait_current_kdamonds_turned_off()
```

### Comparing `damo-1.7.7/src/damo/_damon_args.py` & `damo-1.7.8/src/damo/_damon_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 def kdamonds_from_json_arg(arg):
     try:
         if os.path.isfile(arg):
             with open(arg, 'r') as f:
                 kdamonds_str = f.read()
         else:
             kdamonds_str = arg
-        kdamonds_kvpairs = json.loads(kdamonds_str)
+        kdamonds_kvpairs = json.loads(kdamonds_str)['kdamonds']
         return [kdamond.from_kvpairs(kvp) for kvp in kdamonds_kvpairs], None
     except Exception as e:
         return None, e
 
 def deduce_target_update_args(args):
     args.self_started_target = False
     if args.deducible_target == 'paddr':
```

### Comparing `damo-1.7.7/src/damo/_damon_args_schemes.py` & `damo-1.7.8/src/damo/_damon_args_schemes.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,18 +131,26 @@
     scheme.watermarks.interval_us = _damo_fmt_str.text_to_us(
             fields[14])
     scheme.watermarks.high_permil = int(fields[15])
     scheme.watermarks.mid_permil = int(fields[16])
     scheme.watermarks.low_permil = int(fields[17])
     return scheme
 
+avoid_crashing_single_line_scheme_for_testing = False
 avoid_crashing_v1_v3_schemes_for_testing = False
 def damo_single_line_scheme_to_damos(line):
     '''Returns Damos object and err'''
 
+    # Remove below if someone depends on single scheme is found.
+    if not avoid_crashing_single_line_scheme_for_testing:
+        sys.stderr.write('''
+You're using deprecated single line DAMOS format (%s)
+''' % line)
+        exit(1)
+
     sys.stderr.write('''
 WARNING: single line per-scheme scheme input is deprecated.  The support will
 be removed by 2023-Q2.  Please use json format or --damos_* commandline options
 instead.
 
 Please report your usecase to sj@kernel.org, damon@liss.linux.dev
 and linux-mm@kvack.org if you depend on it.
```

### Comparing `damo-1.7.7/src/damo/_damon_dbgfs.py` & `damo-1.7.8/src/damo/_damon_dbgfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 debugfs_attrs = os.path.join(debugfs_damon, 'attrs')
 debugfs_record = os.path.join(debugfs_damon, 'record')
 debugfs_schemes = os.path.join(debugfs_damon, 'schemes')
 debugfs_target_ids = os.path.join(debugfs_damon, 'target_ids')
 debugfs_init_regions = os.path.join(debugfs_damon, 'init_regions')
 debugfs_monitor_on = os.path.join(debugfs_damon, 'monitor_on')
 
-def turn_damon_on(kdamonds_names):
+def turn_damon_on(kdamonds_idxs):
     return _damo_fs.write_files({debugfs_monitor_on: 'on'})
 
-def turn_damon_off(kdamonds_names):
+def turn_damon_off(kdamonds_idxs):
     return _damo_fs.write_files({debugfs_monitor_on: 'off'})
 
-def is_kdamond_running(kdamond_name):
+def is_kdamond_running(kdamond_idx):
     content, err = _damo_fs.read_file(debugfs_monitor_on)
     if err != None:
         raise Exception('monitor_on file read failed: err')
     return content.strip() == 'on'
 
 'Return error'
-def update_schemes_stats(kdamond_names):
+def update_schemes_stats(kdamond_idxs):
     # DAMON debugfs updates stats always
     return None
 
-# update_schemes_tried_regions are not supported
+def update_schemes_tried_regions(kdamond_idxs):
+    return 'DAMON debugfs doesn\'t support schemes tried regions'
 
 # for stage_kdamonds
 
 def wops_for_target(target, target_has_pid):
     wops = []
     if target_has_pid:
         wops.append({debugfs_target_ids: '%s' % target.pid})
@@ -86,15 +87,15 @@
 def file_content_to_damos_wmarks_metric(metric_file_content):
     for metric_str in damos_wmark_metric_to_int:
         if damos_wmark_metric_to_int[metric_str] == metric_file_content:
             return metric_str
 
 def damos_to_debugfs_input(damos, intervals, scheme_version):
     pattern = damos.access_pattern.converted_for_units(
-            _damon.unit_sample_intervals, _damon.unit_aggr_intervals,
+            _damon.unit_samples, _damon.unit_aggr_intervals,
             intervals)
     quotas = damos.quotas
     watermarks = damos.watermarks
 
     max_nr_accesses = intervals.aggr / intervals.sample
     v0_scheme = '%d\t%d\t%d\t%d\t%d\t%d\t%s' % (
             pattern.sz_bytes[0], pattern.sz_bytes[1],
@@ -270,22 +271,23 @@
 def files_content_to_kdamonds(files_content):
     attrs = [int(x) for x in files_content['attrs'].strip().split()]
 
     intervals = _damon.DamonIntervals(attrs[0], attrs[1], attrs[2])
     nr_regions = _damon.DamonNrRegionsRange(attrs[3], attrs[4])
 
     target_ids = [int(x) for x in files_content['target_ids'].strip().split()]
-    fields = [int(x) for x in files_content['init_regions'].strip().split()]
     regions_dict = {}
-    for i in range(0, len(fields), 3):
-        id_or_index = fields[i]
-        if not id_or_index in regions_dict:
-            regions_dict[id_or_index] = []
-        regions_dict[id_or_index].append(_damon.DamonRegion(
-                fields[i + 1], fields[i + 2]))
+    if feature_supported('init_regions'):
+        fields = [int(x) for x in files_content['init_regions'].strip().split()]
+        for i in range(0, len(fields), 3):
+            id_or_index = fields[i]
+            if not id_or_index in regions_dict:
+                regions_dict[id_or_index] = []
+            regions_dict[id_or_index].append(_damon.DamonRegion(
+                    fields[i + 1], fields[i + 2]))
     ops = 'vaddr'
     is_paddr = False
     if 42 in target_ids:
         ops = 'paddr'
     targets = []
     for idx, target_id in enumerate(target_ids):
         targets.append(_damon.DamonTarget(
@@ -295,33 +297,34 @@
                 else target_id] if len(regions_dict) > 0 else []))
 
     if feature_supported('record'):
         fields = files_content['record'].strip().split()
         record_request = _damon.DamonRecord(int(fields[0]), fields[1].strip())
 
     schemes = []
-    for line in files_content['schemes'].split('\n'):
-        if line.strip() == '':
-            continue
-        schemes.append(debugfs_output_to_damos(line, intervals))
+    if feature_supported('schemes'):
+        for line in files_content['schemes'].split('\n'):
+            if line.strip() == '':
+                continue
+            schemes.append(debugfs_output_to_damos(line, intervals))
 
     ctx = _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
     if feature_supported('record'):
         ctx.record_request = record_request
     state = files_content['monitor_on'].strip()
     pid = files_content['kdamond_pid'].strip()
     return [_damon.Kdamond(state, pid, [ctx])]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(debugfs_damon))
 
-def current_kdamond_names():
-    # TODO: Support created kdamonds
-    return ['0']
+def nr_current_kdamonds():
+    # TODO: Support manually created kdamonds
+    return 1
 
 # features
 
 feature_supports = None
 
 def feature_supported(feature):
     if feature_supports == None:
```

### Comparing `damo-1.7.7/src/damo/_damon_result.py` & `damo-1.7.8/src/damo/_damon_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,76 +412,84 @@
     if file_format != 'perf_data':
         err = update_result_file(file_path, file_format)
         if err != None:
             print('converting format from perf_data to %s failed (%s)' %
                     (file_format, err))
     os.chmod(file_path, file_permission)
 
-def ensure_scheme_installed(kdamonds, scheme_to_install):
+def install_scheme(scheme_to_install):
+    '''Install given scheme to all contexts if effectively same scheme is not
+    installed.
+    Returns whether it found a context doesn't having the scheme, and an error
+    if something wrong.
+    '''
     installed = False
+    kdamonds = _damon.current_kdamonds()
     for kdamond in kdamonds:
         for ctx in kdamond.contexts:
             ctx_has_the_scheme = False
             for scheme in ctx.schemes:
                 if scheme.effectively_equal(scheme_to_install, ctx.intervals):
                     ctx_has_the_scheme = True
                     break
-            if not ctx_has_the_scheme:
-                ctx.schemes.append(scheme_to_install)
-                installed = True
+            if ctx_has_the_scheme:
+                continue
+            ctx.schemes.append(scheme_to_install)
+            installed = True
     if installed:
         err = _damon.commit(kdamonds)
         if err != None:
             return (False,
                     'committing scheme installed kdamonds failed: %s' % err)
     return installed, None
 
-def tried_regions_to_snapshot(tried_regions, aggr_interval_us):
+def tried_regions_to_snapshot(tried_regions, intervals):
     snapshot_end_time_ns = time.time() * 1000000000
-    snapshot_start_time_ns = snapshot_end_time_ns - aggr_interval_us * 1000
+    snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
     snapshot = DAMONSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
         snapshot.regions.append(DAMONRegion(tried_region.start,
-            tried_region.end, tried_region.nr_accesses,
-            tried_region.age * aggr_interval_us,
+            tried_region.end,
+            tried_region.nr_accesses.value_for(_damon.unit_samples,
+                intervals),
+            tried_region.age.value_for(_damon.unit_usec, intervals),
             _damon.unit_usec))
     return snapshot
 
 def tried_regions_to_snapshots(monitor_scheme):
     snapshots = {} # {kdamond idx: {ctx: Snapshot}}
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
         # TODO: Make a cleaner way for passing the index
         kdamond.idx = kdamond_idx
         for ctx in kdamond.contexts:
             for scheme in ctx.schemes:
                 if scheme.effectively_equal(monitor_scheme, ctx.intervals):
                     snapshot = tried_regions_to_snapshot(scheme.tried_regions,
-                            ctx.intervals.aggr)
+                            ctx.intervals)
                     snapshots[kdamond] = {ctx: snapshot}
                     break
     return snapshots
 
 def get_snapshots(access_pattern):
     'return DAMONSnapshots and an error'
-    orig_kdamonds = _damon.current_kdamonds()
-    running_kdamonds = _damon.running_kdamonds()
-    if len(running_kdamonds) == 0:
+    running_kdamond_idxs = _damon.running_kdamond_idxs()
+    if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
-    monitor_scheme = _damon.Damos(access_pattern=access_pattern)
+    orig_kdamonds = _damon.current_kdamonds()
 
-    installed, err = ensure_scheme_installed(running_kdamonds, monitor_scheme)
+    monitor_scheme = _damon.Damos(access_pattern=access_pattern)
+    installed, err = install_scheme(monitor_scheme)
     if err:
         return None, 'monitoring scheme install failed: %s' % err
 
-    err = _damon.update_schemes_tried_regions(['%d' % idx for idx, k in
-        enumerate(running_kdamonds)])
+    err = _damon.update_schemes_tried_regions(running_kdamond_idxs)
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
```

### Comparing `damo-1.7.7/src/damo/_damon_sysfs.py` & `damo-1.7.8/src/damo/_damon_sysfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,77 +15,77 @@
 
 # Use only one kdamond, one context, and one target for now
 root_dir = '/sys/kernel/mm/damon'
 admin_dir = os.path.join(root_dir, 'admin')
 kdamonds_dir = os.path.join(admin_dir, 'kdamonds')
 nr_kdamonds_file = os.path.join(kdamonds_dir, 'nr_kdamonds')
 
-def kdamond_dir_of(kdamond_name):
-    return os.path.join(admin_dir, 'kdamonds', '%s' % kdamond_name)
+def kdamond_dir_of(kdamond_idx):
+    return os.path.join(admin_dir, 'kdamonds', '%s' % kdamond_idx)
 
-def state_file_of(kdamond_name):
-    return os.path.join(kdamond_dir_of(kdamond_name), 'state')
+def state_file_of(kdamond_idx):
+    return os.path.join(kdamond_dir_of(kdamond_idx), 'state')
 
-def ctx_dir_of(kdamond_name, context_name):
+def ctx_dir_of(kdamond_idx, context_idx):
     return os.path.join(
-            kdamond_dir_of(kdamond_name), 'contexts', '%s' % context_name)
+            kdamond_dir_of(kdamond_idx), 'contexts', '%s' % context_idx)
 
-def schemes_dir_of(kdamond_name, context_name):
-    return os.path.join(ctx_dir_of(kdamond_name, context_name), 'schemes')
+def schemes_dir_of(kdamond_idx, context_idx):
+    return os.path.join(ctx_dir_of(kdamond_idx, context_idx), 'schemes')
 
-def scheme_dir_of(kdamond_name, context_name, scheme_name):
+def scheme_dir_of(kdamond_idx, context_idx, scheme_idx):
     return os.path.join(
-            schemes_dir_of(kdamond_name, context_name), '%s' % scheme_name)
+            schemes_dir_of(kdamond_idx, context_idx), '%s' % scheme_idx)
 
-def scheme_tried_regions_dir_of(kdamond_name, context_name, scheme_name):
+def scheme_tried_regions_dir_of(kdamond_idx, context_idx, scheme_idx):
     return os.path.join(
-            scheme_dir_of(kdamond_name, context_name, scheme_name),
+            scheme_dir_of(kdamond_idx, context_idx, scheme_idx),
             'tried_regions')
 
 def supported():
     return os.path.isdir(kdamonds_dir)
 
-def turn_damon_on(kdamonds_names):
+def turn_damon_on(kdamonds_idxs):
     # In case of vaddr, too early monitoring shows unstable mapping changes.
     # Give the process a time to have stable memory mapping.
     time.sleep(0.5)
-    for kdamond_name in kdamonds_names:
-        err = _damo_fs.write_file(state_file_of(kdamond_name), 'on')
+    for kdamond_idx in kdamonds_idxs:
+        err = _damo_fs.write_file(state_file_of(kdamond_idx), 'on')
         if err != None:
             return err
     return None
 
-def turn_damon_off(kdamonds_names):
-    for kdamond_name in kdamonds_names:
-        err = _damo_fs.write_file(state_file_of(kdamond_name), 'off')
+def turn_damon_off(kdamonds_idxs):
+    for kdamond_idx in kdamonds_idxs:
+        err = _damo_fs.write_file(state_file_of(kdamond_idx), 'off')
         if err != None:
             return err
     return None
 
-def is_kdamond_running(kdamond_name):
-    content, err = _damo_fs.read_file(state_file_of(kdamond_name))
+def is_kdamond_running(kdamond_idx):
+    content, err = _damo_fs.read_file(state_file_of(kdamond_idx))
     if err != None:
         print(err)
         return False
     return content.strip() == 'on'
 
 'Return error'
-def update_schemes_stats(kdamond_names):
-    for kdamond_name in kdamond_names:
+def update_schemes_stats(kdamond_idxs):
+    for kdamond_idx in kdamond_idxs:
         err = _damo_fs.write_file(
-                state_file_of(kdamond_name), 'update_schemes_stats')
+                state_file_of(kdamond_idx), 'update_schemes_stats')
         if err != None:
             return err
     return None
 
 'Return error'
-def update_schemes_tried_regions(kdamond_names):
-    for kdamond_name in kdamond_names:
+def update_schemes_tried_regions(kdamond_idxs):
+    for kdamond_idx in kdamond_idxs:
         err = _damo_fs.write_file(
-                state_file_of(kdamond_name), 'update_schemes_tried_regions')
+                state_file_of(kdamond_idx), 'update_schemes_tried_regions')
         if err != None:
             return err
     return None
 
 # for stage_kdamonds
 
 def wops_for_scheme_filter(damos_filter):
@@ -127,15 +127,15 @@
         },
     }
 
 def wops_for_scheme_access_pattern(pattern, ctx):
     if pattern == None:
         return {}
     pattern = pattern.converted_for_units(
-            _damon.unit_sample_intervals, _damon.unit_aggr_intervals,
+            _damon.unit_samples, _damon.unit_aggr_intervals,
             ctx.intervals)
 
     return {
         'sz': {
             'min': '%d' % pattern.sz_bytes[0],
             'max': '%d' % pattern.sz_bytes[1],
         },
@@ -150,24 +150,24 @@
     }
 
 def wops_for_schemes(ctx):
     schemes = ctx.schemes
 
     schemes_wops = {}
     for idx, scheme in enumerate(schemes):
-        scheme_dir_name = '%d' % idx
-        schemes_wops[scheme_dir_name] = {
+        dirname = '%d' % idx
+        schemes_wops[dirname] = {
             'access_pattern': wops_for_scheme_access_pattern(
                 scheme.access_pattern, ctx),
             'action': scheme.action,
             'quotas': wops_for_scheme_quotas(scheme.quotas),
             'watermarks': wops_for_scheme_watermarks(scheme.watermarks),
         }
         if feature_supported('schemes_filters'):
-            schemes_wops[scheme_dir_name]['filters'] = wops_for_scheme_filters(
+            schemes_wops[dirname]['filters'] = wops_for_scheme_filters(
                     scheme.filters)
     return schemes_wops
 
 def wops_for_regions(regions):
     return {'%d' % region_idx: {
         'start': '%d' % region.start,
         'end': '%d' % region.end}
@@ -236,15 +236,15 @@
         _damo_fs.write_file(nr_regions_path, '%d' % len(target.regions))
 
 def __ensure_kdamond_dir_populated(kdamond_dir, kdamond):
     contexts_dir_path = os.path.join(kdamond_dir, 'contexts')
     nr_contexts_path = os.path.join(kdamond_dir, 'contexts', 'nr_contexts')
     nr_contexts, err = _damo_fs.read_file(nr_contexts_path)
     if err != None:
-        raise Exception('kdamond name read fail (%s)' % err)
+        raise Exception('nr_contexts read fail (%s)' % err)
     if int(nr_contexts) != len(kdamond.contexts):
         _damo_fs.write_file(nr_contexts_path, '%d' % len(kdamond.contexts))
 
     for ctx_idx, ctx in enumerate(kdamond.contexts):
         ctx_dir_path = os.path.join(contexts_dir_path, '%d' % ctx_idx)
         targets_dir_path = os.path.join(ctx_dir_path, 'targets')
         nr_targets_path = os.path.join(targets_dir_path, 'nr_targets')
@@ -297,21 +297,34 @@
         return 'currently only <=one target is supported'
     ensure_dirs_populated_for(kdamonds)
 
     return _damo_fs.write_files({kdamonds_dir: wops_for_kdamonds(kdamonds)})
 
 # for current_kdamonds()
 
+def number_sorted_dirs(files_content):
+    number_dirs = {}
+    for filename, content in files_content.items():
+        try:
+            nr = int(filename)
+        except:
+            continue
+        if type(content) != dict:
+            continue
+        number_dirs[nr] = content
+    sorted_numbers = sorted(number_dirs.keys())
+    return [number_dirs[nr] for nr in sorted_numbers]
+
 def files_content_to_access_pattern(files_content):
     return _damon.DamosAccessPattern(
             [int(files_content['sz']['min']),
                 int(files_content['sz']['max'])],
             [int(files_content['nr_accesses']['min']),
                 int(files_content['nr_accesses']['max'])],
-            _damon.unit_sample_intervals, # nr_accesses_unit
+            _damon.unit_samples, # nr_accesses_unit
             [int(files_content['age']['min']),
                 int(files_content['age']['max'])],
             _damon.unit_aggr_intervals) # age_unit
 
 def files_content_to_quotas(files_content):
     return _damon.DamosQuotas(
             int(files_content['ms']),
@@ -326,45 +339,32 @@
             files_content['metric'].strip(),
             int(files_content['interval_us']),
             int(files_content['high']),
             int(files_content['mid']),
             int(files_content['low']))
 
 def files_content_to_damos_filters(files_content):
-    filters = []
-    for filter_dir_name in files_content:
-        if filter_dir_name == 'nr_filters':
-            continue
-        filter_kv = files_content[filter_dir_name]
-        filters.append(_damon.DamosFilter(filter_kv['type'].strip(),
-            filter_kv['memcg_path'].strip(), filter_kv['matching'].strip()))
-    return filters
+    return [_damon.DamosFilter(filter_kv['type'].strip(),
+            filter_kv['memcg_path'].strip(), filter_kv['matching'].strip())
+            for filter_kv in number_sorted_dirs(files_content)]
 
 def files_content_to_damos_stats(files_content):
     return _damon.DamosStats(
             int(files_content['nr_tried']),
             int(files_content['sz_tried']),
             int(files_content['nr_applied']),
             int(files_content['sz_applied']),
             int(files_content['qt_exceeds']))
 
 def files_content_to_damos_tried_regions(files_content):
-    regions = []
-    nr_region_dirs = len(files_content)
-    if 'sz_regions_sum' in files_content:
-        nr_region_dirs -= 1
-    for i in range(nr_region_dirs):
-        regions.append(_damon.DamosTriedRegion(
-            int(files_content['%d' % i]['start']),
-            int(files_content['%d' % i]['end']),
-            int(files_content['%d' % i]['nr_accesses']),
-            int(files_content['%d' % i]['age']),
-            _damon.unit_aggr_intervals
-            ))
-    return regions
+    return [_damon.DamosTriedRegion(
+            int(kv['start']), int(kv['end']),
+            int(kv['nr_accesses']), _damon.unit_samples,
+            int(kv['age']), _damon.unit_aggr_intervals)
+            for kv in number_sorted_dirs(files_content)]
 
 def files_content_to_scheme(files_content):
     return _damon.Damos(
             files_content_to_access_pattern(files_content['access_pattern']),
             files_content['action'].strip(),
             files_content_to_quotas(files_content['quotas']),
             files_content_to_watermarks(files_content['watermarks']),
@@ -372,91 +372,74 @@
                 if 'filters' in files_content else [],
             files_content_to_damos_stats(files_content['stats']),
             files_content_to_damos_tried_regions(
                 files_content['tried_regions'])
                 if 'tried_regions' in files_content else [])
 
 def files_content_to_regions(files_content):
-    regions = []
-    for region_idx in range(int(files_content['nr_regions'])):
-        region_name = '%d' % region_idx
-        regions.append(_damon.DamonRegion(
-            int(files_content[region_name]['start']),
-            int(files_content[region_name]['end'])))
-    return regions
+    return [_damon.DamonRegion(
+            int(kv['start']), int(kv['end']))
+            for kv in number_sorted_dirs(files_content)]
 
 def files_content_to_target(files_content):
     try:
         pid = int(files_content['pid_target'])
     except:
         pid = None
     regions = files_content_to_regions(files_content['regions'])
     return _damon.DamonTarget(pid, regions)
 
-def files_content_to_context(context_name, files_content):
+def files_content_to_context(files_content):
     mon_attrs_content = files_content['monitoring_attrs']
     intervals_content = mon_attrs_content['intervals']
     intervals = _damon.DamonIntervals(
             int(intervals_content['sample_us']),
             int(intervals_content['aggr_us']),
             int(intervals_content['update_us']))
     nr_regions_content = mon_attrs_content['nr_regions']
     nr_regions = _damon.DamonNrRegionsRange(
             int(nr_regions_content['min']),
             int(nr_regions_content['max']))
     ops = files_content['operations'].strip()
 
     targets_content = files_content['targets']
-    targets = []
-    for target_dir_name, target_content in targets_content.items():
-        if target_dir_name == 'nr_targets':
-            continue
-        targets.append(files_content_to_target(target_content))
+    targets = [files_content_to_target(content)
+            for content in number_sorted_dirs(targets_content)]
 
     schemes_content = files_content['schemes']
-    schemes = []
-    for scheme_name, scheme_content in schemes_content.items():
-        if scheme_name == 'nr_schemes':
-            continue
-        schemes.append(files_content_to_scheme(scheme_content))
+    schemes = [files_content_to_scheme(content)
+            for content in number_sorted_dirs(schemes_content)]
 
     return _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
 
 def files_content_to_kdamond(files_content):
     contexts_content = files_content['contexts']
-    contexts = []
-    for ctx_name in contexts_content:
-        if ctx_name == 'nr_contexts':
-            continue
-        contexts.append(files_content_to_context(ctx_name,
-            contexts_content[ctx_name]))
+    contexts = [files_content_to_context(content)
+            for content in number_sorted_dirs(contexts_content)]
     state = files_content['state'].strip()
     pid = files_content['pid'].strip()
     return _damon.Kdamond(state, pid, contexts)
 
 def files_content_to_kdamonds(files_contents):
-    kdamonds = []
-    for kdamond_name in files_contents:
-        if kdamond_name == 'nr_kdamonds':
-            continue
-        kdamonds.append(files_content_to_kdamond(files_contents[kdamond_name]))
-    return kdamonds
+    return [files_content_to_kdamond(content)
+            for content in number_sorted_dirs(files_contents)]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(kdamonds_dir))
 
-def current_kdamond_names():
-    # TODO: Do not read recursive but just one depth
-    return [x for x in _damo_fs.read_files(kdamonds_dir).keys()
-            if x != 'nr_kdamonds']
-
-def commit_staged(kdamond_names):
-    for kdamond_name in kdamond_names:
-        err = _damo_fs.write_file(state_file_of(kdamond_name), 'commit')
+def nr_current_kdamonds():
+    nr_kdamonds, err = _damo_fs.read_file(nr_kdamonds_file)
+    if err != None:
+        raise Exception('nr_kdamonds_file read fail (%s)' % err)
+    return int(nr_kdamonds)
+
+def commit_staged(kdamond_idxs):
+    for kdamond_idx in kdamond_idxs:
+        err = _damo_fs.write_file(state_file_of(kdamond_idx), 'commit')
         if err != None:
             return err
     return None
 
 # features
 
 def feature_supported(feature):
```

### Comparing `damo-1.7.7/src/damo/damo.py` & `damo-1.7.8/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_adjust.py` & `damo-1.7.8/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_features.py` & `damo-1.7.8/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_fmt_json.py` & `damo-1.7.8/src/damo/damo_fmt_json.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,11 +21,12 @@
         set_argparser(parser)
         args = parser.parse_args()
 
     kdamonds, err = _damon_args.kdamonds_for(args)
     if err:
         print('invalid arguments (%s)' % err)
         exit(1)
-    print(json.dumps([k.to_kvpairs(args.raw) for k in kdamonds], indent=4))
+    print(json.dumps({'kdamonds': [k.to_kvpairs(args.raw) for k in kdamonds]},
+        indent=4))
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.7.7/src/damo/damo_heats.py` & `damo-1.7.8/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_lru_sort.py` & `damo-1.7.8/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_monitor.py` & `damo-1.7.8/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_nr_regions.py` & `damo-1.7.8/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_reclaim.py` & `damo-1.7.8/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_record.py` & `damo-1.7.8/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_report.py` & `damo-1.7.8/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_report_raw.py` & `damo-1.7.8/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_schemes.py` & `damo-1.7.8/src/damo/damo_schemes.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import os
 import signal
 
 import _damon
 import _damon_args
 
 def cleanup_exit(exit_code):
-    err = _damon.turn_damon_off([kname for kname in kdamonds_names
-        if _damon.is_kdamond_running(kname)])
+    # ignore returning error, as kdamonds may already finished
+    _damon.turn_damon_off(kdamonds_names)
     if err:
         print('failed to turn damon off (%s)' % err)
     err = _damon.stage_kdamonds(orig_kdamonds)
     if err:
         print('failed restoring previous kdamonds setup (%s)' % err)
     exit(exit_code)
```

### Comparing `damo-1.7.7/src/damo/damo_start.py` & `damo-1.7.8/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_stat.py` & `damo-1.7.8/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_stat_kdamonds.py` & `damo-1.7.8/src/damo/damo_stat_kdamonds.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     if err:
         print(err)
         return
     kdamonds = _damon.current_kdamonds()
     if json_format:
         print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
     else:
-        print('kdamonds')
-        print(_damo_fmt_str.indent_lines(
-            '\n\n'.join([k.to_str(raw_nr) for k in kdamonds]), 4))
+        for idx, k in enumerate(kdamonds):
+            print('kdamond %d' % idx)
+            print(_damo_fmt_str.indent_lines( k.to_str(raw_nr), 4))
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--detail', action='store_true',
             help='print detailed stat of kdamonds')
     parser.add_argument('--json', action='store_true',
             help='print kdamond in json format')
```

### Comparing `damo-1.7.7/src/damo/damo_stat_regions.py` & `damo-1.7.8/src/damo/damo_stat_regions.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     if sortby == 'priority':
         regions.sort(key=lambda region: priority(region, prio_weights))
 
     total_sz = 0
     for region in regions:
         # region is DamonRegion.  Convert to DamosTriedRegion
         region = _damon.DamosTriedRegion(region.start, region.end,
-                region.nr_accesses, region.age / intervals.aggr,
-                _damon.unit_aggr_intervals)
+                region.nr_accesses, _damon.unit_samples,
+                region.age / intervals.aggr, _damon.unit_aggr_intervals)
         if not size_only:
             print(region.to_str(raw_nr, intervals))
         else:
             total_sz += (region.end - region.start)
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
```

### Comparing `damo-1.7.7/src/damo/damo_stat_schemes.py` & `damo-1.7.8/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_stop.py` & `damo-1.7.8/src/damo/damo_stop.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 def main(args=None):
     if not args:
         parser = set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    running_kdamond_names = _damon.running_kdamond_names()
-    if len(running_kdamond_names) == 0:
+    running_kdamond_idxs = _damon.running_kdamond_idxs()
+    if len(running_kdamond_idxs) == 0:
         print('DAMON is not turned on')
         exit(1)
 
-    err = _damon.turn_damon_off(running_kdamond_names)
+    err = _damon.turn_damon_off(running_kdamond_idxs)
     if err:
         print('DAMON turn off failed (%s)' % err)
         exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.7.7/src/damo/damo_translate_damos.py` & `damo-1.7.8/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_tune.py` & `damo-1.7.8/src/damo/damo_tune.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def main(args=None):
     if not args:
         parser = set_argparser(None)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    if _damon.every_kdamond_turned_off():
+    if not _damon.any_kdamond_running():
         print('DAMON is not turned on')
         exit(1)
 
     kdamonds, err = _damon_args.commit_kdamonds(args)
     if err:
         print('tuning failed (%s)' % err)
         exit(1)
```

### Comparing `damo-1.7.7/src/damo/damo_validate.py` & `damo-1.7.8/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo/damo_wss.py` & `damo-1.7.8/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.7/src/damo.egg-info/PKG-INFO` & `damo-1.7.8/src/damo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.7
+Version: 1.7.8
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -102,14 +102,22 @@
 -----------------------------------------------------------------------------
 
 Because the DAMOS input you're using is no more supported.  Please report your
 usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
 depend on those.
 
 
+damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
+----------------------------------------------------------------------------------------
+
+Because the single line DAMOS scheme format is no more supported.  Please
+report your usecase to sj@kernel.org, damon@lists.linux.dev and
+linux-mm@kvack.org if you depend on those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
```

### Comparing `damo-1.7.7/src/damo.egg-info/SOURCES.txt` & `damo-1.7.8/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


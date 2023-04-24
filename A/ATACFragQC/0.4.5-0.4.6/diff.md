# Comparing `tmp/ATACFragQC-0.4.5.tar.gz` & `tmp/ATACFragQC-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ATACFragQC-0.4.5.tar", last modified: Fri Jun 24 00:22:54 2022, max compression
+gzip compressed data, was "dist\ATACFragQC-0.4.6.tar", last modified: Mon Apr 24 09:47:15 2023, max compression
```

## Comparing `ATACFragQC-0.4.5.tar` & `ATACFragQC-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-06-24 00:22:54.000000 ATACFragQC-0.4.5/
-drwxrwxrwx   0        0        0        0 2022-06-24 00:22:54.000000 ATACFragQC-0.4.5/ATACFragQC/
--rw-rw-rw-   0        0        0       62 2022-06-24 00:22:27.000000 ATACFragQC-0.4.5/ATACFragQC/__init__.py
--rw-rw-rw-   0        0        0    12879 2022-06-24 00:21:07.000000 ATACFragQC-0.4.5/ATACFragQC/__main__.py
-drwxrwxrwx   0        0        0        0 2022-06-24 00:22:54.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/
--rw-rw-rw-   0        0        0     1186 2022-06-24 00:22:49.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2022-06-24 00:22:50.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-24 00:22:50.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2022-06-24 00:22:50.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2022-06-24 00:22:50.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-06-24 00:22:50.000000 ATACFragQC-0.4.5/ATACFragQC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2020-12-19 11:09:54.000000 ATACFragQC-0.4.5/LICENSE
--rw-rw-rw-   0        0        0       45 2020-12-19 13:00:27.000000 ATACFragQC-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1186 2022-06-24 00:22:54.000000 ATACFragQC-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      637 2022-06-21 06:16:39.000000 ATACFragQC-0.4.5/README.md
--rw-rw-rw-   0        0        0       91 2020-12-19 12:59:45.000000 ATACFragQC-0.4.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-06-24 00:22:54.000000 ATACFragQC-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1175 2020-12-19 11:17:55.000000 ATACFragQC-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/ATACFragQC/
+-rw-rw-rw-   0        0        0       62 2023-04-24 09:46:00.000000 ATACFragQC-0.4.6/ATACFragQC/__init__.py
+-rw-rw-rw-   0        0        0    13684 2023-04-24 09:44:10.000000 ATACFragQC-0.4.6/ATACFragQC/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/
+-rw-rw-rw-   0        0        0     1186 2023-04-24 09:47:09.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:47:09.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 09:47:10.000000 ATACFragQC-0.4.6/ATACFragQC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2020-12-19 11:09:54.000000 ATACFragQC-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0       45 2020-12-19 13:00:27.000000 ATACFragQC-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1186 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2022-06-21 06:16:39.000000 ATACFragQC-0.4.6/README.md
+-rw-rw-rw-   0        0        0       91 2020-12-19 12:59:45.000000 ATACFragQC-0.4.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:47:15.000000 ATACFragQC-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2020-12-19 11:17:55.000000 ATACFragQC-0.4.6/setup.py
```

### Comparing `ATACFragQC-0.4.5/ATACFragQC/__main__.py` & `ATACFragQC-0.4.6/ATACFragQC/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,18 +126,28 @@
     tss_range = (args.widthtss+100)*2+1
     for index, row in ref.iterrows():
         count = np.zeros(tss_range, dtype=np.int64)
         for frag in fs.fetch(row["seq_id"], row["start"], row["end"]):
             if args.calc_mode == "F":
                 if (frag.flag & 3) == 3 and (frag.flag & 1812) == 0 and frag.mapq > args.quality and frag.isize > 0 and frag.isize < args.isize:
                     count[range(max(0, frag.pos - row["start"]), min(tss_range, frag.pos + frag.isize - row["start"]))] += 1
-            else:
+            elif args.calc_mode == "C":
                 if (frag.flag & 3) == 3 and (frag.flag & 1812) == 0 and frag.mapq > args.quality and frag.isize > 0:
                     count[max(0, frag.pos - row["start"])] += 1
                     count[min(tss_range, frag.pos + frag.isize - row["start"]) - 1] += 1
+            elif args.calc_mode == "M":
+                if (frag.flag & 3) == 3 and (frag.flag & 1812) == 0 and frag.mapq > args.quality and frag.isize > 0:
+                    if length(frag.isize % 2 == 1):
+                        count[frag.pos + (frag.isize - 1)/2 - row["start"]] += 1
+                    else:
+                        count[frag.pos + frag.isize/2 - row["start"]] += 1
+                        count[frag.pos + frag.isize/2 - 1 - row["start"]] += 1
+            else:
+                if (frag.flag & 3) == 3 and (frag.flag & 1812) == 0 and frag.mapq > args.quality and frag.isize > 0 and frag.isize < args.isize:
+                    count[range(max(0, frag.pos - row["start"]), min(tss_range, frag.pos + frag.isize - row["start"]))] += 1
         if sum(count) > 0:
             dist_count.append(count)
     dist_count = np.array(dist_count)
     if dist_count.size > 0:
         factors = np.mean(dist_count[:, list(range(0, 100))+list(range(tss_range-100, tss_range))], axis=1)
         factors[factors == 0] = np.mean(factors) if np.mean(factors) > 0 else 1
         dist_count = pd.DataFrame({"V1": list(range(-args.widthtss, args.widthtss+1)), "V2": list(np.mean(dist_count[:, 100:(tss_range-100)] / factors.reshape(len(factors), 1), axis=0))})
@@ -207,15 +217,15 @@
     help_info = "Usage:\nATACFragQC [options] -i <input.bam> -r <reference.gtf>\nArguments:\n"\
         +"-h, --help\t\tShow this help information\n"\
         +"-i, --input <file>\tA aligned & deduped BAM file\n"\
         +"-r, --reference <file>\tGTF genome annotation\n"\
         +"-g, --group [marker]\tThe TSS of each group would be calculated if -g was set\n"\
         +"-s, --save <name>\tThe name of results (default: same as the bam)\n"\
         +"-o, --output [T/F]\tThe table of results would be saved if -o was set (default: False)\n"\
-        +"-m, --mode [F/C]\tThe TSS enrichment would be calculated by fragments (F) or cutsites(C) (default: F)\n"\
+        +"-m, --mode [F/C/M]\tThe TSS enrichment would be calculated by fragments (F), cutsites(C) or midsites(M) (default: F)\n"\
         +"-q, --quality [1-255]\tThe quality limit of alignment (default: 5)\n"\
         +"-l, --length [50-500]\tThe length limit of nucleosome-free fragment (default: 147)\n"\
         +"-c, --chr [aaa,bbb]\tThe list of chromosomes would be used (default: all)\n"\
         +"-n, --nl [0-X]\tThe length limit of chromosome names (default: 10, 0 is no limit)\n"\
         +"-p, --pic [a,b,c]\tThe list of images would be shown (default: all)\n"\
         +"-f, --filter [aaa,bbb]\tThe list of chromosomes which should be filtered (default: none)\n"\
         +"-w, --widthtss [100-10000]\tThe width of regions around the TSS (default: 900)\n"\
```

### Comparing `ATACFragQC-0.4.5/ATACFragQC.egg-info/PKG-INFO` & `ATACFragQC-0.4.6/ATACFragQC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATACFragQC
-Version: 0.4.5
+Version: 0.4.6
 Summary: Fragment Quality Control for ATAC-seq
 Home-page: https://github.com/0CBH0/ATACFragQC
 Author: 0CBH0
 Author-email: maodatou88@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ATACFragQC-0.4.5/LICENSE` & `ATACFragQC-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ATACFragQC-0.4.5/PKG-INFO` & `ATACFragQC-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATACFragQC
-Version: 0.4.5
+Version: 0.4.6
 Summary: Fragment Quality Control for ATAC-seq
 Home-page: https://github.com/0CBH0/ATACFragQC
 Author: 0CBH0
 Author-email: maodatou88@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ATACFragQC-0.4.5/README.md` & `ATACFragQC-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ATACFragQC-0.4.5/setup.py` & `ATACFragQC-0.4.6/setup.py`

 * *Files identical despite different names*


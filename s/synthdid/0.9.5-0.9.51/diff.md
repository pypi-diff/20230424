# Comparing `tmp/synthdid-0.9.5.tar.gz` & `tmp/synthdid-0.9.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.9.5.tar", last modified: Fri Apr 21 18:48:46 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.51.tar", last modified: Mon Apr 24 17:17:59 2023, max compression
```

## Comparing `synthdid-0.9.5.tar` & `synthdid-0.9.51.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.096260 synthdid-0.9.5/
--rw-rw-rw-   0        0        0      544 2023-04-21 18:48:46.096260 synthdid-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 18:48:46.096260 synthdid-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-04-21 18:48:43.000000 synthdid-0.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.087260 synthdid-0.9.5/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.5/synthdid/plots.py
--rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/solver.py
--rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.5/synthdid/summary.py
--rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.5/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.095260 synthdid-0.9.5/synthdid.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.324706 synthdid-0.9.51/
+-rw-rw-rw-   0        0        0     8824 2023-04-24 17:17:59.324706 synthdid-0.9.51/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:17:59.324706 synthdid-0.9.51/setup.cfg
+-rw-rw-rw-   0        0        0     1858 2023-04-24 17:17:05.000000 synthdid-0.9.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.309706 synthdid-0.9.51/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6066 2023-04-24 17:10:42.000000 synthdid-0.9.51/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/solver.py
+-rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.51/synthdid/summary.py
+-rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.51/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.323704 synthdid-0.9.51/synthdid.egg-info/
+-rw-rw-rw-   0        0        0     8824 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.9.5/setup.py` & `synthdid-0.9.51/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-# with open("./Readme.md", "r", encoding="utf-8") as f:
-#     long_description = f.read()
+with open("./Readme.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
 
 setup(
     dependency_links=[],
     install_requires=[
         "appdirs==1.4.3",
         "attrs==19.1.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
         "black==19.3b0; python_version >= '3.6'",
@@ -30,17 +30,17 @@
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
     author="D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres",
-    version="0.9.5",
+    version="0.9.51",
     packages=find_packages(),
-    # long_description=long_description,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `synthdid-0.9.5/synthdid/get_data.py` & `synthdid-0.9.51/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/placebo_simulations.py` & `synthdid-0.9.51/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/plots.py` & `synthdid-0.9.51/synthdid/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,24 +128,24 @@
                 size_dot = weights_dots.size
                 size_dot = np.interp(size_dot, (size_dot.min(), size_dot.max()), (1, 50))
                 weights_dots["size_dot"] = size_dot
 
             fig, ax = plt.subplots()
 
             ax.scatter("unit", "difs", data = weights_dots, s = "size", c = "color", label = "")
-            # ax.scatter("unit", "difs", data = weights_dots, s = "size", color = "color", marker=shape_dot)
+            ax.set_xticks(range(len(units)))
             ax.set_xticklabels(units, rotation = 90, fontsize = ns);
             ax.set_xlabel("Group")
             ax.set_ylabel("Difference")
             ax.set_title("Adoption: " + str(time_title_cb(times[i])))
             ax.axhline(y=atts[i], linestyle = "--", color = "#E00029", lw = .6, label = f"Att {time_title_cb(times[i])}: {atts[i]}")
             ax.axhline(y=self.att, linestyle = "--", color = "#640257", lw = .8, label = f"Att: {spaces} {real_att}")
-            ax.legend(fontsize = 9)
+            ax.legend(fontsize = 9);
             if weights_dots.difs.max() > 0 and weights_dots.difs.min() < 0:
-                ax.axhline(y=0, lw = .5, c = "#0D3276")
-            plots.append(fig)
+                ax.axhline(y=0, lw = .5, c = "#0D3276");
+            plots.append(fig);
 
         for i, time in enumerate(times):
             plot_times(i)
         self.plot_weights = []
         self.plot_weights = plots
         return self
```

### Comparing `synthdid-0.9.5/synthdid/sdid.py` & `synthdid-0.9.51/synthdid/sdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/solver.py` & `synthdid-0.9.51/synthdid/solver.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/synthdid.py` & `synthdid-0.9.51/synthdid/synthdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/utils.py` & `synthdid-0.9.51/synthdid/utils.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid/vcov.py` & `synthdid-0.9.51/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.5/synthdid.egg-info/requires.txt` & `synthdid-0.9.51/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*


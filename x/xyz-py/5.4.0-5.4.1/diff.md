# Comparing `tmp/xyz_py-5.4.0.tar.gz` & `tmp/xyz_py-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.4.0.tar", last modified: Fri Apr 21 13:17:06 2023, max compression
+gzip compressed data, was "xyz_py-5.4.1.tar", last modified: Mon Apr 24 09:41:24 2023, max compression
```

## Comparing `xyz_py-5.4.0.tar` & `xyz_py-5.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:17:06.598865 xyz_py-5.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-21 13:16:36.000000 xyz_py-5.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-21 13:17:06.596865 xyz_py-5.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-21 13:16:36.000000 xyz_py-5.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-21 13:16:36.000000 xyz_py-5.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 13:17:06.598865 xyz_py-5.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-21 13:17:02.000000 xyz_py-5.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:17:06.591864 xyz_py-5.4.0/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-21 13:16:36.000000 xyz_py-5.4.0/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-21 13:16:36.000000 xyz_py-5.4.0/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     9786 2023-04-21 13:16:36.000000 xyz_py-5.4.0/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-21 13:17:02.000000 xyz_py-5.4.0/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37836 2023-04-21 13:16:36.000000 xyz_py-5.4.0/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:17:06.596865 xyz_py-5.4.0/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-21 13:17:06.000000 xyz_py-5.4.0/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.752729 xyz_py-5.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-24 09:40:57.000000 xyz_py-5.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 09:41:24.750729 xyz_py-5.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-24 09:40:57.000000 xyz_py-5.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-24 09:40:57.000000 xyz_py-5.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 09:41:24.752729 xyz_py-5.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-24 09:41:20.000000 xyz_py-5.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.744729 xyz_py-5.4.1/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9876 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 09:41:20.000000 xyz_py-5.4.1/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.750729 xyz_py-5.4.1/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.4.0/LICENSE` & `xyz_py-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.0/PKG-INFO` & `xyz_py-5.4.1/xyz_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.4.0
+Name: xyz-py
+Version: 5.4.1
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.4.0/README.md` & `xyz_py-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.0/setup.py` & `xyz_py-5.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.4.0"
+__version__ = "5.4.1"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.4.0/xyz_py/atomic.py` & `xyz_py-5.4.1/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.0/xyz_py/cli.py` & `xyz_py-5.4.1/xyz_py/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,16 @@
     coords_1 -= coords_1[0]
     coords_2 -= coords_2[0]
 
     rmsd, alpha, beta, gamma = xyz_py.minimise_rmsd(
         coords_1, coords_2
     )
 
+    print(f'RMSD between structures is {rmsd:.4f}')
+
     _coords_1 = xyz_py.rotate_coords(coords_1, alpha, beta, gamma)
 
     out_coords = np.vstack([_coords_1, coords_2])
 
     out_labels = labels_1 + labels_2
 
     out_f_name = 'overlayed.xyz'
@@ -384,16 +386,16 @@
         metavar='file_name',
         help='Output file name - default is append xyz file with _rotated'
     )
 
     overlay = subparsers.add_parser(
         'overlay',
         description=(
-            'overlay xyz file by alpha, beta, gamma in degrees using '
-            'Easyspin convention'
+            'Overlay two xyz files by rotating file_1 onto file_2'
+            'Files MUST have the same number of atoms, and the same order'
         )
     )
     overlay.set_defaults(func=overlay_func)
 
     overlay.add_argument(
         'xyz_file_1',
         type=str,
```

### Comparing `xyz_py-5.4.0/xyz_py/xyz_py.py` & `xyz_py-5.4.1/xyz_py/xyz_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     if style == 'per_element':
         # Get list of unique elements
         atoms = set(labels_nn)
         # Create dict to keep track of index of current atom of each element
         atom_count = {atom: start_index for atom in atoms}
         # Create labelled list of elements
         labels_wn = []
-        
+
         for lab in labels_nn:
             # Index according to dictionary
             labels_wn.append('{}{:d}'.format(lab, atom_count[lab]))
             # Then add one to dictionary
             atom_count[lab] += 1
 
     return labels_wn
@@ -1281,34 +1281,35 @@
 
     return rot_coords
 
 
 def minimise_rmsd(coords_1, coords_2, mask_1=[], mask_2=[], order_1=[],
                   order_2=[]):
     '''
-    Minimising the RMSD between two structures
+    Minimises the RMSD between two structures
+    by rotating coords_1 onto coords_2
     If coords_1 and coords_2 are not the same length, then a mask array can be
     provided for either/both and is applied prior to the calculation
     coords_1 and coords_2 can also be reordered if new orders are specified
     **note reordering occurs before masking**
 
     Parameters
     ----------
     coords_1 : np.ndarray
         xyz coordinates as (n_atoms, 3) array
     coords_2 : np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    mask_1 : list
-        list of 0 (exclude) and 1 (include) for each element in coords_1
-    mask_2 : list
-        list of 0 (exclude) and 1 (include) for each element in coords_2
-    order_1 : list
-        list of new indices for coords_1 - applied BEFORE masking
-    order_2 : list
-        list of new indices for coords_2 - applied BEFORE masking
+    mask_1 : list[int]
+        0 (exclude) or 1 (include) for each element in coords_1
+    mask_2 : list[int]
+        0 (exclude) or 1 (include) for each element in coords_2
+    order_1 : list[int]
+        new indices for coords_1 - applied BEFORE masking
+    order_2 : list[int]
+        new indices for coords_2 - applied BEFORE masking
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
     float
         alpha angle in radians
@@ -1348,15 +1349,15 @@
         ),
         x0=(1., 1., 1.),
         jac='3-point'
     )
 
     # Get optimum angles
     [alpha, beta, gamma] = result.x
-    rmsd = result.cost
+    rmsd = result.fun[0]
 
     return rmsd, alpha, beta, gamma
 
 
 def _rotate_and_rmsd(angs, coords_1, coords_2):
     '''
     Rotates coords_1 by alpha, beta, gamma using the zyz convention
@@ -1365,15 +1366,15 @@
 
     Parameters
     ----------
     coords_1 : np.ndarray
         xyz coordinates as (n_atoms, 3) array of first system
     coords_2 : np.ndarray
         xyz coordinates as (n_atoms, 3) array of second system
-    angs : list
+    angs : list[float]
         alpha, beta, gamma in radians
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array after rotation
         in same order as input coordinates
@@ -1387,14 +1388,15 @@
 
     return rmsd
 
 
 def calculate_com(labels, coords):
     '''
     Calculates centre-of-mass using relative atomic masses
+
     Parameters
     ----------
     labels : list
         list of atomic labels
     coords : np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
@@ -1405,14 +1407,14 @@
     '''
 
     labels_nn = remove_label_indices(labels)
 
     masses = [atomic.masses[lab] for lab in labels_nn]
 
     com_coords = np.zeros(3)
-    
+
     for trio, mass in zip(coords, masses):
         com_coords += trio * mass
 
     com_coords /= np.sum(masses)
 
     return com_coords
```

### Comparing `xyz_py-5.4.0/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.4.0
+Name: xyz_py
+Version: 5.4.1
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```


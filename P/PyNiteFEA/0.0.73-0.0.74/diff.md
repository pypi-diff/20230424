# Comparing `tmp/PyNiteFEA-0.0.73.tar.gz` & `tmp/PyNiteFEA-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.73.tar", last modified: Wed Apr 19 15:07:44 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.74.tar", last modified: Mon Apr 24 16:34:10 2023, max compression
```

## Comparing `PyNiteFEA-0.0.73.tar` & `PyNiteFEA-0.0.74.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   152624 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    66986 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 15:07:44.000000 PyNiteFEA-0.0.73/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:07:44.852761 PyNiteFEA-0.0.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 15:07:33.000000 PyNiteFEA-0.0.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152953 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67808 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/setup.py
```

### Comparing `PyNiteFEA-0.0.73/LICENSE` & `PyNiteFEA-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PKG-INFO` & `PyNiteFEA-0.0.74/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.73
+Version: 0.0.74
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
 5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
-* The wiki in this repository provides basic guidance on how to use PyNite, although it has fallen behind the development of the program.
+* Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
 # Dependencies
 PyNite depends on the following packages:
 ## Required Dependencies
 * numpy: used for matrix algebra and dense matrix solver
 * matplotlib: used for plotting member diagrams
@@ -89,14 +89,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.74
+* Bug fix for rectangular meshes with very close control points. The program now checks for mesh
+control points that are for all practical purposes the same and eliminates the duplicates.
+
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
 
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
```

### Comparing `PyNiteFEA-0.0.73/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.74/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.74/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.74/PyNite/FEModel3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1375,36 +1375,31 @@
                 D2_indices.append(node.ID*6 + 5)
                 D2.append(0.0)
 
         # Return the indices and the known displacements
         return D1_indices, D2_indices, D2
                
     def K(self, combo_name='Combo 1', log=False, check_stability=True, sparse=True):
-        """
-        Returns the model's global stiffness matrix.
-
-        The stiffness matrix will be returned in scipy's sparse lil format,
-        which reduces memory usage and can be easily converted to other
-        formats.
-
-        Parameters
-        ----------
-        combo_name : str, optional
-            The load combination to get the stiffness matrix for. Default is 'Combo 1'.
-        log : bool, optional
-            Prints updates to the console if set to True. Default is False.
-        sparse : bool, optional
-            Returns a sparse matrix if set to True, and a dense matrix
-            otherwise. Default is True
-        
-        Returns
-        -------
-        K : ndarray or coo_matrix
-            The global stiffness matrix for the structure.
-        """
+        """Returns the model's global stiffness matrix. The stiffness matrix will be returned in
+           scipy's sparse lil format, which reduces memory usage and can be easily converted to
+           other formats.
+
+        :param combo_name: The load combination to get the stiffness matrix for. Defaults to 'Combo 1'.
+        :type combo_name: str, optional
+        :param log: Prints updates to the console if set to True. Defaults to False.
+        :type log: bool, optional
+        :param check_stability: Causes Pynite to check for instabilities if set to True. Defaults
+                                to True. Set to False if you want the model to run faster.
+        :type check_stability: bool, optional
+        :param sparse: Returns a sparse matrix if set to True, and a dense matrix otherwise.
+                       Defaults to True.
+        :type sparse: bool, optional
+        :return: The global stiffness matrix for the structure.
+        :rtype: ndarray or coo_matrix
+        """           
         
         # Determine if a sparse matrix has been requested
         if sparse == True:
             # The stiffness matrix will be stored as a scipy `coo_matrix`. Scipy's
             # documentation states that this type of matrix is ideal for efficient
             # construction of finite element matrices. When converted to another
             # format, the `coo_matrix` sums values at the same (i, j) index. We'll
@@ -1781,22 +1776,22 @@
                             # Now that 'm' and 'n' are known, place the term in the global stiffness matrix
                             Kg[m, n] += member_Kg[(a, b)]
 
         # Return the global geometric stiffness matrix
         return Kg
       
     def FER(self, combo_name='Combo 1'):
-        '''
-        Assembles and returns the global fixed end reaction vector.
+        """Assembles and returns the global fixed end reaction vector for any given load combo.
 
-        Parameters
-        ----------
-        combo_name : str
-            The name of the load combination to get the fixed end reaction vector for (not the load combination itself).
-        '''
+        :param combo_name: The name of the load combination to get the fixed end reaction vector
+                           for. Defaults to 'Combo 1'.
+        :type combo_name: str, optional
+        :return: The fixed end reaction vector
+        :rtype: array
+        """        
         
         # Initialize a zero vector to hold all the terms
         FER = zeros((len(self.Nodes) * 6, 1))
         
         # Step through each physical member in the model
         for phys_member in self.Members.values():
```

### Comparing `PyNiteFEA-0.0.73/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.74/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/LoadCombo.py` & `PyNiteFEA-0.0.74/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.74/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Member3D.py` & `PyNiteFEA-0.0.74/PyNite/Member3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Mesh.py` & `PyNiteFEA-0.0.74/PyNite/Mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,17 +445,35 @@
         # Add the mesh's boundaries to the list of control points
         x_control.append(0)
         x_control.append(width)
         y_control.append(0)
         y_control.append(height)
 
         # Sort the control points and remove duplicate values
-        x_control = sorted(set(x_control))
-        y_control = sorted(set(y_control))
-        
+        x_control = sorted(x_control)
+        y_control = sorted(y_control)
+
+        # Remove any values that are duplicates or near duplicates from `x_control`
+        unique_list = []
+        for i in range(len(x_control) - 1):
+            # Only keep the value at `i` if it's not a duplicate or near duplicate
+            if not isclose(x_control[i], x_control[i+1]):
+                unique_list.append(x_control[i])
+        unique_list.append(x_control[-1])
+        x_control = unique_list
+
+        # Remove any values that are duplicates or near duplicates from `y_control`
+        unique_list = []
+        for i in range(len(y_control) - 1):
+            # Only keep the value at `i` if it's not a duplicate or near duplicate
+            if not isclose(y_control[i], y_control[i+1]):
+                unique_list.append(y_control[i])
+        unique_list.append(y_control[-1])
+        y_control = unique_list
+    
         # Each node number will be increased by the offset calculated below
         node_offset = int(self.start_node[1:]) - 1
 
         # Each element number will be increased by the offset calculated below
         element_offset = int(self.start_element[1:]) - 1
 
         # Determine which prefix to assign to new elements
```

### Comparing `PyNiteFEA-0.0.73/PyNite/Node3D.py` & `PyNiteFEA-0.0.74/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/PhysMember.py` & `PyNiteFEA-0.0.74/PyNite/PhysMember.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Plate3D.py` & `PyNiteFEA-0.0.74/PyNite/Plate3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Quad3D.py` & `PyNiteFEA-0.0.74/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Report_Template.html` & `PyNiteFEA-0.0.74/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Reporting.py` & `PyNiteFEA-0.0.74/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Spring3D.py` & `PyNiteFEA-0.0.74/PyNite/Spring3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNite/Visualization.py` & `PyNiteFEA-0.0.74/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.74/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.73
+Version: 0.0.74
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,15 +62,15 @@
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
 5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
-* The wiki in this repository provides basic guidance on how to use PyNite, although it has fallen behind the development of the program.
+* Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
 # Dependencies
 PyNite depends on the following packages:
 ## Required Dependencies
 * numpy: used for matrix algebra and dense matrix solver
 * matplotlib: used for plotting member diagrams
@@ -89,14 +89,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.74
+* Bug fix for rectangular meshes with very close control points. The program now checks for mesh
+control points that are for all practical purposes the same and eliminates the duplicates.
+
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
 
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
```

### Comparing `PyNiteFEA-0.0.73/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.74/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.73/README.md` & `PyNiteFEA-0.0.74/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
 5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
-* The wiki in this repository provides basic guidance on how to use PyNite, although it has fallen behind the development of the program.
+* Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
 # Dependencies
 PyNite depends on the following packages:
 ## Required Dependencies
 * numpy: used for matrix algebra and dense matrix solver
 * matplotlib: used for plotting member diagrams
@@ -70,14 +70,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.74
+* Bug fix for rectangular meshes with very close control points. The program now checks for mesh
+control points that are for all practical purposes the same and eliminates the duplicates.
+
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
 
 v0.0.72
 * Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
 * Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
 
@@ -120,8 +124,8 @@
 * Fixed obsolete method names that had not been updated.
 * Scalar bar text size can now be controlled. It had strange behavior before. It would change with the window size (until the window size was too small).
 * More work on the new `Renderer` class. This class is being built to give the user more control over the appearance and behavior of renderings.
 * Bug fix for nodal springs applied in the 'RY' and 'RZ' direction. Exceptions were being thrown in some cases.
 
 v0.0.63 thru v0.0.64
 * Fixed the `add_mesh` method. It was not working properly after version 0.0.62.
-* Made stability checks optional. Stability checks add significant solve time. If you are confident your model is stable, you can skip the stability check by toggling `check_stability` to `False` in your call to your analysis command.
+* Made stability checks optional. Stability checks add significant solve time. If you are confident your model is stable, you can skip the stability check by toggling `check_stability` to `False` in your call to your analysis command.
```

### Comparing `PyNiteFEA-0.0.73/setup.py` & `PyNiteFEA-0.0.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.73",
+    version="0.0.74",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
```


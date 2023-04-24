# Comparing `tmp/pyees-1.2.2.tar.gz` & `tmp/pyees-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.2.tar", last modified: Fri Apr 21 11:08:58 2023, max compression
+gzip compressed data, was "pyees-1.2.3.tar", last modified: Mon Apr 24 16:54:33 2023, max compression
```

## Comparing `pyees-1.2.2.tar` & `pyees-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:08:58.267170 pyees-1.2.2/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-04-21 11:08:58.282795 pyees-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:08:57.954655 pyees-1.2.2/pyees/
--rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.2/pyees/__init__.py
--rw-rw-rw-   0        0        0    15015 2023-04-19 12:43:26.000000 pyees-1.2.2/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.2/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9051 2023-04-21 09:09:36.000000 pyees-1.2.2/pyees/prop.py
--rw-rw-rw-   0        0        0    14724 2023-04-19 09:10:47.000000 pyees-1.2.2/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.2.2/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.2/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3889 2023-04-19 12:43:28.000000 pyees-1.2.2/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-04-21 11:06:00.000000 pyees-1.2.2/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-19 12:41:29.000000 pyees-1.2.2/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15043 2023-04-19 08:45:19.000000 pyees-1.2.2/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.2/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.2/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81276 2023-04-19 12:40:55.000000 pyees-1.2.2/pyees/testVariable.py
--rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.2/pyees/unit.py
--rw-rw-rw-   0        0        0    34969 2023-04-19 12:41:14.000000 pyees-1.2.2/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:08:58.157789 pyees-1.2.2/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 11:08:58.298422 pyees-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-21 11:08:50.000000 pyees-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.545760 pyees-1.2.3/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-04-24 16:54:33.549748 pyees-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.409657 pyees-1.2.3/pyees/
+-rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.3/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15214 2023-04-24 08:53:03.000000 pyees-1.2.3/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.3/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9051 2023-04-21 09:09:36.000000 pyees-1.2.3/pyees/prop.py
+-rw-rw-rw-   0        0        0    14733 2023-04-24 15:08:43.000000 pyees-1.2.3/pyees/readData.py
+-rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.3/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.3/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3889 2023-04-19 12:43:28.000000 pyees-1.2.3/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-04-21 11:06:00.000000 pyees-1.2.3/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-19 12:41:29.000000 pyees-1.2.3/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.3/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.3/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.3/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81276 2023-04-19 12:40:55.000000 pyees-1.2.3/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.3/pyees/unit.py
+-rw-rw-rw-   0        0        0    35819 2023-04-24 16:15:04.000000 pyees-1.2.3/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:54:33.526343 pyees-1.2.3/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-24 16:54:33.494428 pyees-1.2.3/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 16:54:32.000000 pyees-1.2.3/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-24 16:54:33.573684 pyees-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-04-24 16:54:27.000000 pyees-1.2.3/setup.py
```

### Comparing `pyees-1.2.2/LICENSE.txt` & `pyees-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/PKG-INFO` & `pyees-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.2
+Version: 1.2.3
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.2/README.md` & `pyees-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/fit.py` & `pyees-1.2.3/pyees/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             label = None
         else:
             raise ValueError('The label has to be a string, a bool or None')
 
         ax.plot(self.xVal, self.yVal, label=label, **kwargs)
 
     def predict(self, x):
-        if not isinstance(x, arrayVariable) or isinstance(x, scalarVariable):
+        if not isinstance(x, scalarVariable):
             x = variable(x, self.xUnit)
         return self.func(x)
 
     def predictDifferential(self, x):
         if not isinstance(x, arrayVariable) or isinstance(x, scalarVariable):
             x = variable(x, self.xUnit)
         return self.d_func(self.popt, x)
@@ -470,22 +470,19 @@
         out += f'\quad x_0={x0}$'
         return out
 
 
 if __name__ == "__main__":
     
     
-    frequency = variable([10,20,30,40,50,60,70,80,90,100,110], 'C')
-    voltage = variable([16, 45, 64, 75,70,115, 142, 167, 183, 160, 221], 'C', [5,5,5,5,30,5,5,5,5,30,5])
-    
-    fit = lin_fit(frequency, voltage)
-    
-    print(fit) 
-    
+    flow = variable([32.77384783, 41.09968726, 49.26071221, 57.3579077, 65.42974152, 73.39579152, 81.71096102, 89.5224963, 97.35493807], 'L/min', [0.09242640187777096, nan, nan, nan, 0.0997230684346466, 0.16573749880130453, 0.3306259756514912, 0.3428053760615392, 0.4003027546277681])
+    dp = variable([43.310, 64.53, 90.0, 118.8, 151.92, 189.4, 231.19, 276.1, 323.4], 'mbar',[0.002, 0.08, 0.1, 0.2, 0.09, 0.6, 0.06, 0.6, 0.4])
     
+    fit = pol_fit(flow, dp)
+    print(fit)    
 
 
 
 ## TODO fit - få det til at virke som i bogen - brug tests - mangler solutions
 ## TODO fit - lav normalized residuals plot
 ## TODO fit - evaluer, om 68% af datapunkterne ligger 1 standard afvigelse fra fittet
```

### Comparing `pyees-1.2.2/pyees/profilePyees.py` & `pyees-1.2.3/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/prop.py` & `pyees-1.2.3/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/readData.py` & `pyees-1.2.3/pyees/readData.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
                     # create the measurements with covariance uncertanties
                     vars = []
                     for i in range(self.nCols):
                         name = headers[i]
                         unit = units[i]
                         val = np.array(data[:, i])
-                        u = np.array([elem[i, i] for elem in uncert])
+                        u = np.array([np.sqrt(elem[i, i]) for elem in uncert])
                         var = variable(val, unit, uncert=u)
                         vars.append(var)
 
                     for i in range(self.nCols):
                         covariance = [elem[:, i] for elem in uncert]
                         for j in range(self.nCols):
                             if i != j:
```

### Comparing `pyees-1.2.2/pyees/solve.py` & `pyees-1.2.3/pyees/solve.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,17 @@
 
     ## define the scalings of each equation. This is only valid if there are more than 1 equaiton
     scales = np.ones(nVariables)
     if nVariables != 1:
         out = ffunc(*x)
         currentIndex = 0
         for i,o in enumerate(out):
-            for bound in o:
-                bound.convert(bound._unitObject._SIBaseUnit) 
+            if not doesUnitsOfEquationsMatch[i]:
+                for elem in o:
+                    elem.convert(elem._unitObject._SIBaseUnit) 
             scales[i] = 1/(o[0].value - o[1].value)**2
     
     
     ## method to keep the variables within the bounda
     ## the method will be given a single input during the minimzation. 
     ## Therefore a single input argument is defined which is never used
     def keepVariablesFeasible(_ = None):
```

### Comparing `pyees-1.2.2/pyees/stackOverflowODR.py` & `pyees-1.2.3/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testFit.py` & `pyees-1.2.3/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testProp.py` & `pyees-1.2.3/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testPyees.py` & `pyees-1.2.3/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testReadData.py` & `pyees-1.2.3/pyees/testReadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,45 +27,54 @@
         np.testing.assert_array_equal(dat.b.uncert, [0, 0, 0, 0, 0])
 
         # csv file
         with self.assertRaises(Exception) as context:
             dat = sheetsFromFile('testData/data1.csv', 'A-B')
         self.assertTrue("The file extension is not supported. The supported extension are ['.xls', '.xlsx']" in str(context.exception))
 
-    def testReadUncertanty(self):
+    def testUncertMatrixVsCovarianceMatrix(self):
+        dat1 = sheetsFromFile('testData/data2.xlsx', 'A-B', 'C-D')
+        dat2 = sheetsFromFile('testData/data2.xlsx', 'A-B', 'G-H')
+        c1 = dat1.a * dat1.b
+        c2 = dat2.a * dat2.b
+        np.testing.assert_array_equal(c1.value, c2.value)
+        self.assertEqual(c1.unit, c2.unit)
+        np.testing.assert_array_equal(c1.uncert, c2.uncert)
+                
+    def testReadUncertanty(self):        
         dat = sheetsFromFile('testData/data3.xlsx', 'A-B', 'C-D')
         np.testing.assert_array_equal(dat.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.a.unit), 'm')
         np.testing.assert_array_equal(dat.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25])
         np.testing.assert_array_equal(dat.b.value, [5, 6, 7, 8, 9])
         self.assertEqual(str(dat.b.unit), 'mA')
         np.testing.assert_array_equal(dat.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9])
 
         dat = sheetsFromFile('testData/data4.xlsx', 'A-B', 'C-D')
         np.testing.assert_array_equal(dat.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat.a.uncert, np.sqrt([0.05, 0.1, 0.15, 0.2, 0.25]))
         np.testing.assert_almost_equal([elemA.covariance[elemB] for elemA, elemB in zip(dat.a, dat.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
         np.testing.assert_array_equal(dat.b.value, [5, 6, 7, 8, 9])
         self.assertEqual(str(dat.b.unit), 'mA')
-        np.testing.assert_array_equal(dat.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_array_equal(dat.b.uncert, np.sqrt([0.5, 0.6, 0.7, 0.8, 0.9]))
         np.testing.assert_almost_equal([elemB.covariance[elemA] for elemA, elemB in zip(dat.a, dat.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
 
         with self.assertRaises(Exception) as context:
             sheetsFromFile('testData/data6.xlsx', 'A-B', 'C-D')
         self.assertTrue("The covariances has to be symmetric" in str(context.exception))
 
         dat = sheetsFromFile('testData/data5.xlsx', dataRange="B-C", uncertRange="H-I")
         np.testing.assert_array_equal(dat.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat.a.uncert, np.sqrt([0.05, 0.1, 0.15, 0.2, 0.25]))
         np.testing.assert_almost_equal([elemA.covariance[elemC] for elemA, elemC in zip(dat.a, dat.c)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
         np.testing.assert_array_equal(dat.c.value, [5, 6, 7, 8, 9])
         self.assertEqual(str(dat.c.unit), 'mA')
-        np.testing.assert_array_equal(dat.c.uncert, [0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_array_equal(dat.c.uncert, np.sqrt([0.5, 0.6, 0.7, 0.8, 0.9]))
         np.testing.assert_almost_equal([elemC.covariance[elemA] for elemA, elemC in zip(dat.a, dat.c)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
         
         dat = sheetsFromFile('testData/data5.xlsx', dataRange="B-C", uncertRange="K-L")
         np.testing.assert_array_equal(dat.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.a.unit), 'L/min')
         np.testing.assert_array_equal(dat.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25])
         for elemA, elemC in zip(dat.a, dat.c):
@@ -102,49 +111,49 @@
         self.assertTrue("You can not set an element of [1, 2, 3, 4, 5] [m] with [1, 2, 3, 4, 5] [L/min] as they do not have the same unit" in str(context.exception))
 
         dat2 = sheetsFromFile('testData/data2.xlsx', 'A-B', 'C-D')
         dat4 = sheetsFromFile('testData/data4.xlsx', 'A-B', 'C-D')
         dat2.append(dat4)
         np.testing.assert_array_equal(dat2.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
         self.assertEqual(str(dat2.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat2.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat2.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05**(1/2), 0.1**(1/2), 0.15**(1/2), 0.2**(1/2), 0.25**(1/2)])
         np.testing.assert_array_equal(dat2.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat2.b.unit), 'mA')
-        np.testing.assert_array_equal(dat2.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_array_equal(dat2.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5**(1/2), 0.6**(1/2), 0.7**(1/2), 0.8**(1/2), 0.9**(1/2)])
         cov = np.array([0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 1000
         for i, (elemA, elemB) in enumerate(zip(dat2.a, dat2.b)):
             if elemB in elemA.covariance:
                 self.assertAlmostEqual(elemA.covariance[elemB], cov[i])
                 self.assertAlmostEqual(elemB.covariance[elemA], cov[i])
                 
             
         dat2 = sheetsFromFile('testData/data2.xlsx', 'A-B', 'C-D')
         dat4 = sheetsFromFile('testData/data4.xlsx', 'A-B', 'C-D')
         dat4.append(dat2)
         np.testing.assert_array_equal(dat4.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
         self.assertEqual(str(dat4.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat4.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat4.a.uncert, [0.05**(1/2), 0.1**(1/2), 0.15**(1/2), 0.2**(1/2), 0.25**(1/2), 0.05, 0.1, 0.15, 0.2, 0.25])
         np.testing.assert_array_equal(dat4.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat4.b.unit), 'mA')
-        np.testing.assert_array_equal(dat4.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_array_equal(dat4.b.uncert, [0.5**(1/2), 0.6**(1/2), 0.7**(1/2), 0.8**(1/2), 0.9**(1/2), 0.5, 0.6, 0.7, 0.8, 0.9])
         cov = np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0]) / 1000 / 60 / 1000
         for i, (elemA, elemB) in enumerate(zip(dat4.a, dat4.b)):
             if elemB in elemA.covariance:
                 self.assertAlmostEqual(elemA.covariance[elemB], cov[i])
                 self.assertAlmostEqual(elemB.covariance[elemA], cov[i])
        
         dat4_1 = sheetsFromFile('testData/data4.xlsx', 'A-B', 'C-D')
         dat4_2 = sheetsFromFile('testData/data4.xlsx', 'A-B', 'C-D')
         dat4_1.append(dat4_2)
         np.testing.assert_array_equal(dat4_1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
         self.assertEqual(str(dat4_1.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat4_1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat4_1.a.uncert, np.sqrt([0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25]))
         np.testing.assert_array_equal(dat4_1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat4_1.b.unit), 'mA')
-        np.testing.assert_array_equal(dat4_1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_array_equal(dat4_1.b.uncert, np.sqrt([0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9]))
         np.testing.assert_almost_equal([elemA.covariance[elemB] for elemA, elemB in zip(dat4_1.a, dat4_1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 6000)
         np.testing.assert_almost_equal([elemB.covariance[elemA] for elemA, elemB in zip(dat4_1.a, dat4_1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 6000)
 
     def testIndex(self):
         dat = sheetsFromFile('testData/data1.xlsx', 'A-B')
         np.testing.assert_array_equal(dat.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.a.unit), 'L/min')
```

### Comparing `pyees-1.2.2/pyees/testSolve.py` & `pyees-1.2.3/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testUnit.py` & `pyees-1.2.3/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/testVariable.py` & `pyees-1.2.3/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/unit.py` & `pyees-1.2.3/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.2/pyees/variable.py` & `pyees-1.2.3/pyees/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
             raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
         
         covUnit = unit(unitStr)
         selfVarUnit = unit(self._unitObject * var._unitObject)
         if not unit._assertEqualStatic(covUnit._SIBaseUnit, selfVarUnit._SIBaseUnit):
             raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
         
-        covariance = covUnit._converterToSI.convert(covariance, useOffset=False)
+        covariance *=  self._converterToSI.convert(1, useOffset=False) * var._converterToSI.convert(1, useOffset=False)
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
     def _calculateUncertanty(self):
  
         # variance from each measurement
@@ -274,15 +274,19 @@
         ## from the above the gradients can be found from self.dependsOn
         
         for var1 in self.dependsOn.keys():
             for var2 in var1.covariance.keys():
                 if var2 in self.dependsOn:
                     grad1 = self.dependsOn[var1][1]
                     grad2 = self.dependsOn[var2][1]
-                    variance += scale**2 * grad1 * grad2 * var1.covariance[var2]
+                    s = scale**2 
+                    cov = var1.covariance[var2]
+                    term = s * grad1 * grad2 * cov
+                    variance += term
+                    # variance += scale**2 * grad1 * grad2 * var1.covariance[var2]
 
         self._uncert = np.sqrt(variance)
         
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
@@ -997,13 +1001,32 @@
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 
 if __name__ == "__main__":
-    A = variable(0.003, 'L/min', 0.2)
-    print(A)
-    a = variable(0.9, '', 3)
-    print(a)    
+  
+    # value  
+    # [0.02994473968569557, 0.212143804427421, 1.8607179520279966]
+
+    # cov
+    # [[ 2.91453531e-06 -3.25319114e-04  7.98892818e-03]
+    #  [-3.25319114e-04  3.72796202e-02 -9.34366573e-01]
+    #  [ 7.98892818e-03 -9.34366573e-01  2.40059033e+01]]
+
+
+    b = variable(0.212143804427421, 'mbar-min/L', np.sqrt(3.72796202e-02))
+    c = variable(1.8607179520279966, 'mbar', np.sqrt(2.40059033e+01))
     
+    b.addCovariance(c, -9.34366573e-01, 'mbar2-min/L')
     
+    flow = variable(100,'L/min')
+    
+    dp = b*flow + c
+
+    print(dp)
+    
+    
+    
+
+## TODO major error - use sheet 1 in PS 2312-1: calculation flow1 - flow2. The covariance will create a negative varianace - and return an uncertanty of nan
```

### Comparing `pyees-1.2.2/pyees.egg-info/PKG-INFO` & `pyees-1.2.3/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.2
+Version: 1.2.3
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.2/setup.py` & `pyees-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.2',
+    version='1.2.3',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```


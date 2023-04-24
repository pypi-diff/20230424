# Comparing `tmp/pymathematics-2023.4.23.1.tar.gz` & `tmp/pymathematics-2023.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.23.1.tar", last modified: Sun Apr 23 06:56:34 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.24.tar", last modified: Mon Apr 24 17:34:56 2023, max compression
```

## Comparing `pymathematics-2023.4.23.1.tar` & `pymathematics-2023.4.24.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:34.095297 pymathematics-2023.4.23.1/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.23.1/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-23 06:56:34.087298 pymathematics-2023.4.23.1/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      125 2023-04-23 06:52:17.000000 pymathematics-2023.4.23.1/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:33.800295 pymathematics-2023.4.23.1/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    18612 2023-04-23 06:50:52.000000 pymathematics-2023.4.23.1/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-23 06:51:57.000000 pymathematics-2023.4.23.1/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:34.028296 pymathematics-2023.4.23.1/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-23 06:56:34.097298 pymathematics-2023.4.23.1/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      691 2023-04-23 06:52:12.000000 pymathematics-2023.4.23.1/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.541397 pymathematics-2023.4.24/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.24/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-24 17:34:56.525775 pymathematics-2023.4.24/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-24 17:29:32.000000 pymathematics-2023.4.24/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.275771 pymathematics-2023.4.24/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    20051 2023-04-24 17:29:11.000000 pymathematics-2023.4.24/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-24 17:29:17.000000 pymathematics-2023.4.24/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-24 17:34:56.478916 pymathematics-2023.4.24/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-24 17:34:53.000000 pymathematics-2023.4.24/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-24 17:34:54.000000 pymathematics-2023.4.24/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-24 17:34:56.541397 pymathematics-2023.4.24/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-24 17:29:26.000000 pymathematics-2023.4.24/setup.py
```

### Comparing `pymathematics-2023.4.23.1/LICENSE` & `pymathematics-2023.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.23.1/pymathematics/__init__.py` & `pymathematics-2023.4.24/pymathematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,20 @@
     elif number == 0:
         return 0
     flag = number/2
     while absolute(flag*flag - number) > 0.00001:
         flag = (flag + number/flag)/2
     return flag
 
+def cbrt(number:int|float) -> float:
+    flag = number/3
+    while absolute(flag**3 - number) > 0.0001:
+        flag = (2*flag+number/flag**2)/3
+    return flag
+
 def quadratic_roots(coefficients:list) -> list:
     if len(coefficients) != 3:
         raise ValueError("there should be only 3 coefficients!")
     D = coefficients[0]**2-4*coefficients[0]*coefficients[2]
     if D < 0:
         x1 = f"{-coefficients[1]} + {sqrt(absolute(D))}i"
         x2 = f"{-coefficients[1]} - {sqrt(absolute(D))}i"
@@ -265,15 +271,14 @@
                 mid = (left+right)/2
                 if 10**mid < number:
                     left = mid
                 else:
                     right = mid
             return n+left
 
-
 def ln(number:int|float) -> int|float:
     """
     `log(number) to the base e`
     """
     if number <= 0:
         raise ValueError("domain error")
     return 2.303*log(number)
@@ -425,14 +430,37 @@
     if len(array1) == len(array2):
         return summation([array1[x]+array2[x] for x in range(array1)])
     raise ValueError(f"length of array1 and array2 aren't equal {len(array1)} != {array2}")
 
 def zscore(array:list,number:int) -> int|float:
     return (number-mean(array))*standard_deviation(array)
 
+def euclidean_distance(array1:list,array2:list) -> float:
+    if len(array1) < len(array2) < 3:
+        raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
+    return sqrt(summation([(array1[x] - array2[x])**2 for x in range(len(array1))]))
+
+def manhattan_distance(array1:list,array2:list) -> float:
+    if len(array1) < len(array2) < 3:
+        raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
+    return summation([absolute(array1[x] - array2[x]) for x in range(len(array1))])
+
+def camberra_distance(array1:list,array2:list) -> float:
+    if len(array1) < len(array2) < 3:
+        raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
+    return summation([absolute(array1[x] - array2[x])/(absolute(array1[x] + array2[x])) for x in range(len(array1))])
+
+def minkowski_distance(array1:list,array2:list,power:int|float) -> float:
+    if len(array1) < len(array2) < 3:
+        raise ValueError("arrays must have the same length and have atleast 3 coordinates both x and y")
+    distance = 0
+    for i in range(len(array1)):
+        distance += absolute(array1[i] - array2[i])**power
+    return distance**(1/power)
+
 def moving_average(array:list,steps:int) -> list:
     if steps <= 0:
         raise ValueError(f"steps must be greater than zero {steps} < {0}")
     if len(array) < steps:
         raise ValueError(f"invalid input {steps} > {len(array)}! array must have atleast as many elements as the number of steps!")
     avgs = []
     for i in range(len(array)-steps+1):
```

### Comparing `pymathematics-2023.4.23.1/setup.py` & `pymathematics-2023.4.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.23.1",
+    version = "2023.4.24",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```


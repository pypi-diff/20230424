# Comparing `tmp/proteinTools-1.3.1.tar.gz` & `tmp/proteinTools-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.3.1.tar", last modified: Mon Apr 24 01:01:09 2023, max compression
+gzip compressed data, was "proteinTools-1.3.2.tar", last modified: Mon Apr 24 17:32:45 2023, max compression
```

## Comparing `proteinTools-1.3.1.tar` & `proteinTools-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.346228 proteinTools-1.3.1/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.1/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 01:01:09.343443 proteinTools-1.3.1/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.1/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.280420 proteinTools-1.3.1/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    52955 2023-04-24 00:59:33.000000 proteinTools-1.3.1/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.1/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.327768 proteinTools-1.3.1/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-24 01:01:09.349979 proteinTools-1.3.1/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-24 00:27:20.000000 proteinTools-1.3.1/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.535031 proteinTools-1.3.2/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.2/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 17:32:45.531756 proteinTools-1.3.2/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.2/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.466620 proteinTools-1.3.2/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    52956 2023-04-24 17:31:02.000000 proteinTools-1.3.2/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.2/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.516576 proteinTools-1.3.2/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-24 17:32:45.539361 proteinTools-1.3.2/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-24 17:32:26.000000 proteinTools-1.3.2/setup.py
```

### Comparing `proteinTools-1.3.1/LICENSE` & `proteinTools-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.3.1/proteinTools/PT.py` & `proteinTools-1.3.2/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
                     print(self.protein + ' not found in any libraries!')
         
         #Atomizes protein file
         os.chdir(destination)
         if self.cif == False:
             with open(self.protein + '.pdb', 'r') as f:
                 data = f.readlines()
-            self.residue_list, curr_residue, curr_lig, currnum, curr_chain = [], -1, '', 0, ''
+            self.residue_list, curr_residue, curr_lig, currnum, curr_chain = [], -.5, '', 0, ''
             if self.ID_type == 'PDB':
                 current_ligand_index, self.ligand_list = -1, []
             for count, line in enumerate(data):
                 if line[0:6] == 'SEQRES':
                     chain = line[11:12]
                     if curr_chain != chain:
                         curr_chain = chain
```

### Comparing `proteinTools-1.3.1/setup.py` & `proteinTools-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.3.1",
+    version = "1.3.2",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```


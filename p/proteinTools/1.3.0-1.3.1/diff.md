# Comparing `tmp/proteinTools-1.3.0.tar.gz` & `tmp/proteinTools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.3.0.tar", last modified: Fri Apr 21 07:36:53 2023, max compression
+gzip compressed data, was "proteinTools-1.3.1.tar", last modified: Mon Apr 24 01:01:09 2023, max compression
```

## Comparing `proteinTools-1.3.0.tar` & `proteinTools-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 07:36:53.487050 proteinTools-1.3.0/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.0/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-21 07:36:53.484286 proteinTools-1.3.0/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.0/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 07:36:53.415424 proteinTools-1.3.0/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    52045 2023-04-21 07:36:44.000000 proteinTools-1.3.0/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.0/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 07:36:53.468773 proteinTools-1.3.0/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-21 07:36:53.000000 proteinTools-1.3.0/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-21 07:36:53.000000 proteinTools-1.3.0/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-21 07:36:53.000000 proteinTools-1.3.0/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-21 07:36:53.000000 proteinTools-1.3.0/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-21 07:36:53.000000 proteinTools-1.3.0/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-21 07:36:53.492759 proteinTools-1.3.0/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-21 07:36:13.000000 proteinTools-1.3.0/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.346228 proteinTools-1.3.1/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.1/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 01:01:09.343443 proteinTools-1.3.1/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.1/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.280420 proteinTools-1.3.1/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    52955 2023-04-24 00:59:33.000000 proteinTools-1.3.1/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.1/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 01:01:09.327768 proteinTools-1.3.1/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-24 01:01:09.000000 proteinTools-1.3.1/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-24 01:01:09.349979 proteinTools-1.3.1/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-24 00:27:20.000000 proteinTools-1.3.1/setup.py
```

### Comparing `proteinTools-1.3.0/LICENSE` & `proteinTools-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.3.0/proteinTools/PT.py` & `proteinTools-1.3.1/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,17 +430,20 @@
                             try:
                                 AA = InverseFASTAdict[AA.strip()]
                             except:
                                 pass
                                 
                         res = residue(amino_acid = AA, index = resnum, chain = chain)
                         self.residue_list.append(res)
-                    element = line[77:79].strip()
+                    element = line[76:79].strip()
                     if element not in atom_keys:
-                        element = element[:1]
+                        e = element[:1]
+                        if e not in atom_keys:
+                            e = element[1:]
+                        element = e
                     try:
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line)
                     except:
                         atm = atom(element, float(line[30:37].strip()), float(line[38:46].strip()), float(line[47:55].strip()), residue = res.chain + str(resnum), data = line)
                     res.atoms.append(atm)
             
             
@@ -455,20 +458,29 @@
                         if ligands != curr_lig:
                             lignum = int(line[22:27])
                             if lignum != currnum:
                                 currnum = lignum
                                 lig = ligand(ligands)
                                 self.ligand_list.append(lig)
                                 current_ligand_index += 1
-                            element = line[76:80].strip()
+                        element = line[76:80].strip()
                         if element not in atom_keys:
-                            element = element[:1]
+                            e = element[:1]
+                            if e not in atom_keys:
+                                e = element[1:]
+                            element = e
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
-                        self.ligand_list[current_ligand_index].atoms.append(atm)
-                     
+                        try:
+                            self.ligand_list[current_ligand_index].atoms.append(atm)
+                        except:
+                            try:
+                                 self.ligand_list[current_ligand_index + 1].atoms.append(atm)
+                            except:
+                                 continue
+                            
                     #Queries secondary structure  
                     elif line[0:5] == 'SHEET':
                         #line = [i for i in line.split(' ') if i != '']
                         try:
                             start = int(numconv.sub('', line[22:27]))
                             end = int(numconv.sub('', line[34:39]))
                             chain = line[19:20]
@@ -544,24 +556,30 @@
                     self.chains[letters[chain_num]] = int(line[1])
                     break
                     
             #Obtains residues from protein file
             self.residue_list, curr_residue = [], -1
             for count, line in enumerate(data):
                 if line[0:4] == 'ATOM':
-                    resnum = int(line[33:37].strip())
+                    try:
+                        resnum = int(line[33:37].strip())
+                    except:
+                        resnum = int(numconv.sub('', line[34:37].strip()))
                     if resnum != curr_residue:
                         curr_residue = resnum
                         chain, AA = line[28:29], line[24:27]
                         res = residue(amino_acid = AA, index = resnum, chain = chain)
                         self.residue_list.append(res)
                     element = line[14:16].strip()
                     if element not in atom_keys:
                         element = element[:1]
-                    atm = atom(element, float(line[39:47].strip()), float(line[47:55].strip()), float(line[55:63].strip()), residue = res.chain + str(resnum), data = line)
+                    try:
+                        atm = atom(element, float(line[39:47].strip()), float(line[47:55].strip()), float(line[55:63].strip()), residue = res.chain + str(resnum), data = line)
+                    except:
+                        atm = atom(element, float(line[34:41].strip()), float(line[42:50].strip()), float(line[50:59].strip()), residue = res.chain + str(resnum), data = line)
                     res.atoms.append(atm)
                     
         #Strips binding sites if available
         counter, firstRun, curr_site, sites = 0, True, '', []
         if self.ID_type == 'PDB' and self.cif == False:
             ligands = []
             for myligand in self.ligand_list:
```

### Comparing `proteinTools-1.3.0/setup.py` & `proteinTools-1.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.3.0",
+    version = "1.3.1",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```


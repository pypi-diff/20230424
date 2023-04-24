# Comparing `tmp/openPMD-validator-1.1.0.3.tar.gz` & `tmp/openPMD-validator-1.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openPMD-validator-1.1.0.3.tar", last modified: Wed Apr  6 17:05:43 2022, max compression
+gzip compressed data, was "openPMD-validator-1.1.0.4.tar", last modified: Mon Apr 24 19:01:33 2023, max compression
```

## Comparing `openPMD-validator-1.1.0.3.tar` & `openPMD-validator-1.1.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2022-04-06 17:05:43.576316 openPMD-validator-1.1.0.3/
--rw-rw-r--   0 axel      (1000) axel      (1000)     4933 2022-04-06 17:05:43.576316 openPMD-validator-1.1.0.3/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     3399 2022-04-06 17:04:59.000000 openPMD-validator-1.1.0.3/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2022-04-06 17:05:43.576316 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/
--rw-r--r--   0 axel      (1000) axel      (1000)     4933 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/PKG-INFO
--rw-r--r--   0 axel      (1000) axel      (1000)      365 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/SOURCES.txt
--rw-r--r--   0 axel      (1000) axel      (1000)        1 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/dependency_links.txt
--rw-r--r--   0 axel      (1000) axel      (1000)      139 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/entry_points.txt
--rw-r--r--   0 axel      (1000) axel      (1000)       48 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/requires.txt
--rw-r--r--   0 axel      (1000) axel      (1000)       18 2022-04-06 17:05:43.000000 openPMD-validator-1.1.0.3/openPMD_validator.egg-info/top_level.txt
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2022-04-06 17:05:43.576316 openPMD-validator-1.1.0.3/openpmd_validator/
--rw-r--r--   0 axel      (1000) axel      (1000)        0 2017-11-24 09:50:14.000000 openPMD-validator-1.1.0.3/openpmd_validator/__init__.py
--rwxrwxr-x   0 axel      (1000) axel      (1000)    38119 2022-04-06 17:04:59.000000 openPMD-validator-1.1.0.3/openpmd_validator/check_h5.py
--rwxrwxr-x   0 axel      (1000) axel      (1000)    24005 2022-04-06 17:04:59.000000 openPMD-validator-1.1.0.3/openpmd_validator/createExamples_h5.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2022-04-06 17:05:43.576316 openPMD-validator-1.1.0.3/setup.cfg
--rw-rw-r--   0 axel      (1000) axel      (1000)     1351 2022-04-06 17:04:59.000000 openPMD-validator-1.1.0.3/setup.py
+drwxrwxr-x   0 axel      (1001) axel      (1001)        0 2023-04-24 19:01:33.362427 openPMD-validator-1.1.0.4/
+-rw-r--r--   0 axel      (1001) axel      (1001)      744 2017-12-01 22:08:44.000000 openPMD-validator-1.1.0.4/LICENSE.txt
+-rw-rw-r--   0 axel      (1001) axel      (1001)     3992 2023-04-24 19:01:33.362427 openPMD-validator-1.1.0.4/PKG-INFO
+-rw-rw-r--   0 axel      (1001) axel      (1001)     3399 2023-04-24 18:56:44.000000 openPMD-validator-1.1.0.4/README.md
+drwxrwxr-x   0 axel      (1001) axel      (1001)        0 2023-04-24 19:01:33.362427 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/
+-rw-r--r--   0 axel      (1001) axel      (1001)     3992 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/PKG-INFO
+-rw-r--r--   0 axel      (1001) axel      (1001)      377 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 axel      (1001) axel      (1001)        1 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 axel      (1001) axel      (1001)      138 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/entry_points.txt
+-rw-r--r--   0 axel      (1001) axel      (1001)       48 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/requires.txt
+-rw-r--r--   0 axel      (1001) axel      (1001)       18 2023-04-24 19:01:33.000000 openPMD-validator-1.1.0.4/openPMD_validator.egg-info/top_level.txt
+drwxrwxr-x   0 axel      (1001) axel      (1001)        0 2023-04-24 19:01:33.362427 openPMD-validator-1.1.0.4/openpmd_validator/
+-rw-r--r--   0 axel      (1001) axel      (1001)        0 2017-11-24 09:50:14.000000 openPMD-validator-1.1.0.4/openpmd_validator/__init__.py
+-rwxrwxr-x   0 axel      (1001) axel      (1001)    38149 2023-04-24 18:53:28.000000 openPMD-validator-1.1.0.4/openpmd_validator/check_h5.py
+-rwxrwxr-x   0 axel      (1001) axel      (1001)    24009 2023-04-24 18:56:14.000000 openPMD-validator-1.1.0.4/openpmd_validator/createExamples_h5.py
+-rw-rw-r--   0 axel      (1001) axel      (1001)       38 2023-04-24 19:01:33.362427 openPMD-validator-1.1.0.4/setup.cfg
+-rw-rw-r--   0 axel      (1001) axel      (1001)     1351 2023-04-24 18:56:48.000000 openPMD-validator-1.1.0.4/setup.py
```

### Comparing `openPMD-validator-1.1.0.3/README.md` & `openPMD-validator-1.1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,36 +39,36 @@
 
 Choose *one* of the install methods below to get started:
 
 ### PyPI
 
 ```bash
 # optional: append --user
-pip install openPMD-validator==1.1.0.3
+pip install openPMD-validator==1.1.0.4
 ```
 
 ### Spack
 
 ```bash
-spack install py-openpmd-validator@1.1.0.3 ^py-h5py~mpi
-spack load --dependencies py-openpmd-validator@1.1.0.3 ^py-h5py~mpi
+spack install py-openpmd-validator@1.1.0.4 ^py-h5py~mpi
+spack load --dependencies py-openpmd-validator@1.1.0.4 ^py-h5py~mpi
 ```
 
 ### Conda
 
 ```bash
-conda install -c ax3l openpmd_validator==1.1.0.3
+conda install -c ax3l openpmd_validator==1.1.0.4
 ```
 
 ### From Source
 
 ```bash
-wget https://github.com/openPMD/openPMD-validator/archive/1.1.0.3.tar.gz
-tar -xf 1.1.0.3.tar.gz
-cd openPMD-validator-1.1.0.3/
+wget https://github.com/openPMD/openPMD-validator/archive/1.1.0.4.tar.gz
+tar -xf 1.1.0.4.tar.gz
+cd openPMD-validator-1.1.0.4/
 
 # optional: append --user
 python setup.py install
 ```
 
 ## Usage
```

### Comparing `openPMD-validator-1.1.0.3/openpmd_validator/check_h5.py` & `openPMD-validator-1.1.0.4/openpmd_validator/check_h5.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,15 @@
                 else : # Vector record
                     # Loop over the components
                     for component_name in list(species[record].keys()):
                         dset = species[ join_path(record, component_name) ]
                         result_array += test_component(dset, v)
 
             # weighting's attributes are fixed
-            if record == "weighting" and result_array[0] == 0:
+            if extensionStates['ED-PIC'] and record == "weighting" and result_array[0] == 0:
                 valid, unitSI = get_attr(species[record], "unitSI")
                 if valid:
                     if not np.isclose(unitSI, 1.0):
                         print("Error: `unitSI` attribute of `weighting` "
                               "record must be `1.0` in species `{0}`! "
                               "Its value is: {1}"
                               .format(species.name, unitSI))
```

### Comparing `openPMD-validator-1.1.0.3/openpmd_validator/createExamples_h5.py` & `openPMD-validator-1.1.0.4/openpmd_validator/createExamples_h5.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     f.attrs["particlesPath"] = np.string_("particles/")
     f.attrs["iterationEncoding"] = np.string_("groupBased")
     f.attrs["iterationFormat"] = np.string_("/data/%T/")
 
     # Recommended attributes
     f.attrs["author"] = np.string_("Axel Huebl <a.huebl@hzdr.de>")
     f.attrs["software"] = np.string_("openPMD Example Script")
-    f.attrs["softwareVersion"] = np.string_("1.1.0.3")
+    f.attrs["softwareVersion"] = np.string_("1.1.0.4")
     f.attrs["softwareDependencies"] = get_software_dependencies()
     f.attrs["machine"] = np.string_(socket.gethostname())
     f.attrs["date"] = np.string_(
         datetime.datetime.now(tzlocal()).strftime('%Y-%m-%d %H:%M:%S %z'))
 
     # Optional
     f.attrs["comment"] = np.string_("This is a dummy file for test purposes.")
@@ -226,17 +226,17 @@
     B["y"].attrs["unitSI"] = np.float64(3.3)
     B["z"].attrs["unitSI"] = np.float64(3.3)
 
     # Fill the array with the field data
     #   the constant record components B.x and B.y have the same shape
     #   (== same mesh discretization) as the non-constant record
     #   component B.z
-    B["x"].attrs["value"] = np.float(0.0)
+    B["x"].attrs["value"] = np.float64(0.0)
     B["x"].attrs["shape"] = np.array(data_ez.shape, dtype=np.uint64)
-    B["y"].attrs["value"] = np.float(0.0)
+    B["y"].attrs["value"] = np.float64(0.0)
     B["y"].attrs["shape"] = np.array(data_ez.shape, dtype=np.uint64)
     B["z"][:,:] =  data_ez[:,:]
 
 def write_e_2d_cartesian(meshes, data_ex, data_ey, data_ez ):
     """
     Write the metadata and the data associated with the vector field E,
     using a 2d Cartesian representation
```

### Comparing `openPMD-validator-1.1.0.3/setup.py` & `openPMD-validator-1.1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read_readme():
     with open('./README.md', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='openPMD-validator',
-    version='1.1.0.3',
+    version='1.1.0.4',
     url='https://github.com/openPMD/openPMD-validator',
     # author=...,  # TODO
     # author_email=...,  # TODO
     # maintainer=...,  # TODO
     # maintainer_email=...,  # TODO
     license='ISC',
     install_requires=read_requirements(),
```


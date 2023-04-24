# Comparing `tmp/riscv_config-3.7.2.tar.gz` & `tmp/riscv_config-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_config-3.7.2.tar", last modified: Fri Apr  7 06:06:00 2023, max compression
+gzip compressed data, was "dist/riscv_config-3.8.0.tar", last modified: Mon Apr 24 03:40:11 2023, max compression
```

## Comparing `riscv_config-3.7.2.tar` & `riscv_config-3.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:06:00.000000 riscv_config-3.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 06:05:42.000000 riscv_config-3.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-07 06:06:00.000000 riscv_config-3.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 06:05:42.000000 riscv_config-3.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92172 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/isa_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/schemaValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/schemas/schema_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   533283 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/schemas/schema_isa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/schemas/schema_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-07 06:05:42.000000 riscv_config-3.7.2/riscv_config/warl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 06:06:00.000000 riscv_config-3.7.2/riscv_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 06:06:00.000000 riscv_config-3.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-07 06:05:42.000000 riscv_config-3.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 03:39:49.000000 riscv_config-3.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 03:40:11.000000 riscv_config-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 03:39:49.000000 riscv_config-3.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93762 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/isa_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemaValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_isa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/warl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 03:40:11.000000 riscv_config-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-24 03:39:49.000000 riscv_config-3.8.0/setup.py
```

### Comparing `riscv_config-3.7.2/PKG-INFO` & `riscv_config-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv_config
-Version: 3.7.2
+Version: 3.8.0
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
@@ -15,8 +15,8 @@
         
         Latest Documentation of RISCV-Config: `HTML <https://riscv-config.readthedocs.io/>`_
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
```

### Comparing `riscv_config-3.7.2/riscv_config/checker.py` & `riscv_config-3.8.0/riscv_config/checker.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,220 +8,259 @@
 
 import itertools
 import riscv_config.utils as utils
 from riscv_config.errors import ValidationError
 from riscv_config.schemaValidator import schemaValidator
 import riscv_config.constants as constants
 from riscv_config.warl import warl_class
+from riscv_config.isa_validator import *
 
 logger = logging.getLogger(__name__)
 
 
 def reset():
     '''Function to set defaults to reset val of misa  based on presence of ISA extensions.'''
     global inp_yaml
     global extensions
     extension_enc = list("00000000000000000000000000")
     value=inp_yaml['ISA']
+    global extension_list
+    global ext_err
+    global ext_err_list
+    (extension_list, ext_err, ext_err_list) = get_extension_list(value)
     if "32" in value:
        xlen = 32
        ext = value[4:]
     elif "64" in value:
        xlen = 64
        ext = value[4:]
     elif "128" in value:
        xlen = 128
        ext = value[5:]
     for x in "ABCDEFHIJKLMNPQSTUVX":
-            if (x in ext):
+            if (x in extension_list):
                 extension_enc[25 - int(ord(x) - ord('A'))] = "1"
     extensions = int("".join(extension_enc), 2)
     ext_b=format(extensions, '#0{}b'.format(xlen+2))
     mxl='10'if xlen==64 else '01'
     ext_b = ext_b[:2] + str(mxl) + ext_b[4:]
     return int(ext_b, 2)
-    
+ 
 def resetsu():
     '''Function to set defaults to reset val of mstatus based on the xlen and S, U extensions'''
     global inp_yaml
-    if 64 in inp_yaml['supported_xlen'] and 'S' not in inp_yaml['ISA'] and 'U' in inp_yaml['ISA']:
+    global extension_list
+    if 64 in inp_yaml['supported_xlen'] and 'S' not in extension_list and 'U' in extension_list:
       return 8589934592
-    elif 64 in inp_yaml['supported_xlen'] and 'U' in inp_yaml['ISA'] and 'S' in inp_yaml['ISA']:
+    elif 64 in inp_yaml['supported_xlen'] and 'U' in extension_list and 'S' in extension_list:
       return 42949672960
     else:	
       return 0
 def reset_vsstatus():
     '''Function to set defaults to reset val of mstatus based on the xlen and S, U extensions'''
     global inp_yaml
-    if 64 in inp_yaml['supported_xlen'] and 'U' in inp_yaml['ISA']:
+    global extension_list
+    if 64 in inp_yaml['supported_xlen'] and 'U' in extension_list:
       return 8589934592
     else:	
       return 0
 
 def uset():
     '''Function to set defaults based on presence of 'U' extension.'''
-    global inp_yaml
-    if 'U' in inp_yaml['ISA']:
+    global extension_list
+    if 'U' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
    
 def hset():
     '''Function to set defaults based on presence of 'U' extension.'''
-    global inp_yaml
-    if 'H' in inp_yaml['ISA']:
+    global extension_list
+    if 'H' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
 
 
 def sset():
     '''Function to set defaults based on presence of 'S' extension.'''
-    global inp_yaml
-    if 'S' in inp_yaml['ISA']:
+    global extension_list
+    if 'S' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
         
 def fsset():
     '''Function to set defaults based on presence of 'F' extension.'''
-    global inp_yaml
-    if 'F' in inp_yaml['ISA'] or 'S' in inp_yaml['ISA']:
+    global extension_list
+    if 'F' in extension_list or 'S' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
         
 
 def uregset():
     '''Function to set defaults based on presence of 'U' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'U' in inp_yaml['ISA']:
+    if 'U' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
       if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
 
 def uregseth():
     '''Function to set defaults based on presence of 'U' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'U' in inp_yaml['ISA']:
+    if 'U' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     return temp
   
 def hregseth():
     '''Function to set defaults based on presence of 'H' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'H' in inp_yaml['ISA']:
+    if 'H' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     return temp      
 def sregset():
     '''Function to set defaults based on presence of 'S' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'S' in inp_yaml['ISA']:
+    if 'S' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
       if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
 
 def nregset():
     '''Function to set defaults based on presence of 'N' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'N' in inp_yaml['ISA']:
+    if 'N' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
       if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
 
 def hregset():
     '''Function to set defaults based on presence of 'H' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'H' in inp_yaml['ISA']:
+    if 'H' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
       if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
     
 def sregseth():
     '''Function to set defaults based on presence of 'S' extension.'''
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'S' in inp_yaml['ISA']:
+    if 'S' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     return temp
 
 
 def nuset():
     '''Function to check and set defaults for all fields which are dependent on
         the presence of 'U' extension and 'N' extension.'''
-    global inp_yaml
-    if 'U' in inp_yaml['ISA'] and 'N' in inp_yaml['ISA']:
+    global extension_list
+    if 'U' in extension_list and 'N' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
 
+def smrnmi_reset():
+  global inp_yaml
+  if 64 in inp_yaml['supported_xlen']:
+    return 0x8000000000000000
+  else:
+    return 0x80000000
+
+def smrnmi_set():
+    '''Function to check and set defaults for all fields which are dependent on
+        the presence of Smrnmi extension'''
+    global inp_yaml
+    global extension_list
+
+    temp = { 'rv32': {'accessible': False},
+             'rv64': {'accessible': False}
+           }
+    if 'Smrnmi' in extension_list:
+        if 32 in inp_yaml['supported_xlen']:
+            temp['rv32']['accessible'] = True
+        else :
+            temp['rv64']['accessible'] = True
+    return temp
 
 def pset():
     '''Function to check and set defaults for all fields which are dependent on
         the presence of P-SIMD sub-extension viz. zpn, zpsf, zbpbo'''
     global inp_yaml
+    global extension_list
 
     temp = { 'rv32': {'accessible': False , 'ov': {'implemented': False}},
              'rv64': {'accessible': False , 'ov': {'implemented': False}}
            }
-    if 'Zpn' in inp_yaml['ISA']:
+    if 'Zpn' in extension_list:
         if 32 in inp_yaml['supported_xlen']:
             temp['rv32']['accessible'] = True
             temp['rv32']['ov']['implemented'] = True
         else :
             temp['rv64']['accessible'] = True
             temp['rv64']['ov']['implemented'] = True
     return temp
 
 def twset():
     '''Function to check and set value for tw field in misa.'''
-    global inp_yaml
-    if 'S' not in inp_yaml['ISA'] and 'U' not in inp_yaml['ISA']:
+    global extension_list
+    if 'S' not in extension_list and 'U' not in extension_list:
         return {'implemented': False}
     else:
         return {'implemented': True}
 
 
 def delegset():
     '''Function to set "implemented" value for mideleg regisrer.'''
     # return True
     global inp_yaml
+    global extension_list
     var = True
-    if 'S' not in inp_yaml['ISA'] and 'N' not in inp_yaml['ISA']:
+    if 'S' not in extension_list and 'N' not in extension_list:
         var = False
 
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True and var
     if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True and var
     return temp
 
 
 def countset():
     global inp_yaml
+    global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
-    if 'S' in inp_yaml['ISA'] or 'U' in inp_yaml["ISA"]:
+    if 'S' in extension_list or 'U' in inp_yaml["ISA"]:
         if 32 in inp_yaml['supported_xlen']:
             temp['rv32']['accessible'] = True
         if 64 in inp_yaml['supported_xlen']:
             temp['rv64']['accessible'] = True
     return temp
 
 
@@ -275,17 +314,18 @@
     rvxlen='rv'+str(xlen)
     extensions=hex(int(format(reset(), '#0{}b'.format(xlen+2))[(xlen-24):(xlen+2)], 2))
     schema_yaml['misa']['schema'][rvxlen]['schema']['extensions']['schema']['type']['default']['warl']['legal'][0]=schema_yaml['misa']['schema'][rvxlen]['schema']['extensions']['schema']['type']['default']['warl']['legal'][0].replace('0x3FFFFFFF', extensions)
     return schema_yaml
     
 def add_fflags_type_setters(schema_yaml):
     global inp_yaml
+    global extension_list
     xlen=inp_yaml['supported_xlen'][0]
     rvxlen='rv'+str(xlen)
-    if 'F' not in inp_yaml['ISA']:
+    if 'F' not in extension_list:
         schema_yaml['fcsr']['schema'][rvxlen]['schema']['frm']['schema']['type']['default'] = {'ro_constant': 0}
         schema_yaml['fcsr']['schema'][rvxlen]['schema']['fflags']['schema']['type']['default'] = {'ro_constant': 0}
     return schema_yaml
     
 def add_def_setters(schema_yaml):
     '''Function to set the default setters for various fields in the schema'''
     regsetter = lambda doc: regset()
@@ -306,14 +346,16 @@
     sregsetterh = lambda doc: sregseth()
     nusetter = lambda doc: nuset()
     usetter = lambda doc: uset()
     hsetter = lambda doc: hset()
     twsetter = lambda doc: twset()
     delegsetter = lambda doc: delegset()
     psetter = lambda doc: pset()
+    smrnmi_setter = lambda doc: smrnmi_set()
+    reset_smrnmi_setter = lambda doc: smrnmi_reset()
 
     schema_yaml['sstatus']['default_setter'] = sregsetter
     schema_yaml['sstatus']['schema']['rv32']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['sstatus']['schema']['rv64']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['sstatus']['schema']['rv32']['schema']['upie'][
@@ -1025,14 +1067,19 @@
     schema_yaml['vstvec']['default_setter'] = sregsetter
     schema_yaml['vsepc']['default_setter'] = sregsetter
     schema_yaml['vstval']['default_setter'] = sregsetter
     schema_yaml['vscause']['default_setter'] = sregsetter
     schema_yaml['vsatp']['default_setter'] = sregsetter
     schema_yaml['vsscratch']['default_setter'] = sregsetter
     schema_yaml['vxsat']['default_setter'] = psetter
+    schema_yaml['mnscratch']['default_setter'] = smrnmi_setter
+    schema_yaml['mnepc']['default_setter'] = smrnmi_setter
+    schema_yaml['mnstatus']['default_setter'] = smrnmi_setter
+    schema_yaml['mncause']['default_setter'] = smrnmi_setter
+    schema_yaml['mncause']['schema']['reset-val']['default_setter'] = reset_smrnmi_setter
     return schema_yaml
 
 
 def trim(foo):
     '''
         Function to trim the dictionary. Any node with implemented field set to false is trimmed of all the other nodes.
 
@@ -1526,19 +1573,19 @@
         wlrl_atleast_one_pass = False
         for entry in csrnode['type']['wlrl']:
             if ":" in entry:
                 [low, high] = [ int(x,0) for x in entry.split(":")]
                 if val >= low and val <= high:
                     wlrl_atleast_one_pass = True
                     break
-                elif val == int(entry, 0):
-                    wlrl_atleast_one_pass = True
-                    break
+            elif val == int(entry, 0):
+                wlrl_atleast_one_pass = True
+                break
         if not wlrl_atleast_one_pass:
-            error.append("Reset value:{hex(val)} \
+            error.append(f"Reset value:{hex(val)} \
 doesn't match the 'wlrl' description :{csrnode['type']['wlrl']} for the register.")
     elif 'ro_constant' in csrnode['type']:
         if val != csrnode['type']['ro_constant']:
             error.append("Reset value doesnt match the \
 'ro_constant' description for the register.")
     elif 'ro_variable' in csrnode['type']:
         pass
```

### Comparing `riscv_config-3.7.2/riscv_config/constants.py` & `riscv_config-3.8.0/riscv_config/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         "Zmmul",
         "Zam",
         "Zfh",
         "Zfinx", "Zdinx", "Zhinx", "Zhinxmin",
         "Ztso",
         "Zba", "Zbb", "Zbc", "Zbe", "Zbf", "Zbkb", "Zbkc", "Zbkx", "Zbm", "Zbp", "Zbpbo", "Zbr", "Zbs", "Zbt",
         "Zk", "Zkn", "Zknd", "Zkne", "Zknh", "Zkr", "Zks", "Zksed", "Zksh", "Zkt",
-        "Zpn", "Zpsf",
-        "Svnapot"
+        "Zpn", "Zpsf"
 ] + Zve_extensions + Zvl_extensions
 
-Zb_extensions = ["Zba", "Zbb", "Zbc", "Zbe", "Zbf", "Zbm", "Zbp", "Zbr", "Zbs", "Zbt"]
-Zp_extensions = ["Zbpbo", "Zpn", "Zpsf"]
+S_extensions = ['Smrnmi','Svnapot']
+
+sub_extensions = Z_extensions + S_extensions
 
 isa_regex = \
-        re.compile("^RV(32|64|128)[IE][ACDFGHJLMNPQSTUV]*(("+'|'.join(Z_extensions)+")(_("+'|'.join(Z_extensions)+"))*){,1}(X[a-z0-9]*)*(_X[a-z0-9]*)*$")
+        re.compile("^RV(32|64|128)[IE][ACDFGHJLMNPQSTUV]*(("+'|'.join(sub_extensions)+")(_("+'|'.join(sub_extensions)+"))*){,1}(X[a-z0-9]*)*(_X[a-z0-9]*)*$")
```

### Comparing `riscv_config-3.7.2/riscv_config/errors.py` & `riscv_config-3.8.0/riscv_config/errors.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config/isa_validator.py` & `riscv_config-3.8.0/riscv_config/isa_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def get_extension_list(isa):
     extension_list = []
     err = False
     err_list = []
     if not constants.isa_regex.match(isa):
         err = True
-        err_list.append('Input ISA string does not match accepted canonical ordering')
+        err_list.append(f'Input ISA string : {isa} does not match accepted canonical ordering')
         return (extension_list, err, err_list)
 
     
     str_match = re.findall('(?P<stdisa>[^\d]*?)(?!_)*(?P<zext>Z.*?)*(?P<sext>S[a-z]*)*(?P<xext>X[a-z0-9]*)*(_|$)',isa)
     extension_list= []
     standard_isa = ''
     zext_list = []
```

### Comparing `riscv_config-3.7.2/riscv_config/main.py` & `riscv_config-3.8.0/riscv_config/main.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config/schemaValidator.py` & `riscv_config-3.8.0/riscv_config/schemaValidator.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,36 @@
         global extensions
         global xlen
         global supported_xlen
         supported_xlen = kwargs.get('xlen')
         xlen = 0 if len(supported_xlen)==0 else max(supported_xlen)
         global isa_string
         isa_string = kwargs.get('isa_string')
+        global extension_list
+        global ext_err
+        global ext_err_list
+        if isa_string :
+          (extension_list, ext_err, ext_err_list) = get_extension_list(isa_string)
         if 32 in supported_xlen:
             rv32 = True
         else:
             rv32 = False
         if 64 in supported_xlen:
             rv64 = True
         else:
             rv64 = False
         super(schemaValidator, self).__init__(*args, **kwargs)
+
+    def _check_with_smrnmi_check(self, field, value):
+      global extension_list
+      if value and 'Smrnmi' not in extension_list:
+        self._error(field,
+                  "Register cannot be implemented without Smrnmi extension in ISA."
+              )
+
     
     def _check_with_satp_modes64(self, field, value):
 
         if 'warl' in value:
             warl = warl_class(value['warl'], 'satp::mode',63, 60)
             for x in [1,2,3,4,5,6,7,11,12,13]:
                 err = warl.islegal(x)
@@ -68,14 +81,17 @@
         '''
         Function to extract and store ISA specific information(such as xlen,user
         spec version and extensions present)
         and check whether the dependencies in ISA extensions are satisfied.
         '''
         global xlen
         global extensions
+        global extension_list
+        global ext_err_list
+        global ext_err
         extension_enc = list("00000000000000000000000000")
         if "32" in value:
             xlen = 32
             ext = value[4:]
         elif "64" in value:
             xlen = 64
             ext = value[4:]
@@ -83,23 +99,21 @@
             xlen = 128
             ext = value[5:]
         else:
             self._error(field, "Invalid width in ISA.")
 
         if not constants.isa_regex.match(value):
             self._error(field, 'Input ISA string does not match regex')
-
-        (extension_list, err, err_list) = get_extension_list(value)
-        if err:
-            for e in err_list:
+        if ext_err:
+            for e in ext_err_list:
                 self._error(field, e)
 
         #ISA encoding for future use.
         for x in "ABCDEFHIJKLMNPQSTUVX":
-            if (x in ext):
+            if (x in extension_list):
                 extension_enc[25 - int(ord(x) - ord('A'))] = "1"
         extensions = int("".join(extension_enc), 2)
         extensions = int("".join(extension_enc), 2)
 
     def _check_with_rv32_check(self, field, value):
         global xlen
         if value:
@@ -143,29 +157,29 @@
             for val in list:
                 if not (val < maxv):
                     self._error(field, "Invalid values.")
 
     def _check_with_s_exists(self, field, value):
         '''Function to check that the value can be true only when 'S' mode
         exists in the ISA string'''
-        global isa_string
+        global extension_list
 
-        if value and 'S' not in isa_string:
+        if value and 'S' not in extension_list:
             self._error(field, "cannot be set to True without 'S' mode support")
 
     def _check_with_mtval_update(self, field, value):
         '''Function to check if the mtval_update bitmap adhered to the required
         restrictions.
         '''
-        global isa_string
+        global extension_list
         if (((value & 0xFFFF000F4000) != 0) or (value > 0xFFFFFFFFFFFFFFFF)):
             self._error(field, 'Bits corresponding to reserved cause values should not be set')
-        if (value & 0xB000) != 0 and 'S' not in isa_string:
+        if (value & 0xB000) != 0 and 'S' not in extension_list:
             self._error(field, 'Bits corresponding to page-faults can only be set when S mode is supported')
-        if (value & 0xF00000) != 0 and 'H' not in isa_string:
+        if (value & 0xF00000) != 0 and 'H' not in extension_list:
             self._error(field, 'Bits corresponding to guest-page faults can only be set when H mode is supported')
 
     def _check_with_s_check(self, field, value):
         s = 18
         check = False
         if 'implemented' in value:
             if value['implemented']:
@@ -224,28 +238,28 @@
             mxl = format(extensions, '#034b')
             if (mxl[33 - u:34 - u] != '1'):
                 self._error(field, "should not be implemented since U is not present")
               
     def _check_with_s_debug_check(self, field, value):
         ''' Function ensures that the ro_constant is hardwired to zero when S is present in the ISA string
             Used mainly for debug schema'''
-        global isa_string
+        global extension_list
 
-        if 'S' not in isa_string :
+        if 'S' not in extension_list :
           if 'ro_constant' not in value:
               self._error(field, "S is not present to dcsr.v should be ro_constant = 0")
           elif value['ro_constant'] != 0:
                 self._error(field, "S is not present but ro constant is not hardwired to zero")
                 
     def _check_with_u_debug_check(self, field, value):
         ''' Function ensures that the ro_constant is hardwired to zero when U is present in the ISA string
             Used mainly for debug schema'''
-        global isa_string
+        global extension_list
 
-        if 'U' not in isa_string :
+        if 'U' not in extension_list :
           if value['ro_constant'] != 0:
                 self._error(field, "U is not present but ro constant is not hardwired to zero")
 
     def _check_with_su_check(self, field, value):
         s = 18
         u = 20
         check = False
@@ -336,38 +350,40 @@
 
         elif rv32 and check:
             mxl = format(extensions, '#034b')
             if (mxl[33 - h:34 - h] != '1'):
                 self._error(field, "h is not present")
 
     def _check_with_mdeleg_checks(self, field, value):
+        global extension_list
         if rv32:
             if (value['rv32']['accessible'] == True and
-                (not 'S' in self.document['ISA'] and
-                 not 'N' in self.document['ISA'])):
+                (not 'S' in extension_list and
+                 not 'N' in extension_list)):
                 value['rv32']['accessible'] = False
                 self._error(field, "S and N are not present")
 
         if rv64:
             if (value['rv64']['accessible'] == True and
-                (not 'S' in self.document['ISA'] and
-                 not 'N' in self.document['ISA'])):
+                (not 'S' in extension_list and
+                 not 'N' in extension_list)):
                 value['rv64']['accessible'] = False
                 self._error(field, "S and N are not present")
 
     def _check_with_ndeleg_checks(self, field, value):
+        global extension_list
         if rv32:
             if (value['rv32']['accessible'] == True and
-                    not 'N' in self.document['ISA']):
+                    not 'N' in extension_list):
                 value['rv32']['accessible'] = False
                 self._error(field, "should not be implemented since N is not present")
 
         if rv64:
             if (value['rv64']['accessible'] == True and
-                    not 'N' in self.document['ISA']):
+                    not 'N' in extension_list):
                 value['rv64']['accessible'] = False
                 self._error(field, "should not be implemented since N is not present")
 
     def _check_with_xcause_check(self, field, value):
         '''Function to verify the inputs for mcause.'''
         if (min(value) < 16):
             self._error(
@@ -391,16 +407,17 @@
         s = format(value, '#{}b'.format(supported_xlen[0] + 2))
         if (s[-11:-8]) != '000' and value >= int("400", 16):
             self._error(field, " 11,10,9 bits should be hardwired to 0")
 
     def _check_with_vxsat_check(self, field, value):
         check = False
         xlen_str = 'rv32' if rv32 else 'rv64'
-        if 'Zpn' in isa_string and not value[xlen_str]['accessible']:
+        global extension_list
+        if 'Zpn' in extension_list and not value[xlen_str]['accessible']:
             self._error(field,f'[{xlen_str}] Field should be accessible since Zpn is present')
-        if not 'Zpn' in isa_string and value[xlen_str]['accessible']:
+        if not 'Zpn' in extension_list and value[xlen_str]['accessible']:
             self._error(field,f'[{xlen_str}] Field should be accessible only when Zpn is present')
-        if not 'Zpn' in isa_string and value[xlen_str]['ov']['implemented']:
+        if not 'Zpn' in extension_list and value[xlen_str]['ov']['implemented']:
             self._error(field, f'[{xlen_str}] Subfield ov should not be implemented since Zpn is not present')
-        if 'Zpn' in isa_string and not value[xlen_str]['ov']['implemented']:
+        if 'Zpn' in extension_list and not value[xlen_str]['ov']['implemented']:
             self._error(field, f'[{xlen_str}] Subfield ov should be implemented since Zpn is present in isa')
```

### Comparing `riscv_config-3.7.2/riscv_config/schemas/schema_debug.yaml` & `riscv_config-3.8.0/riscv_config/schemas/schema_debug.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config/schemas/schema_isa.yaml` & `riscv_config-3.8.0/riscv_config/schemas/schema_isa.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -12971,7 +12971,437 @@
                     - 0:1
               default: {implemented: false}
             accessible:
               type: boolean
               default: true
               check_with: rv64_check
           default: {accessible: False}
+    mnscratch:
+      type: dict
+      schema:
+        description:
+          type: string
+          default: |-
+            The mnscratch CSR holds an MXLEN-bit read-write register which enables the NMI trap 
+            handler to save and restore the context that was interrupted.
+        address: {type: integer, default: 0x740, allowed: [0x740]}
+        priv_mode: {type: string, default: M, allowed: [M]}
+        reset-val:
+          type: integer
+          default: 0
+          check_with: max_length
+        rv32:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            shadow: {type: string, default: , nullable: True}
+            shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+            msb: {type: integer, default: 31, allowed: [31]}
+            lsb: {type: integer, default: 0, allowed: [0]}
+            type:
+              type: dict
+              oneof:
+              - schema: {ro_constant: {type: integer, max:  0xFFFFFFFF}}
+              - schema: {ro_variable: {type: boolean}}
+              - schema: { warl: *ref_warl }
+              default:
+                warl:
+                  dependency_fields: []
+                  legal:
+                  - mnscratch[31:0] in [0x00000000:0xFFFFFFFF]
+                  wr_illegal:
+                  - unchanged
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv32_check
+                - smrnmi_check
+          default: {accessible: false}
+        rv64:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            shadow: {type: string, default: , nullable: True}
+            shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+            msb: {type: integer, default: 63, allowed: [63]}
+            lsb: {type: integer, default: 0, allowed: [0]}
+            type:
+              type: dict
+              oneof:
+              - schema: {ro_constant: {type: integer, max:  0xFFFFFFFFFFFFFFFF}}
+              - schema: {ro_variable: {type: boolean}}
+              - schema: { warl: *ref_warl }
+              default:
+                warl:
+                  dependency_fields: []
+                  legal:
+                  - mnscratch[63:0] in [0x00000000:0xFFFFFFFFFFFFFFFF]
+                  wr_illegal:
+                  - unchanged
+    
+            accessible:
+              default: false
+              check_with: 
+                - rv64_check
+                - smrnmi_check
+          default: {accessible: false}
+    mnepc:
+      type: dict
+      schema:
+        description:
+          type: string
+          default: |-
+            The mnepc CSR is an MXLEN-bit read-write register which on entry to the NMI trap handler holds
+            the PC of the instruction that took the interrupt.
+
+            The low bit of mnepc (mnepc[0]) is always zero. On implementations that support only
+            IALIGN=32, the two low bits (mnepc[1:0]) are always zero.
+
+            If an implementation allows IALIGN to be either 16 or 32 (by changing CSR misa, for example),
+            then, whenever IALIGN=32, bit mnepc[1] is masked on reads so that it appears to be 0. This
+            masking occurs also for the implicit read by the MRET instruction. Though masked, mnepc[1]
+            remains writable when IALIGN=32.
+
+            mnepc is a WARL register that must be able to hold all valid virtual addresses. It need not be
+            capable of holding all possible invalid addresses. Prior to writing mnepc, implementations may
+            convert an invalid address into some other invalid address that mnepc is capable of holding.
+        address: {type: integer, default: 0x741, allowed: [0x741]}
+        priv_mode: {type: string, default: M, allowed: [M]}
+        reset-val:
+          type: integer
+          default: 0
+          check_with: max_length
+        rv32:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            shadow: {type: string, default: , nullable: True}
+            shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+            msb: {type: integer, default: 31, allowed: [31]}
+            lsb: {type: integer, default: 0, allowed: [0]}
+            type:
+              type: dict
+              schema: { warl: *ref_warl }
+              default:
+                warl:
+                  dependency_fields: []
+                  legal:
+                  - mnepc[31:0] in [0x00000000:0xFFFFFFFF]
+                  wr_illegal:
+                  - unchanged
+    
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv32_check
+                - smrnmi_check
+          default: {accessible: false}
+        rv64:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            shadow: {type: string, default: , nullable: True}
+            shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+            msb: {type: integer, default: 63, allowed: [63]}
+            lsb: {type: integer, default: 0, allowed: [0]}
+            type:
+              type: dict
+              schema: { warl: *ref_warl }
+              default:
+                warl:
+                  dependency_fields: []
+                  legal:
+                  - mnepc[63:0] in [0x00000000:0xFFFFFFFFFFFFFFFF]
+                  wr_illegal:
+                  - unchanged
+    
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv64_check
+                - smrnmi_check
+          default: {accessible: false}
+    mncause:
+      type: dict
+      schema:
+        description:
+          type: string
+          default: |-
+            The mncause CSR holds the reason for the NMI, with bit MXLEN-1 set to 1, 
+            and the NMI cause encoded in the least-significant bits or zero if NMI causes are not supported.
+        address: {type: integer, default: 0x742,  allowed: [0x742]}
+        priv_mode: {type: string, default: M, allowed: [M]}
+        reset-val:
+          type: integer
+          check_with: max_length
+          default: 0
+        rv32:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            interrupt:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: Indicates whether the trap was due to an interrupt.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 31, allowed: [31]}
+                lsb: {type: integer, default: 31, allowed: [31]}
+                implemented: {type: boolean, default: true, allowed: [true]}
+                type:
+                  type: dict
+                  schema: {ro_constant: {type: integer, max: 0x1, min: 0x1}}
+                  default: {ro_constant: 1 }
+              default: {implemented: true}
+            exception_code:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: Encodes the exception code.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 30, allowed: [30]}
+                lsb: {type: integer, default: 0, allowed: [0]}
+                implemented: {type: boolean, default: true, allowed: [true]}
+                type:
+                  type: dict
+                  schema: { wlrl: *ref_wlrl }
+                  default:
+                    wlrl: 
+                    - 0:15
+              default: {implemented: true}
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv32_check
+                - smrnmi_check
+          default: {accessible: false}
+        rv64:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            interrupt:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: Indicates whether the trap was due to an interrupt.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 63, allowed: [63]}
+                lsb: {type: integer, default: 63, allowed: [63]}
+                implemented: {type: boolean, default: true, allowed: [true]}
+                type:
+                  type: dict
+                  schema: {ro_constant: {type: integer, max: 0x1, min: 0x1}}
+                  default: {ro_constant: 1 }
+              default: {implemented: true}
+            exception_code:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: Encodes the exception code.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 62, allowed: [62]}
+                lsb: {type: integer, default: 0, allowed: [0]}
+                implemented: {type: boolean, default: true, allowed: [true]}
+                type:
+                  type: dict
+                  schema: { wlrl: *ref_wlrl }
+                  default:
+                    wlrl:
+                    - 0:15
+              default: {implemented: true}
+            accessible:
+              type: boolean
+              default: false
+              check_with: rv64_check
+          default: {accessible: false}
+    mnstatus:
+      type: dict
+      schema:
+        description:
+          type: string
+          default: |-
+
+            The mnstatus CSR holds a two-bit field, MNPP, which on entry to the trap handler holds the
+            privilege mode of the interrupted context, encoded in the same manner as mstatus.MPP. It also
+            
+            holds a one-bit field, MNPV, which on entry to the trap handler holds the virtualization mode of
+            the interrupted context, encoded in the same manner as mstatus.MPV.
+            mnstatus also holds the NMIE bit. When NMIE=1, nonmaskable interrupts are enabled. When
+            NMIE=0, all interrupts are disabled.
+            When NMIE=0, the hart behaves as though mstatus.MPRV were clear, regardless of the current
+            setting of mstatus.MPRV.
+
+            Upon reset, NMIE contains the value 0.
+
+        address: {type: integer, default: 0x742, allowed: [0x742]}
+        priv_mode: {type: string, default: M, allowed: [M]}
+        reset-val:
+          type: integer
+          check_with: max_length
+          default: 0
+        rv32:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            nmie:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    When NMIE=1, nonmaskable interrupts are enabled. When
+                    NMIE=0, all interrupts are disabled. When NMIE=0, the hart behaves as though mstatus.MPRV were 
+                    clear, regardless of the current setting of mstatus.MPRV.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 3, allowed: [3]}
+                lsb: {type: integer, default: 3, allowed: [3]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  oneof:
+                  - schema: { warl: *ref_warl }
+                  - schema: { wlrl: *ref_wlrl }
+                  default: 
+                    warl:
+                      dependency_fields: [writeval]
+                      legal:
+                        - writeval[0] in [1] -> nmie[0] bitmask [1,0]
+                      wr_illegal:
+                        - Unchanged
+              default: {implemented: true}
+            mnpv:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    on entry to the trap handler holds the virtualization mode of the interrupted 
+                    context, encoded in the same manner as mstatus.MPV.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 7, allowed: [7]}
+                lsb: {type: integer, default: 7, allowed: [7]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  schema: { wlrl: *ref_wlrl }
+                  default: { wlrl: [0:1]}
+              default: {implemented: false}
+              check_with: h_check
+            mnpp:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    on entry to the trap handler holds the
+                    privilege mode of the interrupted context, encoded in the same manner as mstatus.MPP.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 12, allowed: [12]}
+                lsb: {type: integer, default: 11, allowed: [11]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  oneof:
+                  - schema: { warl: *ref_warl }
+                  - schema: {ro_constant: {type: integer, max: 3 , min : 0}}
+                  - schema: { wlrl: *ref_wlrl }
+                  default: {ro_constant: 0}
+              default: {implemented: true}
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv32_check
+                - smrnmi_check
+        rv64:
+          type: dict
+          schema:
+            fields: {type: list, default: []}
+            nmie:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    When NMIE=1, nonmaskable interrupts are enabled. When
+                    NMIE=0, all interrupts are disabled. When NMIE=0, the hart behaves as though mstatus.MPRV were 
+                    clear, regardless of the current setting of mstatus.MPRV.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 3, allowed: [3]}
+                lsb: {type: integer, default: 3, allowed: [3]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  oneof:
+                  - schema: { warl: *ref_warl }
+                  - schema: { wlrl: *ref_wlrl }
+                  default: 
+                    warl:
+                      dependency_fields: [writeval]
+                      legal:
+                        - writeval[0] in [1] -> nmie[0] bitmask [1,0]
+                      wr_illegal:
+                        - Unchanged
+              default: {implemented: true}
+            mnpv:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    on entry to the trap handler holds the virtualization mode of
+                    the interrupted context, encoded in the same manner as mstatus.MPV.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 7, allowed: [7]}
+                lsb: {type: integer, default: 7, allowed: [7]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  schema: { wlrl: *ref_wlrl }
+                  default: { wlrl: [0:1]}
+              default: {implemented: false}
+              check_with: h_check
+            mnpp:
+              type: dict
+              schema:
+                description:
+                  type: string
+                  default: |-
+                    on entry to the trap handler holds the
+                    privilege mode of the interrupted context, encoded in the same manner as mstatus.MPP.
+                shadow: {type: string, default: , nullable: True}
+                shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
+                msb: {type: integer, default: 12, allowed: [12]}
+                lsb: {type: integer, default: 11, allowed: [11]}
+                implemented: {type: boolean, default: true}
+                type:
+                  type: dict
+                  oneof:
+                  - schema: { warl: *ref_warl }
+                  - schema: {ro_constant: {type: integer, max: 3 , min : 0}}
+                  - schema: { wlrl: *ref_wlrl }
+                  default: {ro_constant: 0}
+              default: {implemented: true}
+            accessible:
+              type: boolean
+              default: false
+              check_with: 
+                - rv64_check
+                - smrnmi_check
+          default: {accessible: false}
```

### Comparing `riscv_config-3.7.2/riscv_config/schemas/schema_platform.yaml` & `riscv_config-3.8.0/riscv_config/schemas/schema_platform.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config/utils.py` & `riscv_config-3.8.0/riscv_config/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config/warl.py` & `riscv_config-3.8.0/riscv_config/warl.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/riscv_config.egg-info/PKG-INFO` & `riscv_config-3.8.0/riscv_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv-config
-Version: 3.7.2
+Version: 3.8.0
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
@@ -15,8 +15,8 @@
         
         Latest Documentation of RISCV-Config: `HTML <https://riscv-config.readthedocs.io/>`_
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
```

### Comparing `riscv_config-3.7.2/riscv_config.egg-info/SOURCES.txt` & `riscv_config-3.8.0/riscv_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riscv_config-3.7.2/setup.py` & `riscv_config-3.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import codecs
-import pip
 from setuptools import setup, find_packages
 
 import riscv_config
 
 # Base directory of package
 here = os.path.abspath(os.path.dirname(__file__))
 
@@ -31,12 +30,12 @@
       author='InCore Semiconductors Pvt. Ltd.',
       author_email='neelgala@incoresemi.com',
       license='BSD-3-Clause',
       packages=find_packages(),
       install_package_data=True,
       package_dir={'riscv_config': 'riscv_config/'},
       package_data={'riscv_config': ['schemas/*']},
-      install_requires=['Cerberus>=1.3.1', 'ruamel.yaml>=0.16.0', 'pyyaml>=5.1.1'],
-      python_requires=">=3.6.0",
+      install_requires=['Cerberus>=1.3.1', 'ruamel.yaml>=0.17.16', 'pyyaml==5.2'],
+      python_requires=">=3.7.0",
       entry_points={
           "console_scripts": ["riscv-config=riscv_config.main:main"],
       })
```


# Comparing `tmp/appdefender-0.4.2.tar.gz` & `tmp/appdefender-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./dist/appdefender-0.4.2.tar", last modified: Wed Apr 19 02:04:37 2023, max compression
+gzip compressed data, was "./dist/appdefender-0.4.3.tar", last modified: Mon Apr 24 02:54:06 2023, max compression
```

## Comparing `appdefender-0.4.2.tar` & `appdefender-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-19 02:04:37.000000 appdefender-0.4.2/
-drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-19 02:04:37.000000 appdefender-0.4.2/appdefender.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)        1 2023-04-19 02:04:35.000000 appdefender-0.4.2/appdefender.egg-info/dependency_links.txt
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      402 2023-04-19 02:04:35.000000 appdefender-0.4.2/appdefender.egg-info/SOURCES.txt
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2315 2023-04-19 02:04:35.000000 appdefender-0.4.2/appdefender.egg-info/PKG-INFO
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)       12 2023-04-19 02:04:35.000000 appdefender-0.4.2/appdefender.egg-info/top_level.txt
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)        1 2023-04-19 02:04:35.000000 appdefender-0.4.2/appdefender.egg-info/zip-safe
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)       55 2023-04-19 01:46:55.000000 appdefender-0.4.2/LICENSE.txt
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)     1241 2023-04-19 01:46:55.000000 appdefender-0.4.2/setup.py
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2315 2023-04-19 02:04:37.000000 appdefender-0.4.2/PKG-INFO
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)       78 2023-04-19 02:04:37.000000 appdefender-0.4.2/setup.cfg
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)       36 2023-04-19 01:46:55.000000 appdefender-0.4.2/MANIFEST.in
-drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-19 02:04:37.000000 appdefender-0.4.2/appdefender/
-drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-19 02:04:37.000000 appdefender-0.4.2/appdefender/lib/
--rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)   883128 2023-04-19 01:53:29.000000 appdefender-0.4.2/appdefender/lib/libcore.x86_64.gnu.so
--rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)  1224976 2023-04-19 02:04:24.000000 appdefender-0.4.2/appdefender/lib/libcore.aarch64.musl.so
--rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)   853344 2023-04-19 01:55:31.000000 appdefender-0.4.2/appdefender/lib/libcore.x86_64.musl.so
--rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)  1193984 2023-04-19 02:04:24.000000 appdefender-0.4.2/appdefender/lib/libcore.aarch64.gnu.so
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2250 2023-04-19 01:46:55.000000 appdefender-0.4.2/appdefender/__init__.py
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)     1416 2023-04-19 01:46:55.000000 appdefender-0.4.2/README.md
+drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-24 02:54:06.000000 appdefender-0.4.3/
+drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)        1 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/dependency_links.txt
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      402 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/SOURCES.txt
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2315 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/PKG-INFO
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)       12 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/top_level.txt
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)        1 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender.egg-info/zip-safe
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)       55 2023-04-24 02:37:28.000000 appdefender-0.4.3/LICENSE.txt
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)     1241 2023-04-24 02:37:28.000000 appdefender-0.4.3/setup.py
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2315 2023-04-24 02:54:06.000000 appdefender-0.4.3/PKG-INFO
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)       78 2023-04-24 02:54:06.000000 appdefender-0.4.3/setup.cfg
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)       36 2023-04-24 02:37:28.000000 appdefender-0.4.3/MANIFEST.in
+drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender/
+drwxr-xr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-04-24 02:54:06.000000 appdefender-0.4.3/appdefender/lib/
+-rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)   883128 2023-04-24 02:43:27.000000 appdefender-0.4.3/appdefender/lib/libcore.x86_64.gnu.so
+-rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)  1224976 2023-04-24 02:53:57.000000 appdefender-0.4.3/appdefender/lib/libcore.aarch64.musl.so
+-rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)   853344 2023-04-24 02:45:27.000000 appdefender-0.4.3/appdefender/lib/libcore.x86_64.musl.so
+-rwxr-xr-x   0 azureuser  (1000) azureuser  (1000)  1193984 2023-04-24 02:53:57.000000 appdefender-0.4.3/appdefender/lib/libcore.aarch64.gnu.so
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)     2250 2023-04-24 02:37:28.000000 appdefender-0.4.3/appdefender/__init__.py
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)     1416 2023-04-24 02:37:28.000000 appdefender-0.4.3/README.md
```

### Comparing `appdefender-0.4.2/appdefender.egg-info/PKG-INFO` & `appdefender-0.4.3/appdefender.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appdefender
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extrinsec AppDefender: Real time serverless protection
 Home-page: https://www.extrinsec.com
 Author: Extrinsec LLC
 Author-email: support@extrinsec.com
 License: Other/Proprietary License
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appdefender Version: 0.4.2 Summary: Extrinsec
+Metadata-Version: 2.1 Name: appdefender Version: 0.4.3 Summary: Extrinsec
 AppDefender: Real time serverless protection Home-page: https://
 www.extrinsec.com Author: Extrinsec LLC Author-email: support@extrinsec.com
 License: Other/Proprietary License Platform: Linux Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `appdefender-0.4.2/setup.py` & `appdefender-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='appdefender',
-    version="0.4.2",
+    version="0.4.3",
     description='Extrinsec AppDefender: Real time serverless protection',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.extrinsec.com',
     author='Extrinsec LLC',
     author_email='support@extrinsec.com',
     platforms='Linux',
```

### Comparing `appdefender-0.4.2/PKG-INFO` & `appdefender-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appdefender
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extrinsec AppDefender: Real time serverless protection
 Home-page: https://www.extrinsec.com
 Author: Extrinsec LLC
 Author-email: support@extrinsec.com
 License: Other/Proprietary License
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appdefender Version: 0.4.2 Summary: Extrinsec
+Metadata-Version: 2.1 Name: appdefender Version: 0.4.3 Summary: Extrinsec
 AppDefender: Real time serverless protection Home-page: https://
 www.extrinsec.com Author: Extrinsec LLC Author-email: support@extrinsec.com
 License: Other/Proprietary License Platform: Linux Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `appdefender-0.4.2/appdefender/lib/libcore.x86_64.gnu.so` & `appdefender-0.4.3/appdefender/lib/libcore.x86_64.gnu.so`

 * *Files 0% similar despite different names*

#### readelf --wide --dynamic {}

```diff
@@ -2,15 +2,15 @@
 Dynamic section at offset 0xcfd10 contains 29 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [librt.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libdl.so.2]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [ld-linux-x86-64.so.2]
- 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.2]
+ 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.3]
  0x000000000000000c (INIT)               0x5568
  0x000000000000000d (FINI)               0xa9080
  0x0000000000000019 (INIT_ARRAY)         0x2ce548
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x2ce558
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x1f0
```

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 13d0ba3eb12b6f0a4cb8d35047fc0b1037da0df9
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bb45dee9e71fca1926f4146f435f6b81294048d0
```

#### strings --all --bytes=8 {}

```diff
@@ -92,15 +92,15 @@
 crc32_combine
 crc32_combine64
 librt.so.1
 libdl.so.2
 libc.so.6
 ld-linux-x86-64.so.2
 __bss_start
-libappdefender.so.0.4.2
+libappdefender.so.0.4.3
 GLIBC_2.2.5
 GLIBC_2.9
 GLIBC_2.7
 GLIBC_2.14
 GLIBC_2.8
 GLIBC_2.3.2
 GLIBC_2.4
@@ -968,15 +968,15 @@
 [config.c] adding send data hook
 [config.c] adding child process hook
 [config.c] adding file system hook
 [INFO] [appDefender] configuration done
 [config.c] ****** TODO: handle re-configuration!!!! *******
 /etc/resolv.conf
 nameserver 
-v-0.4.2-0-gc6586bf0
+v-0.4.3-0-gcf1b264a
 [config.c] str_json: %s
 {"api_key": ""}
 license_key
 ES_LICENSE_KEY
 policy_group_name
 ES_POLICY_GROUP_NAME
 sdk_version
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -111,15 +111,15 @@
   0x00001948 72633332 5f636f6d 62696e65 3634006c rc32_combine64.l
   0x00001958 69627274 2e736f2e 31006c69 62646c2e ibrt.so.1.libdl.
   0x00001968 736f2e32 006c6962 632e736f 2e36006c so.2.libc.so.6.l
   0x00001978 642d6c69 6e75782d 7838362d 36342e73 d-linux-x86-64.s
   0x00001988 6f2e3200 5f656461 7461005f 5f627373 o.2._edata.__bss
   0x00001998 5f737461 7274005f 656e6400 6c696261 _start._end.liba
   0x000019a8 70706465 66656e64 65722e73 6f2e302e ppdefender.so.0.
-  0x000019b8 342e3200 474c4942 435f322e 322e3500 4.2.GLIBC_2.2.5.
+  0x000019b8 342e3300 474c4942 435f322e 322e3500 4.3.GLIBC_2.2.5.
   0x000019c8 474c4942 435f322e 3900474c 4942435f GLIBC_2.9.GLIBC_
   0x000019d8 322e3700 474c4942 435f322e 31340047 2.7.GLIBC_2.14.G
   0x000019e8 4c494243 5f322e38 00474c49 42435f32 LIBC_2.8.GLIBC_2
   0x000019f8 2e332e32 00474c49 42435f32 2e340047 .3.2.GLIBC_2.4.G
   0x00001a08 4c494243 5f322e33 2e340047 4c494243 LIBC_2.3.4.GLIBC
   0x00001a18 5f322e33 00                         _2.3.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -11729,15 +11729,15 @@
 	mov    %rax,0xb8(%rsp)
 	xor    %eax,%eax
 	lea    0x2c6b11(%rip),%rax        
 	mov    %rcx,(%rax)
 	movb   $0x0,0x8(%rax)
 	xor    %eax,%eax
 	call   14740 <configure@@Base+0x2de0>
-	lea    0x9cf82(%rip),%rax        
+	lea    0x9cd7e(%rip),%rax        
 	sub    $0x8,%rsp
 	lea    0x99b5e(%rip),%rcx        
 	lea    0x9cd54(%rip),%r8        
 	lea    0x98f3b(%rip),%rdi        
 	lea    0xa5789(%rip),%r9        
 	push   %rax
 	lea    0x99b47(%rip),%rsi
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -330,16 +330,16 @@
   0x000aa510 f65af6ff ee5af6ff e35af6ff d85af6ff .Z...Z...Z...Z..
   0x000aa520 cd5af6ff c25af6ff b75af6ff ac5af6ff .Z...Z...Z...Z..
   0x000aa530 285ef6ff 215ef6ff 165ef6ff 0b5ef6ff (^..!^...^...^..
   0x000aa540 005ef6ff f95df6ff ef5df6ff e55df6ff .^...]...]...]..
   0x000aa550 db5df6ff d15df6ff c75df6ff bd5df6ff .]...]...]...]..
   0x000aa560 2f657463 2f726573 6f6c762e 636f6e66 /etc/resolv.conf
   0x000aa570 006e616d 65736572 76657220 00302e34 .nameserver .0.4
-  0x000aa580 2e320076 2d302e34 2e322d30 2d676336 .2.v-0.4.2-0-gc6
-  0x000aa590 35383662 6630005b 636f6e66 69672e63 586bf0.[config.c
+  0x000aa580 2e330076 2d302e34 2e332d30 2d676366 .3.v-0.4.3-0-gcf
+  0x000aa590 31623236 3461005b 636f6e66 69672e63 1b264a.[config.c
   0x000aa5a0 5d207374 725f6a73 6f6e3a20 25730a00 ] str_json: %s..
   0x000aa5b0 7b226170 695f6b65 79223a20 22227d00 {"api_key": ""}.
   0x000aa5c0 6c696365 6e73655f 6b657900 45535f4c license_key.ES_L
   0x000aa5d0 4943454e 53455f4b 45590070 6f6c6963 ICENSE_KEY.polic
   0x000aa5e0 795f6772 6f75705f 6e616d65 0045535f y_group_name.ES_
   0x000aa5f0 504f4c49 43595f47 524f5550 5f4e414d POLICY_GROUP_NAM
   0x000aa600 45007364 6b5f7665 7273696f 6e004553 E.sdk_version.ES
```

### Comparing `appdefender-0.4.2/appdefender/lib/libcore.aarch64.musl.so` & `appdefender-0.4.3/appdefender/lib/libcore.aarch64.musl.so`

 * *Files 0% similar despite different names*

#### readelf --wide --dynamic {}

```diff
@@ -1,12 +1,12 @@
 
 Dynamic section at offset 0x1204f0 contains 24 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.musl-aarch64.so.1]
- 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.2]
+ 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.3]
  0x000000000000000c (INIT)               0x10230
  0x000000000000000d (FINI)               0xb108c
  0x0000000000000019 (INIT_ARRAY)         0x1293f8
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x129408
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x190
```

#### strings --all --bytes=8 {}

```diff
@@ -169,15 +169,15 @@
 A64NamedImmMapper_fromString
 A64NamedImmMapper_validImm
 A64IC_ICMapper
 A64DC_DCMapper
 A64AT_ATMapper
 A64TLBI_TLBIMapper
 libc.musl-aarch64.so.1
-libappdefender.so.0.4.2
+libappdefender.so.0.4.3
 +,@9, @9
 +,@9, @9
 R"i 8b*@
 v^@)tVA)W
 mo TCO$TmOC
 >oBT"OM!
 Tfje8Gke8
@@ -370,15 +370,15 @@
 [WARN] [appDefender] could not parse nameservers
 ***** VALGRIND: Event Streaming is DISABLED *****
 ***** VALGRIND: Event Streaming is ENABLED *****
 ***** UNIT TESTS: Event Streaming is DISABLED *****
 ***** UNIT TESTS: Event Streaming is ENABLED *****
 [ERROR] [appDefender] error occurred trying to create events reader background process: %d
 [config.c] ****** init() ******
-v-0.4.2-0-gc6586bf0
+v-0.4.3-0-gcf1b264a
 [config.c] AppDefender Versions: '%s' | '%s' | '%s' | %i.%i.%i
 [config.c] original stdout file descriptor: %d
 [ERROR] [appDefender] could not determine runtime host. appDefender is disabled
 [ERROR] [appDefender] could not determine runtime language. appDefender is disabled
 [WARN] [appDefender] could not determine runtime language version
 [ERROR] [appDefender] could not determine function name. appDefender is disabled
 [config.c] str_json: %s
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -201,9 +201,9 @@
   0x00002ae8 70706572 5f76616c 6964496d 6d004136 pper_validImm.A6
   0x00002af8 3449435f 49434d61 70706572 00413634 4IC_ICMapper.A64
   0x00002b08 44435f44 434d6170 70657200 41363441 DC_DCMapper.A64A
   0x00002b18 545f4154 4d617070 65720041 3634544c T_ATMapper.A64TL
   0x00002b28 42495f54 4c42494d 61707065 72006c69 BI_TLBIMapper.li
   0x00002b38 62632e6d 75736c2d 61617263 6836342e bc.musl-aarch64.
   0x00002b48 736f2e31 006c6962 61707064 6566656e so.1.libappdefen
-  0x00002b58 6465722e 736f2e30 2e342e32 00       der.so.0.4.2.
+  0x00002b58 6465722e 736f2e30 2e342e33 00       der.so.0.4.3.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -8261,17 +8261,17 @@
 	str	d0, [x2]
 	adrp	x22, b1000 <A64SysRegMapper_toString+0x350>
 	adrp	x23, b1000 <A64SysRegMapper_toString+0x350>
 	bl	1c7a4 <configure+0x2b64>
 	add	x3, x22, #0x860
 	add	x1, x23, #0x868
 	mov	x2, x3
-	adrp	x6, 103000 <_dist_code+0x44888>
+	adrp	x6, 104000 <_dist_code+0x45888>
 	adrp	x5, 104000 <_dist_code+0x45888>
-	add	x6, x6, #0xc50
+	add	x6, x6, #0x9f0
 	add	x5, x5, #0xa00
 	adrp	x4, cb000 <_dist_code+0xc888>
 	adrp	x0, b1000 <A64SysRegMapper_toString+0x350>
 	add	x4, x4, #0x118
 	add	x0, x0, #0x880
 	bl	1c7a4 <configure+0x2b64>
 	ldrb	w0, [x19, #64]
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -120,16 +120,16 @@
   0x000b17f0 726f7220 6f636375 72726564 20747279 ror occurred try
   0x000b1800 696e6720 746f2063 72656174 65206576 ing to create ev
   0x000b1810 656e7473 20726561 64657220 6261636b ents reader back
   0x000b1820 67726f75 6e642070 726f6365 73733a20 ground process: 
   0x000b1830 25640a00 00000000 5b636f6e 6669672e %d......[config.
   0x000b1840 635d202a 2a2a2a2a 2a20696e 69742829 c] ****** init()
   0x000b1850 202a2a2a 2a2a2a0a 00000000 00000000  ******.........
-  0x000b1860 302e342e 32000000 762d302e 342e322d 0.4.2...v-0.4.2-
-  0x000b1870 302d6763 36353836 62663000 00000000 0-gc6586bf0.....
+  0x000b1860 302e342e 33000000 762d302e 342e332d 0.4.3...v-0.4.3-
+  0x000b1870 302d6763 66316232 36346100 00000000 0-gcf1b264a.....
   0x000b1880 5b636f6e 6669672e 635d2041 70704465 [config.c] AppDe
   0x000b1890 66656e64 65722056 65727369 6f6e733a fender Versions:
   0x000b18a0 20272573 27207c20 27257327 207c2027  '%s' | '%s' | '
   0x000b18b0 25732720 7c202569 2e25692e 25690a00 %s' | %i.%i.%i..
   0x000b18c0 5b636f6e 6669672e 635d206f 72696769 [config.c] origi
   0x000b18d0 6e616c20 7374646f 75742066 696c6520 nal stdout file 
   0x000b18e0 64657363 72697074 6f723a20 25640a00 descriptor: %d..
```

### Comparing `appdefender-0.4.2/appdefender/lib/libcore.x86_64.musl.so` & `appdefender-0.4.3/appdefender/lib/libcore.x86_64.musl.so`

 * *Files 0% similar despite different names*

#### readelf --wide --dynamic {}

```diff
@@ -1,12 +1,12 @@
 
 Dynamic section at offset 0xc8930 contains 22 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.musl-x86_64.so.1]
- 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.2]
+ 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.3]
  0x000000000000000c (INIT)               0x6000
  0x000000000000000d (FINI)               0x9e051
  0x0000000000000019 (INIT_ARRAY)         0xc8158
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x270
  0x0000000000000005 (STRTAB)             0x1238
  0x0000000000000006 (SYMTAB)             0x3e0
```

#### strings --all --bytes=8 {}

```diff
@@ -71,15 +71,15 @@
 adler32_combine64
 get_crc_table
 cpu_has_pclmul
 crc32_sse42_simd_
 crc32_combine
 crc32_combine64
 libc.musl-x86_64.so.1
-libappdefender.so.0.4.2
+libappdefender.so.0.4.3
 AWAVAUATSH
 [A\A]A^A_]
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
@@ -865,15 +865,15 @@
 [config.c] adding send data hook
 [config.c] adding child process hook
 [config.c] adding file system hook
 [INFO] [appDefender] configuration done
 [config.c] ****** TODO: handle re-configuration!!!! *******
 /etc/resolv.conf
 nameserver 
-v-0.4.2-0-gc6586bf0
+v-0.4.3-0-gcf1b264a
 [config.c] str_json: %s
 {"api_key": ""}
 license_key
 ES_LICENSE_KEY
 policy_group_name
 ES_POLICY_GROUP_NAME
 sdk_version
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -95,9 +95,9 @@
   0x000017f8 635f7461 626c6500 6370755f 6861735f c_table.cpu_has_
   0x00001808 70636c6d 756c0063 72633332 5f737365 pclmul.crc32_sse
   0x00001818 34325f73 696d645f 00637263 33325f63 42_simd_.crc32_c
   0x00001828 6f6d6269 6e650063 72633332 5f636f6d ombine.crc32_com
   0x00001838 62696e65 3634006c 6962632e 6d75736c bine64.libc.musl
   0x00001848 2d783836 5f36342e 736f2e31 006c6962 -x86_64.so.1.lib
   0x00001858 61707064 6566656e 6465722e 736f2e30 appdefender.so.0
-  0x00001868 2e342e32 00                         .4.2.
+  0x00001868 2e342e33 00                         .4.3.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -9661,15 +9661,15 @@
 	lea    0xc1e98(%rip),%rax        
 	mov    %rdx,(%rax)
 	movb   $0x0,0x8(%rax)
 	xor    %eax,%eax
 	call   12da0 <configure+0x2bc0>
 	sub    $0x8,%rsp
 	mov    %rbp,%rcx
-	lea    0xa0894(%rip),%rax        
+	lea    0x9450f(%rip),%rax        
 	push   %rax
 	lea    0x944ef(%rip),%r8        
 	xor    %eax,%eax
 	mov    %rbp,%rdx
 	lea    0x906f8(%rip),%rdi        
 	lea    0xa087c(%rip),%r9        
 	mov    %r13,%rsi
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -347,16 +347,16 @@
   0x000a0580 64e3f6ff 5ae3f6ff 50e3f6ff 49e3f6ff d...Z...P...I...
   0x000a0590 3fe3f6ff 35e3f6ff 2be3f6ff 22e3f6ff ?...5...+..."...
   0x000a05a0 19e3f6ff 10e3f6ff 6ce6f6ff 66e6f6ff ........l...f...
   0x000a05b0 5ce6f6ff 52e6f6ff 48e6f6ff 41e6f6ff \...R...H...A...
   0x000a05c0 37e6f6ff 2de6f6ff 23e6f6ff 1ae6f6ff 7...-...#.......
   0x000a05d0 11e6f6ff 08e6f6ff 2f657463 2f726573 ......../etc/res
   0x000a05e0 6f6c762e 636f6e66 006e616d 65736572 olv.conf.nameser
-  0x000a05f0 76657220 00302e34 2e320076 2d302e34 ver .0.4.2.v-0.4
-  0x000a0600 2e322d30 2d676336 35383662 6630005b .2-0-gc6586bf0.[
+  0x000a05f0 76657220 00302e34 2e330076 2d302e34 ver .0.4.3.v-0.4
+  0x000a0600 2e332d30 2d676366 31623236 3461005b .3-0-gcf1b264a.[
   0x000a0610 636f6e66 69672e63 5d207374 725f6a73 config.c] str_js
   0x000a0620 6f6e3a20 25730a00 7b226170 695f6b65 on: %s..{"api_ke
   0x000a0630 79223a20 22227d00 6c696365 6e73655f y": ""}.license_
   0x000a0640 6b657900 45535f4c 4943454e 53455f4b key.ES_LICENSE_K
   0x000a0650 45590070 6f6c6963 795f6772 6f75705f EY.policy_group_
   0x000a0660 6e616d65 0045535f 504f4c49 43595f47 name.ES_POLICY_G
   0x000a0670 524f5550 5f4e414d 45007364 6b5f7665 ROUP_NAME.sdk_ve
```

### Comparing `appdefender-0.4.2/appdefender/lib/libcore.aarch64.gnu.so` & `appdefender-0.4.3/appdefender/lib/libcore.aarch64.gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --dynamic {}

```diff
@@ -1,15 +1,15 @@
 
 Dynamic section at offset 0x118a30 contains 28 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [libdl.so.2]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [ld-linux-aarch64.so.1]
- 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.2]
+ 0x000000000000000e (SONAME)             Library soname: [libappdefender.so.0.4.3]
  0x000000000000000c (INIT)               0x10868
  0x000000000000000d (FINI)               0xaa284
  0x0000000000000019 (INIT_ARRAY)         0x121938
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x121948
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x1f0
```

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 08890f46b592bed6462802dc0b2cadf7c63064be
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 009b162c0479bfc3362f1235f30ff975f87a0baf
```

#### strings --all --bytes=8 {}

```diff
@@ -192,15 +192,15 @@
 A64AT_ATMapper
 A64TLBI_TLBIMapper
 libc.so.6
 ld-linux-aarch64.so.1
 __bss_start
 __bss_start__
 __bss_end__
-libappdefender.so.0.4.2
+libappdefender.so.0.4.3
 GLIBC_2.17
  _8 8@9"8
  _8 8@9"8
  _8"8@9#8
 mo TCO$TmO
 4A)>p\)6T])
 8 @)7XC)C|
@@ -451,15 +451,15 @@
 [WARN] [appDefender] could not parse nameservers
 ***** VALGRIND: Event Streaming is DISABLED *****
 ***** VALGRIND: Event Streaming is ENABLED *****
 ***** UNIT TESTS: Event Streaming is DISABLED *****
 ***** UNIT TESTS: Event Streaming is ENABLED *****
 [ERROR] [appDefender] error occurred trying to create events reader background process: %d
 [config.c] ****** init() ******
-v-0.4.2-0-gc6586bf0
+v-0.4.3-0-gcf1b264a
 [config.c] AppDefender Versions: '%s' | '%s' | '%s' | %i.%i.%i
 [config.c] original stdout file descriptor: %d
 [ERROR] [appDefender] could not determine runtime host. appDefender is disabled
 [ERROR] [appDefender] could not determine runtime language. appDefender is disabled
 [WARN] [appDefender] could not determine runtime language version
 [ERROR] [appDefender] could not determine function name. appDefender is disabled
 [config.c] str_json: %s
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -219,10 +219,10 @@
   0x00002db8 544c4249 4d617070 6572006c 6962632e TLBIMapper.libc.
   0x00002dc8 736f2e36 006c642d 6c696e75 782d6161 so.6.ld-linux-aa
   0x00002dd8 72636836 342e736f 2e31005f 65646174 rch64.so.1._edat
   0x00002de8 61005f5f 6273735f 73746172 74005f5f a.__bss_start.__
   0x00002df8 6273735f 73746172 745f5f00 5f5f6273 bss_start__.__bs
   0x00002e08 735f656e 645f5f00 5f5f656e 645f5f00 s_end__.__end__.
   0x00002e18 5f656e64 006c6962 61707064 6566656e _end.libappdefen
-  0x00002e28 6465722e 736f2e30 2e342e32 00474c49 der.so.0.4.2.GLI
+  0x00002e28 6465722e 736f2e30 2e342e33 00474c49 der.so.0.4.3.GLI
   0x00002e38 42435f32 2e313700                   BC_2.17.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -7915,17 +7915,17 @@
 	add	x0, x0, #0xa50
 	str	d0, [x1]
 	adrp	x23, aa000 <A64SysRegMapper_toString@@Base+0x108>
 	strb	wzr, [x1, #8]
 	bl	1c8d0 <configure@@Base+0x2b78>
 	add	x3, x23, #0xa78
 	adrp	x24, aa000 <A64SysRegMapper_toString@@Base+0x108>
-	adrp	x6, fd000 <_dist_code@@Base+0x457d8>
+	adrp	x6, fe000 <_dist_code@@Base+0x467d8>
 	mov	x2, x3
-	add	x6, x6, #0x2c8
+	add	x6, x6, #0x68
 	adrp	x5, fe000 <_dist_code@@Base+0x467d8>
 	adrp	x4, cb000 <_dist_code@@Base+0x137d8>
 	add	x5, x5, #0x78
 	add	x4, x4, #0xe80
 	add	x1, x24, #0xa80
 	adrp	x0, aa000 <A64SysRegMapper_toString@@Base+0x108>
 	add	x0, x0, #0xa98
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -121,17 +121,17 @@
   0x000aaa00 6e646572 5d206572 726f7220 6f636375 nder] error occu
   0x000aaa10 72726564 20747279 696e6720 746f2063 rred trying to c
   0x000aaa20 72656174 65206576 656e7473 20726561 reate events rea
   0x000aaa30 64657220 6261636b 67726f75 6e642070 der background p
   0x000aaa40 726f6365 73733a20 25640a00 00000000 rocess: %d......
   0x000aaa50 5b636f6e 6669672e 635d202a 2a2a2a2a [config.c] *****
   0x000aaa60 2a20696e 69742829 202a2a2a 2a2a2a0a * init() ******.
-  0x000aaa70 00000000 00000000 302e342e 32000000 ........0.4.2...
-  0x000aaa80 762d302e 342e322d 302d6763 36353836 v-0.4.2-0-gc6586
-  0x000aaa90 62663000 00000000 5b636f6e 6669672e bf0.....[config.
+  0x000aaa70 00000000 00000000 302e342e 33000000 ........0.4.3...
+  0x000aaa80 762d302e 342e332d 302d6763 66316232 v-0.4.3-0-gcf1b2
+  0x000aaa90 36346100 00000000 5b636f6e 6669672e 64a.....[config.
   0x000aaaa0 635d2041 70704465 66656e64 65722056 c] AppDefender V
   0x000aaab0 65727369 6f6e733a 20272573 27207c20 ersions: '%s' | 
   0x000aaac0 27257327 207c2027 25732720 7c202569 '%s' | '%s' | %i
   0x000aaad0 2e25692e 25690a00 5b636f6e 6669672e .%i.%i..[config.
   0x000aaae0 635d206f 72696769 6e616c20 7374646f c] original stdo
   0x000aaaf0 75742066 696c6520 64657363 72697074 ut file descript
   0x000aab00 6f723a20 25640a00 5b455252 4f525d20 or: %d..[ERROR]
```

### Comparing `appdefender-0.4.2/appdefender/__init__.py` & `appdefender-0.4.3/appdefender/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Python SDK
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 __author__ = "Extrinsec LLC"
 __credits__ = "Extrinsec LLC"
 
 import json
 import os
 import pkgutil
 import platform
```

### Comparing `appdefender-0.4.2/README.md` & `appdefender-0.4.3/README.md`

 * *Files identical despite different names*


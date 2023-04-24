# Comparing `tmp/dal_python-0.1.4-py3-py3-any.whl.zip` & `tmp/dal_python-0.1.5-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -2,12 +2,12 @@
 -rw-r--r--  2.0 unx      156 b- defN 23-Feb-05 13:23 dal/__init__.py
 -rwxr-xr-x  2.0 unx   565728 b- defN 23-Apr-24 14:54 dal/_dal.cpython-39-x86_64-linux-gnu.so
 -rw-r--r--  2.0 unx    52351 b- defN 23-Apr-24 14:54 dal/dal.py
 -rw-r--r--  2.0 unx   630288 b- defN 23-Apr-24 14:54 dal/dal_wrap.cpp
 -rw-r--r--  2.0 unx  8210832 b- defN 23-Apr-24 15:04 dal/libdal.so
 -rw-r--r--  2.0 unx  8210832 b- defN 23-Apr-24 15:04 dal/libdal.so.1.0.0-dev
 -rw-r--r--  2.0 unx   218232 b- defN 23-Apr-24 15:04 dal/libdal_public.so
--rw-r--r--  2.0 unx      799 b- defN 23-Apr-24 15:42 dal_python-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-24 15:42 dal_python-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-24 15:42 dal_python-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      856 b- defN 23-Apr-24 15:42 dal_python-0.1.4.dist-info/RECORD
+-rw-r--r--  2.0 unx      799 b- defN 23-Apr-24 16:29 dal_python-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-24 16:29 dal_python-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-24 16:29 dal_python-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      856 b- defN 23-Apr-24 16:29 dal_python-0.1.5.dist-info/RECORD
 11 files, 17890181 bytes uncompressed, 6443385 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: dal/libdal.so.1.0.0-dev
 Comment: 
 
 Filename: dal/libdal_public.so
 Comment: 
 
-Filename: dal_python-0.1.4.dist-info/METADATA
+Filename: dal_python-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dal_python-0.1.4.dist-info/WHEEL
+Filename: dal_python-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dal_python-0.1.4.dist-info/top_level.txt
+Filename: dal_python-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dal_python-0.1.4.dist-info/RECORD
+Filename: dal_python-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dal_python-0.1.4.dist-info/METADATA` & `dal_python-0.1.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dal-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python bindings for the DAL library
 Author: cheng li
 Author-email: wegamekinglc@hotmail.copm
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `dal_python-0.1.4.dist-info/RECORD` & `dal_python-0.1.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dal/__init__.py,sha256=rbufEZzRAsLcNIQbmKkYtkQhqSTjRpeMay4YYhF6Gho,156
 dal/_dal.cpython-39-x86_64-linux-gnu.so,sha256=eBVA7Is5rzB-P6seZo9zV-fgUlrf6GNRUAPEyqk0FJc,565728
 dal/dal.py,sha256=cX7NvNieDSepocsp-Vl11flPhlUkJm_T6p-CSIYyhRY,52351
 dal/dal_wrap.cpp,sha256=l9jFLRd5MirEA4a-hZe8QmqpoLUvrKKIaeORNUudr3w,630288
 dal/libdal.so,sha256=n0sJ1bMG9tXyVFgDUP7KKhB-7-Q7QMPZumyv9heG7hA,8210832
 dal/libdal.so.1.0.0-dev,sha256=n0sJ1bMG9tXyVFgDUP7KKhB-7-Q7QMPZumyv9heG7hA,8210832
 dal/libdal_public.so,sha256=Jh12oOk96vd2ZPVo63BUnuz7sCQNRp3_Vhf1VSY3mmE,218232
-dal_python-0.1.4.dist-info/METADATA,sha256=euyIDk1WV8Lwf2NsGekVkQXHHYddekKw4R03gg5wnKU,799
-dal_python-0.1.4.dist-info/WHEEL,sha256=3oXbtF4vYwmQyf0LQIagKtl0VO3gP86556qKiLb0bDc,103
-dal_python-0.1.4.dist-info/top_level.txt,sha256=0NCtz794zxjwhJcMbphMLr-IHz_8WAyZFNMqTPXtulw,4
-dal_python-0.1.4.dist-info/RECORD,,
+dal_python-0.1.5.dist-info/METADATA,sha256=izwI8tJcU_qQhIXoIlACnJdsY5x27r3qYyFaXP4lG5c,799
+dal_python-0.1.5.dist-info/WHEEL,sha256=3oXbtF4vYwmQyf0LQIagKtl0VO3gP86556qKiLb0bDc,103
+dal_python-0.1.5.dist-info/top_level.txt,sha256=0NCtz794zxjwhJcMbphMLr-IHz_8WAyZFNMqTPXtulw,4
+dal_python-0.1.5.dist-info/RECORD,,
```


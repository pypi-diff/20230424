# Comparing `tmp/ormsgpack-1.2.5.tar.gz` & `tmp/ormsgpack-1.2.6.tar.gz`

## Comparing `ormsgpack-1.2.5.tar` & `ormsgpack-1.2.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 ormsgpack-1.2.5/Cargo.toml
--rw-r--r--   0     1001      123     4984 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/CHANGELOG.md
--rw-r--r--   0     1001      123    10847 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/LICENSE-APACHE
--rw-r--r--   0     1001      123     1023 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/LICENSE-MIT
--rw-r--r--   0     1001      123    41848 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/README.md
--rw-r--r--   0     1001      123      111 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/build.rs
--rw-r--r--   0     1001      123     1139 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/pyproject.toml
--rw-r--r--   0     1001      123     1083 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/deserialize/cache.rs
--rw-r--r--   0     1001      123    13846 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/deserialize/deserializer.rs
--rw-r--r--   0     1001      123      301 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/deserialize/error.rs
--rw-r--r--   0     1001      123      205 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/deserialize/mod.rs
--rw-r--r--   0     1001      123      578 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/exc.rs
--rw-r--r--   0     1001      123     1591 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/ffi.rs
--rw-r--r--   0     1001      123    16926 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/lib.rs
--rw-r--r--   0     1001      123     1142 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/opt.rs
--rw-r--r--   0     1001      123      743 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/bytes.rs
--rw-r--r--   0     1001      123     5529 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/dataclass.rs
--rw-r--r--   0     1001      123     9531 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/datetime.rs
--rw-r--r--   0     1001      123     2264 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/default.rs
--rw-r--r--   0     1001      123    13527 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/dict.rs
--rw-r--r--   0     1001      123     1404 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/int.rs
--rw-r--r--   0     1001      123     1536 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/list.rs
--rw-r--r--   0     1001      123      232 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/mod.rs
--rw-r--r--   0     1001      123    16602 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/numpy.rs
--rw-r--r--   0     1001      123    12250 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/serializer.rs
--rw-r--r--   0     1001      123     1446 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/str.rs
--rw-r--r--   0     1001      123     1523 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/tuple.rs
--rw-r--r--   0     1001      123     1945 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/uuid.rs
--rw-r--r--   0     1001      123     5390 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/serialize/writer.rs
--rw-r--r--   0     1001      123     9829 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/typeref.rs
--rw-r--r--   0     1001      123     5142 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/unicode.rs
--rw-r--r--   0     1001      123     2270 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/src/util.rs
--rw-r--r--   0     1001      123    10051 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/Cargo.lock
--rw-r--r--   0     1001      123      133 2023-02-02 10:03:02.000000 ormsgpack-1.2.5/setup.py
--rw-r--r--   0        0        0    43272 1970-01-01 00:00:00.000000 ormsgpack-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 ormsgpack-1.2.6/Cargo.toml
+-rw-r--r--   0     1001      123     5169 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/CHANGELOG.md
+-rw-r--r--   0     1001      123    10847 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1023 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/LICENSE-MIT
+-rw-r--r--   0     1001      123    41848 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/README.md
+-rw-r--r--   0     1001      123      111 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/build.rs
+-rw-r--r--   0     1001      123     1139 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/pyproject.toml
+-rw-r--r--   0     1001      123     1083 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/deserialize/cache.rs
+-rw-r--r--   0     1001      123    13846 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/deserialize/deserializer.rs
+-rw-r--r--   0     1001      123      301 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/deserialize/error.rs
+-rw-r--r--   0     1001      123      205 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/deserialize/mod.rs
+-rw-r--r--   0     1001      123      578 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/exc.rs
+-rw-r--r--   0     1001      123     1591 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/ffi.rs
+-rw-r--r--   0     1001      123     2263 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/lazy.rs
+-rw-r--r--   0     1001      123    16936 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/lib.rs
+-rw-r--r--   0     1001      123     1142 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/opt.rs
+-rw-r--r--   0     1001      123      743 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/bytes.rs
+-rw-r--r--   0     1001      123     5529 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/dataclass.rs
+-rw-r--r--   0     1001      123     9531 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/datetime.rs
+-rw-r--r--   0     1001      123     2264 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/default.rs
+-rw-r--r--   0     1001      123    13527 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/dict.rs
+-rw-r--r--   0     1001      123     1404 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/int.rs
+-rw-r--r--   0     1001      123     1536 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/list.rs
+-rw-r--r--   0     1001      123      232 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/mod.rs
+-rw-r--r--   0     1001      123    16566 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/numpy.rs
+-rw-r--r--   0     1001      123    12250 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/serializer.rs
+-rw-r--r--   0     1001      123     1446 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/str.rs
+-rw-r--r--   0     1001      123     1523 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/tuple.rs
+-rw-r--r--   0     1001      123     1945 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/uuid.rs
+-rw-r--r--   0     1001      123     5390 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/serialize/writer.rs
+-rw-r--r--   0     1001      123     9903 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/typeref.rs
+-rw-r--r--   0     1001      123     5142 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/unicode.rs
+-rw-r--r--   0     1001      123     2270 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/src/util.rs
+-rw-r--r--   0     1001      123    10051 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/Cargo.lock
+-rw-r--r--   0     1001      123      133 2023-04-24 08:03:17.000000 ormsgpack-1.2.6/setup.py
+-rw-r--r--   0        0        0    43272 1970-01-01 00:00:00.000000 ormsgpack-1.2.6/PKG-INFO
```

### Comparing `ormsgpack-1.2.5/Cargo.toml` & `ormsgpack-1.2.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ormsgpack"
-version = "1.2.5"
+version = "1.2.6"
 authors = ["Aviram Hassan <aviramyhassan@gmail.com>"]
 description = "Fast, correct Python msgpack library supporting dataclasses, datetimes, and numpy"
 edition = "2018"
 license = "Apache-2.0 OR MIT"
 repository = "https://github.com/aviramha/ormsgpack"
 homepage = "https://github.com/aviramha/ormsgpack"
 readme = "README.md"
```

### Comparing `ormsgpack-1.2.5/CHANGELOG.md` & `ormsgpack-1.2.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 1.2.6 24/04/2023
+
+### Fixed
+
+- `once_cell` poisoning on parallel initialization by (@Quitlox)[https://github.com/Quitlox] in (#153)[https://github.com/aviramha/ormsgpack/pull/153]
+
+
 ## 1.2.5 02/02/2023
 
 ### Fixed
 
 - aarch64 build on macOS. Took `src/serialize/writer.rs` from upstream orjson. by @ijl
 - Fix release on aarch64 to match orjson's upstream.
```

### Comparing `ormsgpack-1.2.5/LICENSE-APACHE` & `ormsgpack-1.2.6/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/LICENSE-MIT` & `ormsgpack-1.2.6/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/README.md` & `ormsgpack-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/pyproject.toml` & `ormsgpack-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/deserialize/cache.rs` & `ormsgpack-1.2.6/src/deserialize/cache.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/deserialize/deserializer.rs` & `ormsgpack-1.2.6/src/deserialize/deserializer.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/exc.rs` & `ormsgpack-1.2.6/src/exc.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/ffi.rs` & `ormsgpack-1.2.6/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/lib.rs` & `ormsgpack-1.2.6/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 #[macro_use]
 mod util;
 
 mod deserialize;
 mod exc;
 mod ffi;
+mod lazy;
 mod opt;
 mod serialize;
 mod typeref;
 mod unicode;
 
 use pyo3::ffi::*;
 use std::borrow::Cow;
```

### Comparing `ormsgpack-1.2.5/src/opt.rs` & `ormsgpack-1.2.6/src/opt.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/bytes.rs` & `ormsgpack-1.2.6/src/serialize/bytes.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/dataclass.rs` & `ormsgpack-1.2.6/src/serialize/dataclass.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/datetime.rs` & `ormsgpack-1.2.6/src/serialize/datetime.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/default.rs` & `ormsgpack-1.2.6/src/serialize/default.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/dict.rs` & `ormsgpack-1.2.6/src/serialize/dict.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/int.rs` & `ormsgpack-1.2.6/src/serialize/int.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/list.rs` & `ormsgpack-1.2.6/src/serialize/list.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/numpy.rs` & `ormsgpack-1.2.6/src/serialize/numpy.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use crate::typeref::{ARRAY_STRUCT_STR, NUMPY_TYPES};
 use pyo3::ffi::*;
 use serde::ser::{Serialize, SerializeSeq, Serializer};
-use std::ops::DerefMut;
 use std::os::raw::{c_char, c_int, c_void};
 
 macro_rules! slice {
     ($ptr:expr, $size:expr) => {
         unsafe { std::slice::from_raw_parts($ptr, $size) }
     };
 }
@@ -431,15 +430,15 @@
 impl Serialize for NumpyScalar {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         unsafe {
             let ob_type = ob_type!(self.ptr);
-            let scalar_types = NUMPY_TYPES.deref_mut().as_ref().unwrap();
+            let scalar_types = NUMPY_TYPES.as_ref().unwrap();
             if ob_type == scalar_types.float64 {
                 (*(self.ptr as *mut NumpyFloat64)).serialize(serializer)
             } else if ob_type == scalar_types.float32 {
                 (*(self.ptr as *mut NumpyFloat32)).serialize(serializer)
             } else if ob_type == scalar_types.int64 {
                 (*(self.ptr as *mut NumpyInt64)).serialize(serializer)
             } else if ob_type == scalar_types.int32 {
```

### Comparing `ormsgpack-1.2.5/src/serialize/serializer.rs` & `ormsgpack-1.2.6/src/serialize/serializer.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/str.rs` & `ormsgpack-1.2.6/src/serialize/str.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/tuple.rs` & `ormsgpack-1.2.6/src/serialize/tuple.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/uuid.rs` & `ormsgpack-1.2.6/src/serialize/uuid.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/serialize/writer.rs` & `ormsgpack-1.2.6/src/serialize/writer.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/typeref.rs` & `ormsgpack-1.2.6/src/typeref.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 // SPDX-License-Identifier: (Apache-2.0 OR MIT)
 
 use ahash::RandomState;
-use once_cell::unsync::Lazy;
 use pyo3::ffi::*;
 use std::os::raw::c_char;
 use std::ptr::NonNull;
 use std::sync::Once;
 
+use crate::lazy::ThreadSafeLazy;
+
 pub struct NumpyTypes {
     pub array: *mut PyTypeObject,
     pub float64: *mut PyTypeObject,
     pub float32: *mut PyTypeObject,
     pub int64: *mut PyTypeObject,
     pub int32: *mut PyTypeObject,
     pub int8: *mut PyTypeObject,
@@ -33,16 +34,18 @@
 pub static mut DICT_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut DATETIME_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut DATE_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut TIME_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut TUPLE_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut UUID_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut ENUM_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
-pub static mut NUMPY_TYPES: Lazy<Option<NumpyTypes>> = Lazy::new(|| unsafe { load_numpy_types() });
-pub static mut FIELD_TYPE: Lazy<NonNull<PyObject>> = Lazy::new(|| unsafe { look_up_field_type() });
+pub static mut NUMPY_TYPES: ThreadSafeLazy<Option<NumpyTypes>> =
+    ThreadSafeLazy::new(|| unsafe { load_numpy_types() });
+pub static mut FIELD_TYPE: ThreadSafeLazy<NonNull<PyObject>> =
+    ThreadSafeLazy::new(|| unsafe { look_up_field_type() });
 
 pub static mut BYTES_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut BYTEARRAY_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 pub static mut MEMORYVIEW_TYPE: *mut PyTypeObject = 0 as *mut PyTypeObject;
 
 pub static mut INT_ATTR_STR: *mut PyObject = 0 as *mut PyObject;
 pub static mut UTCOFFSET_METHOD_STR: *mut PyObject = 0 as *mut PyObject;
@@ -56,15 +59,16 @@
 pub static mut PYDANTIC_FIELDS_STR: *mut PyObject = 0 as *mut PyObject;
 pub static mut FIELD_TYPE_STR: *mut PyObject = 0 as *mut PyObject;
 pub static mut ARRAY_STRUCT_STR: *mut PyObject = 0 as *mut PyObject;
 pub static mut VALUE_STR: *mut PyObject = 0 as *mut PyObject;
 pub static mut STR_HASH_FUNCTION: Option<hashfunc> = None;
 pub static mut DEFAULT: *mut PyObject = 0 as *mut PyObject;
 pub static mut OPTION: *mut PyObject = 0 as *mut PyObject;
-pub static mut HASH_BUILDER: Lazy<ahash::RandomState> = Lazy::new(|| unsafe {
+
+pub static mut HASH_BUILDER: ThreadSafeLazy<ahash::RandomState> = ThreadSafeLazy::new(|| unsafe {
     RandomState::with_seeds(
         VALUE_STR as u64,
         DICT_TYPE as u64,
         STR_TYPE as u64,
         BYTES_TYPE as u64,
     )
 });
```

### Comparing `ormsgpack-1.2.5/src/unicode.rs` & `ormsgpack-1.2.6/src/unicode.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/src/util.rs` & `ormsgpack-1.2.6/src/util.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.2.5/Cargo.lock` & `ormsgpack-1.2.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 name = "once_cell"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
 
 [[package]]
 name = "ormsgpack"
-version = "1.2.5"
+version = "1.2.6"
 dependencies = [
  "ahash",
  "associative-cache",
  "bytecount",
  "encoding_rs",
  "inlinable_string",
  "itoa",
```

### Comparing `ormsgpack-1.2.5/PKG-INFO` & `ormsgpack-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormsgpack
-Version: 1.2.5
+Version: 1.2.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
```


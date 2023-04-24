# Comparing `tmp/spiff_element_units-0.1.0.tar.gz` & `tmp/spiff_element_units-0.2.0.tar.gz`

## Comparing `spiff_element_units-0.1.0.tar` & `spiff_element_units-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0      238 1970-01-01 00:00:00.000000 spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/Cargo.toml
--rw-r--r--   0     1001      123       20 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/.gitignore
--rw-r--r--   0     1001      123     1165 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/src/cache.rs
--rw-r--r--   0     1001      123     1247 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/workflow_spec.json
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 spiff_element_units-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/.gitignore
--rw-r--r--   0     1001      123      381 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      609 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/spiff-element-units.pyi
--rw-r--r--   0     1001      123      899 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     8534 2023-04-17 16:26:55.000000 spiff_element_units-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 spiff_element_units-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/Cargo.toml
+-rw-r--r--   0     1001      123       20 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/.gitignore
+-rw-r--r--   0     1001      123     1122 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/cache.rs
+-rw-r--r--   0     1001      123     8367 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/domain.rs
+-rw-r--r--   0     1001      123      619 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/element_units.rs
+-rw-r--r--   0     1001      123     3076 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/lib.rs
+-rw-r--r--   0     1001      123      349 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/manifest.rs
+-rw-r--r--   0     1001      123     2452 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/reader.rs
+-rw-r--r--   0     1001      123      910 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/writer.rs
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      473 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      609 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/spiff_element_units.pyi
+-rw-r--r--   0     1001      123     1326 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    11005 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/PKG-INFO
```

### Comparing `spiff_element_units-0.1.0/local_dependencies/spiff-element-units-rs/src/cache.rs` & `spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/cache.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 use std::fs;
-use std::fs::File;
 use std::io;
-use std::io::prelude::*;
 use std::path::{Path, PathBuf};
 
+pub mod entry {
+
+    pub enum Type {
+        OriginalWorkflowSpecsJSON,
+        Manifest,
+        ManifestEntry(String),
+    }
+
+    impl Type {
+        pub fn filename(&self) -> String {
+            use Type::*;
+
+            match self {
+                OriginalWorkflowSpecsJSON => "workflow_specs.json".to_string(),
+                Manifest => "manifest.json".to_string(),
+                ManifestEntry(id) => format!("{}.json", id),
+            }
+        }
+    }
+}
+
 const CACHE_VERSION: &str = "v1";
-const WORKFLOW_SPECS_JSON_FILENAME: &str = "workflow_specs.json";
 
-pub fn write_workflow_specs(
+pub fn created_path_for_entry(
     cache_dir: &str,
     cache_key: &str,
-    workflow_specs_json: &str,
-) -> io::Result<()> {
-    let path = created_cache_path(cache_dir, cache_key)?.join(WORKFLOW_SPECS_JSON_FILENAME);
-    let mut file = File::create(path)?;
-    file.write_all(workflow_specs_json.as_bytes())?;
+    entry_type: entry::Type,
+) -> io::Result<PathBuf> {
+    let cache_path = cache_path(cache_dir, cache_key);
+    fs::create_dir_all(&cache_path)?;
 
-    Ok(())
+    Ok(cache_path.join(entry_type.filename()))
 }
 
-pub fn read_workflow_specs(cache_dir: &str, cache_key: &str) -> io::Result<String> {
-    std::fs::read_to_string(workflow_specs_cache_path(cache_dir, cache_key))
+pub fn path_for_entry(cache_dir: &str, cache_key: &str, entry_type: entry::Type) -> PathBuf {
+    cache_path(cache_dir, cache_key).join(entry_type.filename())
 }
 
 fn cache_path(cache_dir: &str, cache_key: &str) -> PathBuf {
     Path::new(cache_dir).join(CACHE_VERSION).join(cache_key)
 }
-
-fn created_cache_path(cache_dir: &str, cache_key: &str) -> io::Result<PathBuf> {
-    let cache_path = cache_path(cache_dir, cache_key);
-    fs::create_dir_all(&cache_path)?;
-    Ok(cache_path)
-}
-
-fn workflow_specs_cache_path(cache_dir: &str, cache_key: &str) -> PathBuf {
-    cache_path(cache_dir, cache_key).join(WORKFLOW_SPECS_JSON_FILENAME)
-}
```

### Comparing `spiff_element_units-0.1.0/.gitignore` & `spiff_element_units-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spiff_element_units-0.1.0/spiff-element-units.pyi` & `spiff_element_units-0.2.0/spiff_element_units.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     """
 
 def workflow_from_cached_element_unit(
         cache_dir: str,
         cache_key: str,
         element_id: str) -> str:
     """
-    Returns a workflow describes in specs json format that is capable of 
+    Returns a workflow described in specs json format that is capable of 
     executing an element unit that contains element_id and is associated 
     with cache_key.
     """
```

### Comparing `spiff_element_units-0.1.0/Cargo.lock` & `spiff_element_units-0.2.0/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,80 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cpufeatures"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
+name = "digest"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "itoa"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
 name = "libc"
 version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
@@ -164,14 +218,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "ryu"
+version = "1.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
@@ -190,32 +250,56 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
+name = "serde_json"
+version = "1.0.96"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+dependencies = [
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "sha2"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spiff-element-units"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "spiff-element-units-rs",
 ]
 
 [[package]]
 name = "spiff-element-units-rs"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "serde",
+ "serde_json",
+ "sha2",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -239,26 +323,38 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
+name = "typenum"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
```


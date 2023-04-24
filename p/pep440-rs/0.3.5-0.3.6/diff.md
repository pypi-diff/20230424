# Comparing `tmp/pep440_rs-0.3.5.tar.gz` & `tmp/pep440_rs-0.3.6.tar.gz`

## Comparing `pep440_rs-0.3.5.tar` & `pep440_rs-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pep440_rs-0.3.5/Cargo.toml
--rw-r--r--   0      501       20      869 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Changelog.md
--rw-r--r--   0      501       20    10173 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/License-Apache
--rw-r--r--   0      501       20     1293 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/License-BSD
--rw-r--r--   0      501       20     2978 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/README.md
--rw-r--r--   0      501       20     2978 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Readme.md
--rw-r--r--   0      501       20      274 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/pyproject.toml
--rw-r--r--   0      501       20     2105 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/Readme.md
--rw-r--r--   0      501       20     4043 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/lib.rs
--rw-r--r--   0      501       20    39057 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/version.rs
--rw-r--r--   0      501       20    42526 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/version_specifier.rs
--rw-r--r--   0      501       20    10919 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Cargo.lock
--rw-r--r--   0      501       20     1084 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/pep440_rs/__init__.pyi
--rw-r--r--   0      501       20      534 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/pep440_rs/__init__.py
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 pep440_rs-0.3.6/Cargo.toml
+-rw-r--r--   0      501       20      901 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Changelog.md
+-rw-r--r--   0      501       20    10173 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/License-Apache
+-rw-r--r--   0      501       20     1293 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/License-BSD
+-rw-r--r--   0      501       20     2981 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Readme.md
+-rw-r--r--   0      501       20      274 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/pyproject.toml
+-rw-r--r--   0      501       20     2105 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/Readme.md
+-rw-r--r--   0      501       20     4043 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/lib.rs
+-rw-r--r--   0      501       20    39057 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/version.rs
+-rw-r--r--   0      501       20    42526 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/version_specifier.rs
+-rw-r--r--   0      501       20    10917 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Cargo.lock
+-rw-r--r--   0      501       20     1084 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/pep440_rs/__init__.pyi
+-rw-r--r--   0      501       20      534 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/pep440_rs/__init__.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.6/PKG-INFO
```

### Comparing `pep440_rs-0.3.5/Cargo.toml` & `pep440_rs-0.3.6/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [package]
 name = "pep440_rs"
-version = "0.3.5"
+version = "0.3.6"
 description = "A library for python version numbers and specifiers, implementing PEP 440"
 edition = "2021"
+include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
 # Same license as pypa/packaging where the tests are from
 license = "Apache-2.0 OR BSD-2-Clause"
 repository = "https://github.com/konstin/pep440-rs"
-include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
+readme = "Readme.md"
 
 [lib]
 name = "pep440_rs"
 crate-type = ["rlib", "cdylib"]
 
 [dependencies]
 lazy_static = "1.4.0"
```

### Comparing `pep440_rs-0.3.5/Changelog.md` & `pep440_rs-0.3.6/Changelog.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.3.6
+
+* Fix Readme display
+
 ## 0.3.5
 
 * Make string serialization look more like poetry's
 * Implement `__hash__` for `VersionSpecifier`
 
 ## 0.3.4
```

### Comparing `pep440_rs-0.3.5/License-Apache` & `pep440_rs-0.3.6/License-Apache`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/License-BSD` & `pep440_rs-0.3.6/License-BSD`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/README.md` & `pep440_rs-0.3.6/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # PEP440 in rust
 
-[![Crates.io](https://img.shields.io/crates/v/pep440_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
-[![PyPI](https://img.shields.io/pypi/v/pep440_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+[![Crates.io](https://img.shields.io/crates/v/pep440_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/pep440_rs)
+[![PyPI](https://img.shields.io/pypi/v/pep440_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/pep440_rs)
 
 A library for python version numbers and specifiers, implementing
 [PEP 440](https://peps.python.org/pep-0440). See [Reimplementing PEP 440](https://cohost.org/konstin/post/514863-reimplementing-pep-4) for some background.
 
 Higher level bindings to the requirements syntax are available in [pep508_rs](https://github.com/konstin/pep508_rs).
 
 ```rust
 use std::str::FromStr;
 use pep440_rs::{parse_version_specifiers, Version, VersionSpecifier};
 
 let version = Version::from_str("1.19").unwrap();
-let version_specifier = VersionSpecifier::from_str("== 1.*").unwrap();
+let version_specifier = VersionSpecifier::from_str("==1.*").unwrap();
 assert!(version_specifier.contains(&version));
 let version_specifiers = parse_version_specifiers(">=1.16, <2.0").unwrap();
 assert!(version_specifiers.iter().all(|specifier| specifier.contains(&version)));
 ```
 
 In python (`pip install pep440_rs`):
```

### Comparing `pep440_rs-0.3.5/Readme.md` & `pep440_rs-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-# PEP440 in rust
+Metadata-Version: 2.1
+Name: pep440_rs
+Version: 0.3.6
+Summary: A library for python version numbers and specifiers, implementing PEP 440
+License: Apache-2.0 OR BSD-2-Clause
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/konstin/pep440-rs
 
-[![Crates.io](https://img.shields.io/crates/v/pep440_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
-[![PyPI](https://img.shields.io/pypi/v/pep440_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+# PEP440 in rust
 
 A library for python version numbers and specifiers, implementing
-[PEP 440](https://peps.python.org/pep-0440). See [Reimplementing PEP 440](https://cohost.org/konstin/post/514863-reimplementing-pep-4) for some background.
-
-Higher level bindings to the requirements syntax are available in [pep508_rs](https://github.com/konstin/pep508_rs).
+[PEP 440](https://peps.python.org/pep-0440)
 
-```rust
-use std::str::FromStr;
-use pep440_rs::{parse_version_specifiers, Version, VersionSpecifier};
-
-let version = Version::from_str("1.19").unwrap();
-let version_specifier = VersionSpecifier::from_str("== 1.*").unwrap();
-assert!(version_specifier.contains(&version));
-let version_specifiers = parse_version_specifiers(">=1.16, <2.0").unwrap();
-assert!(version_specifiers.iter().all(|specifier| specifier.contains(&version)));
+```shell
+pip install pep440_rs
 ```
 
-In python (`pip install pep440_rs`):
-
 ```python
 from pep440_rs import Version, VersionSpecifier
 
 assert Version("1.1a1").any_prerelease()
 assert Version("1.1.dev2").any_prerelease()
 assert not Version("1.1").any_prerelease()
 assert VersionSpecifier(">=1.0").contains(Version("1.1a1"))
 assert not VersionSpecifier(">=1.1").contains(Version("1.1a1"))
-# Note that python comparisons are the version ordering, not the version specifiers operators
-assert Version("1.1") >= Version("1.1a1")
 assert Version("2.0") in VersionSpecifier("==2")
 ```
 
+Unlike [pypa/packaging](https://github.com/pypa/packaging), this library always matches preleases. To only match final releases, filter with `.any_prelease()` beforehand.
+
 PEP 440 has a lot of unintuitive features, including:
 
 * An epoch that you can prefix the version which, e.g. `1!1.2.3`. Lower epoch always means lower
   version (`1.0 <=2!0.1`)
 * post versions, which can be attached to both stable releases and prereleases
 * dev versions, which can be attached to sbpth table releases and prereleases. When attached to a
   prerelease the dev version is ordered just below the normal prerelease, however when attached
@@ -50,7 +44,8 @@
 * prelease vs. prerelease incl. dev is fuzzy
 * local versions on top of all the others, which are added with a + and have implicitly typed
   string and number segments
 * no semver-caret (`^`), but a pseudo-semver tilde (`~=`)
 * ordering contradicts matching: We have e.g. `1.0+local > 1.0` when sorting,
   but `==1.0` matches `1.0+local`. While the ordering of versions itself is a total order
   the version matching needs to catch all sorts of special cases
+
```

### Comparing `pep440_rs-0.3.5/python/Readme.md` & `pep440_rs-0.3.6/python/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/src/lib.rs` & `pep440_rs-0.3.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/src/version.rs` & `pep440_rs-0.3.6/src/version.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/src/version_specifier.rs` & `pep440_rs-0.3.6/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/Cargo.lock` & `pep440_rs-0.3.6/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -45,17 +45,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -105,15 +105,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.5"
+version = "0.3.6"
 dependencies = [
  "indoc 2.0.1",
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
@@ -124,75 +124,75 @@
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.55"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc 1.0.9",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -211,53 +211,53 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
@@ -271,17 +271,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `pep440_rs-0.3.5/python/pep440_rs/__init__.pyi` & `pep440_rs-0.3.6/python/pep440_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.5/python/pep440_rs/__init__.py` & `pep440_rs-0.3.6/python/pep440_rs/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/biobear-0.1.6.tar.gz` & `tmp/biobear-0.2.0.tar.gz`

## Comparing `biobear-0.1.6.tar` & `biobear-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,43 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 biobear-0.1.6/Cargo.toml
--rw-r--r--   0     1001      123     2663 2023-04-23 00:24:08.000000 biobear-0.1.6/.github/workflows/build-test-release.yml
--rw-r--r--   0     1001      123     4135 2023-04-23 00:24:08.000000 biobear-0.1.6/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-23 00:24:08.000000 biobear-0.1.6/LICENSE
--rw-r--r--   0     1001      123       68 2023-04-23 00:24:08.000000 biobear-0.1.6/Makefile
--rw-r--r--   0     1001      123     6254 2023-04-23 00:24:08.000000 biobear-0.1.6/README.md
--rw-r--r--   0     1001      123      167 2023-04-23 00:24:08.000000 biobear-0.1.6/cz.json
--rw-r--r--   0     1001      123      421 2023-04-23 00:24:08.000000 biobear-0.1.6/pyproject.toml
--rw-r--r--   0     1001      123      401 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/__init__.py
--rw-r--r--   0     1001      123      895 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      383 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      383 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      373 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123      838 2023-04-23 00:24:08.000000 biobear-0.1.6/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123     6152 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     8296 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      212 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123      286 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      112 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/test.gff
--rw-r--r--   0     1001      123     4302 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      483 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123      411 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123      300 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      280 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123      591 2023-04-23 00:24:08.000000 biobear-0.1.6/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123     7737 2023-04-23 00:24:08.000000 biobear-0.1.6/src/bam_reader.rs
--rw-r--r--   0     1001      123     2989 2023-04-23 00:24:08.000000 biobear-0.1.6/src/fasta_reader.rs
--rw-r--r--   0     1001      123     3505 2023-04-23 00:24:08.000000 biobear-0.1.6/src/fastq_reader.rs
--rw-r--r--   0     1001      123     4645 2023-04-23 00:24:08.000000 biobear-0.1.6/src/gff_reader.rs
--rw-r--r--   0     1001      123      526 2023-04-23 00:24:08.000000 biobear-0.1.6/src/lib.rs
--rw-r--r--   0     1001      123     6420 2023-04-23 00:24:08.000000 biobear-0.1.6/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37517 2023-04-23 00:25:00.000000 biobear-0.1.6/Cargo.lock
--rw-r--r--   0        0        0     6632 1970-01-01 00:00:00.000000 biobear-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 biobear-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2566 2023-04-24 15:23:51.000000 biobear-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      890 2023-04-24 15:23:51.000000 biobear-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-04-24 15:23:51.000000 biobear-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-24 15:23:51.000000 biobear-0.2.0/LICENSE
+-rw-r--r--   0     1001      123       68 2023-04-24 15:23:51.000000 biobear-0.2.0/Makefile
+-rw-r--r--   0     1001      123     5677 2023-04-24 15:23:51.000000 biobear-0.2.0/README.md
+-rw-r--r--   0     1001      123      167 2023-04-24 15:23:51.000000 biobear-0.2.0/cz.json
+-rw-r--r--   0     1001      123      555 2023-04-24 15:23:51.000000 biobear-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      453 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123      895 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      536 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123      969 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123      991 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      373 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123      840 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123     6152 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8296 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      212 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123     4302 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      822 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123      855 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123      855 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      399 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      901 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-04-24 15:23:51.000000 biobear-0.2.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     8562 2023-04-24 15:23:51.000000 biobear-0.2.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123     3991 2023-04-24 15:23:51.000000 biobear-0.2.0/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     4420 2023-04-24 15:23:51.000000 biobear-0.2.0/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     4949 2023-04-24 15:23:51.000000 biobear-0.2.0/src/gff_reader.rs
+-rw-r--r--   0     1001      123      640 2023-04-24 15:23:51.000000 biobear-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     8074 2023-04-24 15:23:51.000000 biobear-0.2.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    37528 2023-04-24 15:24:48.000000 biobear-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 biobear-0.2.0/PKG-INFO
```

### Comparing `biobear-0.1.6/.github/workflows/build-test-release.yml` & `biobear-0.2.0/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-# This file is autogenerated by maturin v0.14.17
-# To update, run
-#
-#    maturin generate-ci github
-#
-name: CI
+name: Release
 
 on:
   push:
     tags:
       - 'v*'
 
 permissions:
```

### Comparing `biobear-0.1.6/.gitignore` & `biobear-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/LICENSE` & `biobear-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/README.md` & `biobear-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -86,17 +86,7 @@
 ```python
 import biobear as bb
 reader = bb.BamIndexedReader("test.bam", "test.bam.bai")
 result = reader.query("chr1", 1, 1000)
 
 print(result)
 ```
-
-## Limitations
-
-Currently, the library reads the entire file (or query result) into memory. This probably isn't a problem unless you're working with very large sequence files or query results.
-
-## Future Plans
-
-Eventually, I'd like to move over the rest of the code from https://github.com/tshauck/brrrr/ and eventually incorporate better parsing of VCF's (as demonstrated in https://github.com/natir/vcf2parquet and https://www.wheretrue.dev/docs/wtt01/api-reference/table-functions#read_vcf_file_records).
-
-Please open an issue if there's something you'd like to see added!
```

### Comparing `biobear-0.1.6/python/biobear/bam_reader.py` & `biobear-0.2.0/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/biobear/vcf_reader.py` & `biobear-0.2.0/python/biobear/vcf_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from pathlib import Path
 
 from .biobear import _VCFReader, _VCFIndexedReader
 
 import polars as pl
 
+
 class VCFReader:
     def __init__(self, path: Path):
         self._vcf_reader = _VCFReader(str(path))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
 
     def to_polars(self) -> pl.DataFrame:
         contents = self._vcf_reader.read()
         return pl.read_ipc(contents)
 
+
 class VCFIndexedReader:
     def __init__(self, path: Path):
         self._vcf_reader = _VCFIndexedReader(str(path))
 
     def read(self) -> pl.DataFrame:
         return self.to_polars()
```

### Comparing `biobear-0.1.6/python/tests/data/bedcov.bam` & `biobear-0.2.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/data/bedcov.bam.bai` & `biobear-0.2.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/data/file.vcf` & `biobear-0.2.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/data/index.vcf.gz` & `biobear-0.2.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/data/vcf_file.vcf` & `biobear-0.2.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/data/vcf_file.vcf.gz` & `biobear-0.2.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.1.6/python/tests/test_vcf_reader.py` & `biobear-0.2.0/python/tests/test_vcf_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 # Test the fasta reader can be converted to a polars dataframe
 
 from pathlib import Path
 
+import pytest
+
 from biobear import VCFReader, VCFIndexedReader
 
 DATA = Path(__file__).parent / "data"
 
 
 def test_vcf_reader():
     reader = VCFReader(DATA / "vcf_file.vcf")
-    df = reader.to_polars()
+    df = reader.read()
 
     assert len(df) == 15
 
-def test_sam_indexed_reader_read():
+def test_vcf_reader_missing_file():
+    with pytest.raises(FileNotFoundError):
+        VCFReader("test.vcf")
+
+def test_vcf_indexed_reader_read():
     reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
     df = reader.read()
 
     assert len(df) == 15
 
-
-def test_sam_indexed_reader_quer():
+def test_vcf_indexed_reader_query():
     reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
     df = reader.query("1")
 
     assert len(df) == 11
+
+    with pytest.raises(ValueError):
+        reader.query("chr1")
+
+def test_vcf_indexed_reader_query_missing_file():
+    with pytest.raises(OSError):
+        VCFIndexedReader("test.vcf.gz")
```

### Comparing `biobear-0.1.6/src/bam_reader.rs` & `biobear-0.2.0/src/bam_reader.rs`

 * *Files 25% similar despite different names*

```diff
@@ -149,33 +149,33 @@
     reader: bam::Reader<bgzf::Reader<BufReader<File>>>,
     header: sam::Header,
 }
 
 #[pymethods]
 impl BamReader {
     #[new]
-    fn new(path: &str) -> Self {
-        let file = File::open(path).unwrap();
+    fn new(path: &str) -> PyResult<Self> {
+        let file = File::open(path)?;
         let buf_reader = BufReader::new(file);
         let mut reader = bam::Reader::new(buf_reader);
         let header = reader.read_header().unwrap();
 
-        Self { reader, header }
+        Ok(Self { reader, header })
     }
 
-    fn read(&mut self) -> PyObject {
+    fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = BamBatch::new();
 
         for record in self.reader.records(&self.header) {
-            let record = record.unwrap();
+            let record = record?;
             batch.add(record, &self.header);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
@@ -186,65 +186,91 @@
     reader: bam::IndexedReader<bgzf::Reader<BufReader<File>>>,
     header: sam::Header,
 }
 
 #[pymethods]
 impl BamIndexedReader {
     #[new]
-    fn new(path: &str, index_path: Option<&str>) -> Self {
-        let file = File::open(path).unwrap();
+    fn new(path: &str, index_path: Option<&str>) -> PyResult<Self> {
+        let file = File::open(path)?;
+
         let buf_reader = BufReader::new(file);
 
-        let infered_path = match index_path {
+        let inferred_path = match index_path {
             Some(path) => path.to_string(),
             None => format!("{}.bai", path),
         };
 
-        let index = bam::bai::read(infered_path).unwrap();
+        let index = bam::bai::read(inferred_path)?;
 
-        let mut reader = bam::indexed_reader::Builder::default()
+        let mut reader = match bam::indexed_reader::Builder::default()
             .set_index(index)
             .build_from_reader(buf_reader)
-            .unwrap();
+        {
+            Ok(reader) => reader,
+            Err(_) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
+                    "Failed to open file: {}",
+                    path
+                )))
+            }
+        };
 
-        let header = reader.read_header().unwrap();
+        let header = match reader.read_header() {
+            Ok(header) => header,
+            Err(_) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
+                    "Failed to read header: {}",
+                    path
+                )))
+            }
+        };
 
-        Self { reader, header }
+        Ok(Self { reader, header })
     }
 
-    fn read(&mut self) -> PyObject {
+    fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = BamBatch::new();
 
         for record in self.reader.records(&self.header) {
-            let record = record.unwrap();
+            let record = record?;
             batch.add(record, &self.header);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
-    fn query(&mut self, chromosome: &str, start: usize, end: usize) -> PyObject {
+    fn query(&mut self, chromosome: &str, start: usize, end: usize) -> PyResult<PyObject> {
         let mut batch = BamBatch::new();
 
-        let start = Position::try_from(start).unwrap();
-        let end = Position::try_from(end).unwrap();
-        let query = self
+        let start = Position::try_from(start)?;
+        let end = Position::try_from(end)?;
+        let query_result = self
             .reader
-            .query(&self.header, &Region::new(chromosome, start..=end))
-            .unwrap();
+            .query(&self.header, &Region::new(chromosome, start..=end));
+
+        let query = match query_result {
+            Ok(query) => query,
+            Err(_) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                    "Failed to query region: {}:{}-{}",
+                    chromosome, start, end
+                )))
+            }
+        };
 
         for record in query {
-            let record = record.unwrap();
+            let record = record?;
             batch.add(record, &self.header);
         }
 
         let ipc = batch.to_ipc();
 
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
```

### Comparing `biobear-0.1.6/src/fasta_reader.rs` & `biobear-0.2.0/src/fasta_reader.rs`

 * *Files 20% similar despite different names*

```diff
@@ -80,33 +80,70 @@
 pub struct FastaReader {
     reader: Reader<BufReader<std::fs::File>>,
 }
 
 #[pymethods]
 impl FastaReader {
     #[new]
-    fn new(fasta_path: &str) -> Self {
-        let file = std::fs::File::open(fasta_path).unwrap();
+    fn new(fasta_path: &str) -> PyResult<Self> {
+        let file = std::fs::File::open(fasta_path)?;
         let buf_reader = BufReader::new(file);
 
         let reader = Reader::new(buf_reader);
 
-        Self { reader }
+        Ok(Self { reader })
     }
 
-    pub fn read(&mut self) -> PyObject {
+    pub fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = FastaBatch::new();
 
         for result in self.reader.records() {
-            let record = result.unwrap();
+            let record = result?;
             batch.add(record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
+    }
+
+    pub fn __enter__(slf: Py<Self>) -> Py<Self> {
+        slf
+    }
+
+    pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
+}
+
+#[pyclass(name = "_FastaGzippedReader")]
+pub struct FastaGzippedReader {
+    reader: Reader<BufReader<flate2::read::GzDecoder<std::fs::File>>>,
+}
+
+#[pymethods]
+impl FastaGzippedReader {
+    #[new]
+    fn new(fasta_path: &str) -> PyResult<Self> {
+        let file = std::fs::File::open(fasta_path)?;
+        let gz_decoder = flate2::read::GzDecoder::new(file);
+        let buf_reader = BufReader::new(gz_decoder);
+
+        let reader = Reader::new(buf_reader);
+
+        Ok(Self { reader })
+    }
+
+    pub fn read(&mut self) -> PyResult<PyObject> {
+        let mut batch = FastaBatch::new();
+
+        for result in self.reader.records() {
+            let record = result?;
+            batch.add(record);
+        }
+
+        let ipc = batch.to_ipc();
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
```

### Comparing `biobear-0.1.6/src/fastq_reader.rs` & `biobear-0.2.0/src/fastq_reader.rs`

 * *Files 18% similar despite different names*

```diff
@@ -95,31 +95,65 @@
 pub struct FastqReader {
     reader: Reader<BufReader<std::fs::File>>,
 }
 
 #[pymethods]
 impl FastqReader {
     #[new]
-    fn new(path: &str) -> Self {
-        let file = std::fs::File::open(path).unwrap();
+    fn new(path: &str) -> PyResult<Self> {
+        let file = std::fs::File::open(path)?;
         let reader = Reader::new(BufReader::new(file));
 
-        Self { reader }
+        Ok(Self { reader })
     }
 
-    pub fn read(&mut self) -> PyObject {
+    pub fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = FastqBatch::new();
 
         for record in self.reader.records() {
-            let record = record.unwrap();
+            let record = record?;
             batch.add(record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
+    }
+
+    pub fn __enter__(slf: Py<Self>) -> Py<Self> {
+        slf
+    }
+
+    pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
+}
+
+#[pyclass(name = "_FastqGzippedReader")]
+pub struct FastqGzippedReader {
+    reader: Reader<BufReader<flate2::read::GzDecoder<std::fs::File>>>,
+}
+
+#[pymethods]
+impl FastqGzippedReader {
+    #[new]
+    fn new(path: &str) -> PyResult<Self> {
+        let file = std::fs::File::open(path)?;
+        let reader = Reader::new(BufReader::new(flate2::read::GzDecoder::new(file)));
+
+        Ok(Self { reader })
+    }
+
+    pub fn read(&mut self) -> PyResult<PyObject> {
+        let mut batch = FastqBatch::new();
+
+        for record in self.reader.records() {
+            let record = record?;
+            batch.add(record);
+        }
+
+        let ipc = batch.to_ipc();
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
```

### Comparing `biobear-0.1.6/src/gff_reader.rs` & `biobear-0.2.0/src/gff_reader.rs`

 * *Files 3% similar despite different names*

```diff
@@ -122,28 +122,36 @@
 pub struct GFFReader {
     reader: noodles::gff::Reader<BufReader<File>>,
 }
 
 #[pymethods]
 impl GFFReader {
     #[new]
-    fn new(path: &str) -> Self {
-        let file = File::open(path).unwrap();
+    fn new(path: &str) -> PyResult<Self> {
+        let file = File::open(path)?;
         let reader = noodles::gff::Reader::new(BufReader::new(file));
 
-        Self { reader }
+        Ok(Self { reader })
     }
 
-    fn read(&mut self) -> PyObject {
+    fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = GFFBatch::new();
         for record in self.reader.records() {
-            let record = record.unwrap();
+            let record = match record {
+                Ok(record) => record,
+                Err(e) => {
+                    return Err(PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
+                        "Error reading record: {}",
+                        e
+                    )))
+                }
+            };
             batch.add(record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| {
+        Ok(Python::with_gil(|py| {
             let pybytes = PyBytes::new(py, &ipc);
             pybytes.into()
-        })
+        }))
     }
 }
```

### Comparing `biobear-0.1.6/src/lib.rs` & `biobear-0.2.0/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 mod fastq_reader;
 mod gff_reader;
 mod vcf_reader;
 
 #[pymodule]
 fn biobear(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<fasta_reader::FastaReader>()?;
+    m.add_class::<fasta_reader::FastaGzippedReader>()?;
+
     m.add_class::<fastq_reader::FastqReader>()?;
+    m.add_class::<fastq_reader::FastqGzippedReader>()?;
+
     m.add_class::<gff_reader::GFFReader>()?;
     m.add_class::<bam_reader::BamReader>()?;
     m.add_class::<bam_reader::BamIndexedReader>()?;
     m.add_class::<vcf_reader::VCFReader>()?;
     m.add_class::<vcf_reader::VCFIndexedReader>()?;
     Ok(())
 }
```

### Comparing `biobear-0.1.6/src/vcf_reader.rs` & `biobear-0.2.0/src/vcf_reader.rs`

 * *Files 14% similar despite different names*

```diff
@@ -133,32 +133,32 @@
     reader: vcf::Reader<BufReader<File>>,
     header: vcf::Header,
 }
 
 #[pymethods]
 impl VCFReader {
     #[new]
-    fn new(path: &str) -> Self {
-        let file = File::open(path).unwrap();
+    fn new(path: &str) -> PyResult<Self> {
+        let file = File::open(path)?;
         let mut reader = vcf::Reader::new(BufReader::new(file));
-        let header = reader.read_header().unwrap();
+        let header = reader.read_header()?;
 
-        Self { reader, header }
+        Ok(Self { reader, header })
     }
 
-    fn read(&mut self) -> PyObject {
+    fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = VcfBatch::new();
 
         for record in self.reader.records(&self.header) {
-            let record = record.unwrap();
+            let record = record?;
             batch.add(&record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
@@ -169,49 +169,97 @@
     reader: vcf::IndexedReader<File>,
     header: vcf::Header,
 }
 
 #[pymethods]
 impl VCFIndexedReader {
     #[new]
-    fn new(path: &str) -> Self {
-        let mut reader = vcf::indexed_reader::Builder::default()
-            .build_from_path(path)
-            .unwrap();
+    fn new(path: &str) -> PyResult<Self> {
+        let reader = vcf::indexed_reader::Builder::default().build_from_path(path);
+        let mut reader = match reader {
+            Ok(reader) => reader,
+            Err(e) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
+                    "Error reading VCF file: {}",
+                    e
+                )))
+            }
+        };
+
+        let header = match reader.read_header() {
+            Ok(header) => header,
+            Err(e) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                    "Error reading VCF header: {}",
+                    e
+                )))
+            }
+        };
 
-        let header = reader.read_header().unwrap();
-
-        Self { reader, header }
+        Ok(Self { reader, header })
     }
 
-    fn read(&mut self) -> PyObject {
+    fn read(&mut self) -> PyResult<PyObject> {
         let mut batch = VcfBatch::new();
 
         for record in self.reader.records(&self.header) {
-            let record = record.unwrap();
+            let record = match record {
+                Ok(record) => record,
+                Err(e) => {
+                    return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                        "Error reading VCF record: {}",
+                        e
+                    )))
+                }
+            };
             batch.add(&record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
-    fn query(&mut self, region: &str) -> PyObject {
+    fn query(&mut self, region: &str) -> PyResult<PyObject> {
         let mut batch = VcfBatch::new();
 
-        let region = region.parse().unwrap();
-        let mut iter = self.reader.query(&self.header, &region).unwrap();
+        let region = match region.parse() {
+            Ok(region) => region,
+            Err(e) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                    "Error parsing region: {}",
+                    e
+                )))
+            }
+        };
+
+        let mut iter = match self.reader.query(&self.header, &region) {
+            Ok(iter) => iter,
+            Err(e) => {
+                return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                    "Error querying VCF file: {}",
+                    e
+                )))
+            }
+        };
 
         while let Some(record) = iter.next() {
-            let record = record.unwrap();
+            let record = match record {
+                Ok(record) => record,
+                Err(e) => {
+                    return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
+                        "Error reading VCF record: {}",
+                        e
+                    )))
+                }
+            };
             batch.add(&record);
         }
 
         let ipc = batch.to_ipc();
-        Python::with_gil(|py| PyBytes::new(py, &ipc).into())
+        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
     }
 
     pub fn __enter__(slf: Py<Self>) -> Py<Self> {
         slf
     }
 
     pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
```

### Comparing `biobear-0.1.6/Cargo.lock` & `biobear-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -251,17 +251,18 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.1.6"
+version = "0.2.0"
 dependencies = [
  "arrow",
+ "flate2",
  "noodles",
  "pyo3",
 ]
 
 [[package]]
 name = "bit-vec"
 version = "0.6.3"
@@ -272,17 +273,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.1.0"
+version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c70beb79cbb5ce9c4f8e20849978f34225931f665bb49efa6982875a4d5facb3"
+checksum = "24a6904aef64d73cf10ab17ebace7befb918b82164785cb89907993be7f83813"
 
 [[package]]
 name = "bumpalo"
 version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
@@ -835,15 +836,15 @@
 
 [[package]]
 name = "noodles-sam"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dfc20f345e8220c2c2471298a99567dcf5f19c50fe1a2c275d9fc2633a0f54"
 dependencies = [
- "bitflags 2.1.0",
+ "bitflags 2.2.1",
  "indexmap",
  "lexical-core",
  "memchr",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-fasta",
```

### Comparing `biobear-0.1.6/PKG-INFO` & `biobear-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: biobear
-Version: 0.1.6
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars>=0.17.0
 License-File: LICENSE
+Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # biobear
 
 [![PyPI version](https://badge.fury.io/py/biobear.svg)](https://badge.fury.io/py/biobear)
 
@@ -98,17 +99,7 @@
 import biobear as bb
 reader = bb.BamIndexedReader("test.bam", "test.bam.bai")
 result = reader.query("chr1", 1, 1000)
 
 print(result)
 ```
 
-## Limitations
-
-Currently, the library reads the entire file (or query result) into memory. This probably isn't a problem unless you're working with very large sequence files or query results.
-
-## Future Plans
-
-Eventually, I'd like to move over the rest of the code from https://github.com/tshauck/brrrr/ and eventually incorporate better parsing of VCF's (as demonstrated in https://github.com/natir/vcf2parquet and https://www.wheretrue.dev/docs/wtt01/api-reference/table-functions#read_vcf_file_records).
-
-Please open an issue if there's something you'd like to see added!
-
```


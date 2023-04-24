# Comparing `tmp/lnschema_lamin1-0.15.1.tar.gz` & `tmp/lnschema_lamin1-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.15.1.tar", last modified: Sat Apr 22 11:07:31 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.16.0.tar", last modified: Mon Apr 24 17:50:09 2023, max compression
```

## Comparing `lnschema_lamin1-0.15.1.tar` & `lnschema_lamin1-0.16.0.tar`

### file list

```diff
@@ -1,34 +1,28 @@
--rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.15.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.15.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.15.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.15.1/.gitignore
--rw-r--r--   0        0        0     1753 2023-04-22 03:48:11.222542 lnschema_lamin1-0.15.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.15.1/README.md
--rw-r--r--   0        0        0      276 2023-04-22 11:06:42.620232 lnschema_lamin1-0.15.1/docs/changelog.md
--rw-r--r--   0        0        0     5036 2023-04-22 04:45:45.601083 lnschema_lamin1-0.15.1/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-22 04:45:45.613158 lnschema_lamin1-0.15.1/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5395 2023-04-22 04:45:45.614909 lnschema_lamin1-0.15.1/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.15.1/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.15.1/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.15.1/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.15.1/lamin-project.yaml
--rw-r--r--   0        0        0      607 2023-04-22 11:06:31.753223 lnschema_lamin1-0.15.1/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     2738 2023-04-22 05:28:10.791910 lnschema_lamin1-0.15.1/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     1460 2023-04-22 05:28:10.792065 lnschema_lamin1-0.15.1/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      250 2023-04-22 05:28:10.792423 lnschema_lamin1-0.15.1/lnschema_lamin1/link.py
--rw-r--r--   0        0        0      979 2023-03-24 23:23:34.184309 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-14-3ed88d3699fd-v0_6_0.py
--rw-r--r--   0        0        0     1188 2023-03-24 23:23:34.184393 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-01360b6492cc-v0_7_0.py
--rw-r--r--   0        0        0      630 2023-03-24 23:23:34.184479 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-05efb2ed6192-v0_6_0.post1.py
--rw-r--r--   0        0        0      940 2023-03-24 23:23:34.184551 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-a171e861e473-v0_7_1.py
--rw-r--r--   0        0        0      620 2023-03-24 23:23:34.184623 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-e2507b7564f0-v0_7_0.post1.py
--rw-r--r--   0        0        0     2173 2023-03-24 23:23:34.184690 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-20-a5d6b07f1401-v0_7_2.py
--rw-r--r--   0        0        0     2174 2023-03-24 23:23:34.184767 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-11-03-bfda12fc80a8-v0_8_0.py
--rw-r--r--   0        0        0      777 2023-04-22 05:28:10.792624 lnschema_lamin1-0.15.1/noxfile.py
--rw-r--r--   0        0        0      742 2023-04-22 11:07:17.974070 lnschema_lamin1-0.15.1/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.15.1/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.15.1/tests/test_notebooks.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 lnschema_lamin1-0.15.1/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.16.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.16.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.16.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.16.0/.gitignore
+-rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.16.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.16.0/README.md
+-rw-r--r--   0        0        0      432 2023-04-24 17:49:45.305188 lnschema_lamin1-0.16.0/docs/changelog.md
+-rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.16.0/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.16.0/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.16.0/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.16.0/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.16.0/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.16.0/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.16.0/lamin-project.yaml
+-rw-r--r--   0        0        0      617 2023-04-24 17:49:37.492197 lnschema_lamin1-0.16.0/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     2685 2023-04-24 17:49:33.168641 lnschema_lamin1-0.16.0/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     1765 2023-04-24 17:49:33.169143 lnschema_lamin1-0.16.0/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      284 2023-04-24 17:49:33.169327 lnschema_lamin1-0.16.0/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.16.0/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.16.0/noxfile.py
+-rw-r--r--   0        0        0      655 2023-04-24 16:22:20.030267 lnschema_lamin1-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.16.0/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.16.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.0/PKG-INFO
```

### Comparing `lnschema_lamin1-0.15.1/.github/workflows/build.yml` & `lnschema_lamin1-0.16.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.16.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/.gitignore` & `lnschema_lamin1-0.16.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/.pre-commit-config.yaml` & `lnschema_lamin1-0.16.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,26 @@
           )
       - id: check-yaml
       - id: check-added-large-files
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black-jupyter
+        args: [--line-length=176]
   - repo: https://github.com/pycqa/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-black==0.3.3
           - flake8-typing-imports==1.10.0
         language_version: python3
         args:
-          - --max-line-length=88
-          - --ignore=E203
+          - --max-line-length=176
+          - --ignore=E203,BLK100
         exclude: |
           (?x)(
               __init__.py
           )
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.6.2
     hooks:
```

### Comparing `lnschema_lamin1-0.15.1/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.16.0/docs/guide/01-get-started.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": "{18: {'source': ['ln.__version__']}}"}*

```diff
@@ -182,15 +182,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e66a1fd2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.__version__ == \"0.38.0\""
+                "ln.__version__"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fef7fe5a",
             "metadata": {},
```

### Comparing `lnschema_lamin1-0.15.1/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.16.0/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.16.0/docs/guide/10-migrate.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990942028985508%*

 * *Differences: {"'cells'": "{10: {'source': ['ln.select(ln1.dev.version_tvhn).df()']}, 18: {'source': "*

 * *            "['ln.select(ln1.dev.version_tvhn).df()']}}"}*

```diff
@@ -95,15 +95,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fa2a19d7-5683-4807-bbd1-321a914ec988",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.select(rt.dev.version_tvhn).df()"
+                "ln.select(ln1.dev.version_tvhn).df()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5a43308d-33a8-4681-9c78-3a15f1e00a1c",
             "metadata": {},
             "source": [
@@ -168,15 +168,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2d2fc7b0-81d5-40e3-bfd7-66ece095f09f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.select(rt.dev.version_tvhn).df()"
+                "ln.select(ln1.dev.version_tvhn).df()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "79613866-465e-4ad2-b050-434bbf8ab228",
             "metadata": {},
             "source": [
```

### Comparing `lnschema_lamin1-0.15.1/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.16.0/lnschema_lamin1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
    dev
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
-_migration = None
-__version__ = "0.15.1"
+_migration = "652443621d5a"
+__version__ = "0.16.0"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.15.1/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.16.0/lnschema_lamin1/_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,81 +9,64 @@
 from lnschema_bionty import CellType, Disease, Species, Tissue
 from lnschema_core import File
 from lnschema_core.dev.sqlmodel import add_relationship_keys, schema_sqlmodel
 from sqlalchemy.orm import relationship
 from sqlmodel import Field, Relationship
 
 from . import _name as schema_name
-from .link import BiosampleTechsample, FileBiosample, FileExperiment
+from .link import BiosampleTechsample, FileBiosample, FileCellType, FileExperiment
 
 _, prefix, schema_arg = schema_sqlmodel(schema_name)
 
 
 class Experiment(ExperimentBase, table=True):  # type: ignore
     """Experiments."""
 
-    experiment_type_id: str = Field(
-        default=None, foreign_key="lamin1.experiment_type.id", index=True
-    )
+    experiment_type_id: str = Field(default=None, foreign_key="lamin1.experiment_type.id", index=True)
     files: File = Relationship(
         back_populates="experiments",
         sa_relationship_kwargs=dict(secondary=FileExperiment.__table__),
     )
 
 
-File.experiments = relationship(
-    Experiment, back_populates="files", secondary=FileExperiment.__table__
-)
+File.experiments = relationship(Experiment, back_populates="files", secondary=FileExperiment.__table__)
 File.__sqlmodel_relationships__["experiments"] = None
 
 
 class ExperimentType(ExperimentTypeBase, table=True):  # type: ignore
     """Experiment types."""
 
     __tablename__ = f"{prefix}experiment_type"
 
 
 class Biosample(BiosampleBase, table=True):  # type: ignore
     """Biological samples that are registered in experiments."""
 
     batch: Optional[str] = None
-    species_id: Optional[str] = Field(
-        default=None, foreign_key="bionty.species.id", index=True
-    )
+    species_id: Optional[str] = Field(default=None, foreign_key="bionty.species.id", index=True)
     species: Species = Relationship()
-    tissue_id: Optional[str] = Field(
-        default=None, foreign_key="bionty.tissue.id", index=True
-    )
+    tissue_id: Optional[str] = Field(default=None, foreign_key="bionty.tissue.id", index=True)
     tissue: Tissue = Relationship()
-    cell_type_id: Optional[str] = Field(
-        default=None, foreign_key="bionty.cell_type.id", index=True
-    )
+    cell_type_id: Optional[str] = Field(default=None, foreign_key="bionty.cell_type.id", index=True)
     cell_type: CellType = Relationship()
-    disease_id: Optional[str] = Field(
-        default=None, foreign_key="bionty.disease.id", index=True
-    )
+    disease_id: Optional[str] = Field(default=None, foreign_key="bionty.disease.id", index=True)
     disease: Disease = Relationship()
     files: File = Relationship(
         back_populates="biosamples",
         sa_relationship_kwargs=dict(secondary=FileBiosample.__table__),
     )
 
 
-File.biosamples = relationship(
-    Biosample, back_populates="files", secondary=FileBiosample.__table__
-)
-File.__sqlmodel_relationships__["biosamples"] = None
-
+File.biosamples = relationship(Biosample, back_populates="files", secondary=FileBiosample.__table__)
+File.cell_types = relationship(CellType, secondary=FileCellType.__table__)
 add_relationship_keys(Biosample)
 
 
 class Techsample(TechsampleBase, table=True):  # type: ignore
     biosamples: Biosample = Relationship(
         back_populates="techsamples",
         sa_relationship_kwargs=dict(secondary=BiosampleTechsample.__table__),
     )
 
 
-Biosample.techsamples = relationship(
-    Techsample, back_populates="biosamples", secondary=BiosampleTechsample.__table__
-)
+Biosample.techsamples = relationship(Techsample, back_populates="biosamples", secondary=BiosampleTechsample.__table__)
 Biosample.__sqlmodel_relationships__["techsamples"] = None
```

### Comparing `lnschema_lamin1-0.15.1/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.16.0/lnschema_lamin1/_link.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,7 +36,16 @@
 class FileBiosample(SQLModel, table=True):  # type: ignore
     """Links for `File` and `Biosample`."""
 
     __tablename__ = f"{prefix}file_biosample"
 
     file_id: str = Field(foreign_key="core.file.id", primary_key=True)
     biosample_id: str = Field(foreign_key="lamin1.biosample.id", primary_key=True)
+
+
+class FileCellType(SQLModel, table=True):  # type: ignore
+    """Links for `File` and `CellType`."""
+
+    __tablename__ = f"{prefix}file_cell_type"
+
+    file_id: str = Field(foreign_key="core.file.id", primary_key=True)
+    cell_type_id: str = Field(foreign_key="bionty.cell_type.id", primary_key=True)
```

### Comparing `lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/noxfile.py` & `lnschema_lamin1-0.16.0/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from pathlib import Path
 
 import nox
 from laminci import move_built_docs_to_docs_slash_project_slug
-from laminci.nox import (  # setup_test_instances_from_main_branch,
+from laminci.nox import (
     build_docs,
     login_testuser1,
     run_pre_commit,
     run_pytest,
+    setup_test_instances_from_main_branch,
 )
 
 nox.options.reuse_existing_virtualenvs = True
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     run_pre_commit(session)
 
 
 @nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
 def build(session):
     login_testuser1(session)
-    # setup_test_instances_from_main_branch(session, schema="bionty,lamin1")
+    setup_test_instances_from_main_branch(session, schema="bionty,lamin1")
     session.install(".[dev,test]")
     Path("./lnschema_lamin1/migrations/versions").mkdir(parents=True, exist_ok=True)
     run_pytest(session)
     build_docs(session)
     move_built_docs_to_docs_slash_project_slug()
```

### Comparing `lnschema_lamin1-0.15.1/pyproject.toml` & `lnschema_lamin1-0.16.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,29 @@
 
 [project]
 name = "lnschema_lamin1"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    "lnschema_core",
-    "lnbase_biolab",
-    "openpyxl",
-    "psycopg2-binary",
-    "gcsfs",
+    "lamindb[bionty,lamin1]",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-lamin1"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "nbproject_test>=0.4.1",
-    "lamindb[bionty]",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lnschema_lamin1-0.15.1/tests/test_migrations.py` & `lnschema_lamin1-0.16.0/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.1/PKG-INFO` & `lnschema_lamin1-0.16.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.15.1
+Version: 0.16.0
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnschema_core
-Requires-Dist: lnbase_biolab
-Requires-Dist: openpyxl
-Requires-Dist: psycopg2-binary
-Requires-Dist: gcsfs
+Requires-Dist: lamindb[bionty,lamin1]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
-Requires-Dist: lamindb[bionty] ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
 Provides-Extra: dev
 Provides-Extra: test
 
 # lnschema-lamin1: Customized schema of Lamin
 
 Latest developer docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app/docs/lnschema-lamin1/).
```


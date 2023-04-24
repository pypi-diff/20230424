# Comparing `tmp/mipdb-2.0.4.tar.gz` & `tmp/mipdb-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipdb-2.0.4.tar", max compression
+gzip compressed data, was "mipdb-2.1.0.tar", max compression
```

## Comparing `mipdb-2.0.4.tar` & `mipdb-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      965 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/__init__.py
--rw-r--r--   0        0        0    13744 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/commands.py
--rw-r--r--   0        0        0      696 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/data_frame.py
--rw-r--r--   0        0        0     2345 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/data_frame_schema.py
--rw-r--r--   0        0        0    18348 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/database.py
--rw-r--r--   0        0        0     2947 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/dataelements.py
--rw-r--r--   0        0        0     2623 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/exceptions.py
--rw-r--r--   0        0        0     1697 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/properties.py
--rw-r--r--   0        0        0     1061 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/reader.py
--rw-r--r--   0        0        0      746 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/schema.py
--rw-r--r--   0        0        0    16150 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/tables.py
--rw-r--r--   0        0        0    39144 2023-03-26 23:47:54.446868 mipdb-2.0.4/mipdb/usecases.py
--rw-r--r--   0        0        0     1133 2023-03-26 23:47:54.446868 mipdb-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 mipdb-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      965 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/__init__.py
+-rw-r--r--   0        0        0    13744 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/commands.py
+-rw-r--r--   0        0        0      696 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/data_frame.py
+-rw-r--r--   0        0        0     2345 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/data_frame_schema.py
+-rw-r--r--   0        0        0    18348 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/database.py
+-rw-r--r--   0        0        0     4140 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/dataelements.py
+-rw-r--r--   0        0        0     2623 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/exceptions.py
+-rw-r--r--   0        0        0     1697 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/properties.py
+-rw-r--r--   0        0        0     1061 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/reader.py
+-rw-r--r--   0        0        0      746 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/schema.py
+-rw-r--r--   0        0        0    16219 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/tables.py
+-rw-r--r--   0        0        0    41554 2023-04-24 10:54:41.260132 mipdb-2.1.0/mipdb/usecases.py
+-rw-r--r--   0        0        0     1133 2023-04-24 10:54:41.260132 mipdb-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 mipdb-2.1.0/PKG-INFO
```

### Comparing `mipdb-2.0.4/mipdb/__init__.py` & `mipdb-2.1.0/mipdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/commands.py` & `mipdb-2.1.0/mipdb/commands.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/data_frame.py` & `mipdb-2.1.0/mipdb/data_frame.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/data_frame_schema.py` & `mipdb-2.1.0/mipdb/data_frame_schema.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/database.py` & `mipdb-2.1.0/mipdb/database.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/dataelements.py` & `mipdb-2.1.0/mipdb/dataelements.py`

 * *Files 27% similar despite different names*

```diff
@@ -55,14 +55,51 @@
         )
     if dataset_metadata["sql_type"] != "text":
         raise InvalidDataModelError(
             "CDE 'dataset' must have the 'sql_type' property equal to 'text'."
         )
 
 
+def validate_longitudinal_data_model(cdes):
+    subject_id_metadata = None
+    visit_id_metadata = None
+
+    for cde in cdes:
+        if cde.code == "subjectid":
+            subject_id_metadata = json.loads(cde.metadata)
+        elif cde.code == "visitid":
+            visit_id_metadata = json.loads(cde.metadata)
+
+    if not subject_id_metadata:
+        raise InvalidDataModelError(
+            "There is no 'subjectid' CDE in the longitudinal data model."
+        )
+    if not visit_id_metadata:
+        raise InvalidDataModelError(
+            "There is no 'visitid' CDE in the longitudinal data model."
+        )
+
+    validate_visitid_cde(visit_id_metadata)
+
+
+def validate_visitid_cde(metadata):
+    if not metadata["is_categorical"]:
+        raise InvalidDataModelError(
+            "CDE 'visitid' must have the 'isCategorical' property equal to 'true'."
+        )
+    if metadata["sql_type"] != "text":
+        raise InvalidDataModelError(
+            "CDE 'visitid' must have the 'sql_type' property equal to 'text'."
+        )
+    if "enumerations" not in metadata:
+        raise InvalidDataModelError(
+            "CDE 'visitid' must contain the 'enumerations' property."
+        )
+
+
 def reformat_metadata(metadata):
     new_key_assign = {
         "isCategorical": "is_categorical",
         "minValue": "min",
         "maxValue": "max",
     }
     for old_key, new_key in new_key_assign.items():
```

### Comparing `mipdb-2.0.4/mipdb/exceptions.py` & `mipdb-2.1.0/mipdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/properties.py` & `mipdb-2.1.0/mipdb/properties.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/reader.py` & `mipdb-2.1.0/mipdb/reader.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/schema.py` & `mipdb-2.1.0/mipdb/schema.py`

 * *Files identical despite different names*

### Comparing `mipdb-2.0.4/mipdb/tables.py` & `mipdb-2.1.0/mipdb/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from mipdb.database import DataBase, Connection
 from mipdb.database import METADATA_SCHEMA
 from mipdb.database import METADATA_TABLE
 from mipdb.dataelements import CommonDataElement
 from mipdb.exceptions import UserInputError
 from mipdb.schema import Schema
+
 RECORDS_PER_COPY = 100000
 
 
 class User(Enum):
     executor = "executor"
     admin = "admin"
     guest = "guest"
@@ -391,15 +392,17 @@
         )
 
     def validate_csv(self, csv_path, cdes_with_min_max, cdes_with_enumerations, db):
         validated_datasets = []
         offset = 2
 
         while True:
-            self.load_csv(csv_path=csv_path, offset=offset, records=RECORDS_PER_COPY, db=db)
+            self.load_csv(
+                csv_path=csv_path, offset=offset, records=RECORDS_PER_COPY, db=db
+            )
             offset += RECORDS_PER_COPY
 
             table_count = self.get_row_count(db=db)
             if not table_count:
                 break
 
             validated_datasets = set(validated_datasets) | set(
@@ -412,15 +415,14 @@
             # If the temp contains fewer rows than RECORDS_PER_COPY
             # that means we have read all the records in the csv and we need to stop the iteration.
             if table_count < RECORDS_PER_COPY:
                 break
 
         return validated_datasets
 
-
     def _validate_min_max_restriction(self, cdes_with_min_max, db):
         for cde, min_max in cdes_with_min_max.items():
             min_value, max_value = min_max
             cde_invalid_values = db.execute(
                 f"SELECT \"{cde}\" FROM {self.table.fullname} WHERE \"{cde}\" NOT BETWEEN '{min_value}' AND '{max_value}' "
             ).fetchone()
             if cde_invalid_values:
@@ -443,15 +445,17 @@
             table_name=self.table.name,
         )
 
     def _validate_csv_contains_eof(self, csv_path):
         with open(csv_path, "rb") as f:
             last_line = f.readlines()[-1]
         if not last_line.endswith(b"\n"):
-            raise UserInputError(f"CSV:'{csv_path}' does not end with a blank line.")
+            raise UserInputError(
+                f"CSV:'{csv_path}' does not end with a valid EOF delimiter."
+            )
 
     def _validate_enumerations_restriction(self, cdes_with_enumerations, db):
         for cde, enumerations in cdes_with_enumerations.items():
             cde_invalid_values = db.execute(
                 f'SELECT "{cde}" from {self.table.fullname} where "{cde}" not in ({str(enumerations)[1:-1]})'
             ).fetchone()
             if cde_invalid_values:
```

### Comparing `mipdb-2.0.4/mipdb/usecases.py` & `mipdb-2.1.0/mipdb/usecases.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,29 @@
 from mipdb.exceptions import UserInputError
 from mipdb.properties import Properties
 from mipdb.reader import CSVDataFrameReader
 from mipdb.schema import Schema
 from mipdb.dataelements import (
     make_cdes,
     validate_dataset_present_on_cdes_with_proper_format,
+    validate_longitudinal_data_model,
 )
 from mipdb.tables import (
     DataModelTable,
     DatasetsTable,
     ActionsTable,
     MetadataTable,
     PrimaryDataTable,
-    TemporaryTable, RECORDS_PER_COPY,
+    TemporaryTable,
+    RECORDS_PER_COPY,
 )
 from mipdb.data_frame import DataFrame
 
 DATASET_COLUMN_NAME = "dataset"
+LONGITUDINAL = "longitudinal"
 
 
 class UseCase(ABC):
     """Abstract use case class."""
 
     @abstractmethod
     def execute(self, *args, **kwargs) -> None:
@@ -121,14 +124,22 @@
             AddPropertyToDataModel(self.db).execute(
                 code=code,
                 version=version,
                 key="cdes",
                 value=data_model_metadata,
                 force=True,
             )
+            if (
+                LONGITUDINAL in data_model_metadata
+                and data_model_metadata[LONGITUDINAL]
+            ):
+                validate_longitudinal_data_model(cdes)
+                TagDataModel(self.db).execute(
+                    code=code, version=version, tag=LONGITUDINAL
+                )
 
     def _create_schema(self, name, conn):
         schema = Schema(name)
         schema.create(conn)
         return schema
 
     def _create_primary_data_table(self, schema, cdes, conn):
@@ -226,15 +237,17 @@
                     conn=conn,
                 )
             else:
                 imported_datasets = self._import_csv(
                     csv_path=csv_path, data_model=data_model, conn=conn
                 )
 
-            existing_datasets = datasets_table.get_values(columns=["code"], data_model_id=data_model_id, db=conn)
+            existing_datasets = datasets_table.get_values(
+                columns=["code"], data_model_id=data_model_id, db=conn
+            )
             for dataset in set(imported_datasets) - set(existing_datasets):
                 dataset_id = self._get_next_dataset_id(conn)
                 values = dict(
                     data_model_id=data_model_id,
                     dataset_id=dataset_id,
                     code=dataset,
                     label=dataset_enumerations[dataset],
@@ -304,15 +317,17 @@
         primary_data_table = PrimaryDataTable.from_db(data_model, db)
         offset = 2
         imported_datasets = []
         # If we load a csv to 'temp' and then insert them to the 'primary_data' in the case of a big file (3gb),
         # for a sort period of time will have a spike of memory usage because the data will be stored in both tables.
         # The workaround for that is to load the csv in batches.
         while True:
-            temporary_table.load_csv(csv_path=csv_path, offset=offset, records=RECORDS_PER_COPY, db=db)
+            temporary_table.load_csv(
+                csv_path=csv_path, offset=offset, records=RECORDS_PER_COPY, db=db
+            )
             offset += RECORDS_PER_COPY
 
             table_count = temporary_table.get_row_count(db=db)
             if not table_count:
                 break
 
             imported_datasets = set(imported_datasets) | set(
@@ -336,15 +351,46 @@
                 dataframe = DataFrame(dataset_data)
                 imported_datasets = set(imported_datasets) | set(dataframe.datasets)
                 values = dataframe.to_dict()
                 primary_data_table.insert_values(values, conn)
         return imported_datasets
 
 
+def are_data_valid_longitudinal(csv_path):
+    df = pd.read_csv(csv_path, usecols=["subjectid", "visitid"])
+    check_unique_longitudinal_dataset_primary_keys(df)
+    check_subjectid_is_full(df)
+    check_visitid_is_full(df)
+
+
+def check_unique_longitudinal_dataset_primary_keys(df):
+    duplicates = df[df.duplicated(subset=["visitid", "subjectid"], keep=False)]
+    if not duplicates.empty:
+        raise InvalidDatasetError(
+            f"Invalid csv: the following visitid and subjectid pairs are duplicated:\n{duplicates}"
+        )
+
+
+def check_subjectid_is_full(df):
+    if df["subjectid"].isnull().any():
+        raise InvalidDatasetError("Column 'subjectid' should never contain null values")
+
+
+def check_visitid_is_full(df):
+    if df["visitid"].isnull().any():
+        raise InvalidDatasetError("Column 'visitid' should never contain null values")
+
+
 class ValidateDataset(UseCase):
+    """
+    We separate the data validation from the importation to make sure that a csv is valid as a whole before committing it to the main table.
+    In the data validation we use chunking in order to reduce the memory footprint of the process.
+    Database constraints must NOT be used as part of the validation process since that could result in partially imported csvs.
+    """
+
     def __init__(self, db: DataBase) -> None:
         self.db = db
         is_db_initialized(db)
 
     def execute(
         self, csv_path, copy_from_file, data_model_code, data_model_version
     ) -> None:
@@ -362,14 +408,20 @@
             metadata_table = MetadataTable.from_db(data_model, conn)
             sql_type_per_column = metadata_table.get_sql_type_per_column()
             cdes_with_min_max = metadata_table.get_cdes_with_min_max(csv_columns)
             cdes_with_enumerations = metadata_table.get_cdes_with_enumerations(
                 csv_columns
             )
             dataset_enumerations = metadata_table.get_dataset_enums()
+            if self.is_data_model_longitudinal(
+                data_model_code, data_model_version, conn
+            ):
+                print("is_data_model_longitudinal")
+                are_data_valid_longitudinal(csv_path)
+
             if copy_from_file:
                 validated_datasets = self.validate_csv_with_volume(
                     csv_path,
                     sql_type_per_column,
                     cdes_with_min_max,
                     cdes_with_enumerations,
                     conn,
@@ -382,14 +434,23 @@
                     cdes_with_enumerations,
                 )
             self.verify_datasets_exist_in_enumerations(
                 datasets=validated_datasets,
                 dataset_enumerations=dataset_enumerations,
             )
 
+    def is_data_model_longitudinal(self, data_model_code, data_model_version, conn):
+        metadata = Schema(METADATA_SCHEMA)
+        data_model_table = DataModelTable(schema=metadata)
+        data_model_id = data_model_table.get_data_model_id(
+            data_model_code, data_model_version, conn
+        )
+        properties = data_model_table.get_data_model_properties(data_model_id, conn)
+        return "longitudinal" in json.loads(properties)["tags"]
+
     def validate_csv(
         self, csv_path, sql_type_per_column, cdes_with_min_max, cdes_with_enumerations
     ):
         imported_datasets = []
 
         csv_columns = pd.read_csv(csv_path, nrows=0).columns.tolist()
         dataframe_schema = DataFrameSchema(
@@ -413,15 +474,17 @@
         csv_columns = pd.read_csv(csv_path, nrows=0).columns.tolist()
         dataframe_sql_type_per_column = self._get_dataframe_sql_type_per_column(
             csv_columns, sql_type_per_column
         )
         temporary_table = self._create_temporary_table(
             dataframe_sql_type_per_column, conn
         )
-        validated_datasets = temporary_table.validate_csv(csv_path, cdes_with_min_max, cdes_with_enumerations, conn)
+        validated_datasets = temporary_table.validate_csv(
+            csv_path, cdes_with_min_max, cdes_with_enumerations, conn
+        )
         temporary_table.drop(conn)
         return validated_datasets
 
     def _get_dataframe_sql_type_per_column(self, csv_columns, sql_type_per_column):
         if set(csv_columns) <= set(sql_type_per_column.keys()):
             return {
                 dataframe_column: sql_type_per_column[dataframe_column]
```

### Comparing `mipdb-2.0.4/pyproject.toml` & `mipdb-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mipdb"
-version = "2.0.4"
+version = "2.1.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.8"
 SQLAlchemy = "~1.3"
 sqlalchemy_monetdb = "~1.0"
```


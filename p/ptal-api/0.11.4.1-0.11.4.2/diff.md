# Comparing `tmp/ptal_api-0.11.4.1.tar.gz` & `tmp/ptal_api-0.11.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.4.1.tar", max compression
+gzip compressed data, was "ptal_api-0.11.4.2.tar", max compression
```

## Comparing `ptal_api-0.11.4.1.tar` & `ptal_api-0.11.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 11:37:57.842945 ptal_api-0.11.4.1/ptal_api/__init__.py
--rw-r--r--   0        0        0    98067 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/adapter.py
--rw-r--r--   0        0        0      127 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      752 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12105 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      905 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3240 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2107 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1399 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4565 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    22266 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1830 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3364 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4803 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1211 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   288848 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    92810 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   136157 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3641 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1047 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 ptal_api-0.11.4.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:02:15.010257 ptal_api-0.11.4.2/ptal_api/__init__.py
+-rw-r--r--   0        0        0    98013 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/adapter.py
+-rw-r--r--   0        0        0      127 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      752 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    12105 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      905 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3240 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2107 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1399 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4565 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    22266 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1828 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-04-24 15:02:14.958256 ptal_api-0.11.4.2/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3364 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4803 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1211 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   288848 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    92810 2023-04-24 15:02:14.962257 ptal_api-0.11.4.2/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   136157 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3641 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:02:15.014257 ptal_api-0.11.4.2/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1047 2023-04-24 15:02:14.966256 ptal_api-0.11.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 ptal_api-0.11.4.2/PKG-INFO
```

### Comparing `ptal_api-0.11.4.1/README.md` & `ptal_api-0.11.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/adapter.py` & `ptal_api-0.11.4.2/ptal_api/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,15 +572,15 @@
 
         return res.concept_link
 
     def get_all_concepts(
         self, filter_settings: ConceptFilterSettings = None,
         direction: SortDirection = 'descending', sort_field: ConceptSorting = 'score',
         with_aliases: bool = False, with_properties: bool = False, with_links: bool = False,
-        with_link_properties: bool = False, with_facts: bool = False
+        with_link_properties: bool = False, with_facts: bool = False, with_potential_facts: bool = False
     ) -> Iterable[Concept]:
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
         total = self.get_concept_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
             had_creation_date = hasattr(filter_settings, 'creation_date')
@@ -589,19 +589,20 @@
                 old_timestamp_interval = copy(filter_settings.creation_date)
             start: int = getattr(old_timestamp_interval, 'start', self.kb_iterator_config.earliest_created_time)
             end: int = getattr(old_timestamp_interval, 'end', int(time()))
             middle: int = (end + start) // 2
 
             for start, end in (start, middle), (middle, end):
                 filter_settings.creation_date = TimestampInterval(start=start, end=end)
-                for c in self.get_all_concepts(filter_settings=filter_settings,
-                                               direction=direction, sort_field=sort_field, with_aliases=with_aliases,
-                                               with_properties=with_properties, with_links=with_links,
-                                               with_link_properties=with_link_properties, with_facts=with_facts):
-                    yield c
+                yield from self.get_all_concepts(
+                    filter_settings=filter_settings, direction=direction, sort_field=sort_field,
+                    with_aliases=with_aliases, with_properties=with_properties, with_links=with_links,
+                    with_link_properties=with_link_properties, with_facts=with_facts,
+                    with_potential_facts=with_potential_facts
+                )
 
             if had_creation_date:
                 filter_settings.creation_date = old_timestamp_interval
             else:
                 delattr(filter_settings, 'creation_date')
             return
         elif not total:
@@ -610,15 +611,16 @@
         concepts: Iterable = [None]
         i: int = 0
         while concepts:
             concepts = self.get_concepts(
                 skip=i * self._limit, take=self._limit, filter_settings=filter_settings,
                 direction=direction, sort_field=sort_field, with_aliases=with_aliases,
                 with_properties=with_properties, with_links=with_links,
-                with_link_properties=with_link_properties, with_facts=with_facts
+                with_link_properties=with_link_properties, with_facts=with_facts,
+                with_potential_facts=with_potential_facts
             )
             for c in concepts:
                 yield c
             i += 1
 
     def get_concepts(
         self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptFilterSettings = None,
@@ -2025,90 +2027,90 @@
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.composite_concept.paginate_single_widget
 
     def add_concept_fact(self, concept_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.add_concept_fact(
+        op.add_concept_fact(
             id=concept_id,
             fact=FactInput(
                 document_id=document_id
             )
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_fact
 
     def delete_concept_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.delete_concept_fact(
+        op.delete_concept_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_fact
 
     def add_concept_property_fact(self, property_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.add_concept_property_fact(
+        op.add_concept_property_fact(
             id=property_id,
             fact=FactInput(
                 document_id=document_id
             )
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_property_fact
 
     def delete_concept_property_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.delete_concept_property_fact(
+        op.delete_concept_property_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_property_fact
 
     def add_concept_link_fact(self, link_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.add_concept_link_fact(
+        op.add_concept_link_fact(
             id=link_id,
             fact=FactInput(
                 document_id=document_id
             )
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_link_fact
 
     def delete_concept_link_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.delete_concept_link_fact(
+        op.delete_concept_link_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_link_fact
 
     def add_concept_link_property_fact(self, link_property_id: str, document_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.add_concept_link_property_fact(
+        op.add_concept_link_property_fact(
             id=link_property_id,
             fact=FactInput(
                 document_id=document_id
             )
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.add_concept_link_property_fact
 
     def delete_concept_link_property_fact(self, fact_id: str) -> State:
         op = Operation(Mutation)
-        state: State = op.delete_concept_link_property_fact(
+        op.delete_concept_link_property_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_link_property_fact
 
     # region Crawlers methods
@@ -2169,15 +2171,15 @@
 
         return res.get_or_add_concept
 
     @check_utils_gql_client
     def get_tdm(self, doc_id: str):
         op = Operation(uas.Query)
         op.tdm(
-            id = doc_id
+            id=doc_id
         )
         res = self._utils_gql_client.execute(op)
         res = op + res
         return res
 
     # endregion
```

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.4.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         except Exception as ex:
             self._logger.info(f"Failed to load type mapping from file \"{file_path}\"")
             raise ex
 
     def _load_type_mapping_from_dict(self, input_dict: dict) -> Optional[TypeMapping]:
         try:
             type_mapping = marshmallow_dataclass.class_schema(TypeMapping)().load(input_dict)
-            self._logger.info(f"Loaded type mapping from input dictionary")
+            self._logger.info("Loaded type mapping from input dictionary")
             return type_mapping
         except Exception as ex:
-            self._logger.info(f"Failed to load type mapping from input dictionary")
+            self._logger.info("Failed to load type mapping from input dictionary")
             raise ex
 
     def load_type_mapping(self, input_data: Optional[Union[str, dict, TypeMapping]]) -> TypeMapping:
         if isinstance(input_data, TypeMapping):
             return input_data
         elif isinstance(input_data, str):
             return self._load_type_mapping_from_file(input_data)
```

### Comparing `ptal_api-0.11.4.1/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.4.2/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.4.2/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/schema/README.md` & `ptal_api-0.11.4.2/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/schema/api_schema.py` & `ptal_api-0.11.4.2/ptal_api/schema/api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.4.2/ptal_api/schema/crawlers_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.4.2/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.4.2/ptal_api/schema/utils_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.4.2/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.4.2/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4.1/pyproject.toml` & `ptal_api-0.11.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.4.1"
+version = "0.11.4.2"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.4.1/PKG-INFO` & `ptal_api-0.11.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.4.1
+Version: 0.11.4.2
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


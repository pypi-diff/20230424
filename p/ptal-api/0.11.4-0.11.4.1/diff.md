# Comparing `tmp/ptal_api-0.11.4.tar.gz` & `tmp/ptal_api-0.11.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.4.tar", max compression
+gzip compressed data, was "ptal_api-0.11.4.1.tar", max compression
```

## Comparing `ptal_api-0.11.4.tar` & `ptal_api-0.11.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-17 12:02:16.437018 ptal_api-0.11.4/README.md
--rw-r--r--   0        0        0        0 2023-04-17 12:02:16.497018 ptal_api-0.11.4/ptal_api/__init__.py
--rw-r--r--   0        0        0    96789 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/adapter.py
--rw-r--r--   0        0        0      127 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      752 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12105 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      905 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3240 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2107 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1399 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4565 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    22266 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1830 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3364 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4803 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1211 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   288635 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    92810 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   135944 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3641 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1045 2023-04-17 12:02:16.449018 ptal_api-0.11.4/pyproject.toml
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.4/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 11:37:57.842945 ptal_api-0.11.4.1/ptal_api/__init__.py
+-rw-r--r--   0        0        0    98067 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/adapter.py
+-rw-r--r--   0        0        0      127 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      752 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    12105 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      905 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3240 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2107 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1399 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4565 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    22266 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1830 2023-04-24 11:37:57.778944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3364 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4803 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1211 2023-04-24 11:37:57.782944 ptal_api-0.11.4.1/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   288848 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    92810 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   136157 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3641 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:37:57.846945 ptal_api-0.11.4.1/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1047 2023-04-24 11:37:57.786944 ptal_api-0.11.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 ptal_api-0.11.4.1/PKG-INFO
```

### Comparing `ptal_api-0.11.4/README.md` & `ptal_api-0.11.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/adapter.py` & `ptal_api-0.11.4.1/ptal_api/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from .core.type_mapper.data_model.base_data_model import TypeMapping
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader import TypeMappingLoader
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader_interface import TypeMappingLoaderInterface
 from .core.kb_sync.kb_iterator_config import KBIteratorConfig
 from .core.kb_sync.object_time_interval import ObjectTimeInterval
 from .tdm_builder.tdm_builder import AbstractTdmBuilder
 from .providers.gql_providers import AbstractGQLClient
-from .schema.api_schema import Query, Mutation, StoryPagination, ConceptLinkPagination, ConceptFactPagination, \
-    ConceptPropertyPagination, SortDirection, ConceptSorting, DocumentSorting, DocumentGrouping, TimestampInterval, \
-    PerformSynchronously, ConceptPropertyTypeSorting, ConceptTypeSorting, ConceptLinkTypeSorting, \
-    ConceptPropertyValueTypeSorting, CompositePropertyTypeSorting
+from .schema.api_schema import ConceptCandidateFact, Query, Mutation, StoryPagination, ConceptLinkPagination, \
+    ConceptFactPagination, ConceptPropertyPagination, SortDirection, ConceptSorting, DocumentSorting, \
+    DocumentGrouping, TimestampInterval, PerformSynchronously, ConceptPropertyTypeSorting, ConceptTypeSorting, \
+    ConceptLinkTypeSorting, ConceptPropertyValueTypeSorting, CompositePropertyTypeSorting
 from .schema.api_schema import \
     ValueInput, IntValueInput, StringValueInput, DateTimeValue, StringLocaleValue, StringValue, LinkValue, \
     DoubleValue, IntValue, ConceptPropertyFilterSettings, ConceptLinkFilterSettings, ExtraSettings, Story, Document,\
     DocumentFilterSettings, Concept, ConceptLink, ConceptPagination, ConceptFilterSettings, PropertyFilterSettings, \
     StringFilter, ConceptType, ConceptTypeFilterSettings, ConceptTypePagination, ConceptPropertyType, \
     ConceptPropertyTypePagination, ConceptPropertyTypeFilterSettings, ConceptLinkType, ConceptLinkTypePagination, \
     ConceptLinkTypeFilterSettings, ConceptPropertyValueType, ConceptPropertyValueTypePagination, \
@@ -208,15 +208,15 @@
         graphql_value.__fragment__(iv_frag)
         graphql_value.__fragment__(dtv_frag)
         graphql_value.__fragment__(cv_frag)
         # graphql_value.__fragment__(dtiv_frag)
 
     def _configure_output_concept_fields(
         self, concept_object, with_aliases=False, with_properties=False, with_links=False,
-        with_link_properties=False, with_facts=False
+        with_link_properties=False, with_facts=False, with_potential_facts=False
     ):
         concept_object.__fields__(*self.concept_fields)
         concept_object.concept_type.__fields__(*self.concept_type_fields)
         if with_aliases:
             sv_frag = Fragment(StringValue, 'StringFull')
             sv_frag.value()
             concept_object.list_alias.value.__fragment__(sv_frag)
@@ -246,14 +246,22 @@
             lcf = pcf.list_concept_fact()
             lcf.__fields__(*self.concept_fact_fields)
             d = lcf.document()
             d.__fields__(*self.document_fields_extended)
             dm = d.metadata()
             dm.platform().__fields__(*self.document_platform_fields)
             dm.account().__fields__(*self.document_account_fields)
+        if with_potential_facts:
+            lccf: List[ConceptCandidateFact] = concept_object.list_concept_candidate_fact()
+            lccf.__fields__(*self.concept_fact_fields)
+            d = lccf.document()
+            d.__fields__(*self.document_fields_extended)
+            dm = d.metadata()
+            dm.platform().__fields__(*self.document_platform_fields)
+            dm.account().__fields__(*self.document_account_fields)
 
     def _configure_output_link_fields(
         self, link_object, with_link_properties=False
     ):
         link_object.__fields__(*self.concept_link_fields)
         link_object.concept_from().__fields__(*self.concept_link_concept_from_fields)
         link_object.concept_to().__fields__(*self.concept_link_concept_to_fields)
@@ -497,23 +505,25 @@
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.total
 
     def get_concept(
         self, concept_id: str, with_aliases: bool = False,
         with_properties: bool = True, with_links: bool = True,
-        with_link_properties: bool = True, with_facts: bool = False
+        with_link_properties: bool = True, with_facts: bool = False,
+        with_potential_facts: bool = False
     ) -> Concept:
         op = Operation(Query)
         c: Concept = op.concept(
             id=concept_id
         )
         self._configure_output_concept_fields(
             c, with_aliases=with_aliases, with_properties=with_properties,
-            with_links=with_links, with_link_properties=with_link_properties, with_facts=with_facts
+            with_links=with_links, with_link_properties=with_link_properties,
+            with_facts=with_facts, with_potential_facts=with_potential_facts
         )
         res = self._gql_client.execute(op)
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.concept)
 
@@ -610,15 +620,15 @@
                 yield c
             i += 1
 
     def get_concepts(
         self, skip: int = 0, take: Optional[int] = None, filter_settings: ConceptFilterSettings = None,
         direction: SortDirection = 'descending', sort_field: ConceptSorting = 'score',
         with_aliases: bool = False, with_properties: bool = False, with_links: bool = False,
-        with_link_properties: bool = False, with_facts: bool = False
+        with_link_properties: bool = False, with_facts: bool = False, with_potential_facts=False
     ) -> Sequence[Concept]:
         take = self.get_take_value(take)
         pagination_concept_kwargs = dict()
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
 
         op = Operation(Query)
@@ -628,32 +638,36 @@
             filter_settings=filter_settings,
             direction=direction,
             sort_field=sort_field,
             **pagination_concept_kwargs
         )
         self._configure_output_concept_fields(
             cp.list_concept(), with_aliases=with_aliases, with_properties=with_properties,
-            with_links=with_links, with_link_properties=with_link_properties, with_facts=with_facts
+            with_links=with_links, with_link_properties=with_link_properties,
+            with_facts=with_facts, with_potential_facts=with_potential_facts
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_limit_offset_filter_settings(
         self, skip: int = 0, take: Optional[int] = None, filter_settings: Optional[ConceptFilterSettings] = None,
-        with_aliases: bool = False, with_facts: bool = False
+        with_aliases: bool = False, with_facts: bool = False, with_potential_facts=False
     ) -> Sequence[Concept]:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=filter_settings if filter_settings else ConceptFilterSettings(),
             offset=skip,
             limit=take
         )
-        self._configure_output_concept_fields(cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts)
+        self._configure_output_concept_fields(
+            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
+            with_potential_facts=with_potential_facts
+        )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_all_concept_links(
         self, filter_settings: ConceptLinkFilterSettings = None, with_link_properties: bool = False
     ) -> Iterable[ConceptLink]:
@@ -711,15 +725,16 @@
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.list_concept_link
 
     def get_concepts_by_type_id_with_offset(
         self, type_id: str, skip: int, take: Optional[int] = None, direction='descending',
         sort_field='systemRegistrationDate', with_aliases: bool = False, with_properties: bool = False,
-        with_links: bool = False, with_link_properties: bool = False, with_facts: bool = False
+        with_links: bool = False, with_link_properties: bool = False, with_facts: bool = False,
+        with_potential_facts=False
     ) -> ConceptPagination:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
                 concept_type_ids=[type_id]
             ),
@@ -727,45 +742,48 @@
             offset=skip,
             direction=direction,
             sort_field=sort_field
         )
         cp.total()
         self._configure_output_concept_fields(
             cp.list_concept(), with_aliases=with_aliases, with_properties=with_properties, with_links=with_links,
-            with_link_properties=with_link_properties, with_facts=with_facts
+            with_link_properties=with_link_properties, with_facts=with_facts, with_potential_facts=with_potential_facts
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
     def get_concepts_by_type_id_with_offset_with_markers(
         self, type_id: str, skip: int = 0, take: Optional[int] = None, markers: Optional[List[str]] = None,
         direction='descending', sort_field='systemRegistrationDate', with_aliases: bool = False,
-        with_facts: bool = False
+        with_facts: bool = False, with_potential_facts=False
     ) -> ConceptPagination:
         take = self.get_take_value(take)
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
                 concept_type_ids=[type_id],
                 markers=markers,
             ),
             limit=take,
             offset=skip,
             direction=direction,
             sort_field=sort_field
         )
         cp.total()
-        self._configure_output_concept_fields(cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts)
+        self._configure_output_concept_fields(
+            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
+            with_potential_facts=with_potential_facts)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
     def get_concepts_by_name(
-        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False, with_facts: bool = False
+        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False,
+        with_facts: bool = False, with_potential_facts=False
     ) -> Sequence[Concept]:
 
         op = Operation(Query)
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 exact_name=name,
                 concept_type_ids=[type_id]
@@ -773,21 +791,25 @@
         else:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 exact_name=name
             )
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=concept_filter_settings
         )
-        self._configure_output_concept_fields(cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts)
+        self._configure_output_concept_fields(
+            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
+            with_potential_facts=with_potential_facts
+        )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_near_name(
-        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False, with_facts: bool = False
+        self, name: str, type_id: Optional[str] = None, with_aliases: bool = False,
+        with_facts: bool = False, with_potential_facts=False
     ) -> Sequence[Concept]:
 
         op = Operation(Query)
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 name=name,
                 concept_type_ids=[type_id]
@@ -795,37 +817,43 @@
         else:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 name=name
             )
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=concept_filter_settings
         )
-        self._configure_output_concept_fields(cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts)
+        self._configure_output_concept_fields(
+            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
+            with_potential_facts=with_potential_facts
+        )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concepts_by_property_name(
         self, property_type_id: str, string_filter: str, property_type: str = 'concept', with_aliases: bool = False,
-        with_facts: bool = False
+        with_facts: bool = False, with_potential_facts=False
     ) -> Sequence[Concept]:
 
         op = Operation(Query)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
                 property_filter_settings=[PropertyFilterSettings(
                     property_type=property_type,
                     property_type_id=property_type_id,
                     string_filter=StringFilter(
                         str=string_filter
                     )
                 )]
             )
         )
-        self._configure_output_concept_fields(cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts)
+        self._configure_output_concept_fields(
+            cp.list_concept(), with_aliases=with_aliases, with_facts=with_facts,
+            with_potential_facts=with_potential_facts
+        )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_concept_properties(self, concept_id: str, with_facts: bool = False) -> Sequence[ConceptProperty]:
         op = Operation(Query)
         concept: Concept = op.concept(
```

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.4.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.4.1/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.4.1/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/schema/README.md` & `ptal_api-0.11.4.1/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/schema/api_schema.py` & `ptal_api-0.11.4.1/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -3894,15 +3894,15 @@
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     component_value_types = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(CompositePropertyValueType))), graphql_name='componentValueTypes')
 
 
 class Concept(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'is_actual', 'name', 'notes', 'markers', 'start_date', 'end_date', 'concept_type', 'pagination_concept_property', 'pagination_concept_link', 'pagination_concept_fact', 'pagination_concept_property_documents', 'pagination_concept_link_documents', 'list_concept_fact', 'image', 'metric', 'list_alias', 'pagination_alias', 'pagination_merged_concept', 'list_header_concept_property', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'list_subscription', 'pagination_research_map')
+    __field_names__ = ('id', 'is_actual', 'name', 'notes', 'markers', 'start_date', 'end_date', 'concept_type', 'pagination_concept_property', 'pagination_concept_link', 'pagination_concept_fact', 'pagination_concept_property_documents', 'pagination_concept_link_documents', 'list_concept_fact', 'list_concept_candidate_fact', 'image', 'metric', 'list_alias', 'pagination_alias', 'pagination_merged_concept', 'list_header_concept_property', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'list_subscription', 'pagination_research_map')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     is_actual = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isActual')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     start_date = sgqlc.types.Field(DateTimeValue, graphql_name='startDate')
     end_date = sgqlc.types.Field(DateTimeValue, graphql_name='endDate')
@@ -3934,14 +3934,15 @@
     pagination_concept_link_documents = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationConceptLinkDocuments', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptLinkFilterSettings), graphql_name='filterSettings', default=None)),
 ))
     )
     list_concept_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptFact'))), graphql_name='listConceptFact')
+    list_concept_candidate_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptCandidateFact'))), graphql_name='listConceptCandidateFact')
     image = sgqlc.types.Field(Image, graphql_name='image')
     metric = sgqlc.types.Field(sgqlc.types.non_null(ConceptStatistics), graphql_name='metric')
     list_alias = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptProperty'))), graphql_name='listAlias')
     pagination_alias = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyPagination), graphql_name='paginationAlias', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
 ))
```

### Comparing `ptal_api-0.11.4/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.4.1/ptal_api/schema/crawlers_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.4.1/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.4.1/ptal_api/schema/utils_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1572,15 +1572,15 @@
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     component_value_types = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(CompositePropertyValueType))), graphql_name='componentValueTypes')
 
 
 class Concept(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'is_actual', 'name', 'notes', 'markers', 'start_date', 'end_date', 'concept_type', 'pagination_concept_property', 'pagination_concept_link', 'pagination_concept_fact', 'pagination_concept_property_documents', 'pagination_concept_link_documents', 'list_concept_fact', 'image', 'metric', 'list_alias', 'pagination_alias', 'pagination_merged_concept', 'list_header_concept_property', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'list_subscription', 'pagination_research_map')
+    __field_names__ = ('id', 'is_actual', 'name', 'notes', 'markers', 'start_date', 'end_date', 'concept_type', 'pagination_concept_property', 'pagination_concept_link', 'pagination_concept_fact', 'pagination_concept_property_documents', 'pagination_concept_link_documents', 'list_concept_fact', 'list_concept_candidate_fact', 'image', 'metric', 'list_alias', 'pagination_alias', 'pagination_merged_concept', 'list_header_concept_property', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'list_subscription', 'pagination_research_map')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     is_actual = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isActual')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     start_date = sgqlc.types.Field(DateTimeValue, graphql_name='startDate')
     end_date = sgqlc.types.Field(DateTimeValue, graphql_name='endDate')
@@ -1612,14 +1612,15 @@
     pagination_concept_link_documents = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationConceptLinkDocuments', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptLinkFilterSettings), graphql_name='filterSettings', default=None)),
 ))
     )
     list_concept_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptFact'))), graphql_name='listConceptFact')
+    list_concept_candidate_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptCandidateFact'))), graphql_name='listConceptCandidateFact')
     image = sgqlc.types.Field(Image, graphql_name='image')
     metric = sgqlc.types.Field(sgqlc.types.non_null(ConceptStatistics), graphql_name='metric')
     list_alias = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ConceptProperty'))), graphql_name='listAlias')
     pagination_alias = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyPagination), graphql_name='paginationAlias', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
 ))
```

### Comparing `ptal_api-0.11.4/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.4.1/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.4.1/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.4/pyproject.toml` & `ptal_api-0.11.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.4"
+version = "0.11.4.1"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.4/PKG-INFO` & `ptal_api-0.11.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.4
+Version: 0.11.4.1
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


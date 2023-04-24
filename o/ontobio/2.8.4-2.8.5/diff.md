# Comparing `tmp/ontobio-2.8.4.tar.gz` & `tmp/ontobio-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ontobio-2.8.4.tar", last modified: Wed Feb 22 00:22:24 2023, max compression
+gzip compressed data, was "dist/ontobio-2.8.5.tar", last modified: Mon Apr 24 19:08:51 2023, max compression
```

## Comparing `ontobio-2.8.4.tar` & `ontobio-2.8.5.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/
--rw-r--r--   0 ebertdu    (502) staff       (20)     1960 2023-02-22 00:22:24.000000 ontobio-2.8.4/PKG-INFO
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/bin/
--rwxr-xr-x   0 ebertdu    (502) staff       (20)     7331 2019-04-03 22:15:31.000000 ontobio-2.8.4/bin/ontobio-lexmap.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)    20798 2021-09-28 22:21:40.000000 ontobio-2.8.4/bin/ontobio-assoc.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1778 2019-11-14 00:02:57.000000 ontobio-2.8.4/bin/rdfgen.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)    31600 2021-06-10 18:33:04.000000 ontobio-2.8.4/bin/validate.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6455 2019-11-14 00:02:57.000000 ontobio-2.8.4/bin/materialize.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)      171 2019-11-14 00:02:57.000000 ontobio-2.8.4/bin/clear-cache.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)     7499 2018-05-21 17:20:38.000000 ontobio-2.8.4/bin/ogr.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)     9695 2022-05-06 22:21:58.000000 ontobio-2.8.4/bin/ontobio-parse-assocs.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/tests/
--rw-r--r--   0 ebertdu    (502) staff       (20)     3363 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_remote_scigraph.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4310 2021-01-14 21:39:16.000000 ontobio-2.8.4/tests/test_rdfgen.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      761 2020-12-16 06:27:04.000000 ontobio-2.8.4/tests/test_gpad_writer.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    31765 2023-02-22 00:16:20.000000 ontobio-2.8.4/tests/test_qc.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      719 2021-03-10 22:27:40.000000 ontobio-2.8.4/tests/test_expand_tsv.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1706 2021-02-05 22:01:47.000000 ontobio-2.8.4/tests/test_ontol.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      510 2019-01-19 00:32:49.000000 ontobio-2.8.4/tests/test_alt_id.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      351 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_write_obo.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2022-02-23 01:04:29.000000 ontobio-2.8.4/tests/test_gpaddiffer.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1159 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_local_ttl.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      983 2023-02-21 22:50:51.000000 ontobio-2.8.4/tests/test_golr_query.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     8525 2022-05-11 03:09:32.000000 ontobio-2.8.4/tests/test_gpad_parser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1756 2019-11-14 00:02:57.000000 ontobio-2.8.4/tests/test_evidence_table.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1043 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_lexmap.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1281 2021-01-14 21:39:16.000000 ontobio-2.8.4/tests/test_sparql_connection.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      775 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_bgiparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5578 2019-11-14 00:02:57.000000 ontobio-2.8.4/tests/test_golr_associations.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     8184 2022-02-23 02:15:06.000000 ontobio-2.8.4/tests/test_local_json.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    12770 2022-05-11 03:09:32.000000 ontobio-2.8.4/tests/test_assoc_writer.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3528 2019-01-19 00:32:49.000000 ontobio-2.8.4/tests/test_assocfactory.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5319 2020-04-07 23:32:20.000000 ontobio-2.8.4/tests/test_gaference.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4535 2020-12-16 06:27:04.000000 ontobio-2.8.4/tests/test_parse_ids.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1912 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_map2slim.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1846 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_semsearch.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      736 2021-12-01 01:44:20.000000 ontobio-2.8.4/tests/test_ecomap.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1536 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_golr_map2slim.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    23194 2022-05-04 01:09:09.000000 ontobio-2.8.4/tests/test_gafparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3636 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_assocmodel.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2199 2021-12-01 01:44:20.000000 ontobio-2.8.4/tests/test_hpoaparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      915 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_config.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    11952 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_lexmap_local.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3463 2020-04-07 23:32:20.000000 ontobio-2.8.4/tests/test_validation_rules.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1478 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_enrich.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      963 2021-06-10 18:33:04.000000 ontobio-2.8.4/tests/test_gpiwriter.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1301 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_wd.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      695 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_mutable.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      664 2019-01-19 00:32:49.000000 ontobio-2.8.4/tests/test_parse_taxon.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      550 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_skos_local.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2234 2018-07-24 17:48:08.000000 ontobio-2.8.4/tests/test_golr_search.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5059 2018-05-21 17:20:38.000000 ontobio-2.8.4/tests/test_remote_sparql.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5151 2021-02-05 22:01:47.000000 ontobio-2.8.4/tests/test_collections.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4929 2021-02-16 19:21:55.000000 ontobio-2.8.4/tests/test_goassociation_model.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1610 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_wd_ontol.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5390 2019-11-14 00:02:57.000000 ontobio-2.8.4/tests/test_phenosim_engine.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5645 2021-09-27 18:33:21.000000 ontobio-2.8.4/tests/test_gocamgen.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      450 2021-02-05 22:01:47.000000 ontobio-2.8.4/tests/test_relations.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1043 2021-02-05 22:01:47.000000 ontobio-2.8.4/tests/test_gpiparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3967 2019-01-31 01:39:32.000000 ontobio-2.8.4/tests/test_owlsim2_int.py
--rw-r--r--   0 ebertdu    (502) staff       (20)       28 2018-05-21 17:20:38.000000 ontobio-2.8.4/MANIFEST.in
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/golr/
--rw-r--r--   0 ebertdu    (502) staff       (20)     2174 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/golr_matrix.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3013 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/beacon_query.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        1 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/golr_entities.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4799 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/golr_stats.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1450 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/golr/golr_sim.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    10470 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/golr/golr_associations.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    68763 2023-02-21 22:52:52.000000 ontobio-2.8.4/ontobio/golr/golr_query.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3867 2022-05-11 03:09:32.000000 ontobio-2.8.4/ontobio/ecomap.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     7379 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/config.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/analysis/
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-19 00:32:49.000000 ontobio-2.8.4/ontobio/analysis/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      457 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/analysis/semsim.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/neo/
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/neo/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     8261 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/neo/scigraph_ontology.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/sparql/
--rw-r--r--   0 ebertdu    (502) staff       (20)    12491 2019-01-19 00:32:49.000000 ontobio-2.8.4/ontobio/sparql/sparql_go.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5814 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/wikidata_ontology.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/sparql/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     8756 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/sparql_ontology.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    11088 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/sparql_ontol_utils.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1531 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/rdflib_bridge.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2261 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sparql/rdf2nx.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4673 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/wikidata.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4073 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sparql/skos.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/util/
--rw-r--r--   0 ebertdu    (502) staff       (20)      903 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/util/user_agent.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/util/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2826 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/util/go_utils.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      516 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/util/curie_map.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    18224 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/util/scigraph_util.py
--rwxr-xr-x   0 ebertdu    (502) staff       (20)      736 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/util/obog2cg.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    17363 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/assocmodel.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      310 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/xref_util.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6821 2020-12-16 06:27:04.000000 ontobio-2.8.4/ontobio/assoc_factory.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/io/
--rw-r--r--   0 ebertdu    (502) staff       (20)    22536 2022-05-11 03:09:32.000000 ontobio-2.8.4/ontobio/io/gpadparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    23795 2022-02-23 02:15:06.000000 ontobio-2.8.4/ontobio/io/gafparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    42009 2023-02-22 00:16:20.000000 ontobio-2.8.4/ontobio/io/qc.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1633 2019-11-14 00:02:57.000000 ontobio-2.8.4/ontobio/io/parsereport.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6903 2022-02-23 01:04:29.000000 ontobio-2.8.4/ontobio/io/hpoaparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1544 2021-06-10 18:33:04.000000 ontobio-2.8.4/ontobio/io/gafgpibridge.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6271 2021-03-10 22:27:40.000000 ontobio-2.8.4/ontobio/io/assocwriter.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    18018 2022-02-23 01:04:29.000000 ontobio-2.8.4/ontobio/io/differ.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    38501 2022-05-04 15:55:33.000000 ontobio-2.8.4/ontobio/io/assocparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      228 2020-12-16 06:27:04.000000 ontobio-2.8.4/ontobio/io/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    13053 2021-06-10 18:33:04.000000 ontobio-2.8.4/ontobio/io/entityparser.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    12899 2021-01-14 21:39:16.000000 ontobio-2.8.4/ontobio/io/ontol_renderers.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6868 2021-03-22 22:20:40.000000 ontobio-2.8.4/ontobio/io/gaference.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2902 2021-06-10 18:33:04.000000 ontobio-2.8.4/ontobio/io/entitywriter.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1084 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/config.yaml
--rw-r--r--   0 ebertdu    (502) staff       (20)     1697 2023-02-22 00:19:10.000000 ontobio-2.8.4/ontobio/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2961 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/slimmer.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1642 2021-03-10 22:27:40.000000 ontobio-2.8.4/ontobio/tsv_expander.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    37123 2022-04-26 22:49:10.000000 ontobio-2.8.4/ontobio/ontol.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6351 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/ontol_factory.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/model/
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/model/mme/
--rw-r--r--   0 ebertdu    (502) staff       (20)     1928 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/model/mme/request.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/model/mme/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      607 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/model/mme/response.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      972 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/model/OBOGraph.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2252 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/model/similarity.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/model/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1227 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/model/nlp.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    27873 2022-07-14 23:42:25.000000 ontobio-2.8.4/ontobio/model/association.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     5399 2022-02-23 01:04:29.000000 ontobio-2.8.4/ontobio/model/collections.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3211 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/model/bbop_graph.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1527 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/model/GolrResults.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3589 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/model/biomodel.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/rdfgen/
--rw-r--r--   0 ebertdu    (502) staff       (20)     8382 2022-03-29 20:57:48.000000 ontobio-2.8.4/ontobio/rdfgen/relations.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/rdfgen/__init__.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/
--rw-r--r--   0 ebertdu    (502) staff       (20)    11120 2021-02-25 21:25:49.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/collapsed_assoc.bk.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     7567 2021-01-27 23:04:39.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     9655 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/collapsed_assoc.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    13135 2021-06-10 20:11:11.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/gocam_builder.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2021-01-27 23:04:39.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     8070 2021-03-10 20:26:34.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/subgraphs.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6653 2021-03-02 01:48:14.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/utils.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    56549 2022-03-29 20:57:48.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/gocamgen.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     4947 2021-01-27 23:04:39.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      489 2021-06-10 18:33:04.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/errors.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3330 2021-01-27 23:04:39.000000 ontobio-2.8.4/ontobio/rdfgen/gocamgen/filter_rule.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    12608 2021-03-10 20:26:34.000000 ontobio-2.8.4/ontobio/rdfgen/assoc_rdfgen.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    35539 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/lexmap.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     3665 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/assoc_schema.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2114 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/cgraph.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/sim/
--rw-r--r--   0 ebertdu    (502) staff       (20)     7583 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/sim/phenosim_engine.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1290 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sim/sim_engine.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-19 00:32:49.000000 ontobio-2.8.4/ontobio/sim/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     6273 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sim/annotation_scorer.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/sim/api/
--rw-r--r--   0 ebertdu    (502) staff       (20)     2397 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sim/api/interfaces.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sim/api/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     7262 2020-04-07 23:32:20.000000 ontobio-2.8.4/ontobio/sim/api/semsearch.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    17404 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/sim/api/owlsim2.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2163 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/sim/api/owlsim3.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     2918 2021-12-01 01:44:20.000000 ontobio-2.8.4/ontobio/sim/mme.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/vocabulary/
--rw-r--r--   0 ebertdu    (502) staff       (20)      955 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/vocabulary/similarity.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      239 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/vocabulary/categories.py
--rw-r--r--   0 ebertdu    (502) staff       (20)      823 2019-01-31 01:39:32.000000 ontobio-2.8.4/ontobio/vocabulary/upper.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1226 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/vocabulary/relations.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.4/ontobio/vocabulary/__init__.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio/validation/
--rw-r--r--   0 ebertdu    (502) staff       (20)     5693 2021-01-14 21:39:16.000000 ontobio-2.8.4/ontobio/validation/metadata.py
--rw-r--r--   0 ebertdu    (502) staff       (20)     1322 2019-11-14 00:02:57.000000 ontobio-2.8.4/ontobio/validation/tools.py
--rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-11-14 00:02:57.000000 ontobio-2.8.4/ontobio/validation/__init__.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    10167 2020-07-21 21:04:11.000000 ontobio-2.8.4/ontobio/validation/rules.py
--rw-r--r--   0 ebertdu    (502) staff       (20)    12801 2021-09-28 22:21:40.000000 ontobio-2.8.4/ontobio/obograph_util.py
-drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/
--rw-r--r--   0 ebertdu    (502) staff       (20)     1960 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/PKG-INFO
--rw-r--r--   0 ebertdu    (502) staff       (20)     4395 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/SOURCES.txt
--rw-r--r--   0 ebertdu    (502) staff       (20)      471 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/requires.txt
--rw-r--r--   0 ebertdu    (502) staff       (20)       14 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/top_level.txt
--rw-r--r--   0 ebertdu    (502) staff       (20)        1 2023-02-22 00:22:24.000000 ontobio-2.8.4/ontobio.egg-info/dependency_links.txt
--rw-r--r--   0 ebertdu    (502) staff       (20)     2370 2021-03-01 23:16:52.000000 ontobio-2.8.4/setup.py
--rw-r--r--   0 ebertdu    (502) staff       (20)       80 2023-02-22 00:22:24.000000 ontobio-2.8.4/setup.cfg
--rw-r--r--   0 ebertdu    (502) staff       (20)      970 2018-05-21 17:20:38.000000 ontobio-2.8.4/README.rst
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1960 2023-04-24 19:08:51.000000 ontobio-2.8.5/PKG-INFO
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/bin/
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)     7331 2019-04-03 22:15:31.000000 ontobio-2.8.5/bin/ontobio-lexmap.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)    20798 2021-09-28 22:21:40.000000 ontobio-2.8.5/bin/ontobio-assoc.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1778 2019-11-14 00:02:57.000000 ontobio-2.8.5/bin/rdfgen.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)    31600 2021-06-10 18:33:04.000000 ontobio-2.8.5/bin/validate.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6455 2019-11-14 00:02:57.000000 ontobio-2.8.5/bin/materialize.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)      171 2019-11-14 00:02:57.000000 ontobio-2.8.5/bin/clear-cache.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)     7499 2018-05-21 17:20:38.000000 ontobio-2.8.5/bin/ogr.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)     9695 2022-05-06 22:21:58.000000 ontobio-2.8.5/bin/ontobio-parse-assocs.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/tests/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3363 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_remote_scigraph.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4310 2021-01-14 21:39:16.000000 ontobio-2.8.5/tests/test_rdfgen.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      761 2020-12-16 06:27:04.000000 ontobio-2.8.5/tests/test_gpad_writer.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    31765 2023-02-22 00:16:20.000000 ontobio-2.8.5/tests/test_qc.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      719 2021-03-10 22:27:40.000000 ontobio-2.8.5/tests/test_expand_tsv.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1706 2021-02-05 22:01:47.000000 ontobio-2.8.5/tests/test_ontol.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      510 2019-01-19 00:32:49.000000 ontobio-2.8.5/tests/test_alt_id.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      351 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_write_obo.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2022-02-23 01:04:29.000000 ontobio-2.8.5/tests/test_gpaddiffer.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1159 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_local_ttl.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      983 2023-02-21 22:50:51.000000 ontobio-2.8.5/tests/test_golr_query.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    10349 2023-04-24 19:07:00.000000 ontobio-2.8.5/tests/test_gpad_parser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1756 2019-11-14 00:02:57.000000 ontobio-2.8.5/tests/test_evidence_table.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1043 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_lexmap.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1281 2021-01-14 21:39:16.000000 ontobio-2.8.5/tests/test_sparql_connection.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      775 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_bgiparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5578 2019-11-14 00:02:57.000000 ontobio-2.8.5/tests/test_golr_associations.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     8184 2022-02-23 02:15:06.000000 ontobio-2.8.5/tests/test_local_json.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    12770 2022-05-11 03:09:32.000000 ontobio-2.8.5/tests/test_assoc_writer.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3528 2019-01-19 00:32:49.000000 ontobio-2.8.5/tests/test_assocfactory.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5319 2020-04-07 23:32:20.000000 ontobio-2.8.5/tests/test_gaference.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4535 2020-12-16 06:27:04.000000 ontobio-2.8.5/tests/test_parse_ids.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1912 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_map2slim.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1846 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_semsearch.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      736 2021-12-01 01:44:20.000000 ontobio-2.8.5/tests/test_ecomap.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1536 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_golr_map2slim.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    26463 2023-04-24 19:07:00.000000 ontobio-2.8.5/tests/test_gafparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3636 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_assocmodel.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2199 2021-12-01 01:44:20.000000 ontobio-2.8.5/tests/test_hpoaparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      915 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_config.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    11952 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_lexmap_local.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3463 2020-04-07 23:32:20.000000 ontobio-2.8.5/tests/test_validation_rules.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1478 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_enrich.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      963 2021-06-10 18:33:04.000000 ontobio-2.8.5/tests/test_gpiwriter.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1301 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_wd.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      695 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_mutable.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      664 2019-01-19 00:32:49.000000 ontobio-2.8.5/tests/test_parse_taxon.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      550 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_skos_local.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2234 2018-07-24 17:48:08.000000 ontobio-2.8.5/tests/test_golr_search.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5059 2018-05-21 17:20:38.000000 ontobio-2.8.5/tests/test_remote_sparql.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5151 2021-02-05 22:01:47.000000 ontobio-2.8.5/tests/test_collections.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4929 2021-02-16 19:21:55.000000 ontobio-2.8.5/tests/test_goassociation_model.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1610 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_wd_ontol.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5390 2019-11-14 00:02:57.000000 ontobio-2.8.5/tests/test_phenosim_engine.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5645 2021-09-27 18:33:21.000000 ontobio-2.8.5/tests/test_gocamgen.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      450 2021-02-05 22:01:47.000000 ontobio-2.8.5/tests/test_relations.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1043 2021-02-05 22:01:47.000000 ontobio-2.8.5/tests/test_gpiparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3967 2019-01-31 01:39:32.000000 ontobio-2.8.5/tests/test_owlsim2_int.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)       28 2018-05-21 17:20:38.000000 ontobio-2.8.5/MANIFEST.in
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/golr/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2174 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/golr_matrix.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3013 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/beacon_query.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        1 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/golr_entities.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4799 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/golr_stats.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1450 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/golr/golr_sim.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    10470 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/golr/golr_associations.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    68763 2023-02-21 22:52:52.000000 ontobio-2.8.5/ontobio/golr/golr_query.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3867 2022-05-11 03:09:32.000000 ontobio-2.8.5/ontobio/ecomap.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     7379 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/config.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/analysis/
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-19 00:32:49.000000 ontobio-2.8.5/ontobio/analysis/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      457 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/analysis/semsim.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/neo/
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/neo/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     8261 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/neo/scigraph_ontology.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/sparql/
+-rw-r--r--   0 ebertdu    (502) staff       (20)    12491 2019-01-19 00:32:49.000000 ontobio-2.8.5/ontobio/sparql/sparql_go.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5814 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/wikidata_ontology.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/sparql/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     8756 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/sparql_ontology.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    11088 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/sparql_ontol_utils.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1531 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/rdflib_bridge.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2261 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sparql/rdf2nx.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4673 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/wikidata.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4073 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sparql/skos.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/util/
+-rw-r--r--   0 ebertdu    (502) staff       (20)      903 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/util/user_agent.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/util/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2826 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/util/go_utils.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      516 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/util/curie_map.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    18224 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/util/scigraph_util.py
+-rwxr-xr-x   0 ebertdu    (502) staff       (20)      736 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/util/obog2cg.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    17363 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/assocmodel.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      310 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/xref_util.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6821 2020-12-16 06:27:04.000000 ontobio-2.8.5/ontobio/assoc_factory.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/io/
+-rw-r--r--   0 ebertdu    (502) staff       (20)    23204 2023-04-24 19:07:00.000000 ontobio-2.8.5/ontobio/io/gpadparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    24503 2023-04-24 19:07:00.000000 ontobio-2.8.5/ontobio/io/gafparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    42009 2023-02-22 00:16:20.000000 ontobio-2.8.5/ontobio/io/qc.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1633 2019-11-14 00:02:57.000000 ontobio-2.8.5/ontobio/io/parsereport.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6903 2022-02-23 01:04:29.000000 ontobio-2.8.5/ontobio/io/hpoaparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1544 2021-06-10 18:33:04.000000 ontobio-2.8.5/ontobio/io/gafgpibridge.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6271 2021-03-10 22:27:40.000000 ontobio-2.8.5/ontobio/io/assocwriter.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    18018 2022-02-23 01:04:29.000000 ontobio-2.8.5/ontobio/io/differ.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    40091 2023-04-24 19:07:00.000000 ontobio-2.8.5/ontobio/io/assocparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      228 2020-12-16 06:27:04.000000 ontobio-2.8.5/ontobio/io/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    13053 2021-06-10 18:33:04.000000 ontobio-2.8.5/ontobio/io/entityparser.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    12899 2021-01-14 21:39:16.000000 ontobio-2.8.5/ontobio/io/ontol_renderers.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6868 2021-03-22 22:20:40.000000 ontobio-2.8.5/ontobio/io/gaference.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2902 2021-06-10 18:33:04.000000 ontobio-2.8.5/ontobio/io/entitywriter.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1084 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/config.yaml
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1697 2023-04-24 19:08:24.000000 ontobio-2.8.5/ontobio/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2961 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/slimmer.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1642 2021-03-10 22:27:40.000000 ontobio-2.8.5/ontobio/tsv_expander.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    37123 2022-04-26 22:49:10.000000 ontobio-2.8.5/ontobio/ontol.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6351 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/ontol_factory.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/model/
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/model/mme/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1928 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/model/mme/request.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/model/mme/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      607 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/model/mme/response.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      972 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/model/OBOGraph.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2252 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/model/similarity.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/model/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1227 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/model/nlp.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    27873 2022-07-14 23:42:25.000000 ontobio-2.8.5/ontobio/model/association.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5399 2022-02-23 01:04:29.000000 ontobio-2.8.5/ontobio/model/collections.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3211 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/model/bbop_graph.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1527 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/model/GolrResults.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3589 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/model/biomodel.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/rdfgen/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     8382 2022-03-29 20:57:48.000000 ontobio-2.8.5/ontobio/rdfgen/relations.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/rdfgen/__init__.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/
+-rw-r--r--   0 ebertdu    (502) staff       (20)    11120 2021-02-25 21:25:49.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/collapsed_assoc.bk.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     7567 2021-01-27 23:04:39.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     9655 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/collapsed_assoc.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    13135 2021-06-10 20:11:11.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/gocam_builder.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2021-01-27 23:04:39.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     8070 2021-03-10 20:26:34.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/subgraphs.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6653 2021-03-02 01:48:14.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/utils.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    56549 2022-03-29 20:57:48.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/gocamgen.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4947 2021-01-27 23:04:39.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      489 2021-06-10 18:33:04.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/errors.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3330 2021-01-27 23:04:39.000000 ontobio-2.8.5/ontobio/rdfgen/gocamgen/filter_rule.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    12608 2021-03-10 20:26:34.000000 ontobio-2.8.5/ontobio/rdfgen/assoc_rdfgen.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    35539 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/lexmap.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     3665 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/assoc_schema.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2114 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/cgraph.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/sim/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     7583 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/sim/phenosim_engine.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1290 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sim/sim_engine.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-19 00:32:49.000000 ontobio-2.8.5/ontobio/sim/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     6273 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sim/annotation_scorer.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/sim/api/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2397 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sim/api/interfaces.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sim/api/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     7262 2020-04-07 23:32:20.000000 ontobio-2.8.5/ontobio/sim/api/semsearch.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    17404 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/sim/api/owlsim2.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2163 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/sim/api/owlsim3.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2918 2021-12-01 01:44:20.000000 ontobio-2.8.5/ontobio/sim/mme.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/vocabulary/
+-rw-r--r--   0 ebertdu    (502) staff       (20)      955 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/vocabulary/similarity.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      239 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/vocabulary/categories.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)      823 2019-01-31 01:39:32.000000 ontobio-2.8.5/ontobio/vocabulary/upper.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1226 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/vocabulary/relations.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2018-05-21 17:20:38.000000 ontobio-2.8.5/ontobio/vocabulary/__init__.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio/validation/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     5693 2021-01-14 21:39:16.000000 ontobio-2.8.5/ontobio/validation/metadata.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1322 2019-11-14 00:02:57.000000 ontobio-2.8.5/ontobio/validation/tools.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)        0 2019-11-14 00:02:57.000000 ontobio-2.8.5/ontobio/validation/__init__.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    10167 2020-07-21 21:04:11.000000 ontobio-2.8.5/ontobio/validation/rules.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)    12801 2021-09-28 22:21:40.000000 ontobio-2.8.5/ontobio/obograph_util.py
+drwxr-xr-x   0 ebertdu    (502) staff       (20)        0 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/
+-rw-r--r--   0 ebertdu    (502) staff       (20)     1960 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/PKG-INFO
+-rw-r--r--   0 ebertdu    (502) staff       (20)     4395 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/SOURCES.txt
+-rw-r--r--   0 ebertdu    (502) staff       (20)      471 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/requires.txt
+-rw-r--r--   0 ebertdu    (502) staff       (20)       14 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/top_level.txt
+-rw-r--r--   0 ebertdu    (502) staff       (20)        1 2023-04-24 19:08:51.000000 ontobio-2.8.5/ontobio.egg-info/dependency_links.txt
+-rw-r--r--   0 ebertdu    (502) staff       (20)     2370 2021-03-01 23:16:52.000000 ontobio-2.8.5/setup.py
+-rw-r--r--   0 ebertdu    (502) staff       (20)       80 2023-04-24 19:08:51.000000 ontobio-2.8.5/setup.cfg
+-rw-r--r--   0 ebertdu    (502) staff       (20)      970 2018-05-21 17:20:38.000000 ontobio-2.8.5/README.rst
```

### Comparing `ontobio-2.8.4/PKG-INFO` & `ontobio-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.4
+Version: 2.8.5
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Description: |PyPI|
```

### Comparing `ontobio-2.8.4/bin/ontobio-lexmap.py` & `ontobio-2.8.5/bin/ontobio-lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/ontobio-assoc.py` & `ontobio-2.8.5/bin/ontobio-assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/rdfgen.py` & `ontobio-2.8.5/bin/rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/validate.py` & `ontobio-2.8.5/bin/validate.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/materialize.py` & `ontobio-2.8.5/bin/materialize.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/ogr.py` & `ontobio-2.8.5/bin/ogr.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/bin/ontobio-parse-assocs.py` & `ontobio-2.8.5/bin/ontobio-parse-assocs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_remote_scigraph.py` & `ontobio-2.8.5/tests/test_remote_scigraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_rdfgen.py` & `ontobio-2.8.5/tests/test_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gpad_writer.py` & `ontobio-2.8.5/tests/test_gpad_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_qc.py` & `ontobio-2.8.5/tests/test_qc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_expand_tsv.py` & `ontobio-2.8.5/tests/test_expand_tsv.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_ontol.py` & `ontobio-2.8.5/tests/test_ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_local_ttl.py` & `ontobio-2.8.5/tests/test_local_ttl.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_golr_query.py` & `ontobio-2.8.5/tests/test_golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gpad_parser.py` & `ontobio-2.8.5/tests/test_gpad_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,44 @@
             # repaired test GO elements
             ConjunctiveSet(elements=[Curie(namespace='GO', identity='2'), Curie(namespace='GO', identity='3')]),
             # non GO elements stay the same, could be obsolete or not
             ConjunctiveSet(elements=[Curie(namespace='ZFIN', identity='ZDB-MRPHLNO-010101-1'),
                                      Curie(namespace='MGI', identity='1232453')])] == assoc.evidence.with_support_from
 
 
+def test_obsolete_term_repair_extensions():
+
+    vals = ["ZFIN",
+            "ZFIN:ZDB-GENE-980526-362",
+            "acts_upstream_of_or_within",
+            "GO:0007155",
+            "PMID:15494018",
+            "ECO:0000305",
+            "ZFIN:ZDB-MRPHLNO-010101-1,MGI:1232453",
+            "",
+            "20041026",
+            "ZFIN",
+            "part_of(GO:0005913)|occurs_in(GO:1),has_input(GO:4)|enables(ZFIN:ZDB-MRPHLNO-010101-1),enables(MGI:1232453)",
+            "contributor=GOC:zfin_curators|model-state=production|noctua-model-id=gomodel:ZFIN_ZDB-GENE-980526-362"
+            ]
+    ont = OntologyFactory().create(ALT_ID_ONT)
+    config = assocparser.AssocParserConfig(ontology=ont, rule_set=assocparser.RuleSet.ALL)
+    parser = GpadParser(config=config)
+    result = parser.parse_line("\t".join(vals))
+    assoc = result.associations[0]
+    # GO:0005913 should be repaired to its replacement term, GO:00005912
+    object_extensions = [association.ConjunctiveSet([association.ExtensionUnit(association.Curie("BFO", "0000050"), association.Curie("GO", "0005912"))]),
+            # repaired test GO elements
+            association.ConjunctiveSet([association.ExtensionUnit(association.Curie("BFO", "0000066"), association.Curie(namespace='GO', identity='2')),association.ExtensionUnit(association.Curie("RO", "0002233"), association.Curie(namespace='GO', identity='3'))]),
+            # non GO elements stay the same, could be obsolete or not
+            association.ConjunctiveSet([association.ExtensionUnit(association.Curie("RO", "0002327"), association.Curie(namespace='ZFIN', identity='ZDB-MRPHLNO-010101-1')),association.ExtensionUnit(association.Curie("RO", "0002327"), association. Curie(namespace='MGI', identity='1232453'))])
+            ]
+    assert object_extensions == assoc.object_extensions
+
+
 def test_skim():
     p = GpadParser()
     results = p.skim(open(POMBASE,"r"))
     print(str(results))
 
 
 def test_parse():
```

### Comparing `ontobio-2.8.4/tests/test_evidence_table.py` & `ontobio-2.8.5/tests/test_evidence_table.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_lexmap.py` & `ontobio-2.8.5/tests/test_lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_sparql_connection.py` & `ontobio-2.8.5/tests/test_sparql_connection.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_bgiparser.py` & `ontobio-2.8.5/tests/test_bgiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_golr_associations.py` & `ontobio-2.8.5/tests/test_golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_local_json.py` & `ontobio-2.8.5/tests/test_local_json.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_assoc_writer.py` & `ontobio-2.8.5/tests/test_assoc_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_assocfactory.py` & `ontobio-2.8.5/tests/test_assocfactory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gaference.py` & `ontobio-2.8.5/tests/test_gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_parse_ids.py` & `ontobio-2.8.5/tests/test_parse_ids.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_map2slim.py` & `ontobio-2.8.5/tests/test_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_semsearch.py` & `ontobio-2.8.5/tests/test_semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_ecomap.py` & `ontobio-2.8.5/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_golr_map2slim.py` & `ontobio-2.8.5/tests/test_golr_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gafparser.py` & `ontobio-2.8.5/tests/test_gafparser.py`

 * *Files 13% similar despite different names*

```diff
@@ -485,14 +485,57 @@
 
 def test_object_extensions_error():
     p = GafParser()
     assoc_result = p.parse_line("PomBase\tSPAC25B8.17\typf1\t\tGO:0000007\tGO_REF:0000024\tISO\tSGD:S000001583\tC\tintramembrane aspartyl protease of the perinuclear ER membrane Ypf1 (predicted)\tppp81\tprotein\ttaxon:4896\t20181024\tPomBase\tpart_of(X)\tUniProtKB:P12345")
     assert len(p.report.to_report_json()["messages"]["gorule-0000001"]) == 1
 
 
+def test_obsolete_replair_of_extensions():
+    p = GafParser(config=assocparser.AssocParserConfig(
+        ontology=OntologyFactory().create(OBSOLETE_ONT))) 
+    assoc_result = p.parse_line("ZFIN\tZDB-GENE-980526-362\tctnnb1\t\tGO:0007155\tPMID:15494018\tIC\tGO:0005913\tP\tcatenin (cadherin-associated protein), beta 1\tctnnb|id:ibd2058|wu:fb73e10|wu:fi81c06|wu:fk25h01\tprotein_coding_gene\ttaxon:7955\t20041026\tZFIN\tpart_of(GO:0005913)\tUniProtKB:P12345")
+    print(p.report.to_markdown())
+    assert len(assoc_result.associations[0].object_extensions) > 0
+    object_extensions = [
+        association.ConjunctiveSet([
+            association.ExtensionUnit(association.Curie("BFO", "0000050"), association.Curie("GO", "0005912"))
+        ])
+    ]
+    assert assoc_result.associations[0].object_extensions == object_extensions
+    
+    #Reset the report
+    p = GafParser(config=assocparser.AssocParserConfig(
+        ontology=OntologyFactory().create(OBSOLETE_ONT))) 
+    assoc_result = p.parse_line("ZFIN\tZDB-GENE-980526-362\tctnnb1\t\tGO:0007155\tPMID:15494018\tIC\tGO:0005912\tP\tcatenin (cadherin-associated protein), beta 1\tctnnb|id:ibd2058|wu:fb73e10|wu:fi81c06|wu:fk25h01\tprotein_coding_gene\ttaxon:7955\t20041026\tZFIN\tpart_of(GO:0005913)|part_of(GO:0016458)\tUniProtKB:P12345")
+    print(p.report.to_markdown())
+    assert assoc_result.associations == []
+    assert p.report.to_report_json()["messages"]["gorule-0000020"][0]["obj"] == "GO:0005913"    
+    assert p.report.to_report_json()["messages"]["gorule-0000020"][1]["obj"] == "GO:0016458"          
+    
+    #Reset the report
+    p = GafParser(config=assocparser.AssocParserConfig(
+        ontology=OntologyFactory().create(OBSOLETE_ONT))) 
+    assoc_result = p.parse_line("ZFIN\tZDB-GENE-980526-362\tctnnb1\t\tGO:0007155\tPMID:15494018\tIC\tGO:0005912\tP\tcatenin (cadherin-associated protein), beta 1\tctnnb|id:ibd2058|wu:fb73e10|wu:fi81c06|wu:fk25h01\tprotein_coding_gene\ttaxon:7955\t20041026\tZFIN\tpart_of(GO:0005913)|part_of(GO:0007155),occurs_in(Y:1)\tUniProtKB:P12345")
+    print(p.report.to_markdown())
+    assert len(assoc_result.associations[0].object_extensions) > 0
+    object_extensions = [
+        association.ConjunctiveSet([association.ExtensionUnit(association.Curie("BFO", "0000050"), association.Curie("GO", "0005912"))]),
+        association.ConjunctiveSet([association.ExtensionUnit(association.Curie("BFO", "0000050"), association.Curie("GO", "0007155")),association.ExtensionUnit(association.Curie("BFO", "0000066"), association.Curie("Y", "1"))])        
+    ]
+    assert assoc_result.associations[0].object_extensions == object_extensions    
+    
+    #Reset the report
+    p = GafParser(config=assocparser.AssocParserConfig(
+        ontology=OntologyFactory().create(OBSOLETE_ONT)))
+    assoc_result = p.parse_line("ZFIN\tZDB-GENE-980526-362\tctnnb1\t\tGO:0007155\tPMID:15494018\tIC\tGO:0005912\tP\tcatenin (cadherin-associated protein), beta 1\tctnnb|id:ibd2058|wu:fb73e10|wu:fi81c06|wu:fk25h01\tprotein_coding_gene\ttaxon:7955\t20041026\tZFIN\tpart_of(GO:0016458)\tUniProtKB:P12345")
+    print(p.report.to_markdown())
+    assert assoc_result.associations == []
+    assert p.report.to_report_json()["messages"]["gorule-0000020"][0]["obj"] == "GO:0016458"    
+    
+
 def test_factory():
     afa = AssociationSetFactory()
     ont = OntologyFactory().create(ONT)
     aset = afa.create_from_file(POMBASE, ontology=ont, skim=False)
 
     found = 0
     for s in aset.subjects:
```

### Comparing `ontobio-2.8.4/tests/test_assocmodel.py` & `ontobio-2.8.5/tests/test_assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_hpoaparser.py` & `ontobio-2.8.5/tests/test_hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_config.py` & `ontobio-2.8.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_lexmap_local.py` & `ontobio-2.8.5/tests/test_lexmap_local.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_validation_rules.py` & `ontobio-2.8.5/tests/test_validation_rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_enrich.py` & `ontobio-2.8.5/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gpiwriter.py` & `ontobio-2.8.5/tests/test_gpiwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_wd.py` & `ontobio-2.8.5/tests/test_wd.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_mutable.py` & `ontobio-2.8.5/tests/test_mutable.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_parse_taxon.py` & `ontobio-2.8.5/tests/test_parse_taxon.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_skos_local.py` & `ontobio-2.8.5/tests/test_skos_local.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_golr_search.py` & `ontobio-2.8.5/tests/test_golr_search.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_remote_sparql.py` & `ontobio-2.8.5/tests/test_remote_sparql.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_collections.py` & `ontobio-2.8.5/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_goassociation_model.py` & `ontobio-2.8.5/tests/test_goassociation_model.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_wd_ontol.py` & `ontobio-2.8.5/tests/test_wd_ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_phenosim_engine.py` & `ontobio-2.8.5/tests/test_phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gocamgen.py` & `ontobio-2.8.5/tests/test_gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_gpiparser.py` & `ontobio-2.8.5/tests/test_gpiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/tests/test_owlsim2_int.py` & `ontobio-2.8.5/tests/test_owlsim2_int.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/golr_matrix.py` & `ontobio-2.8.5/ontobio/golr/golr_matrix.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/beacon_query.py` & `ontobio-2.8.5/ontobio/golr/beacon_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/golr_stats.py` & `ontobio-2.8.5/ontobio/golr/golr_stats.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/golr_sim.py` & `ontobio-2.8.5/ontobio/golr/golr_sim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/golr_associations.py` & `ontobio-2.8.5/ontobio/golr/golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/golr/golr_query.py` & `ontobio-2.8.5/ontobio/golr/golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/ecomap.py` & `ontobio-2.8.5/ontobio/ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/config.py` & `ontobio-2.8.5/ontobio/config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/neo/scigraph_ontology.py` & `ontobio-2.8.5/ontobio/neo/scigraph_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/sparql_go.py` & `ontobio-2.8.5/ontobio/sparql/sparql_go.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/wikidata_ontology.py` & `ontobio-2.8.5/ontobio/sparql/wikidata_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/sparql_ontology.py` & `ontobio-2.8.5/ontobio/sparql/sparql_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/sparql_ontol_utils.py` & `ontobio-2.8.5/ontobio/sparql/sparql_ontol_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/rdflib_bridge.py` & `ontobio-2.8.5/ontobio/sparql/rdflib_bridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/rdf2nx.py` & `ontobio-2.8.5/ontobio/sparql/rdf2nx.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/wikidata.py` & `ontobio-2.8.5/ontobio/sparql/wikidata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sparql/skos.py` & `ontobio-2.8.5/ontobio/sparql/skos.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/util/user_agent.py` & `ontobio-2.8.5/ontobio/util/user_agent.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/util/go_utils.py` & `ontobio-2.8.5/ontobio/util/go_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/util/curie_map.py` & `ontobio-2.8.5/ontobio/util/curie_map.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/util/scigraph_util.py` & `ontobio-2.8.5/ontobio/util/scigraph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/util/obog2cg.py` & `ontobio-2.8.5/ontobio/util/obog2cg.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/assocmodel.py` & `ontobio-2.8.5/ontobio/assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/assoc_factory.py` & `ontobio-2.8.5/ontobio/assoc_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/gpadparser.py` & `ontobio-2.8.5/ontobio/io/gpadparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,14 +155,26 @@
 
         assoc = parsed.associations[0]
 
         split_line = assocparser.SplitLine(line=line, values=vals, taxon="")
 
         # repair any GO terms in the with/from field that may be obsolete
         assoc.evidence.with_support_from = self._unroll_withfrom_and_replair_obsoletes(split_line, 'gpad')
+        
+        # repair, if possible any GO terms in the extensions that may be obsolete
+        if (0 < len(assoc.object_extensions)):
+            for ext in assoc.object_extensions:
+                validated = self.validate_curie_ids([e.term for e in ext.elements], split_line)
+                if validated is None:
+                    return assocparser.ParseResult(line, [], True)
+            repaired = self._repair_extensions(assoc.object_extensions, split_line)
+            if repaired is None:
+                    assoc.object_extensions = []
+                    return assocparser.ParseResult(line, [], True)
+            assoc.object_extensions = repaired 
 
         valid_goid = self._validate_ontology_class_id(str(assoc.object.id), split_line)
         if valid_goid is None:
             return assocparser.ParseResult(line, [], True)
         assoc.object.id = association.Curie.from_str(valid_goid)
 
         go_rule_results = qc.test_go_rules(assoc, self.config)
```

### Comparing `ontobio-2.8.4/ontobio/io/gafparser.py` & `ontobio-2.8.5/ontobio/io/gafparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,28 @@
             validated = self.validate_curie_ids(wf.elements, split_line)
             if validated is None:
                 return assocparser.ParseResult(line, [], True)
         with_support_from = self._unroll_withfrom_and_replair_obsoletes(split_line, 'gaf')
         if with_support_from is None:
             return assocparser.ParseResult(line, [], True)
         assoc.evidence.with_support_from = with_support_from
+        
+        # Extension
+        # repair, if possible any GO terms in the extensions that may be obsolete
+        if (0 < len(assoc.object_extensions)):
+            for ext in assoc.object_extensions:
+                validated = self.validate_curie_ids([e.term for e in ext.elements], split_line)
+                if validated is None:
+                    return assocparser.ParseResult(line, [], True)
+            repaired = self._repair_extensions(assoc.object_extensions, split_line)
+            if repaired is None:
+                    assoc.object_extensions = []        
+                    return assocparser.ParseResult(line, [], True)
+            assoc.object_extensions = repaired    
+        
         # validation
         self._validate_symbol(assoc.subject.label, split_line)
 
 
         ## --
         ## taxon CARD={1,2}
         ## --
```

### Comparing `ontobio-2.8.4/ontobio/io/qc.py` & `ontobio-2.8.5/ontobio/io/qc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/parsereport.py` & `ontobio-2.8.5/ontobio/io/parsereport.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/hpoaparser.py` & `ontobio-2.8.5/ontobio/io/hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/gafgpibridge.py` & `ontobio-2.8.5/ontobio/io/gafgpibridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/assocwriter.py` & `ontobio-2.8.5/ontobio/io/assocwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/differ.py` & `ontobio-2.8.5/ontobio/io/differ.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/assocparser.py` & `ontobio-2.8.5/ontobio/io/assocparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,22 @@
 
     def to_report_json(self):
         """
         Generate a summary in json format
         """
 
         return self.reporter.json(self.n_lines, self.n_assocs, self.skipped)
+    
+    def sort_messages(self, r, messages):
+        if len(messages) > 0:
+            # Messages for GORULE:0000020 are sorted by level (Error before Warning), then by GO id 
+            if r != "GORULE:0000020":
+                return None
+            messages.sort(key=lambda x: x.get('level'))
+            messages.sort(key=lambda x: x.get('obj'))
 
     def to_markdown(self):
         """
         Generate a summary in markdown format
         """
         json = self.to_report_json()
         # summary = json['summary']
@@ -459,14 +467,16 @@
 
             s += "### {rule}\n\n".format(rule=rule)
             if rule != "other" and self.config.rule_metadata:
                 s += "{title}\n\n".format(title=self.config.rule_metadata.get(rule, {}).get("title", ""))
             s += "* total: {amount}\n".format(amount=len(messages))
             if len(messages) > 0:
                 s += "#### Messages\n"
+                
+            self.sort_messages(rule, messages)    
             for message in messages:
                 obj = " ({})".format(message["obj"]) if message["obj"] else ""
                 s += "* {level} - {type}: {message}{obj} -- `{line}`\n".format(level=message["level"], type=message["type"], message=message["message"], line=message["line"], obj=obj)
 
         return s
 
 @dataclass
@@ -727,14 +737,38 @@
                     id = None
             else:
                 self.report.warning(line.line, Report.OBSOLETE_CLASS, id, msg="Violates GORULE:0000020",
                     taxon=line.taxon, rule=20)
                 id = None
 
         return id
+    
+            
+    # repair extensions
+    def _repair_extensions(self, extensions, line: SplitLine, subclassof=None):
+        # nothing to repair
+        if len(extensions) == 0:
+            return extensions
+        
+        grouped_set = []
+        for ext in extensions:
+            curSet = []
+            for e in ext.elements:               
+                if e.term.namespace =='GO':
+                    fixed_element_individual = self._validate_ontology_class_id(str(e.term), line)
+                    if fixed_element_individual is None:
+                        return None
+                    else:         
+                        curSet.append(association.ExtensionUnit(relation = association.Curie(e.relation.namespace, e.relation.identity), term = association.Curie.from_str(fixed_element_individual)))
+                else:
+                    curSet.append(association.ExtensionUnit(relation = association.Curie(e.relation.namespace, e.relation.identity), term = association.Curie(e.term.namespace, e.term.identity)))        
+
+            grouped_set.append(association.ConjunctiveSet(curSet))
+                         
+        return grouped_set
 
     def _validate_symbol(self, symbol, line: SplitLine):
         if symbol is None or symbol == "":
             self.report.warning(line.line, Report.INVALID_SYMBOL, symbol, "GORULE:0000027: symbol is empty",
                 taxon=line.taxon, rule=27)
 
     non_id_regex = re.compile(r"[^\.:_\-0-9a-zA-Z]")
```

### Comparing `ontobio-2.8.4/ontobio/io/entityparser.py` & `ontobio-2.8.5/ontobio/io/entityparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/ontol_renderers.py` & `ontobio-2.8.5/ontobio/io/ontol_renderers.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/gaference.py` & `ontobio-2.8.5/ontobio/io/gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/io/entitywriter.py` & `ontobio-2.8.5/ontobio/io/entitywriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/config.yaml` & `ontobio-2.8.5/ontobio/config.yaml`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/__init__.py` & `ontobio-2.8.5/ontobio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import absolute_import
 
-__version__ = '2.8.4'
+__version__ = '2.8.5'
 
 
 from .ontol_factory import OntologyFactory
 from .ontol import Ontology, Synonym, TextDefinition
 from .assoc_factory import AssociationSetFactory
 from .io.ontol_renderers import GraphRenderer
```

### Comparing `ontobio-2.8.4/ontobio/slimmer.py` & `ontobio-2.8.5/ontobio/slimmer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/tsv_expander.py` & `ontobio-2.8.5/ontobio/tsv_expander.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/ontol.py` & `ontobio-2.8.5/ontobio/ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/ontol_factory.py` & `ontobio-2.8.5/ontobio/ontol_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/mme/request.py` & `ontobio-2.8.5/ontobio/model/mme/request.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/mme/response.py` & `ontobio-2.8.5/ontobio/model/mme/response.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/OBOGraph.py` & `ontobio-2.8.5/ontobio/model/OBOGraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/similarity.py` & `ontobio-2.8.5/ontobio/model/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/nlp.py` & `ontobio-2.8.5/ontobio/model/nlp.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/association.py` & `ontobio-2.8.5/ontobio/model/association.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/collections.py` & `ontobio-2.8.5/ontobio/model/collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/bbop_graph.py` & `ontobio-2.8.5/ontobio/model/bbop_graph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/GolrResults.py` & `ontobio-2.8.5/ontobio/model/GolrResults.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/model/biomodel.py` & `ontobio-2.8.5/ontobio/model/biomodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/relations.py` & `ontobio-2.8.5/ontobio/rdfgen/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/collapsed_assoc.bk.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/collapsed_assoc.bk.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/triple_pattern_finder.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/triple_pattern_finder.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/collapsed_assoc.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/collapsed_assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/gocam_builder.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/gocam_builder.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/subgraphs.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/subgraphs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/utils.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/gocamgen.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/gocamgen/filter_rule.py` & `ontobio-2.8.5/ontobio/rdfgen/gocamgen/filter_rule.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/rdfgen/assoc_rdfgen.py` & `ontobio-2.8.5/ontobio/rdfgen/assoc_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/lexmap.py` & `ontobio-2.8.5/ontobio/lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/assoc_schema.py` & `ontobio-2.8.5/ontobio/assoc_schema.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/cgraph.py` & `ontobio-2.8.5/ontobio/cgraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/phenosim_engine.py` & `ontobio-2.8.5/ontobio/sim/phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/sim_engine.py` & `ontobio-2.8.5/ontobio/sim/sim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/annotation_scorer.py` & `ontobio-2.8.5/ontobio/sim/annotation_scorer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/api/interfaces.py` & `ontobio-2.8.5/ontobio/sim/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/api/semsearch.py` & `ontobio-2.8.5/ontobio/sim/api/semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/api/owlsim2.py` & `ontobio-2.8.5/ontobio/sim/api/owlsim2.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/api/owlsim3.py` & `ontobio-2.8.5/ontobio/sim/api/owlsim3.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/sim/mme.py` & `ontobio-2.8.5/ontobio/sim/mme.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/vocabulary/similarity.py` & `ontobio-2.8.5/ontobio/vocabulary/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/vocabulary/upper.py` & `ontobio-2.8.5/ontobio/vocabulary/upper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/vocabulary/relations.py` & `ontobio-2.8.5/ontobio/vocabulary/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/validation/metadata.py` & `ontobio-2.8.5/ontobio/validation/metadata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/validation/tools.py` & `ontobio-2.8.5/ontobio/validation/tools.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/validation/rules.py` & `ontobio-2.8.5/ontobio/validation/rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio/obograph_util.py` & `ontobio-2.8.5/ontobio/obograph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/ontobio.egg-info/PKG-INFO` & `ontobio-2.8.5/ontobio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.4
+Version: 2.8.5
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Description: |PyPI|
```

### Comparing `ontobio-2.8.4/ontobio.egg-info/SOURCES.txt` & `ontobio-2.8.5/ontobio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/setup.py` & `ontobio-2.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.4/README.rst` & `ontobio-2.8.5/README.rst`

 * *Files identical despite different names*


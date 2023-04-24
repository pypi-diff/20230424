# Comparing `tmp/lmcv_tools-0.0.5.tar.gz` & `tmp/lmcv_tools-0.0.6.tar.gz`

## Comparing `lmcv_tools-0.0.5.tar` & `lmcv_tools-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,105 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/docs/To Do.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/commands/__init__.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/commands/extract.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/commands/generate.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/commands/translate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/databases/__init__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/databases/element_relations.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/databases/extraction_attributes.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/databases/help_messages.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/interface/__init__.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/interface/core.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/interface/filer.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/interface/messenger.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/interface/searcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/custom_errors.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/extraction_components.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/generation_artifacts.py
--rw-r--r--   0        0        0    14092 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/graphical_interfaces.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/lmcv_tools/models/translation_entities.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/test_extract.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/test_generate.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/test_translate.py
--rw-r--r--   0        0        0   113958 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic.pos
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_and.csv
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_df.csv
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_eq.csv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ge.csv
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_gt.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_1.csv
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_2.csv
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_le.csv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ls.csv
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_or.csv
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_1.csv
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv
--rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_1.csv
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_2.csv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_node_id.csv
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_node_x.csv
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_node_y.csv
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_node_z.csv
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_factor.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_id.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_w.csv
--rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate.pos
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_factor.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_id.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_node_u.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_node_v.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_shell.inp
--rw-r--r--   0        0        0    13613 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp
--rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_solid.inp
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_voight.inp
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Circle_S3_S4R_4x4.inp
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Circle_S3_S4R_4x4_exp.dat
--rw-r--r--   0        0        0    45691 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_C3D20R.inp
--rw-r--r--   0        0        0    52587 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_C3D20R_exp.dat
--rw-r--r--   0        0        0    50506 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_S8R.inp
--rw-r--r--   0        0        0    59740 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_S8R_exp.dat
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_1x1x1.inp
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_1x1x1_exp.dat
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_2x2x2.inp
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_2x2x2_exp.dat
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_1x1x1.inp
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_1x1x1_exp.dat
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_2x2x2.inp
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_2x2x2_exp.dat
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_1x1.inp
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_1x1_exp.dat
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_2x2.inp
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_2x2_exp.dat
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_1x1.inp
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_1x1_exp.dat
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_2x2.inp
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_2x2_exp.dat
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_1x1.inp
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_1x1_exp.dat
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_2x2.inp
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_2x2_exp.dat
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_1x1.inp
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_1x1_exp.dat
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_2x2.inp
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_2x2_exp.dat
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/LICENSE
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     9858 2020-02-02 00:00:00.000000 lmcv_tools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/docs/To Do.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/commands/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/commands/extract.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/commands/generate.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/commands/translate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/databases/__init__.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/databases/extraction_attributes.json
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/databases/help_messages.json
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/databases/translation_reference.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/interface/__init__.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/interface/core.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/interface/filer.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/interface/messenger.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/interface/searcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/custom_errors.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/extraction_components.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/generation_artifacts.py
+-rw-r--r--   0        0        0    14092 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/graphical_interfaces.py
+-rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/lmcv_tools/models/translation_components.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/test_extract.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/test_generate.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/test_translate.py
+-rw-r--r--   0        0        0   113958 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic.pos
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_and.csv
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_df.csv
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_eq.csv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ge.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_gt.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_1.csv
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_2.csv
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_le.csv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ls.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_or.csv
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_1.csv
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv
+-rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_1.csv
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_2.csv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_node_id.csv
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_node_x.csv
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_node_y.csv
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_node_z.csv
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_factor.csv
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_id.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_w.csv
+-rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate.pos
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_factor.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_id.csv
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_node_u.csv
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_node_v.csv
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_shell.inp
+-rw-r--r--   0        0        0    13613 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp
+-rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_solid.inp
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_voight.inp
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4_exp.svg
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2.dat
+-rw-r--r--   0        0        0    12375 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2_exp.svg
+-rw-r--r--   0        0        0    47634 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4.dat
+-rw-r--r--   0        0        0    60976 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4_exp.svg
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2.dat
+-rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2_exp.svg
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4_exp.dat
+-rw-r--r--   0        0        0    45691 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp
+-rw-r--r--   0        0        0    52988 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat
+-rw-r--r--   0        0        0    50506 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp
+-rw-r--r--   0        0        0    60178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_1x1_exp.dat
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1_exp.dat
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1_exp.dat
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/LICENSE
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 lmcv_tools-0.0.6/PKG-INFO
```

### Comparing `lmcv_tools-0.0.5/lmcv_tools/commands/extract.py` & `lmcv_tools-0.0.6/lmcv_tools/commands/extract.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/lmcv_tools/commands/generate.py` & `lmcv_tools-0.0.6/lmcv_tools/commands/generate.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/lmcv_tools/databases/extraction_attributes.json` & `lmcv_tools-0.0.6/lmcv_tools/databases/extraction_attributes.json`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/lmcv_tools/databases/help_messages.json` & `lmcv_tools-0.0.6/lmcv_tools/databases/help_messages.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9549679487179488%*

 * *Differences: {"'generate'": "{'topics': {'Possible Arguments': {'[args]': 'Series of arguments that depend on "*

 * *               "the artifact. See the topics bellow for more details'}, 'Arguments for "*

 * *               "virtual_laminas': {'[Smart Laminas]': 'Required boolean argument. If True, the "*

 * *               "laminas will be generated by a new smart method'}}}",*

 * * "'translate'": "{'usage': 'translate [path/to/file] to [extension]', 'topics': {'Possible "*

 * *                "Arguments': {replace: OrderedDict([('[path/to/f […]*

```diff
@@ -29,36 +29,40 @@
                 "[E2]": "Required float point argument. Elastic Modulus of Material 2",
                 "[Element Type]": "Required string argument. Supported element types: Solid, Shell",
                 "[Laminas Count]": "Required integer argument",
                 "[Laminas Thickness]": "Required floatpoint argument",
                 "[Micromechanical Model]": "Required string argument. Supported micromechanical models: voight, mori_tanaka",
                 "[Number of Integration Points]": "Required integer argument",
                 "[Power Law Exponent]": "Required float point argument. Exponent of Power Law, a mathematical function that determines the volume fractions of the Functionally Graded Material represented by virtual laminas",
-                "[Smart Laminas]": "Required boolean argument. If True, the laminas will be generated by a new smart method.",
+                "[Smart Laminas]": "Required boolean argument. If True, the laminas will be generated by a new smart method",
                 "[nu1]": "Required float point argument. Poisson's Coefficient of Material 1",
                 "[nu2]": "Required float point argument. Poisson's Coefficient of Material 2",
                 "[pho1]": "Required float point argument. Density of Material 1",
                 "[pho2]": "Required float point argument. Density of Material 2"
             },
             "Possible Arguments": {
-                "[args]": "Series of arguments that depend on the artifact. See the topics bellow for more details.",
+                "[args]": "Series of arguments that depend on the artifact. See the topics bellow for more details",
                 "[artifact name]": "Required argument. Name of the artifact. Supported artifacts: virtual_laminas",
                 "[path/to/artifact]": "Optional argument. Relative path to artifact output files. If it is not given, it will be the file with the same name of artifact in the current directory"
             }
         },
         "usage": "generate [artifact name] [args] [path/to/artifact]"
     },
     "translate": {
         "topics": {
             "Possible Arguments": {
-                "[path/to/.dat]": "Optional argument. Relative path to .dat file. If it is not given, it will be the same as the .inp file",
-                "[path/to/.inp]": "Required argument. Relative path to .inp file"
+                "[new extension]": "Required argument. Extension to which the file will be translated",
+                "[path/to/file]": "Required argument. Relative path to file"
+            },
+            "Possible Translations": {
+                ".dat to .svg": "Example: translate Plate.dat to .svg",
+                ".inp to .dat": "Example: translate Job-1.inp to .dat"
             }
         },
-        "usage": "translate [path/to/.inp] [path/to/.dat]"
+        "usage": "translate [path/to/file] to [extension]"
     },
     "version": {
         "topics": {
             "Details": {
                 "No Arguments": "This command shows the version of this program"
             }
         },
```

### Comparing `lmcv_tools-0.0.5/lmcv_tools/interface/core.py` & `lmcv_tools-0.0.6/lmcv_tools/interface/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import messenger, searcher
 from ..models.custom_errors import CommandError
 
 # Constantes Globais
-version = '0.0.5'
+version = '0.0.6'
 in_interactive_mode = False
 message_welcome = '''
 LMCV Tools is a command line tool that provides a series of useful functionali-
 ties for the day-to-day simulations of the "Laboratório de Mecânica Computacio-
 nal e Visualização" of the "Universidade Federal do Ceará" (UFC). 
 
 Since a command was not typed, interactive mode was started. Here, you can type
@@ -66,28 +66,33 @@
 
       # Quebra de Linha Final do Tópico
       messenger.show('')
 
 def pre_translate(file_paths: list[str]):
    from ..commands import translate
 
-   # Verificando Path do .inp
+   # Verificando Path do Input
    try:
-      inp_path = file_paths[0]
+      input_path = file_paths[0]
    except IndexError:
-      raise CommandError('The Path to .inp file is required.')
+      raise CommandError('An Input File Path is required.')
 
-   # Verificando Path do .dat
+   # Verificando Extensão do Output
    try:
-      dat_path = file_paths[1]
+      if 'to' != file_paths[1]:
+         raise CommandError('"to" keyword after Input File Path is required.')
    except IndexError:
-      dat_path = inp_path[:-3] + 'dat'
+      raise CommandError('"to" keyword after Input File Path is required.')
+   try:
+      output_extension = file_paths[2]
+   except IndexError:
+      raise CommandError('An Extension for Output File after "to" keyword is required.')
    
-   # Traduzindo Arquivo .inp
-   translate.start(inp_path, dat_path)
+   # Iniciando Tradução
+   translate.start(input_path, output_extension)
 
 def pre_extract(terms: list[str]):
    from ..commands import extract
 
    # Verificando Sintaxe Básica da Sentença
    if 'from' not in terms:
       raise CommandError('The keyword "from" is required.', help=True)
```

### Comparing `lmcv_tools-0.0.5/lmcv_tools/models/extraction_components.py` & `lmcv_tools-0.0.6/lmcv_tools/models/extraction_components.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/lmcv_tools/models/generation_artifacts.py` & `lmcv_tools-0.0.6/lmcv_tools/models/generation_artifacts.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/lmcv_tools/models/graphical_interfaces.py` & `lmcv_tools-0.0.6/lmcv_tools/models/graphical_interfaces.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/test_extract.py` & `lmcv_tools-0.0.6/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/test_generate.py` & `lmcv_tools-0.0.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/test_translate.py` & `lmcv_tools-0.0.6/tests/test_translate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import unittest
 import os
 
 class DefaultTest(unittest.TestCase):
-   def default_test(self, benchmark_name: str):
+   def default_test(self, benchmark_name: str, input_extension: str, output_extension: str):
       # Definindo paths
-      inp_path = 'tests/benchmark/translate/' + benchmark_name + '.inp'
-      dat_path = inp_path[:-3] + 'dat'
-      exp_path = inp_path[:-4] + '_exp.dat'
+      benchmark_name = 'tests/benchmark/translate/' + benchmark_name
+      input_path = benchmark_name + input_extension
+      output_path = benchmark_name + output_extension
+      exp_path = input_path[:-4] + '_exp' + output_extension
 
       # Traduzindo Benchmark
-      code = os.system(f'python -m lmcv_tools translate {inp_path}')
+      code = os.system(f'python -m lmcv_tools translate {input_path} to {output_extension}')
       self.assertEqual(code, 0, 'A tradução falhou.')
 
       # Comparando Tradução com o Resultado Esperado
-      dat_file = open(dat_path, 'r')
+      output_file = open(output_path, 'r')
       exp_file = open(exp_path, 'r')
-      dat_data = dat_file.read()
+      output_data = output_file.read()
       exp_data = exp_file.read()
-      dat_file.close()
+      output_file.close()
       exp_file.close()
-      self.assertEqual(dat_data, exp_data, 'A tradução está incorreta.')
+      self.assertEqual(output_data, exp_data, 'A tradução está incorreta.')
+
+      # Removendo Arquivo Gerado
+      os.remove(output_path)
 
-      # Removendo Arquivo .dat Gerado
-      os.remove(dat_path)
+class Test_inp_to_dat(DefaultTest):
+   def default_test(self, benchmark_name: str):
+      super().default_test('inp_to_dat/' + benchmark_name, '.inp', '.dat')
 
-class Test2D(DefaultTest):
    def test_triangle_S3_1x1(self):
       self.default_test('Triangle_S3_1x1')
 
    def test_triangle_S3_2x2(self):
       self.default_test('Triangle_S3_2x2')
 
    def test_triangle_STRI65_1x1(self):
@@ -48,25 +52,41 @@
    
    def test_square_S8R_2x2(self):
       self.default_test('Square_S8R_2x2')
    
    def test_circle_S3_S4R_4x4(self):
       self.default_test('Circle_S3_S4R_4x4')
 
-   def test_complex_part_S8R_2x2(self):
+   def test_complex_part_S8R(self):
       self.default_test('ComplexPart_S8R')
 
-class Test3D(DefaultTest):
    def test_cube_C3D8_1x1x1(self):
       self.default_test('Cube_C3D8_1x1x1')
 
    def test_cube_C3D8_2x2x2(self):
       self.default_test('Cube_C3D8_2x2x2')
    
    def test_cube_C3D20_1x1x1(self):
       self.default_test('Cube_C3D20_1x1x1')
 
    def test_cube_C3D20_2x2x2(self):
       self.default_test('Cube_C3D20_2x2x2')
 
    def test_complex_part_C3D20R(self):
       self.default_test('ComplexPart_C3D20R')
+
+
+class Test_dat_to_svg(DefaultTest):
+   def default_test(self, benchmark_name: str):
+      super().default_test('dat_to_svg/' + benchmark_name, '.dat', '.svg')
+
+   def test_circle_T3_Q4_4x4(self):
+      self.default_test('Circle_T3_Q4_4x4')
+
+   def test_heart_plate_Q8_2x2(self):
+      self.default_test('HeartPlate_Q8_2x2')
+
+   def test_heart_plate_BT2_2x2(self):
+      self.default_test('HeartPlate_BT2_2x2')
+
+   def test_heart_plate_BT3_4x4(self):
+      self.default_test('HeartPlate_BT3_4x4')
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic.pos` & `lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic.pos`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv` & `lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv` & `lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv` & `lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv` & `lmcv_tools-0.0.6/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate.pos` & `lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate.pos`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv` & `lmcv_tools-0.0.6/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp` & `lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp` & `lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp` & `lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/generate/virtual_laminas_exp_voight.inp` & `lmcv_tools-0.0.6/tests/benchmark/generate/virtual_laminas_exp_voight.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Circle_S3_S4R_4x4.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Circle_S3_S4R_4x4_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat`

 * *Files 2% similar despite different names*

```diff
@@ -34,32 +34,32 @@
 27   -8.88098329e-02   +2.58625090e-01   +0.00000000e+00
 
 %ELEMENT
 20
 
 %ELEMENT.PLSTRESS.T3
 1
-1   1  1   7   8   18
+1   1  1    7    8   18
 
 %ELEMENT.PLSTRESS.Q4
 19
-2    1  1   14   2   3   22
-3    1  1   6   17   23   5
+2    1  1   14    2    3   22
+3    1  1    6   17   23    5
 4    1  1   16   23   17   27
-5    1  1   8   9   24   18
+5    1  1    8    9   24   18
 6    1  1   21   27   17   18
-7    1  1   17   6   7   18
+7    1  1   17    6    7   18
 8    1  1   16   27   14   22
 9    1  1   19   21   18   24
 10   1  1   20   25   21   19
 11   1  1   20   11   12   25
-12   1  1   1   2   14   15
-13   1  1   26   13   1   15
-14   1  1   5   23   16   4
-15   1  1   9   10   19   24
+12   1  1    1    2   14   15
+13   1  1   26   13    1   15
+14   1  1    5   23   16    4
+15   1  1    9   10   19   24
 16   1  1   20   19   10   11
 17   1  1   13   26   25   12
 18   1  1   14   27   21   15
-19   1  1   4   16   22   3
+19   1  1    4   16   22    3
 20   1  1   25   26   15   21
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_C3D20R.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_C3D20R_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat`

 * *Files 11% similar despite different names*

```diff
@@ -686,70 +686,70 @@
 679   +1.46239185e+01   -4.00000000e+01   -3.33781385e+00
 
 %ELEMENT
 98
 
 %ELEMENT.BRICK20
 98
-1    1  1   40   210   15   204   14   209   39   205   208   201   203   206   29   212   4   202   21   211   46   207
-2    1  1   35   220   10   215   1   219   26   216   218   213   214   217   46   211   21   202   4   212   29   207
-3    1  1   42   227   17   223   10   220   35   224   226   221   213   218   50   228   25   222   21   211   46   225
-4    1  1   27   238   2   232   16   237   41   233   236   229   231   234   33   240   8   230   9   239   34   235
-5    1  1   35   220   10   242   16   237   41   243   216   215   232   233   26   219   1   241   2   238   27   244
-6    1  1   49   252   24   247   3   251   28   248   250   245   246   249   33   240   8   229   2   238   27   236
-7    1  1   30   259   5   255   3   251   28   256   258   253   247   248   31   260   6   254   24   252   49   257
-8    1  1   48   269   23   264   25   228   50   265   268   261   263   266   44   271   19   262   20   270   45   267
-9    1  1   37   281   12   275   18   280   43   276   279   272   274   277   38   283   13   273   22   282   47   278
-10   1  1   42   227   17   221   25   228   50   226   287   284   264   265   36   288   11   285   23   269   48   286
-11   1  1   46   211   21   203   14   209   39   206   225   222   289   290   50   228   25   263   20   270   45   266
-12   1  1   48   269   23   292   22   282   47   293   286   285   274   277   36   288   11   291   18   280   43   294
-13   1  1   48   269   23   261   19   271   44   268   293   292   295   296   47   282   22   273   13   283   38   278
-14   1  1   33   240   8   298   7   301   32   299   250   245   297   300   49   252   24   254   6   260   31   257
-15   1  1   65   307   40   205   39   306   64   302   305   208   206   303   54   309   29   207   46   308   71   304
-16   1  1   60   314   35   216   26   313   51   310   312   218   217   311   71   308   46   207   29   309   54   304
-17   1  1   67   318   42   224   35   314   60   315   317   226   218   312   75   319   50   225   46   308   71   316
-18   1  1   52   325   27   233   41   324   66   320   323   236   234   321   58   327   33   235   34   326   59   322
-19   1  1   60   314   35   243   41   324   66   328   310   216   233   320   51   313   26   244   27   325   52   329
-20   1  1   74   334   49   248   28   333   53   330   332   250   249   331   58   327   33   236   27   325   52   323
-21   1  1   55   338   30   256   28   333   53   335   337   258   248   330   56   339   31   257   49   334   74   336
-22   1  1   73   344   48   265   50   319   75   340   343   268   266   341   69   346   44   267   45   345   70   342
-23   1  1   62   352   37   276   43   351   68   347   350   279   277   348   63   354   38   278   47   353   72   349
-24   1  1   67   318   42   226   50   319   75   317   356   287   265   340   61   357   36   286   48   344   73   355
-25   1  1   71   308   46   206   39   306   64   303   316   225   290   358   75   319   50   266   45   345   70   341
-26   1  1   73   344   48   293   47   353   72   359   355   286   277   348   61   357   36   294   43   351   68   360
-27   1  1   73   344   48   268   44   346   69   343   359   293   296   361   72   353   47   278   38   354   63   349
-28   1  1   58   327   33   299   32   364   57   362   332   250   300   363   74   334   49   257   31   339   56   336
-29   1  1   90   370   65   302   64   369   89   365   368   305   303   366   79   372   54   304   71   371   96   367
-30   1  1   85   377   60   310   51   376   76   373   375   312   311   374   96   371   71   304   54   372   79   367
-31   1  1   92   381   67   315   60   377   85   378   380   317   312   375   100   382   75   316   71   371   96   379
-32   1  1   77   388   52   320   66   387   91   383   386   323   321   384   83   390   58   322   59   389   84   385
-33   1  1   85   377   60   328   66   387   91   391   373   310   320   383   76   376   51   329   52   388   77   392
-34   1  1   99   397   74   330   53   396   78   393   395   332   331   394   83   390   58   323   52   388   77   386
-35   1  1   80   401   55   335   53   396   78   398   400   337   330   393   81   402   56   336   74   397   99   399
-36   1  1   98   407   73   340   75   382   100   403   406   343   341   404   94   409   69   342   70   408   95   405
-37   1  1   87   415   62   347   68   414   93   410   413   350   348   411   88   417   63   349   72   416   97   412
-38   1  1   92   381   67   317   75   382   100   380   419   356   340   403   86   420   61   355   73   407   98   418
-39   1  1   96   371   71   303   64   369   89   366   379   316   358   421   100   382   75   341   70   408   95   404
-40   1  1   98   407   73   359   72   416   97   422   418   355   348   411   86   420   61   360   68   414   93   423
-41   1  1   98   407   73   343   69   409   94   406   422   359   361   424   97   416   72   349   63   417   88   412
-42   1  1   83   390   58   362   57   427   82   425   395   332   363   426   99   397   74   336   56   402   81   399
-43   1  1   115   433   90   365   89   432   114   428   431   368   366   429   104   435   79   367   96   434   121   430
-44   1  1   110   440   85   373   76   439   101   436   438   375   374   437   121   434   96   367   79   435   104   430
-45   1  1   117   444   92   378   85   440   110   441   443   380   375   438   125   445   100   379   96   434   121   442
-46   1  1   102   451   77   383   91   450   116   446   449   386   384   447   108   453   83   385   84   452   109   448
-47   1  1   110   440   85   391   91   450   116   454   436   373   383   446   101   439   76   392   77   451   102   455
-48   1  1   124   460   99   393   78   459   103   456   458   395   394   457   108   453   83   386   77   451   102   449
-49   1  1   105   464   80   398   78   459   103   461   463   400   393   456   106   465   81   399   99   460   124   462
-50   1  1   123   470   98   403   100   445   125   466   469   406   404   467   119   472   94   405   95   471   120   468
-51   1  1   112   478   87   410   93   477   118   473   476   413   411   474   113   480   88   412   97   479   122   475
-52   1  1   117   444   92   380   100   445   125   443   482   419   403   466   111   483   86   418   98   470   123   481
-53   1  1   121   434   96   366   89   432   114   429   442   379   421   484   125   445   100   404   95   471   120   467
-54   1  1   123   470   98   422   97   479   122   485   481   418   411   474   111   483   86   423   93   477   118   486
-55   1  1   123   470   98   406   94   472   119   469   485   422   424   487   122   479   97   412   88   480   113   475
-56   1  1   108   453   83   425   82   490   107   488   458   395   426   489   124   460   99   399   81   465   106   462
+1    1  1    40   210    15   204    14   209    39   205   208   201   203   206    29   212     4   202    21   211    46   207
+2    1  1    35   220    10   215     1   219    26   216   218   213   214   217    46   211    21   202     4   212    29   207
+3    1  1    42   227    17   223    10   220    35   224   226   221   213   218    50   228    25   222    21   211    46   225
+4    1  1    27   238     2   232    16   237    41   233   236   229   231   234    33   240     8   230     9   239    34   235
+5    1  1    35   220    10   242    16   237    41   243   216   215   232   233    26   219     1   241     2   238    27   244
+6    1  1    49   252    24   247     3   251    28   248   250   245   246   249    33   240     8   229     2   238    27   236
+7    1  1    30   259     5   255     3   251    28   256   258   253   247   248    31   260     6   254    24   252    49   257
+8    1  1    48   269    23   264    25   228    50   265   268   261   263   266    44   271    19   262    20   270    45   267
+9    1  1    37   281    12   275    18   280    43   276   279   272   274   277    38   283    13   273    22   282    47   278
+10   1  1    42   227    17   221    25   228    50   226   287   284   264   265    36   288    11   285    23   269    48   286
+11   1  1    46   211    21   203    14   209    39   206   225   222   289   290    50   228    25   263    20   270    45   266
+12   1  1    48   269    23   292    22   282    47   293   286   285   274   277    36   288    11   291    18   280    43   294
+13   1  1    48   269    23   261    19   271    44   268   293   292   295   296    47   282    22   273    13   283    38   278
+14   1  1    33   240     8   298     7   301    32   299   250   245   297   300    49   252    24   254     6   260    31   257
+15   1  1    65   307    40   205    39   306    64   302   305   208   206   303    54   309    29   207    46   308    71   304
+16   1  1    60   314    35   216    26   313    51   310   312   218   217   311    71   308    46   207    29   309    54   304
+17   1  1    67   318    42   224    35   314    60   315   317   226   218   312    75   319    50   225    46   308    71   316
+18   1  1    52   325    27   233    41   324    66   320   323   236   234   321    58   327    33   235    34   326    59   322
+19   1  1    60   314    35   243    41   324    66   328   310   216   233   320    51   313    26   244    27   325    52   329
+20   1  1    74   334    49   248    28   333    53   330   332   250   249   331    58   327    33   236    27   325    52   323
+21   1  1    55   338    30   256    28   333    53   335   337   258   248   330    56   339    31   257    49   334    74   336
+22   1  1    73   344    48   265    50   319    75   340   343   268   266   341    69   346    44   267    45   345    70   342
+23   1  1    62   352    37   276    43   351    68   347   350   279   277   348    63   354    38   278    47   353    72   349
+24   1  1    67   318    42   226    50   319    75   317   356   287   265   340    61   357    36   286    48   344    73   355
+25   1  1    71   308    46   206    39   306    64   303   316   225   290   358    75   319    50   266    45   345    70   341
+26   1  1    73   344    48   293    47   353    72   359   355   286   277   348    61   357    36   294    43   351    68   360
+27   1  1    73   344    48   268    44   346    69   343   359   293   296   361    72   353    47   278    38   354    63   349
+28   1  1    58   327    33   299    32   364    57   362   332   250   300   363    74   334    49   257    31   339    56   336
+29   1  1    90   370    65   302    64   369    89   365   368   305   303   366    79   372    54   304    71   371    96   367
+30   1  1    85   377    60   310    51   376    76   373   375   312   311   374    96   371    71   304    54   372    79   367
+31   1  1    92   381    67   315    60   377    85   378   380   317   312   375   100   382    75   316    71   371    96   379
+32   1  1    77   388    52   320    66   387    91   383   386   323   321   384    83   390    58   322    59   389    84   385
+33   1  1    85   377    60   328    66   387    91   391   373   310   320   383    76   376    51   329    52   388    77   392
+34   1  1    99   397    74   330    53   396    78   393   395   332   331   394    83   390    58   323    52   388    77   386
+35   1  1    80   401    55   335    53   396    78   398   400   337   330   393    81   402    56   336    74   397    99   399
+36   1  1    98   407    73   340    75   382   100   403   406   343   341   404    94   409    69   342    70   408    95   405
+37   1  1    87   415    62   347    68   414    93   410   413   350   348   411    88   417    63   349    72   416    97   412
+38   1  1    92   381    67   317    75   382   100   380   419   356   340   403    86   420    61   355    73   407    98   418
+39   1  1    96   371    71   303    64   369    89   366   379   316   358   421   100   382    75   341    70   408    95   404
+40   1  1    98   407    73   359    72   416    97   422   418   355   348   411    86   420    61   360    68   414    93   423
+41   1  1    98   407    73   343    69   409    94   406   422   359   361   424    97   416    72   349    63   417    88   412
+42   1  1    83   390    58   362    57   427    82   425   395   332   363   426    99   397    74   336    56   402    81   399
+43   1  1   115   433    90   365    89   432   114   428   431   368   366   429   104   435    79   367    96   434   121   430
+44   1  1   110   440    85   373    76   439   101   436   438   375   374   437   121   434    96   367    79   435   104   430
+45   1  1   117   444    92   378    85   440   110   441   443   380   375   438   125   445   100   379    96   434   121   442
+46   1  1   102   451    77   383    91   450   116   446   449   386   384   447   108   453    83   385    84   452   109   448
+47   1  1   110   440    85   391    91   450   116   454   436   373   383   446   101   439    76   392    77   451   102   455
+48   1  1   124   460    99   393    78   459   103   456   458   395   394   457   108   453    83   386    77   451   102   449
+49   1  1   105   464    80   398    78   459   103   461   463   400   393   456   106   465    81   399    99   460   124   462
+50   1  1   123   470    98   403   100   445   125   466   469   406   404   467   119   472    94   405    95   471   120   468
+51   1  1   112   478    87   410    93   477   118   473   476   413   411   474   113   480    88   412    97   479   122   475
+52   1  1   117   444    92   380   100   445   125   443   482   419   403   466   111   483    86   418    98   470   123   481
+53   1  1   121   434    96   366    89   432   114   429   442   379   421   484   125   445   100   404    95   471   120   467
+54   1  1   123   470    98   422    97   479   122   485   481   418   411   474   111   483    86   423    93   477   118   486
+55   1  1   123   470    98   406    94   472   119   469   485   422   424   487   122   479    97   412    88   480   113   475
+56   1  1   108   453    83   425    82   490   107   488   458   395   426   489   124   460    99   399    81   465   106   462
 57   1  1   140   496   115   428   114   495   139   491   494   431   429   492   129   498   104   430   121   497   146   493
 58   1  1   135   503   110   436   101   502   126   499   501   438   437   500   146   497   121   430   104   498   129   493
 59   1  1   142   507   117   441   110   503   135   504   506   443   438   501   150   508   125   442   121   497   146   505
 60   1  1   127   514   102   446   116   513   141   509   512   449   447   510   133   516   108   448   109   515   134   511
 61   1  1   135   503   110   454   116   513   141   517   499   436   446   509   126   502   101   455   102   514   127   518
 62   1  1   149   523   124   456   103   522   128   519   521   458   457   520   133   516   108   449   102   514   127   512
 63   1  1   130   527   105   461   103   522   128   524   526   463   456   519   131   528   106   462   124   523   149   525
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_S8R.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/ComplexPart_S8R_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat`

 * *Files 5% similar despite different names*

```diff
@@ -766,264 +766,264 @@
 759   +1.25000000e+01   -2.00000000e+01   +0.00000000e+00
 760   -1.25000000e+01   -2.00000000e+01   +0.00000000e+00
 761   +0.00000000e+00   -2.00000000e+01   +1.25000000e+01
 
 %ELEMENT
 253
 
-%ELEMENT.PLSTRESS.Q8
+%ELEMENT.SHALLOWSHELL.Q8
 253
-1     1  1   93   258   26   259   1   256   25   257
-2     1  1   94   262   93   257   25   260   24   261
-3     1  1   95   265   94   261   24   263   23   264
-4     1  1   96   268   95   264   23   266   22   267
-5     1  1   97   271   96   267   22   269   21   270
-6     1  1   98   274   97   270   21   272   20   273
-7     1  1   99   277   98   273   20   275   19   276
-8     1  1   100   280   99   276   19   278   18   279
-9     1  1   101   283   100   279   18   281   17   282
-10    1  1   102   286   101   282   17   284   16   285
-11    1  1   103   289   102   285   16   287   15   288
-12    1  1   104   292   103   288   15   290   14   291
-13    1  1   105   295   104   291   14   293   13   294
-14    1  1   106   298   105   294   13   296   12   297
-15    1  1   107   301   106   297   12   299   11   300
-16    1  1   26   303   107   300   11   302   1   259
-17    1  1   108   305   27   306   26   258   93   304
-18    1  1   109   308   108   304   93   262   94   307
-19    1  1   110   310   109   307   94   265   95   309
-20    1  1   111   312   110   309   95   268   96   311
-21    1  1   112   314   111   311   96   271   97   313
-22    1  1   113   316   112   313   97   274   98   315
-23    1  1   114   318   113   315   98   277   99   317
-24    1  1   115   320   114   317   99   280   100   319
+1     1  1    93   258    26   259     1   256    25   257
+2     1  1    94   262    93   257    25   260    24   261
+3     1  1    95   265    94   261    24   263    23   264
+4     1  1    96   268    95   264    23   266    22   267
+5     1  1    97   271    96   267    22   269    21   270
+6     1  1    98   274    97   270    21   272    20   273
+7     1  1    99   277    98   273    20   275    19   276
+8     1  1   100   280    99   276    19   278    18   279
+9     1  1   101   283   100   279    18   281    17   282
+10    1  1   102   286   101   282    17   284    16   285
+11    1  1   103   289   102   285    16   287    15   288
+12    1  1   104   292   103   288    15   290    14   291
+13    1  1   105   295   104   291    14   293    13   294
+14    1  1   106   298   105   294    13   296    12   297
+15    1  1   107   301   106   297    12   299    11   300
+16    1  1    26   303   107   300    11   302     1   259
+17    1  1   108   305    27   306    26   258    93   304
+18    1  1   109   308   108   304    93   262    94   307
+19    1  1   110   310   109   307    94   265    95   309
+20    1  1   111   312   110   309    95   268    96   311
+21    1  1   112   314   111   311    96   271    97   313
+22    1  1   113   316   112   313    97   274    98   315
+23    1  1   114   318   113   315    98   277    99   317
+24    1  1   115   320   114   317    99   280   100   319
 25    1  1   116   322   115   319   100   283   101   321
 26    1  1   117   324   116   321   101   286   102   323
 27    1  1   118   326   117   323   102   289   103   325
 28    1  1   119   328   118   325   103   292   104   327
 29    1  1   120   330   119   327   104   295   105   329
 30    1  1   121   332   120   329   105   298   106   331
 31    1  1   122   334   121   331   106   301   107   333
-32    1  1   27   335   122   333   107   303   26   306
-33    1  1   123   337   28   338   27   305   108   336
+32    1  1    27   335   122   333   107   303    26   306
+33    1  1   123   337    28   338    27   305   108   336
 34    1  1   124   340   123   336   108   308   109   339
 35    1  1   125   342   124   339   109   310   110   341
 36    1  1   126   344   125   341   110   312   111   343
 37    1  1   127   346   126   343   111   314   112   345
 38    1  1   128   348   127   345   112   316   113   347
 39    1  1   129   350   128   347   113   318   114   349
 40    1  1   130   352   129   349   114   320   115   351
 41    1  1   131   354   130   351   115   322   116   353
 42    1  1   132   356   131   353   116   324   117   355
 43    1  1   133   358   132   355   117   326   118   357
 44    1  1   134   360   133   357   118   328   119   359
 45    1  1   135   362   134   359   119   330   120   361
 46    1  1   136   364   135   361   120   332   121   363
 47    1  1   137   366   136   363   121   334   122   365
-48    1  1   28   367   137   365   122   335   27   338
-49    1  1   43   369   2   370   28   337   123   368
-50    1  1   42   372   43   368   123   340   124   371
-51    1  1   41   374   42   371   124   342   125   373
-52    1  1   40   376   41   373   125   344   126   375
-53    1  1   39   378   40   375   126   346   127   377
-54    1  1   38   380   39   377   127   348   128   379
-55    1  1   37   382   38   379   128   350   129   381
-56    1  1   36   384   37   381   129   352   130   383
-57    1  1   35   386   36   383   130   354   131   385
-58    1  1   34   388   35   385   131   356   132   387
-59    1  1   33   390   34   387   132   358   133   389
-60    1  1   32   392   33   389   133   360   134   391
-61    1  1   31   394   32   391   134   362   135   393
-62    1  1   30   396   31   393   135   364   136   395
-63    1  1   29   398   30   395   136   366   137   397
-64    1  1   2   399   29   397   137   367   28   370
-65    1  1   57   402   4   403   3   400   50   401
-66    1  1   56   406   57   401   50   404   49   405
-67    1  1   55   409   56   405   49   407   48   408
-68    1  1   54   412   55   408   48   410   47   411
-69    1  1   53   415   54   411   47   413   46   414
-70    1  1   52   418   53   414   46   416   45   417
-71    1  1   51   421   52   417   45   419   44   420
-72    1  1   4   423   51   420   44   422   3   403
-73    1  1   50   400   3   426   5   424   64   425
-74    1  1   49   404   50   425   64   427   63   428
-75    1  1   48   407   49   428   63   429   62   430
-76    1  1   47   410   48   430   62   431   61   432
-77    1  1   46   413   47   432   61   433   60   434
-78    1  1   45   416   46   434   60   435   59   436
-79    1  1   44   419   45   436   59   437   58   438
-80    1  1   3   422   44   438   58   439   5   426
-81    1  1   64   424   5   442   6   440   71   441
-82    1  1   63   427   64   441   71   443   70   444
-83    1  1   62   429   63   444   70   445   69   446
-84    1  1   61   431   62   446   69   447   68   448
-85    1  1   60   433   61   448   68   449   67   450
-86    1  1   59   435   60   450   67   451   66   452
-87    1  1   58   437   59   452   66   453   65   454
-88    1  1   5   439   58   454   65   455   6   442
-89    1  1   85   458   8   459   7   456   78   457
-90    1  1   84   462   85   457   78   460   77   461
-91    1  1   83   465   84   461   77   463   76   464
-92    1  1   82   468   83   464   76   466   75   467
-93    1  1   81   471   82   467   75   469   74   470
-94    1  1   80   474   81   470   74   472   73   473
-95    1  1   79   477   80   473   73   475   72   476
-96    1  1   8   479   79   476   72   478   7   459
+48    1  1    28   367   137   365   122   335    27   338
+49    1  1    43   369     2   370    28   337   123   368
+50    1  1    42   372    43   368   123   340   124   371
+51    1  1    41   374    42   371   124   342   125   373
+52    1  1    40   376    41   373   125   344   126   375
+53    1  1    39   378    40   375   126   346   127   377
+54    1  1    38   380    39   377   127   348   128   379
+55    1  1    37   382    38   379   128   350   129   381
+56    1  1    36   384    37   381   129   352   130   383
+57    1  1    35   386    36   383   130   354   131   385
+58    1  1    34   388    35   385   131   356   132   387
+59    1  1    33   390    34   387   132   358   133   389
+60    1  1    32   392    33   389   133   360   134   391
+61    1  1    31   394    32   391   134   362   135   393
+62    1  1    30   396    31   393   135   364   136   395
+63    1  1    29   398    30   395   136   366   137   397
+64    1  1     2   399    29   397   137   367    28   370
+65    1  1    57   402     4   403     3   400    50   401
+66    1  1    56   406    57   401    50   404    49   405
+67    1  1    55   409    56   405    49   407    48   408
+68    1  1    54   412    55   408    48   410    47   411
+69    1  1    53   415    54   411    47   413    46   414
+70    1  1    52   418    53   414    46   416    45   417
+71    1  1    51   421    52   417    45   419    44   420
+72    1  1     4   423    51   420    44   422     3   403
+73    1  1    50   400     3   426     5   424    64   425
+74    1  1    49   404    50   425    64   427    63   428
+75    1  1    48   407    49   428    63   429    62   430
+76    1  1    47   410    48   430    62   431    61   432
+77    1  1    46   413    47   432    61   433    60   434
+78    1  1    45   416    46   434    60   435    59   436
+79    1  1    44   419    45   436    59   437    58   438
+80    1  1     3   422    44   438    58   439     5   426
+81    1  1    64   424     5   442     6   440    71   441
+82    1  1    63   427    64   441    71   443    70   444
+83    1  1    62   429    63   444    70   445    69   446
+84    1  1    61   431    62   446    69   447    68   448
+85    1  1    60   433    61   448    68   449    67   450
+86    1  1    59   435    60   450    67   451    66   452
+87    1  1    58   437    59   452    66   453    65   454
+88    1  1     5   439    58   454    65   455     6   442
+89    1  1    85   458     8   459     7   456    78   457
+90    1  1    84   462    85   457    78   460    77   461
+91    1  1    83   465    84   461    77   463    76   464
+92    1  1    82   468    83   464    76   466    75   467
+93    1  1    81   471    82   467    75   469    74   470
+94    1  1    80   474    81   470    74   472    73   473
+95    1  1    79   477    80   473    73   475    72   476
+96    1  1     8   479    79   476    72   478     7   459
 97    1  1   147   482   146   483   148   480   161   481
-98    1  1   140   486   9   487   86   484   158   485
-99    1  1   157   490   43   372   42   488   138   489
-100   1  1   41   491   139   492   138   488   42   374
-101   1  1   39   494   141   495   143   493   40   378
-102   1  1   141   494   39   380   38   496   142   497
-103   1  1   142   496   38   382   37   498   144   499
-104   1  1   36   500   149   501   144   498   37   384
-105   1  1   35   502   146   503   149   500   36   386
-106   1  1   31   505   160   506   155   504   32   394
-107   1  1   30   507   153   508   160   505   31   396
+98    1  1   140   486     9   487    86   484   158   485
+99    1  1   157   490    43   372    42   488   138   489
+100   1  1    41   491   139   492   138   488    42   374
+101   1  1    39   494   141   495   143   493    40   378
+102   1  1   141   494    39   380    38   496   142   497
+103   1  1   142   496    38   382    37   498   144   499
+104   1  1    36   500   149   501   144   498    37   384
+105   1  1    35   502   146   503   149   500    36   386
+106   1  1    31   505   160   506   155   504    32   394
+107   1  1    30   507   153   508   160   505    31   396
 108   1  1   152   510   151   511   160   508   153   509
-109   1  1   156   514   29   399   2   512   87   513
-110   1  1   156   513   87   517   86   515   159   516
-111   1  1   143   518   139   491   41   376   40   493
-112   1  1   34   519   148   483   146   502   35   388
-113   1  1   32   504   155   521   150   520   33   392
-114   1  1   148   519   34   390   33   520   150   522
+109   1  1   156   514    29   399     2   512    87   513
+110   1  1   156   513    87   517    86   515   159   516
+111   1  1   143   518   139   491    41   376    40   493
+112   1  1    34   519   148   483   146   502    35   388
+113   1  1    32   504   155   521   150   520    33   392
+114   1  1   148   519    34   390    33   520   150   522
 115   1  1   139   518   143   524   140   485   158   523
-116   1  1   157   526   158   484   86   517   87   525
-117   1  1   157   525   87   512   2   369   43   490
+116   1  1   157   526   158   484    86   517    87   525
+117   1  1   157   525    87   512     2   369    43   490
 118   1  1   142   528   145   529   162   527   141   497
-119   1  1   145   531   9   486   140   530   162   529
+119   1  1   145   531     9   486   140   530   162   529
 120   1  1   143   495   141   527   162   530   140   524
-121   1  1   147   533   154   534   9   531   145   532
+121   1  1   147   533   154   534     9   531   145   532
 122   1  1   152   536   159   537   154   535   151   510
 123   1  1   154   533   147   481   161   538   151   535
 124   1  1   155   506   160   511   151   538   161   539
 125   1  1   153   540   156   516   159   536   152   509
-126   1  1   156   540   153   507   30   398   29   514
-127   1  1   154   537   159   515   86   487   9   534
+126   1  1   156   540   153   507    30   398    29   514
+127   1  1   154   537   159   515    86   487     9   534
 128   1  1   138   492   139   523   158   526   157   489
 129   1  1   150   521   155   539   161   480   148   522
 130   1  1   145   528   142   499   144   501   149   541
 131   1  1   147   532   145   541   149   503   146   482
 132   1  1   164   544   228   545   168   542   163   543
-133   1  1   171   548   170   549   90   546   91   547
+133   1  1   171   548   170   549    90   546    91   547
 134   1  1   172   552   169   553   170   550   173   551
-135   1  1   167   556   22   266   23   554   166   555
+135   1  1   167   556    22   266    23   554   166   555
 136   1  1   167   559   174   560   176   557   177   558
-137   1  1   228   562   88   563   89   561   168   545
-138   1  1   217   566   218   567   90   564   89   565
-139   1  1   225   570   173   571   220   568   56   569
+137   1  1   228   562    88   563    89   561   168   545
+138   1  1   217   566   218   567    90   564    89   565
+139   1  1   225   570   173   571   220   568    56   569
 140   1  1   173   570   225   573   184   572   172   551
 141   1  1   167   555   166   575   165   574   174   559
-142   1  1   20   272   21   578   177   576   227   577
-143   1  1   19   275   20   577   227   579   180   580
+142   1  1    20   272    21   578   177   576   227   577
+143   1  1    19   275    20   577   227   579   180   580
 144   1  1   200   583   197   584   198   581   201   582
 145   1  1   204   587   200   582   201   585   221   586
 146   1  1   202   590   194   591   193   588   199   589
-147   1  1   194   593   226   594   14   290   15   592
-148   1  1   193   591   194   592   15   287   16   595
-149   1  1   180   596   181   597   18   278   19   580
+147   1  1   194   593   226   594    14   290    15   592
+148   1  1   193   591   194   592    15   287    16   595
+149   1  1   180   596   181   597    18   278    19   580
 150   1  1   191   600   188   601   189   598   234   599
 151   1  1   229   604   198   605   234   602   223   603
-152   1  1   223   607   55   412   54   606   229   603
+152   1  1   223   607    55   412    54   606   229   603
 153   1  1   188   610   179   611   178   608   237   609
 154   1  1   179   613   190   614   181   596   180   612
 155   1  1   176   616   182   617   237   608   178   615
 156   1  1   236   620   203   621   199   618   196   619
-157   1  1   14   594   226   623   209   622   13   293
+157   1  1    14   594   226   623   209   622    13   293
 158   1  1   208   626   209   627   195   624   205   625
-159   1  1   210   629   217   565   89   563   88   628
-160   1  1   11   631   210   628   88   630   1   302
-161   1  1   12   632   207   633   210   631   11   299
+159   1  1   210   629   217   565    89   563    88   628
+160   1  1    11   631   210   628    88   630     1   302
+161   1  1    12   632   207   633   210   631    11   299
 162   1  1   204   636   232   637   206   634   203   635
 163   1  1   202   589   199   621   203   634   206   638
-164   1  1   52   421   51   641   222   639   231   640
+164   1  1    52   421    51   641   222   639   231   640
 165   1  1   204   586   221   643   224   642   232   636
-166   1  1   4   645   91   646   219   644   51   423
+166   1  1     4   645    91   646   219   644    51   423
 167   1  1   218   649   215   650   216   647   219   648
 168   1  1   211   653   215   654   214   651   208   652
 169   1  1   217   629   210   633   207   655   214   656
 170   1  1   207   657   209   626   208   651   214   655
-171   1  1   13   622   209   657   207   632   12   296
+171   1  1    13   622   209   657   207   632    12   296
 172   1  1   205   658   212   659   211   652   208   625
 173   1  1   206   661   233   662   205   624   195   660
-174   1  1   17   281   18   597   181   663   192   664
-175   1  1   22   556   167   558   177   578   21   269
-176   1  1   166   554   23   263   24   665   164   666
-177   1  1   164   665   24   260   25   667   228   544
-178   1  1   228   667   25   256   1   630   88   562
+174   1  1    17   281    18   597   181   663   192   664
+175   1  1    22   556   167   558   177   578    21   269
+176   1  1   166   554    23   263    24   665   164   666
+177   1  1   164   665    24   260    25   667   228   544
+178   1  1   228   667    25   256     1   630    88   562
 179   1  1   182   670   235   671   183   668   186   669
 180   1  1   187   673   230   674   186   668   183   672
 181   1  1   184   573   225   676   187   672   183   675
-182   1  1   90   549   170   677   168   561   89   564
+182   1  1    90   549   170   677   168   561    89   564
 183   1  1   163   542   168   677   170   553   169   678
 184   1  1   165   681   163   678   169   679   175   680
 185   1  1   166   666   164   543   163   681   165   575
 186   1  1   174   574   165   680   175   682   235   683
 187   1  1   173   550   170   548   171   684   220   571
 188   1  1   172   572   184   685   175   679   169   552
 189   1  1   182   616   176   560   174   683   235   670
 190   1  1   188   609   237   687   185   686   189   601
 191   1  1   237   617   182   669   186   688   185   687
 192   1  1   179   612   180   579   227   689   178   611
 193   1  1   188   600   191   690   190   613   179   610
 194   1  1   190   691   196   692   192   663   181   614
 195   1  1   186   674   230   693   189   686   185   688
 196   1  1   183   671   235   682   175   685   184   675
-197   1  1   225   569   56   409   55   694   187   676
+197   1  1   225   569    56   409    55   694   187   676
 198   1  1   198   584   197   695   191   599   234   605
 199   1  1   197   696   196   691   190   690   191   695
 200   1  1   200   697   236   619   196   696   197   583
 201   1  1   199   588   193   698   192   692   196   618
 202   1  1   215   653   211   659   212   699   216   650
-203   1  1   231   701   232   642   224   700   52   640
+203   1  1   231   701   232   642   224   700    52   640
 204   1  1   233   702   213   703   212   658   205   662
-205   1  1   16   284   17   664   192   698   193   595
+205   1  1    16   284    17   664   192   698   193   595
 206   1  1   202   638   206   660   195   704   194   590
-207   1  1   53   418   52   700   224   643   221   705
+207   1  1    53   418    52   700   224   643   221   705
 208   1  1   236   697   200   587   204   635   203   620
 209   1  1   213   706   222   707   216   699   212   703
 210   1  1   218   566   217   656   214   654   215   649
-211   1  1   219   647   216   707   222   641   51   644
-212   1  1   90   567   218   648   219   646   91   546
-213   1  1   57   708   171   547   91   645   4   402
-214   1  1   57   406   56   568   220   684   171   708
+211   1  1   219   647   216   707   222   641    51   644
+212   1  1    90   567   218   648   219   646    91   546
+213   1  1    57   708   171   547    91   645     4   402
+214   1  1    57   406    56   568   220   684   171   708
 215   1  1   229   709   221   585   201   581   198   604
-216   1  1   229   606   54   415   53   705   221   709
+216   1  1   229   606    54   415    53   705   221   709
 217   1  1   223   602   234   598   189   693   230   710
-218   1  1   223   710   230   673   187   694   55   607
+218   1  1   223   710   230   673   187   694    55   607
 219   1  1   226   593   194   704   195   627   209   623
 220   1  1   176   615   178   689   227   576   177   557
 221   1  1   222   706   213   702   233   711   231   639
 222   1  1   233   661   206   637   232   701   231   711
 223   1  1   239   714   246   715   242   712   238   713
-224   1  1   84   465   83   718   249   716   248   717
-225   1  1   70   443   71   721   242   719   240   720
-226   1  1   244   723   241   724   68   447   69   722
-227   1  1   251   726   249   718   83   468   82   725
+224   1  1    84   465    83   718   249   716   248   717
+225   1  1    70   443    71   721   242   719   240   720
+226   1  1   244   723   241   724    68   447    69   722
+227   1  1   251   726   249   718    83   468    82   725
 228   1  1   241   729   250   730   247   727   252   728
-229   1  1   92   733   8   458   85   731   243   732
-230   1  1   243   731   85   462   84   717   248   734
-231   1  1   79   479   8   733   92   735   245   736
-232   1  1   81   474   80   738   247   730   250   737
+229   1  1    92   733     8   458    85   731   243   732
+230   1  1   243   731    85   462    84   717   248   734
+231   1  1    79   479     8   733    92   735   245   736
+232   1  1    81   474    80   738   247   730   250   737
 233   1  1   252   727   247   741   245   739   253   740
-234   1  1   82   471   81   737   250   742   251   725
+234   1  1    82   471    81   737   250   742   251   725
 235   1  1   239   744   248   716   249   743   246   714
-236   1  1   71   440   6   745   238   712   242   721
-237   1  1   92   732   243   747   238   745   6   746
+236   1  1    71   440     6   745   238   712   242   721
+237   1  1    92   732   243   747   238   745     6   746
 238   1  1   248   744   239   713   238   747   243   734
-239   1  1   6   455   65   748   245   735   92   746
-240   1  1   69   445   70   720   240   749   244   722
-241   1  1   252   740   253   751   66   451   67   750
-242   1  1   241   728   252   750   67   449   68   724
+239   1  1     6   455    65   748   245   735    92   746
+240   1  1    69   445    70   720   240   749   244   722
+241   1  1   252   740   253   751    66   451    67   750
+242   1  1   241   728   252   750    67   449    68   724
 243   1  1   249   726   251   753   254   752   246   743
-244   1  1   245   741   247   738   80   477   79   736
+244   1  1   245   741   247   738    80   477    79   736
 245   1  1   246   752   254   754   240   719   242   715
 246   1  1   255   756   250   729   241   723   244   755
 247   1  1   251   742   250   756   255   757   254   753
-248   1  1   253   739   245   748   65   453   66   751
+248   1  1   253   739   245   748    65   453    66   751
 249   1  1   254   757   255   755   244   749   240   754
-250   1  1   78   456   7   759   10   758   77   460
-251   1  1   76   463   77   758   10   760   75   466
-252   1  1   10   761   73   472   74   469   75   760
-253   1  1   10   759   7   478   72   475   73   761
+250   1  1    78   456     7   759    10   758    77   460
+251   1  1    76   463    77   758    10   760    75   466
+252   1  1    10   761    73   472    74   469    75   760
+253   1  1    10   759     7   478    72   475    73   761
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_1x1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_1x1x1_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat`

 * *Files 7% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 20   +5.00000000e-01   +0.00000000e+00   +0.00000000e+00
 
 %ELEMENT
 1
 
 %ELEMENT.BRICK20
 1
-1   1  1   1   18   5   12   6   17   2   13   16   9   11   14   3   20   7   10   8   19   4   15
+1   1  1    1   18    5   12    6   17    2   13   16    9   11   14    3   20    7   10    8   19    4   15
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_2x2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D20_2x2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,17 @@
 81   +7.50000000e-01   +1.00000000e+00   +0.00000000e+00
 
 %ELEMENT
 8
 
 %ELEMENT.BRICK20
 8
-1   1  1   1   37   10   31   11   36   2   32   35   28   30   33   4   39   13   29   14   38   5   34
-2   1  1   2   36   11   42   12   46   3   43   33   30   41   44   5   38   14   40   15   47   6   45
-3   1  1   4   39   13   29   14   38   5   34   53   48   50   51   7   55   16   49   17   54   8   52
-4   1  1   5   38   14   40   15   47   6   45   51   50   57   58   8   54   17   56   18   60   9   59
+1   1  1    1   37   10   31   11   36    2   32   35   28   30   33    4   39   13   29   14   38    5   34
+2   1  1    2   36   11   42   12   46    3   43   33   30   41   44    5   38   14   40   15   47    6   45
+3   1  1    4   39   13   29   14   38    5   34   53   48   50   51    7   55   16   49   17   54    8   52
+4   1  1    5   38   14   40   15   47    6   45   51   50   57   58    8   54   17   56   18   60    9   59
 5   1  1   10   66   19   64   20   65   11   31   28   61   63   30   13   68   22   62   23   67   14   29
 6   1  1   11   65   20   71   21   72   12   42   30   63   70   41   14   67   23   69   24   73   15   40
 7   1  1   13   68   22   62   23   67   14   29   48   74   76   50   16   78   25   75   26   77   17   49
 8   1  1   14   67   23   69   24   73   15   40   50   76   80   57   17   77   26   79   27   81   18   56
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_1x1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_1x1x1_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_2x2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Cube_C3D8_2x2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 27   +1.00000000e+00   +1.00000000e+00   +0.00000000e+00
 
 %ELEMENT
 8
 
 %ELEMENT.BRICK8
 8
-1   1  1   1   10   11   2   4   13   14   5
-2   1  1   2   11   12   3   5   14   15   6
-3   1  1   4   13   14   5   7   16   17   8
-4   1  1   5   14   15   6   8   17   18   9
+1   1  1    1   10   11    2    4   13   14    5
+2   1  1    2   11   12    3    5   14   15    6
+3   1  1    4   13   14    5    7   16   17    8
+4   1  1    5   14   15    6    8   17   18    9
 5   1  1   10   19   20   11   13   22   23   14
 6   1  1   11   20   21   12   14   23   24   15
 7   1  1   13   22   23   14   16   25   26   17
 8   1  1   14   23   24   15   17   26   27   18
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S4_2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 7   +1.00000000e+00   +0.00000000e+00   +0.00000000e+00
 8   +5.00000000e-01   +0.00000000e+00   +0.00000000e+00
 9   +0.00000000e+00   +0.00000000e+00   +0.00000000e+00
 
 %ELEMENT
 4
 
-%ELEMENT.PLSTRESS.Q4
+%ELEMENT.SHALLOWSHELL.Q4
 4
 1   1  1   5   4   1   2
 2   1  1   6   5   2   3
 3   1  1   8   7   4   5
 4   1  1   9   8   5   6
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_1x1_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 6   +0.00000000e+00   +5.00000000e-01   +0.00000000e+00
 7   +5.00000000e-01   +0.00000000e+00   +0.00000000e+00
 8   +1.00000000e+00   +5.00000000e-01   +0.00000000e+00
 
 %ELEMENT
 1
 
-%ELEMENT.PLSTRESS.Q8
+%ELEMENT.SHALLOWSHELL.Q8
 1
 1   1  1   4   7   3   8   1   5   2   6
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Square_S8R_2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 19   +1.00000000e+00   +2.50000000e-01   +0.00000000e+00
 20   +0.00000000e+00   +2.50000000e-01   +0.00000000e+00
 21   +2.50000000e-01   +0.00000000e+00   +0.00000000e+00
 
 %ELEMENT
 4
 
-%ELEMENT.PLSTRESS.Q8
+%ELEMENT.SHALLOWSHELL.Q8
 4
-1   1  1   5   12   4   13   1   10   2   11
-2   1  1   6   16   5   11   2   14   3   15
-3   1  1   8   18   7   19   4   12   5   17
-4   1  1   9   21   8   17   5   16   6   20
+1   1  1    5   12    4   13    1   10    2   11
+2   1  1    6   16    5   11    2   14    3   15
+3   1  1    8   18    7   19    4   12    5   17
+4   1  1    9   21    8   17    5   16    6   20
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_S3_2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 4   +2.50000000e-01   +4.33012694e-01   +0.00000000e+00
 5   +5.00000000e-01   +0.00000000e+00   +0.00000000e+00
 6   +7.50000000e-01   +4.33012694e-01   +0.00000000e+00
 
 %ELEMENT
 4
 
-%ELEMENT.PLSTRESS.T3
+%ELEMENT.SHALLOWSHELL.T3
 4
 1   1  1   4   5   6
 2   1  1   2   5   4
 3   1  1   5   3   6
 4   1  1   1   4   6
 
 %END
```

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_1x1.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_2x2.inp` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/tests/benchmark/translate/Triangle_STRI65_2x2_exp.dat` & `lmcv_tools-0.0.6/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 13   +8.75000000e-01   +2.16506347e-01   +0.00000000e+00
 14   +6.25000000e-01   +6.49519026e-01   +0.00000000e+00
 15   +3.75000000e-01   +6.49519026e-01   +0.00000000e+00
 
 %ELEMENT
 4
 
-%ELEMENT.PLSTRESS.T6
+%ELEMENT.SHALLOWSHELL.T6
 4
-1   1  1   4   8   5   9   6   7
-2   1  1   2   11   5   8   4   10
-3   1  1   5   12   3   13   6   9
-4   1  1   1   15   4   7   6   14
+1   1  1    4    8    5    9    6    7
+2   1  1    2   11    5    8    4   10
+3   1  1    5   12    3   13    6    9
+4   1  1    1   15    4    7    6   14
 
 %END
```

### Comparing `lmcv_tools-0.0.5/LICENSE` & `lmcv_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.5/README.md` & `lmcv_tools-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,28 +52,38 @@
 Considering that the routine activities for which LMCV Tools was developed are quite varied, specific commands were developed for each one of them. These commands are:
 - translate (in implementation)
 - extract (in implementation)
 - generate (in implementation)
 
 ### 2.1 - Translate
 
-The command **translate**, in short, aims to convert .inp files created by Abaqus in .dat files for FAST.
-
-Abaqus is a suite for Finite Element Analysis (FEA) developed by "Dassault Systèmes", while FAST is a console based FEA tool developed by "Laboratório de Mecânica Computacional e Visualização" of "Universidade Federal do Ceará" (UFC). Both of these softwares can simulate complex problems, but FAST has a clear disadvantage: differently of Abaqus, it hasn't a native GUI to generate its meshes. With that in mind, this command specifically seeks to translate meshes generated in Abaqus and exported in .inp format into meshes in .dat format to be used in FAST simulations.
+The command **translate**, in short, aims to convert different types of files used in LMCV.
 
 Its usage is quite simple:
 
 ```text
-$ lmcv_tools translate [relative path to .inp file]
+$ lmcv_tools translate [path/to/file] to [extension]
 ```
 
-If you need to specify the .dat output path, another possible way is:
+### 2.1.1 - Translate .inp to .dat
+
+Abaqus is a suite for Finite Element Analysis (FEA) developed by "Dassault Systèmes", while FAST is a console based FEA tool developed by "Laboratório de Mecânica Computacional e Visualização" of "Universidade Federal do Ceará" (UFC). Both of these softwares can simulate complex problems, but FAST has a clear disadvantage: differently of Abaqus, it hasn't a native GUI to generate its meshes. With that in mind, this command specifically seeks to translate meshes generated in Abaqus and exported in .inp format into meshes in .dat format to be used in FAST simulations.
+
+Example:
+```text
+$ lmcv_tools translate Job-1.inp to .dat
+```
+
+### 2.1.2 - Translate .dat to .svg
+
+Articles for scientific publications in the LMCV study field generally require images of the used meshes. Generating bitmat images in PNG format is a valid possibility, but for very discretized meshes this approach results in loss of details. Thinking about it, this command translates .dat files of 2D meshes to the SVG (Scalable Vector Graphics) image format, which does not lose quality with zoom (perfect for meshes with many elements).
 
+Example:
 ```text
-$ lmcv_tools translate [relative path to .inp file] [relative path to .dat file]
+$ lmcv_tools translate Plate.dat to .svg
 ```
 
 ### 2.2 - Extract
 
 The command **extract**, in short, aims to extract data from .pos files generate by FAST and save this data in CSV format).
 
 Files with extension ".pos" are the standard output from FAST simulations. They can store data about nodal displacements, element stresses, gauss points stresses and other informations, all distributed over a series of steps. In some contexts, it is necessary to obtain specific data from these files, but the manual search can take a lot of time and still fail. Alternatively, this command allows to extract entire set of related atributes by a simple expression.
```

### Comparing `lmcv_tools-0.0.5/pyproject.toml` & `lmcv_tools-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lmcv_tools"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name = "Dev-Gabriel-Braga", email = "gabriel.braga.matos@gmail.com" },
 ]
 description = "Command line tool that provides useful functionalities to LMCV Members"
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = ">=3.9"
@@ -20,12 +20,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering"
 ]
 
+[project.urls]
+repository = "https://github.com/Dev-Gabriel-Braga/lmcv_tools"
+
 [project.scripts]
 lmcv_tools = "lmcv_tools.__main__:main"
 
 [tool.hatch.build.targets.wheel]
 packages = ["lmcv_tools"]
```

### Comparing `lmcv_tools-0.0.5/PKG-INFO` & `lmcv_tools-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: lmcv_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool that provides useful functionalities to LMCV Members
+Project-URL: repository, https://github.com/Dev-Gabriel-Braga/lmcv_tools
 Author-email: Dev-Gabriel-Braga <gabriel.braga.matos@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -70,28 +71,38 @@
 Considering that the routine activities for which LMCV Tools was developed are quite varied, specific commands were developed for each one of them. These commands are:
 - translate (in implementation)
 - extract (in implementation)
 - generate (in implementation)
 
 ### 2.1 - Translate
 
-The command **translate**, in short, aims to convert .inp files created by Abaqus in .dat files for FAST.
-
-Abaqus is a suite for Finite Element Analysis (FEA) developed by "Dassault Systèmes", while FAST is a console based FEA tool developed by "Laboratório de Mecânica Computacional e Visualização" of "Universidade Federal do Ceará" (UFC). Both of these softwares can simulate complex problems, but FAST has a clear disadvantage: differently of Abaqus, it hasn't a native GUI to generate its meshes. With that in mind, this command specifically seeks to translate meshes generated in Abaqus and exported in .inp format into meshes in .dat format to be used in FAST simulations.
+The command **translate**, in short, aims to convert different types of files used in LMCV.
 
 Its usage is quite simple:
 
 ```text
-$ lmcv_tools translate [relative path to .inp file]
+$ lmcv_tools translate [path/to/file] to [extension]
 ```
 
-If you need to specify the .dat output path, another possible way is:
+### 2.1.1 - Translate .inp to .dat
+
+Abaqus is a suite for Finite Element Analysis (FEA) developed by "Dassault Systèmes", while FAST is a console based FEA tool developed by "Laboratório de Mecânica Computacional e Visualização" of "Universidade Federal do Ceará" (UFC). Both of these softwares can simulate complex problems, but FAST has a clear disadvantage: differently of Abaqus, it hasn't a native GUI to generate its meshes. With that in mind, this command specifically seeks to translate meshes generated in Abaqus and exported in .inp format into meshes in .dat format to be used in FAST simulations.
+
+Example:
+```text
+$ lmcv_tools translate Job-1.inp to .dat
+```
+
+### 2.1.2 - Translate .dat to .svg
+
+Articles for scientific publications in the LMCV study field generally require images of the used meshes. Generating bitmat images in PNG format is a valid possibility, but for very discretized meshes this approach results in loss of details. Thinking about it, this command translates .dat files of 2D meshes to the SVG (Scalable Vector Graphics) image format, which does not lose quality with zoom (perfect for meshes with many elements).
 
+Example:
 ```text
-$ lmcv_tools translate [relative path to .inp file] [relative path to .dat file]
+$ lmcv_tools translate Plate.dat to .svg
 ```
 
 ### 2.2 - Extract
 
 The command **extract**, in short, aims to extract data from .pos files generate by FAST and save this data in CSV format).
 
 Files with extension ".pos" are the standard output from FAST simulations. They can store data about nodal displacements, element stresses, gauss points stresses and other informations, all distributed over a series of steps. In some contexts, it is necessary to obtain specific data from these files, but the manual search can take a lot of time and still fail. Alternatively, this command allows to extract entire set of related atributes by a simple expression.
```


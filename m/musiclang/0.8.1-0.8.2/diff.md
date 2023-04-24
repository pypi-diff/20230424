# Comparing `tmp/musiclang-0.8.1.tar.gz` & `tmp/musiclang-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclang-0.8.1.tar", last modified: Sat Feb 11 13:43:11 2023, max compression
+gzip compressed data, was "musiclang-0.8.2.tar", last modified: Mon Apr 24 08:43:15 2023, max compression
```

## Comparing `musiclang-0.8.1.tar` & `musiclang-0.8.2.tar`

### file list

```diff
@@ -1,161 +1,213 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-02-11 13:43:08.000000 musiclang-0.8.1/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3961 2023-02-11 13:43:11.446517 musiclang-0.8.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2607 2023-02-11 13:43:08.000000 musiclang-0.8.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.434517 musiclang-0.8.1/musiclang/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.434517 musiclang-0.8.1/musiclang/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/analyze/augmented_net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/chord_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/feature_representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9175 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/inference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/input_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/keydistance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/output_representations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/score_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/augmented_net/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/midi_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9663 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8501 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/to_musiclang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/analyze/voice_separation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/library.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/predict/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/predict/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/predict/predictors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/predict/predictors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/predict/predictors/windowed.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/predict/tokenizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/predict/tokenizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/predict/tokenizers/chord_tokenizer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/base_transformer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/transform/chord/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/chord/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/chord/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/transform/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/composing/arrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11207 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/composing/counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14178 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/composing/project.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/transform/features/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/features/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/features/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.438517 musiclang-0.8.1/musiclang/transform/generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/generators/rythm_generator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/mask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/transform/melody/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/melody/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/melody/basics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/merger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/transform/note/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/note/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/note/basics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/transform/score/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/score/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/score/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/transform/score_merger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/score_merger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/score_merger/basics.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/transform/structure_graphs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/structure_graphs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/structure_graphs/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/transformer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/transform/utils_random.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/arrange_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/arrange_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/arrange_utils/arrange_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/arrange_utils/skyline_algorithm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32697 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13514 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/element.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12067 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/library.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8767 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19641 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      805 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/note_pitch.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9674 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/midi_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/to_code.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4282 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/to_midi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9129 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/out/to_mxl.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5034 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/pitches/pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6848 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/properties/note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.442517 musiclang-0.8.1/musiclang/write/rhythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/rhythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12519 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/rhythm/metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/rhythm/utils_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21375 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/score.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/musiclang/write/sequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/sequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/sequence/sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/sequence/sequence_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/musiclang/write/time_utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/time_utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/time_utils/time_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9026 2023-02-11 13:43:08.000000 musiclang-0.8.1/musiclang/write/tonality.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.434517 musiclang-0.8.1/musiclang.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3961 2023-02-11 13:43:11.000000 musiclang-0.8.1/musiclang.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4320 2023-02-11 13:43:11.000000 musiclang-0.8.1/musiclang.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-11 13:43:11.000000 musiclang-0.8.1/musiclang.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-02-11 13:43:11.000000 musiclang-0.8.1/musiclang.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-02-11 13:43:11.000000 musiclang-0.8.1/musiclang.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-02-11 13:43:09.000000 musiclang-0.8.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-02-11 13:43:11.450517 musiclang-0.8.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2023-02-11 13:43:09.000000 musiclang-0.8.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/analyze/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/analyze/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/analyze/test_analyze.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/composing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/composing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/composing/test_counterpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/composing/test_project.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/transform/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/test_mask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/test_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/test_transform_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/transform/test_transforms.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/write/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/write/out/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/out/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3465 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/out/test_to_midi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/write/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/pitches/test_pitches_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/write/properties/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/properties/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/properties/test_note_properties.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:11.446517 musiclang-0.8.1/tests/write/rythm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/rythm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/rythm/test_metric.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_absolute_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_bass_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1317 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_chord.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_chord_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_drum_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_extensions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_melody.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3174 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_score.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-02-11 13:43:08.000000 musiclang-0.8.1/tests/write/test_tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1302 2023-04-24 08:43:11.000000 musiclang-0.8.2/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5238 2023-04-24 08:43:15.869644 musiclang-0.8.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3620 2023-04-24 08:43:11.000000 musiclang-0.8.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.841644 musiclang-0.8.2/musiclang/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.845644 musiclang-0.8.2/musiclang/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/analyze/augmented_net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5042 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    69481 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/chord_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4367 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/feature_representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8996 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/inference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18747 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/input_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/keydistance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6149 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/output_representations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6283 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/score_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2667 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/augmented_net/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7290 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2887 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/midi_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12879 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15745 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/pattern_analyzer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/pattern_sampler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10479 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/roman_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10759 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/score_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11992 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/score_formatter_elements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8592 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/to_musiclang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8870 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/analyze/voice_separation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/library.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/arranger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8579 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/arranger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/arranger/arranger_trainer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/composer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       39 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6139 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/auto_composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/composer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/composer/harmony.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/predictors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/huggin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7398 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/predictors/windowed.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.849644 musiclang-0.8.2/musiclang/predict/tokenizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/tokenizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2644 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/predict/tokenizers/chord_tokenizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.853644 musiclang-0.8.2/musiclang/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7925 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/base_transformer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.853644 musiclang-0.8.2/musiclang/transform/chord/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/chord/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/chord/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/arrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11465 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6105 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6234 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1680 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/patternator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13358 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18038 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/composing/voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/dynamics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       37 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/dynamics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/dynamics/dynamizer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/features/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/features/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/features/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/generators/rythm_generator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4258 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19220 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/mask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/melody/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4570 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/basics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/continuation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/melody/filler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/merger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/note/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/note/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/note/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/orchestrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/epic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/orchestrations/nocturne.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.857644 musiclang-0.8.2/musiclang/transform/score/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/transform/score_merger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score_merger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/score_merger/basics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/transform/structure_graphs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/structure_graphs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/structure_graphs/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/transformer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/transform/utils_random.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/arrange_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4580 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/arrange_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2174 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/arrange_utils/skyline_algorithm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40204 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13534 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/element.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.861644 musiclang-0.8.2/musiclang/write/elements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/bar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/beat.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/element.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/free_text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/rhythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/time_signature.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/tonality.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/voice_leading.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/elements/voicing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13661 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/library.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14137 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26909 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/note_pitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8464 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/ornementation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12085 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/midi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3540 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_code.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8425 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_midi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12321 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/out/to_mxl.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5393 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/pitches/pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6890 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/properties/note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/rhythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14944 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/score_rythm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/rhythm/utils_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32073 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/score.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/sequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4656 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/sequence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12288 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/sequence/sequence_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/musiclang/write/time_utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/time_utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5584 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/time_utils/time_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9483 2023-04-24 08:43:11.000000 musiclang-0.8.2/musiclang/write/tonality.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.841644 musiclang-0.8.2/musiclang.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5238 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6111 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-24 08:43:15.000000 musiclang-0.8.2/musiclang.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-04-24 08:43:13.000000 musiclang-0.8.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-24 08:43:15.869644 musiclang-0.8.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2023-04-24 08:43:13.000000 musiclang-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/analyze/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/test_analyze.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8605 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/analyze/test_score_formatter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/composing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_counterpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1920 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/composing/test_voice_leading.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/predict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/predict/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1951 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/predict/test_auto_composer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.865645 musiclang-0.8.2/tests/transform/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2557 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_mask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transform_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/transform/test_transforms.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/out/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/out/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3633 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/out/test_to_midi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/pitches/test_pitches_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/properties/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/properties/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/properties/test_note_properties.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:15.869644 musiclang-0.8.2/tests/write/rythm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/rythm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/rythm/test_metric.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      324 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_absolute_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_bass_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chord.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chord_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_chromatic_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_drum_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3164 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_extensions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_melody.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5540 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_score.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2485 2023-04-24 08:43:11.000000 musiclang-0.8.2/tests/write/test_tonality.py
```

### Comparing `musiclang-0.8.1/LICENSE.md` & `musiclang-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/PKG-INFO` & `musiclang-0.8.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,121 @@
-Metadata-Version: 2.1
-Name: musiclang
-Version: 0.8.1
-Summary: A python package for music notation and generation
-Home-page: UNKNOWN
-Author: Florian GARDIN
-Author-email: fgardin.pro@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://musiclang.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/MusicLang/musiclang/
-Project-URL: Tracker, https://github.com/MusicLang/musiclang/issues
-Description: Musiclang
-        =========
-        
-        ![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
-        
-        
-        [![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
-        
-        The Python framework to write, analyze, transform and predict music.
-        
-        
-        What is MusicLang ?
-        --------------------
-        
-        MusicLang which simply stands for "music language" is a Python framework
-        that allows composers to write symbolic music in a condensed and high level manner.
-        The way one write music with this tool should be close to how one create music
-        in practice. This framework is not only another notation software but also
-        an assistant that is able to automate some tasks that would normally be tedious for a composer.
-        It is naturally good at analyzing and manipulating existing
-        pieces of music in musicxml or midi format.
-        
-        [Read our documentation](https://musiclang.readthedocs.io/en/latest).
-        
-        
-        How to install
-        --------------
-        
-        MusicLang is available on Pypi :
-        
-        ```
-        pip install musiclang
-        ```
-        
-        Or use this repo for the latest version :
-        
-        ```
-        pip install git+https://github.com/MusicLang/musiclang
-        ```
-            
-        
-        Examples
-        ---------
-        
-        1. A hello world example to create a C-major chord in musiclang and save it to midi :
-        
-        ```python
-        from musiclang.library import *
-        
-        # Write A C major chord
-        score = (I % I.M)(piano=[s0, s2, s4])
-        
-        # Store it to midi
-        score.to_midi('c_major.mid')
-        ```
-        
-        2. Create, transform and harmonize a theme quickly : 
-        
-        ```python
-        from musiclang.library import *
-        
-        # Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
-        melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
-        
-        # Create a simple accompaniment with a cello and a oboe
-        acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
-        accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
-        
-        # Play it in F-major
-        score = (I % IV.M)(violin__0=melody, **accomp)
-        
-        # Repeat the score a second time in F-minor and forte
-        score += (score % I.m).f
-        
-        # Just to create an anachrusis at the first bar
-        score = (I % I.M)(violin__0=r.h) + score
-        
-        # Transform a bit the accompaniment by applying counterpoint rules automatically
-        from musiclang.transform.library import create_counterpoint_on_score
-        score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
-        
-        # Save it to musicxml
-        score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
-        
-        # Et voilà !
-        ```
-        
-        ![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Musiclang
+=========
+
+![MusicLang logo](https://github.com/MusicLang/musiclang/blob/main/documentation/images/MusicLang.png?raw=true "MusicLang")
+
+
+[![Documentation Status](https://readthedocs.org/projects/musiclang/badge/?version=latest)](https://musiclang.readthedocs.io/en/latest/?badge=latest)
+
+The Python framework to write, analyze, transform and predict music.
+
+
+What is MusicLang ?
+--------------------
+
+MusicLang which simply stands for "music language" is a Python framework
+that allows composers to write symbolic music in a condensed and high level manner.
+It can be used to write, arrange, transform or predict new music.
+This framework is not only another notation software but also
+an assistant that is able to automate some tasks that would normally be tedious for a composer.
+It is naturally good at analyzing and manipulating existing
+pieces of music in musicxml or midi format.
+
+[Read our documentation](https://musiclang.readthedocs.io/en/latest).
+
+
+How to install
+--------------
+
+MusicLang is available on Pypi :
+
+```
+pip install musiclang
+```
+
+Or use this repo for the latest version :
+
+```
+pip install git+https://github.com/MusicLang/musiclang
+```
+    
+
+Examples
+---------
+
+1. A hello world example to create a C-major chord in musiclang and save it to midi :
+
+```python
+from musiclang.library import *
+
+# Write A C major chord
+score = (I % I.M)(piano=[s0, s2, s4])
+
+# Store it to midi
+score.to_midi('c_major.mid')
+```
+
+2. Create, transform and harmonize a theme quickly : 
+
+```python
+from musiclang.library import *
+
+# Create a cool melody (the beginning of happy birthday, independant of any harmonic context)
+melody = s4.ed + s4.s + s5 + s4 + s0.o(1) + s6.h
+
+# Create a simple accompaniment with a cello and a oboe
+acc_melody = r + s0.o(-1).q * 3 + s0.o(-1).h
+accomp = {'cello__0': acc_melody, 'oboe__0': acc_melody.o(1)}
+
+# Play it in F-major
+score = (I % IV.M)(violin__0=melody, **accomp)
+
+# Repeat the score a second time in F-minor and forte
+score += (score % I.m).f
+
+# Just to create an anachrusis at the first bar
+score = (I % I.M)(violin__0=r.h) + score
+
+# Transform a bit the accompaniment by applying counterpoint rules automatically
+from musiclang.transform.library import create_counterpoint_on_score
+score = create_counterpoint_on_score(score, fixed_parts=['violin__0'])
+
+# Save it to musicxml
+score.to_musicxml('happy_birthday.musicxml', signature=(3, 4), title='Happy birthday !')
+
+# Et voilà !
+```
+![Happy birthday score](https://github.com/MusicLang/musiclang/blob/main/documentation/images/happy_birthday.png?raw=true "Happy Birthday")
+
+
+3. Predict a score using a deep learning model trained on musiclang language :
+
+```python
+from musiclang.library import *
+from musiclang import Score
+
+# Some random bar of chopin op18 Waltz
+score = ((V % III.b.M)(
+	piano__0=s0 + s2.e.mp + s3.e.mp, 
+	piano__4=s0.e.o(-2).p + r.e + s0.ed.o(-1).mp + r.s, 
+	piano__5=r + s4.ed.o(-1).mp + r.s, 
+	piano__6=r + s6.ed.o(-1).mp + r.s)+ 
+(V['7'] % III.b.M)(
+	piano__0=s2.ed.mp + r.s, 
+	piano__2=s4.ed.mp + r.s, 
+	piano__4=s6.ed.o(-1).mp + r.s, 
+	piano__5=s0.ed.o(-1).mp + r.s, 
+	piano__6=s4.ed.o(-1).mp + r.s))
+
+# Predict a continuation of the score using hugginface musiclang model
+predicted_score = score.predict_score()
+# Save it to midi
+predicted_score.to_midi('test.mid')
+```
+
+Please note that this feature is still experimental, it will only work with
+piano music for now and the model is not yet trained on a large corpus of music.
+If you want to help us train a better model, please contact [us](mailto:fgardin.pro@gmail.com)
+
+
+4. Mix everything together to create a new pieces of music !
+
```

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/cache.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/cache.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/chord_vocabulary.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/chord_vocabulary.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/feature_representation.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/feature_representation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/inference.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/inference.py`

 * *Files 7% similar despite different names*

```diff
@@ -309,19 +309,15 @@
             prevkey = thiskey
         else:
             rn2fig = rn2
         bass.addLyric(formatRomanNumeral(rn2fig, thiskey))
         bass.addLyric(formatChordLabel(chordLabel))
     rntxt = generateRomanText(schord, ts)
     filename, _ = inputPath.rsplit(".", 1)
-    annotatedScore = f"{filename}_annotated.musicxml"
-    annotationCSV = f"{filename}_annotated.csv"
     annotatedRomanText = f"{filename}_annotated.rntxt"
-    schord.stream().write(fp=annotatedScore)
-    dfout.to_csv(annotationCSV)
     with open(annotatedRomanText, "w") as fd:
         fd.write(rntxt)
 
 
 def infer_chords(inputPath, useGpu=False):
     """
```

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/input_representations.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/input_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/keydistance.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/keydistance.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/models.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/models.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/output_representations.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/output_representations.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/score_parser.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/score_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/augmented_net/utils.py` & `musiclang-0.8.2/musiclang/analyze/augmented_net/utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/item.py` & `musiclang-0.8.2/musiclang/analyze/item.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/midi_parser.py` & `musiclang-0.8.2/musiclang/analyze/midi_parser.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/analyze/parser.py` & `musiclang-0.8.2/musiclang/analyze/roman_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,238 +1,121 @@
-"""
-Copyright (c) 2023, Florian GARDIN
-All rights reserved.
-
-This source code is licensed under the BSD-style license found in the
-LICENSE file in the root directory of this source tree.
-"""
-
-"""
-This file groups a set of functions to parse files into MusicLang objects
-"""
-
-def parse_to_musiclang(input_file: str):
-    """Parse an input file into a musiclang Score
-    - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
-    - Get voice separation and parsing
+import music21
+import re
+import numpy as np
+from .constants import DICT_RELATIVE_CHANGE, DICT_TONALITY, EXTENSION_REPLACER, DEGREE_REGEX
 
-    Parameters
-    ----------
-    input_file : str
-        Input filepath
-        
-    Returns
-    -------
-    score: musiclang.Score
-        Parsed score
-
-    config: dict
-        Dict of score configuration
-
-    """
-    extension = input_file.split('.')[-1]
-    if extension in ['mid', 'midi']:
-        return parse_midi_to_musiclang(input_file)
-    elif extension in ['mxl', 'xml', 'musicxml', 'krn']:
-        return parse_mxl_to_musiclang(input_file)
-    else:
-        raise Exception('Unknown extension {}'.format(extension))
-
-def parse_midi_to_musiclang(input_file: str):
-    """Parse a midi input file into a musiclang Score
-    - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
-    - Get voice separation and parsing
-
-    Parameters
-    ----------
-    input_file : str
-        Input midi filepath
-
-    Returns
-    -------
-    score: musiclang.Score
-        Parsed score
 
-    config: dict
-     Dict of score configuration
 
+def annotation_to_musiclang(text):
     """
-    import tempfile
-    import os
-    import shutil
-    from .augmented_net import m21Parse
-    with tempfile.TemporaryDirectory() as di:
-        midi_file = os.path.join(di, 'data.mid')
-        mxl_file = os.path.join(di, 'data.mxl')
-        obj = m21Parse(input_file, remove_perc=True)
-        obj.write('musicxml', fp=os.path.join(di, mxl_file))
-        shutil.copy(input_file, midi_file)
-        result = parse_directory_to_musiclang(di)
-    return result
-
-
-def parse_mxl_to_musiclang(input_file: str):
-    """Parse a music xml input file into a musiclang Score
-    - Get chords with the AugmentedNet (https://github.com/napulen/AugmentedNet)
-    - Separate into monophonic voice with the proper instrument
+    Parse an annotation file or string to musiclang chords with proper durations
 
     Parameters
     ----------
-    input_file: str :
-            Filepath of the input
-
-    Returns
-    -------
-    score : musiclang.Score
-
-    config: dict
-        Dict of score configuration
-
-    """
-
-    import tempfile
-    import os
-    import music21
-    import shutil
-    from .augmented_net import m21Parse
-    with tempfile.TemporaryDirectory() as di:
-        midi_file = os.path.join(di, 'data.mid')
-        mxl_file = os.path.join(di, 'data.mxl')
-        obj = m21Parse(input_file)
-        obj.write('midi', fp=os.path.join(di, midi_file))
-        shutil.copy(input_file, mxl_file)
-        result = parse_directory_to_musiclang(di)
-    return result
-
-def parse_directory_to_musiclang(directory: str):
-    """Parse a directory containing a 'data.mid' and 'data_annotated.rntxt' file (midi file and chord annotation file)
-
-    Parameters
-    ----------
-    directory : str
-        Directory with a "data.mid" file and a "data_annotated.rntxt" annotation file
+    text: str
+        Filepath or annotation to parse
 
     Returns
     -------
     score: Score
-        MusicLang score parsed
-
-    config: dict
-        Dict of score configuration
+        MusicLang score
 
     """
-    import os
-    from .augmented_net import infer_chords
-    print('1/2 : Analyze the score (This may takes a while)')
-    annotation_file = os.path.join(directory, 'data_annotated.rntxt')
-    midi_file = os.path.join(directory, 'data.mid')
-    mxl_file = os.path.join(directory, 'data.mxl')
-    infer_chords(mxl_file)
-    score, tempo = parse_midi_to_musiclang_with_annotation(midi_file, annotation_file)
-    annotation = open(annotation_file, 'r').read()
-    return score, {'annotation': annotation, 'tempo': tempo}
-
-
+    from .parser import chords_to_musiclang
+    print(text)
+    chords = analyze_roman_notation(text)
+    score = chords_to_musiclang(chords)
+    return score
 
 
-def parse_midi_to_musiclang_with_annotation(midi_file: str, annotation_file: str):
+def analyze_roman_notation(text):
     """
+    Given a text or a string representing a roman annotation, extract informations
 
     Parameters
     ----------
-    midi_file: str :
-        Filepath to the midi file to parse
-        
-    annotation_file: str :
-        Filepath to the anotation file to parse
-        
+    text: str
+        Filepath or annotation string to parse
 
     Returns
     -------
-    score: Score
-        MusicLang score parsed
 
-    tempo: int
-        Tempo of the score
 
     """
 
-    chords = get_chords_from_analysis(annotation_file)
-    score, tempo = parse_musiclang_sequence(midi_file, chords)
-    return score, tempo
-
-
-# Helpers for parser
-
-
-def parse_tonality(element):
-    """Parse tonality as written in musicLang from Music21 object
+    text = _first_clean(text)
+    analysis = music21.converter.parse(text, format="romanText")
+    romans = analysis.recurse().getElementsByClass('RomanNumeral')
+    chords = []
 
-    Parameters
-    ----------
-    element :
-        return: key_tonic : Degree of the key (in 0-12)
+    for roman in romans:
+        prim, sec, key, mode, duration = _get_roman_full(roman)
+        notes = [(n.pitch.pitchClass, n.pitch.octave - 5) for n in roman.notes]
+        final_degree, extension, final_key, final_mode = _analyze_one_chord(prim, sec, key, mode)
+        # Use it
+        chords.append([notes, duration, final_degree, extension, (final_key, final_mode)])
 
-    Returns
-    -------
-    type
-        key_tonic : Degree of the key (in 0-12)
+    return chords
 
-    """
 
-    DICT_MODE = {'major': 'M', 'minor': 'm'}
-    if element.secondaryRomanNumeralKey is not None:
-        key_tonic = element.secondaryRomanNumeralKey.tonic.pitchClass
-        key_mode = DICT_MODE[element.secondaryRomanNumeralKey.mode]
+def _first_clean(text):
+    text = text.replace('%', 'ø')
+    return text
+
+def analyze_one_chord(figure, key, mode):
+    figure = figure.replace('/4', '4').replace('/3', '').replace('/2', '').replace('/5', '5')
+    if mode == 'major':
+        figure = figure.replace('III+', 'III(+)')
+
+    res = figure.split('/')
+    if len(res) == 1:
+        prim, sec, ter = res[0], None, None
+    elif len(res) == 2:
+        prim, sec, ter = res[0], res[1], None
+    elif len(res) == 3:
+        prim, sec, ter = res[0], res[1], res[2]
     else:
-        key_tonic = element.key.tonic.pitchClass
-        key_mode = DICT_MODE[element.key.mode]
-    if 'N' in element.primaryFigure:
-        key_tonic += 1
-        key_mode = 'M'
-    elif 'Ger' in element.primaryFigure:
-        key_tonic += 1  # For musiclang it will be a V % II.b.M
-        key_mode = 'M'
-    elif 'It' in element.primaryFigure:
-        key_tonic += 1  # For musiclang it will be a I % II.b.M
-        key_mode = 'M'
-    elif 'Fr' in element.primaryFigure:
-        key_tonic += 3
-        key_mode = 'mm'
-    return key_tonic, key_mode
-
-
-def get_degree(element):
-    """Get the scale degree of an element (from Music21)
-
-    Parameters
-    ----------
-    element :
-        Music21 element
-
-    Returns
-    -------
-    degree : int
-
-    """
-    degree = element.scaleDegree - 1
-    if 'Ger' in element.primaryFigure:
-        degree = 4
-    if 'It' in element.primaryFigure:
-        degree = 4
-    elif 'N' in element.primaryFigure:
-        degree = 0
-    elif 'Fr' in element.primaryFigure:
-        degree = 3
+        raise Exception(f'Issue with figure {figure}')
 
-    return degree
+    return _analyze_one_chord(prim, sec, ter, key, mode)
 
+def _analyze_one_chord(prim, sec, ter, key, mode):
+    mode = {'major': 'M', 'minor': 'm', 'M': 'M', 'm': 'm'}[mode]
+    prim = _clean(prim)
+    prim = _replace_special_cases(prim)
+    degree, extension = _get_degree_and_extension(prim)
+    sec_degree, _ = _get_degree_and_extension(sec)
+    ter_degree, _ = _get_degree_and_extension(ter)
+    extension = _clean_extension(extension)
+    # Get the key, mode of the sec_degree
+    final_degree, final_key, final_mode = _get_degree_and_tonality(sec_degree, ter_degree, degree, key, mode)
+    return final_degree, extension, final_key, final_mode
+
+def _replace_special_cases(prim):
+
+    #Ge* = ivo*[b3]
+    #It* = #ivo*[b3]
+    #N = bII6
+    #Fr = II*[bV]
+    #N6 = bII6
+
+    # if 'N6' in prim:
+    #     prim = prim.replace('N6', 'bII6')
+    # elif 'N' in prim:
+    #     prim = prim.replace('N', 'bII6')
+    if 'Ger' in prim:
+        pass
+    elif 'It' in prim:
+        prim = 'It' + prim.replace('It', '')
+    elif 'Fr' in prim:
+        prim = 'Fr' + prim.replace('Fr', '')
 
+    return prim
 
-def get_duration(roman):
+def _get_duration(roman):
     """Get the duration of a chord
 
     Parameters
     ----------
     roman :
 
 
@@ -242,138 +125,202 @@
         result, fractions.Fraction with denominator limited to 8
 
     """
     from fractions import Fraction as frac
     return frac(roman.duration.quarterLength).limit_denominator(8)
 
 
-def parse_musiclang_sequence(midi_file, chords):
-    """Parse a midi file into MusicLang and chords with chords duration
-
-    Parameters
-    ----------
-    midi_file :
-
-    chords :
-        
-
-    Returns
-    -------
-
-    """
-    from .midi_parser import parse_midi
-    from .item import convert_to_items
-    from .to_musiclang import infer_voices_per_tracks, infer_score_with_chords_durations
-    notes, instruments, tempo = parse_midi(midi_file)
-    sequence = convert_to_items(notes)
-    print('2/3 : Performing voice separation (This may takes a while)')
-    sequence = infer_voices_per_tracks(sequence)
-    print('3/3 : Create the score')
-    score = infer_score_with_chords_durations(sequence, chords, instruments)
-    print('Finished creating score')
-    return score, tempo
-
-
-def get_chords_from_mxl(input_file):
-    """Given a mxl file, return a MusicLang score parsing only the chord progression
-
-    Parameters
-    ----------
-    input_file : str
-        MusicXML file to parse
-
-    Returns
-    -------
-    score: musiclang.Score
-
-    """
-    import shutil
-    import tempfile
-    import os
-    from .augmented_net import infer_chords
-    with tempfile.TemporaryDirectory() as di:
-        mxl_file = os.path.join(di, 'data.mxl')
-        annotated_file = os.path.join(di, 'data_annotated.rntxt')
-        shutil.copy(input_file, mxl_file)
-        infer_chords(mxl_file)
-        return get_chords_from_analysis(annotated_file)
-
-
-def get_chords_from_analysis(analysis):
-    """Given an analysis file (.rntxt), return a MusicLang score parsing only the chord progression
-
-    Parameters
-    ----------
-    analysis : str,
-        Filepath of analysis file (.rntxt) format
-        
-
-    Returns
-    -------
-    score: musiclang.Score
-
-    """
-    import music21
-    analysis = music21.converter.parse(analysis, format="romanText")
-    chords = music21_roman_analysis_to_chords(analysis)
-    ml = chords_to_musiclang(chords)
-    return ml
-
-
-
-def chords_to_musiclang(chords):
-    """
-
-    Parameters
-    ----------
-    chords :
-        
-
-    Returns
-    -------
-
-    """
-    from musiclang import Tonality, Chord, Note
-    new_score = None
-    for notes, duration, degree, figure, key in chords:
-        key_tonic, key_mode = key
-        tonality = Tonality(key_tonic, mode=key_mode)
-        chord = Chord(degree, tonality=tonality, extension=figure)
-        scale_notes = []
-        for pitch_class, octave in notes:
-            # Parse the note in musiclang
-            scale_notes.append(chord.parse(pitch_class).o(octave + 1).augment(duration))
-
-        chord_score = {f'piano__{idx}': sn for idx, sn in enumerate(scale_notes)}
-        new_score += chord(**chord_score)
-
-    return new_score
-
-
-def music21_roman_analysis_to_chords(score):
-    """
-
-    Parameters
-    ----------
-    score :
-        
-
-    Returns
-    -------
+def _get_roman_full(roman):
+    secondary = None
+    if roman.secondaryRomanNumeral is not None:
+        secondary = roman.secondaryRomanNumeral.primaryFigure
+    duration = _get_duration(roman)
+    return roman.primaryFigure, secondary, roman.key.tonic.pitchClass, roman.key.mode, duration
+
+def _get_degree_and_extension(data):
+    if data is None:
+        return None, None
+    else:
+        degree = DEGREE_REGEX.match(data)[0]
+        extension = data.replace(degree, '')
+        if degree == 'N' and extension == '':
+            extension = '6'
+        elif degree == "Ger" and extension == '':
+            extension = '7'
+        elif degree == "Ger" and extension == '6':
+            extension = '65'
+        elif degree == "It" and extension == '':
+            extension = "7[no5]"
+        elif degree == "It" and extension == '53':
+            extension = "7[no5]"
+        elif degree == "It" and extension == '6':
+            extension = "65[no5]"
+        elif degree == "It" and extension == '64':
+            extension = "2[no5]"
+        elif degree == "Fr" and extension == '':
+            extension = "7[b5]"
+        elif degree == "Fr" and extension == '6':
+            extension = "65[b5]"
+        elif degree == "Fr":
+            extension = extension + "[b5]"
+        elif degree == "It":
+            extension = extension + "[no5]"
+        return degree, extension
+
+
+from musiclang.analyze.constants import DICT_TONALITY_REVERSE
+
+TONALITY_DICT = {
+    "c": 0,
+    "d": 2,
+    "e": 4,
+    "f": 5,
+    "g": 7,
+    "a": 9,
+    "b": 11
+}
+
+
+def get_relative_tone(first_degree, first_mode, current_degree, current_mode):
+    delta_degree = (current_degree - first_degree) % 12
+    figure = DICT_TONALITY_REVERSE[first_mode][delta_degree, current_mode]
+    return figure
+
+
+def convert_harmony(harmony, get_features=False):
+    """
+    Convert harmony to relative modulations (Using ternary "/" modulations instead of named modulation).
+    That way the harmony does not modulate through the piece.
+
+    Parameters
+    ----------
+    harmony: str
+        Harmony to convert
+
+    Returns
+    -------
+    new_harmony: str
+
+    """
+    lines = harmony.split('\n')
+    new_harmony = []
+    current_degree = 0
+    current_mode = 'M'
+    first_degree = 0
+    nb_chords = 0
+    nb_modulations = 0
+    nb_time_signature_change = 0
+    bar_duration = 4
+    time_signature_den = 4
+    time_signature_nom = 4
+    has_time = False
+    bar_numbers = []
+    nb_bars = 0
+    first_mode = 'M'
+    tonality_line = None
+    first = True
+    for line in lines:
+        if line == "":
+            continue
+        elif not line.startswith('m'):
+            if line.lower().startswith("time"):
+                if not has_time:
+                    time_signature_nom = int(line.split(':')[1].strip().split('/')[0])
+                    time_signature_den = int(line.split(':')[1].strip().split('/')[1])
+                    bar_duration = time_signature_nom * 4 / time_signature_den
+                nb_time_signature_change += 1
+                has_time = True
+            new_harmony.append(line)
+        else:
+            elements = line.split(' ')
+            new_line = []
+            for el in elements:
+                if ":" in el:
+                    degree = TONALITY_DICT[el[0].lower()]
+                    mode = 'm' if el[0] == el[0].lower() else 'M'
+                    flats = len([e for e in el[1:] if e in ['b', '-']])
+                    sharps = len([e for e in el[1:] if e in ['#', 's']])
+                    degree = degree + sharps - flats
+                    if first:
+                        first_degree = degree
+                        first_mode = mode
+                        #new_line.append(el)
+                        tonality_line = el.replace(':', '')
+                    else:
+                        nb_modulations += 1
+                    current_degree = degree
+                    current_mode = mode
+                    first = False
+                elif el.startswith('m'):
+                    bar_number = int(el[1:].replace('.', '', 1))
+                    bar_numbers.append(bar_number)
+                    nb_bars = max(bar_number, nb_bars)
+                    new_line.append(el)
+                elif el.startswith('b') and el[1:].replace('.', '', 1).isdigit():
+                    new_el = el
+                    new_line.append(new_el)
+                else:
+                    nb_chords += 1
+                    if current_degree != first_degree or current_mode != first_mode:
+                        # Relative tone
+                        new_el = el + "/" + get_relative_tone(first_degree,
+                                                              first_mode, current_degree, current_mode)
+                    else:
+                        new_el = el
+                    new_line.append(new_el)
+
+            new_harmony.append(' '.join(new_line))
+    if tonality_line is not None:
+        new_harmony.insert(0, "Tonality : " + tonality_line)
+
+    if get_features:
+        new_harmony = "\n".join(new_harmony)
+        data = {
+                "raw_annotation": harmony,
+                "annotation": new_harmony,
+                "nb_chords": float(nb_chords),
+                "nb_bars": float(nb_bars),
+                "nb_chords_per_bar": float(nb_chords / nb_bars),
+                "nb_modulations": float(nb_modulations),
+                "nb_modulations_per_bar": float(nb_modulations / nb_bars),
+                "nb_time_signature_change": float(nb_time_signature_change),
+                "time_signature_nom": int(time_signature_nom),
+                "time_signature_den": int(time_signature_den),
+                "bar_duration": float(bar_duration),
+                "max_bar_jump": float(np.max(np.diff(bar_numbers))) if len(bar_numbers) > 1 else 0,
+                "mode": first_mode,
+                "degree": int(first_degree)
+                }
+        return new_harmony, data
+
+    return "\n".join(new_harmony)
+
+def _get_degree_and_tonality(sec_degree, ter_degree, degree, key, mode):
+    if ter_degree is not None:
+        # Change the key, mode
+        key_add, new_mode = DICT_TONALITY[mode][ter_degree]
+        key, mode = (key + key_add) % 12, new_mode
 
-    """
-    time_sig = None
+    if sec_degree is None:
+        new_key, new_mode = key, mode
+    else:
+        key_add, new_mode = DICT_TONALITY[mode][sec_degree]
+        new_key, new_mode = (key + key_add) % 12, new_mode
+    degree, new_mode, key_add = DICT_RELATIVE_CHANGE[new_mode][degree]
+    new_key = (new_key + key_add) % 12
+    return degree, new_key, new_mode
+
+
+def _clean(data):
+    data = data.replace('42', '2').replace('4/3', '43').replace('/3', '').replace('/', '').replace('/4', '4')
+    data = data.replace('%', 'ø')
+    return data
+
+
+def _clean_extension(figure):
+    figure = figure.replace('[', '').replace('(', '').replace(']', '').replace(')', '')
+    figure = figure.replace('66', '6').replace('67', '7').replace('62', '2').replace('643', '43')
+    for key, val in EXTENSION_REPLACER:
+        figure = figure.replace(key, val)
+    return figure
 
-    chords = []
-    # Get time sigs
-    romans = score.recurse().getElementsByClass('RomanNumeral')
-    for roman in romans:
-        key_tonic, key_mode = parse_tonality(roman)
-        notes = [(n.pitch.pitchClass, n.pitch.octave - 5) for n in roman.notes]
-        duration = get_duration(roman)
-        degree = get_degree(roman)
-        figure = roman.figuresWritten.replace('/', '')
-        if figure == 'ar':
-            figure = ''
-        chords.append([notes, duration, degree, figure, (key_tonic, key_mode)])
 
-    return chords
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `musiclang-0.8.1/musiclang/analyze/to_musiclang.py` & `musiclang-0.8.2/musiclang/analyze/to_musiclang.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,16 @@
         melody += Silence((bar_time_end - local_time_end) * tick_value)
     if local_time_end > bar_time_end:
         return_cont = Continuation((local_time_end - bar_time_end) * tick_value)
         melody.notes[-1].duration -= (local_time_end - bar_time_end) * tick_value
         if melody.notes[-1].duration == 0:
             melody.notes.pop()
 
+    from musiclang import Note
+    assert all([isinstance(m, Note) for m in melody.notes])
     assert melody.duration == (bar_time_end - bar_time_start) * tick_value
 
     return melody, return_cont
```

### Comparing `musiclang-0.8.1/musiclang/analyze/voice_separation.py` & `musiclang-0.8.2/musiclang/analyze/voice_separation.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/predict/predictors/windowed.py` & `musiclang-0.8.2/musiclang/predict/predictors/windowed.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/predict/tokenizers/chord_tokenizer.py` & `musiclang-0.8.2/musiclang/predict/tokenizers/chord_tokenizer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/base_transformer.py` & `musiclang-0.8.2/musiclang/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/chord/basics.py` & `musiclang-0.8.2/musiclang/transform/chord/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/composing/arrange.py` & `musiclang-0.8.2/musiclang/transform/composing/arrange.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/composing/counterpoint.py` & `musiclang-0.8.2/musiclang/transform/composing/counterpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,15 @@
     # Deal with bass and chord notes
     chord, _, chords_offsets, _, chords = project_on_one_chord(score)
     fixed_voices = [chord.score[part] for part in fixed_parts]
     moving_voices = [chord.score[part] for part in counterpoint_parts]
     moving_voices = create_counterpoint(fixed_voices, moving_voices)
     for voice, part in zip(moving_voices, counterpoint_parts):
         chord.score[part] = voice
-
-    projection = chord.to_score().project_on_score(score, keep_score=False)
-    projection = Score([s & (-i) for s, i in zip(projection.chords, chords_offsets)])
+    projection = chord.to_score().project_on_score(score)
     return projection
 
 
 def create_counterpoint_on_chord(chord, subject_parts, counterpoint_parts):
     """
 
     Parameters
@@ -202,15 +200,18 @@
     elif delta > 0:
         return -delta
     else:
         return -delta + 1
 
 def get_delta_list():
     """ """
-    return [0, 1, -1, 2, -2, 3, -3, 4, -4]
+    deltas = [0, 1, -1, 2, -2, 3, -3, 4, -4]
+    #deltas = [0, 1, -2, 2, -2]
+    np.random.shuffle(deltas)
+    return deltas
 
 def is_dissonnance(n1, n2):
     """
 
     Parameters
     ----------
     n1 :
@@ -310,14 +311,16 @@
             continue
         elif inter is None:
             continue
         elif is_parallel_dissonnance(inter, s, candidate):
             count += 1
     return count
 
+
+
 def is_triton(candidate, subject_note):
     """
 
     Parameters
     ----------
     candidate :
         
@@ -326,15 +329,15 @@
 
     Returns
     -------
 
     """
     return {candidate % 7, subject_note % 7} == {3, 6}
 
-def scorer(subject_notes, note, delta, last_intervals):
+def scorer(subject_notes, note, delta, last_intervals, last_notes):
     """
 
     Parameters
     ----------
     subject_notes :
         
     note :
@@ -352,17 +355,22 @@
     not_silenced_subject_notes = [s for s in subject_notes if s is not None]
     candidate = note + delta
     NB_DISSONNANCES = sum([1 * is_dissonnance(candidate, s) for s in not_silenced_subject_notes])
     NB_FORBIDDEN_PARALLELS = nb_forbidden_parallel(last_intervals[-1], subject_notes, candidate)
     NB_PARALLEL_DISSONNANCES = nb_parallel_dissonnances(last_intervals[-1], subject_notes, candidate)
     NB_TRITON = sum([1 * is_triton(candidate, s) for s in not_silenced_subject_notes])
     DISTANCE = abs(delta)
-    return 10 - 4 * NB_DISSONNANCES - 4 * NB_FORBIDDEN_PARALLELS - 4 * NB_PARALLEL_DISSONNANCES - 0.2 * DISTANCE - 0.2 * NB_TRITON
+    LAST_NOTE_SAME = 1.0 * (candidate == last_notes[-1]) if len(last_notes) > 0 else 0.0
+    score = 10 - 3.0 * NB_DISSONNANCES
+    score += - 2.0 * NB_TRITON
+    score += - 4 * NB_FORBIDDEN_PARALLELS - 4 * NB_PARALLEL_DISSONNANCES - 0.5 * DISTANCE
+    score += - 2.0 * LAST_NOTE_SAME
+    return score
 
-def get_counterpoint_for_one_note(subjects_notes, note, last_intervals, delta=0):
+def get_counterpoint_for_one_note(subjects_notes, note, last_intervals, last_notes, delta=0):
     """
 
     Parameters
     ----------
     subjects_notes :
         
     note :
@@ -374,18 +382,18 @@
 
     Returns
     -------
 
     """
 
     deltas = get_delta_list()
-    scores = [scorer(subjects_notes, note, delta, last_intervals) for delta in deltas]
+    scores = [scorer(subjects_notes, note, delta, last_intervals, last_notes) for delta in deltas]
     max_score, max_score_idx = np.max(scores), np.argmax(scores)
-
     best_delta = deltas[max_score_idx]
+
     chosen_candidate = note + best_delta
     assert len(subjects_notes) == len(last_intervals[-1]), "{} {}".format(len(subjects_notes), len(last_intervals[-1]))
     last_intervals.append([interval(s, chosen_candidate, replace=old_inter) for s, old_inter in zip(subjects_notes, last_intervals[-1])])
     return chosen_candidate, last_intervals, max_score
 
 
 
@@ -445,21 +453,23 @@
     -------
 
     """
     subjects = np.asarray(subjects)
     last_intervals = [[None for s in subjects]]
     result = []
     total_score = 0
+    last_notes = []
     for i, n in enumerate(to_fix):
         if n is None:
             result.append(None)
         else:
-            new_note, last_intervals, max_score = get_counterpoint_for_one_note(subjects[:, i].tolist(), n, last_intervals)
+            new_note, last_intervals, max_score = get_counterpoint_for_one_note(subjects[:, i].tolist(), n, last_intervals, last_notes)
             result.append(new_note)
             total_score += max_score
+            last_notes.append(new_note)
 
         last_intervals = clear_list_intervals(last_intervals)
 
     return result
 
 
 def convert_array_to_melody(rythm, notes):
```

### Comparing `musiclang-0.8.1/musiclang/transform/composing/project.py` & `musiclang-0.8.2/musiclang/transform/composing/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
     """
     from musiclang.write.constants import DEGREE_TO_SCALE_DEGREE
     offset_degrees = c2.element - c1.element
 
     c1_degree = c1.tonality.degree if c1.tonality is not None else 0
     c2_degree = c2.tonality.degree if c2.tonality is not None else 0
-    c1_octave = c1.tonality.octave if c1.tonality is not None else 0
-    c2_octave = c2.tonality.octave if c2.tonality is not None else 0
+    c1_octave = c1.full_octave if c1.tonality is not None else 0
+    c2_octave = c2.full_octave if c2.tonality is not None else 0
     offset_tonalities = int(np.sign(c2_degree - c1_degree) * DEGREE_TO_SCALE_DEGREE[abs(c2_degree - c1_degree)])
-    offset_octave = c2_octave - c1_octave
+    offset_octave = c1_octave - c2_octave
     offset_octave_chords = c2.octave - c1.octave
 
     return offset_degrees + offset_tonalities + 7 * (offset_octave + offset_octave_chords)
 
 
 def project_on_several_chord(score, chords):
     """
@@ -63,15 +63,15 @@
     Returns
     -------
 
     """
     from musiclang import Score
     chord, _, _, _, chords = project_on_one_chord(score1)
     _, _, chords_offsets, _, _ = project_on_one_chord(score2)
-    projection = chord.to_score().project_on_score(score2, keep_score=False)
+    projection = chord.to_score().project_on_score(score2, voice_leading=False)
     projection = Score([s & (-i) for s, i in zip(projection.chords, chords_offsets)])
     return projection
 
 
 def project_on_one_chord(score):
     """Clever projection of a score in several chords into the first chord
     :return:
@@ -309,14 +309,15 @@
                           9: 5,
                           10: 6,
                           11: 6
                           }
             new_note = note.copy()
             new_note.type = "s"
             new_note.val = DICT_NOTES[new_note.val]
+            result += new_note
         else:
             raise Exception('Could not handle type in project rhythm : {}'.format(note.type))
 
     return result
 
 
 def is_continuation(note, silence_as_continuation=True):
@@ -434,33 +435,14 @@
     Returns
     -------
 
     """
     candidate_val = min(candidates, key=lambda x: abs(x.val - note.val))
     return get_nearest_val(note, candidate_val.val)
 
-
-def get_nearest_note(candidates, note):
-    """
-
-    Parameters
-    ----------
-    candidates :
-        
-    note :
-        
-
-    Returns
-    -------
-
-    """
-    candidate_val = min(candidates, key=lambda x: abs(x.val - note.val))
-    return get_nearest_val(note, candidate_val.val)
-
-
 def get_nearest_val(n, new_val):
     """
 
     Parameters
     ----------
     n :
         
@@ -571,41 +553,15 @@
         elif rhythm_note.val == TONIC_OR_FIFTH.val:
             return [Note("s", 0, 0, 1), Note("s", 4, 0, 1)]
         elif rhythm_note.val == SCALE_DISSONNANCE.val:
             return chord.scale_dissonances
     return [rhythm_note]
 
 
-def get_nearest_note_in_context(rhythm_note, note, chord, dict_notes=None):
-    """
 
-    Parameters
-    ----------
-    rhythm_note :
-        
-    note :
-        
-    chord :
-        
-    dict_notes :
-         (Default value = None)
-
-    Returns
-    -------
-
-    """
-    if dict_notes is None:
-        dict_notes = {}
-    candidates = get_notes_candidate_in_context(rhythm_note, chord, dict_notes=dict_notes)
-    if len(candidates) == 0:
-        return note
-    elif note.is_note:
-        return get_nearest_note(candidates, note)
-    else:
-        return note
 
 
 def get_absolute_voice(voice):
     """Transform a relative melody to an absolute one
 
     Parameters
     ----------
```

### Comparing `musiclang-0.8.1/musiclang/transform/features/basics.py` & `musiclang-0.8.2/musiclang/transform/features/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/graph.py` & `musiclang-0.8.2/musiclang/transform/graph.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/library.py` & `musiclang-0.8.2/musiclang/transform/library.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from .melody import CircularPermutationMelody, SelectRangeMelody, ReverseMelody, \
     InvertMelody, ReverseMelodyWithoutRhythm
 from .note import LimitRegister, ApplySilence, TransposeDiatonic, TransposeChromatic, ApplyContinuation
 from .score import RepeatScore
 from .features import ExtractMainTonality, MostCommonTonalities
 from .chord import RepeatChord, Modulate, ModulateKeepOriginMode
 from .score_merger import ConcatScores, ConcatWithPattern, TakeSlice, TakeFirst, TakeLast, TakeIdx
+from .composing import VoiceLeading, Patternator
+from .dynamics import PitchDynamizer
+from .melody import ContinuationWhenSameNote
 
 __all__ = ['create_counterpoint', 'create_counterpoint_on_score',
            'CircularPermutationMelody', 'SelectRangeMelody', 'ReverseMelody', 'InvertMelody',
            'RepeatScore', 'ReverseMelodyWithoutRhythm',
             'LimitRegister', 'ApplySilence', 'TransposeDiatonic', 'TransposeChromatic', 'ApplyContinuation',
             'ExtractMainTonality', 'MostCommonTonalities',
             'RepeatChord', 'Modulate', 'ModulateKeepOriginMode',
-           'ConcatScores', 'ConcatWithPattern', 'TakeSlice', 'TakeFirst', 'TakeLast', 'TakeIdx'
+           'ConcatScores', 'ConcatWithPattern', 'TakeSlice', 'TakeFirst', 'TakeLast', 'TakeIdx',
+           'VoiceLeading', 'PitchDynamizer', 'ContinuationWhenSameNote', 'Patternator'
            ]
```

### Comparing `musiclang-0.8.1/musiclang/transform/mask.py` & `musiclang-0.8.2/musiclang/transform/mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/melody/basics.py` & `musiclang-0.8.2/musiclang/transform/melody/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/note/basics.py` & `musiclang-0.8.2/musiclang/transform/note/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/pipeline.py` & `musiclang-0.8.2/musiclang/transform/pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/score_merger/basics.py` & `musiclang-0.8.2/musiclang/transform/score_merger/basics.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/structure_graphs/forms.py` & `musiclang-0.8.2/musiclang/transform/structure_graphs/forms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/transformer.py` & `musiclang-0.8.2/musiclang/transform/transformer.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/transform/utils_random.py` & `musiclang-0.8.2/musiclang/transform/utils_random.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/arrange_utils/arrange_utils.py` & `musiclang-0.8.2/musiclang/write/arrange_utils/arrange_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/arrange_utils/skyline_algorithm.py` & `musiclang-0.8.2/musiclang/write/arrange_utils/skyline_algorithm.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/chord.py` & `musiclang-0.8.2/musiclang/write/chord.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                 Represents the tonality of the chord
         score: dict, optional
                Represents the melodies and instruments played by this chord
         octave: int, optional
                 Represents the base octave of the chord
         """
         self.element = element
-        self.extension = extension
+        self.extension = str(extension)
+        self.extension = self.normalize_extension()
         self.tonality = tonality
         self.octave = octave
         self.score = {} if score is None else score
         self.tags = set(tags) if tags is not None else set()
 
     def has_tag(self, tag):
         """
@@ -124,14 +125,31 @@
         chord: Chord
 
         """
         cp = self.copy()
         cp.tags = cp.tags.union(set(tags))
         return cp
 
+    def clear_note_tags(self):
+        """
+        Clear all tags from this object
+        Returns a copy of the object
+        Parameters
+        ----------
+        tag: str
+
+        Returns
+        -------
+        chord: Chord
+        """
+        cp = self.copy()
+        for k, v in cp.score.items():
+            cp.score[k] = v.clear_note_tags()
+        return cp
+
     def remove_tags(self, tags):
         """
         Remove several tags from the object.
         Returns a copy of the object
 
         Parameters
         ----------
@@ -175,14 +193,31 @@
         -------
         chord: Chord
         """
         cp = self.copy()
         cp.tags = set()
         return cp
 
+    def has_pitch(self, pitch):
+        """
+        Check whether the pitch belong to the chord or not
+
+        Parameters
+        ----------
+        pitch: int
+        Pitch to check
+
+        Returns
+        -------
+        result: boolean
+            True if the chord has this pitch
+
+        """
+        return (pitch % 12) in [p % 12 for p in self.chord_pitches]
+
     def parse(self, pitch):
         """
         Parse an integer pitch (0=C5)
         Parameters
         ----------
         pitch :
             
@@ -200,14 +235,27 @@
             type = 'h'
 
         scale_mod = [s % 12 for s in scale]
         idx = scale_mod.index(pitch % 12)
         oct = (pitch - scale[0]) // 12
         return Note(type, idx, oct, 1)
 
+    def project_on_score(self, score2, **kwargs):
+        """
+        Transform chord into a score and apply Score.project_on_score
+        Parameters
+        ----------
+        score2: other score on which to project
+        voice_leading:
+        kwargs
+        Returns
+        -------
+        """
+        return self.to_score().project_on_score(score2, **kwargs)
+
     def decompose_duration(self):
         """ """
         return self(**{key: melody.decompose_duration() for key, melody in self.score.items()}, tags=self.tags)
 
     @property
     def degree(self):
         return self.element
@@ -239,14 +287,21 @@
         -------
 
         """
         new_chord = self.copy()
         new_chord.tonality = new_chord.tonality.change_mode(mode)
         return new_chord
 
+    @property
+    def pedal(self):
+        """
+        Apply pedal on first note and release on last
+        """
+        return self(**{key: item.to_melody().pedal for key, item in self.score.items()}, tags=set(self.tags))
+
     def to_pitch(self, note, last_pitch=None):
         """
 
         Parameters
         ----------
         note :
             
@@ -254,32 +309,43 @@
              (Default value = None)
 
         Returns
         -------
 
         """
         from .out.to_midi import note_to_pitch_result
+        if note.is_continuation:
+            return last_pitch
+
         if not note.is_note:
             return None
         return note_to_pitch_result(note, self, last_pitch=last_pitch)
 
+    def to_absolute_note(self):
+        return self(**{part: melody.to_absolute_note(self) for part, melody in self.score.items()})
+
+    @property
+    def bass_pitch(self):
+        return self.chord_extension_pitches[0]
+
     def to_sequence(self):
         """
         See :func:`~Score.to_sequence()
         """
         sequence_dict = []
         for inst in self.instruments:
             sequence_dict += self.score[inst].to_sequence(self, inst)
 
         return sequence_dict
 
-    def to_score(self):
+    def to_score(self, copy=True):
         """ """
         from .score import Score
-        return Score([self])
+        chord = self if not copy else self.copy()
+        return Score([chord])
 
     def show(self, *args, **kwargs):
         """
         See :func:`~Score.show()
         """
         return self.to_score().show(*args, **kwargs)
 
@@ -354,14 +420,28 @@
         notes = self.chord_notes
         return [self.to_pitch(n) for n in notes]
 
     def remove_accidents(self):
         return Chord(**{key: val.remove_accidents() for key, val in self.score.items()}, tags=set(self.tags))
 
 
+    def get_scale_from_type(self, type):
+        if type == "h":
+            return self.chromatic_pitches
+        elif type == "s":
+            return self.scale_pitches
+        elif type == "b":
+            return self.chord_extension_pitches
+        elif type == "c":
+            return self.chord_pitches
+        else:
+            raise ValueError("This type is not associated to a scale")
+    @property
+    def chromatic_pitches(self):
+        return [self.scale_pitches[0] + i for i in range(12)]
     @property
     def scale_pitches(self):
         """
         Get the scale absolute pitches (integers) starting with the chord root.
 
         See Also
         --------
@@ -385,14 +465,15 @@
             return (self % Tonality(0)).scale_pitches
         tonality_scale_pitches = self.tonality.scale_pitches
         start_idx = self.element
         scale_pitches = tonality_scale_pitches[start_idx:] + [t + 12 for t in tonality_scale_pitches[:start_idx]]
         scale_pitches = [n + 12 * self.octave for n in scale_pitches]
         return scale_pitches
 
+
     @property
     def chromatic_scale_pitches(self):
         """ """
         return [self.scale_pitches[0] + i for i in range(12)]
 
     @property
     def chord_extension_pitches(self):
@@ -420,21 +501,27 @@
         [-1, 0, 2, 4, 9]
         """
 
         notes = self.extension_notes
         return [self.to_pitch(n) for n in notes]
 
     @property
+    def chord_extension_pitch_classes(self):
+        return [i % 12 for i in self.chord_extension_pitches]
+    @property
     def parts(self):
         """
         Get the list of all parts names
         Same as :func:`~Chord.instruments`
         """
         return list(self.score.keys())
 
+    def to_drum(self):
+        return self(**{key: val.to_drum() if key.startswith('drum') else val for key, val in self.items()})
+
     @property
     def instruments(self):
         """
         Get the list of all part names
         """
         return list(self.score.keys())
 
@@ -592,20 +679,20 @@
         chord: Chord
                A new chord with the figured bass extension
 
         """
         item = str(item)
         res = self.copy()
         res.extension = str(item)
-        res.extension = res.normalize_extension()
         try:
             n = res.extension_notes
         except Exception as e:
             raise e
             #raise ValueError(f'Could not parse extension : {item} {e}')
+        res.extension = res.normalize_extension()
 
         return res
 
     #
     # def __getattr__(self, item):
     #     chord = self.copy()
     #     chord.score = {k: getattr(s, item) for k, s in self.score.items()}
@@ -621,14 +708,17 @@
         duration: fractions.Fraction or int
                   duration of the chord
         """
         if len(self.score.keys()) == 0:
             return 0
         return max([self.score[key].duration for key in self.score.keys()])
 
+    def set_amp(self, amp):
+        return self(**{key: val.set_amp(amp) for key, val in self.items()}, tags=set(self.tags))
+
     def set_part(self, part, melody, inplace=False):
         """
         Set a part on the chord (inplace operation)
         Parameters
         ----------
         part : part name
 
@@ -823,14 +913,24 @@
         """Chord up one octave (=o(-1))"""
         return self.o(-1)
 
     def u(self):
         """Chord down one octave (=o(-1))"""
         return self.o(1)
 
+    def to_extension_note(self):
+        return self(**{key: val.to_extension_note(self) for key, val in self.items()}, tags=set(self.tags))
+
+    def to_chord_note(self):
+        return self(**{key: val.to_chord_note(self) for key, val in self.items()}, tags=set(self.tags))
+
+    def to_standard_note(self):
+        return self(**{key: val.to_standard_note(self) for key, val in self.items()}, tags=set(self.tags))
+
+
     def o_melody(self, octave):
         """Change the octave of the melody (not the chord)
 
         Parameters
         ----------
         octave : int,
                 Number of octaves
@@ -842,14 +942,77 @@
         """
         new_parts = {}
         for part in self.score.keys():
             new_parts[part] = self.score[part].o(octave)
 
         return self(**new_parts).add_tags(self.tags)
 
+    def patternize(self,
+                 nb_excluded_instruments=0,
+                 fixed_bass=True,
+                 voice_leading=True,
+                 melody=False,
+                 instruments=None,
+                 voicing=None,
+                 add_metadata=True,
+                   max_duration=16,
+                   **kwargs):
+        """
+        Extract the pattern from the chord
+
+        Parameters
+        ----------
+        nb_excluded_instruments: int (Default value = 0)
+            Number of instruments to exclude from the pattern
+        fixed_bass: bool (Default value = True)
+            If True, the bass will be fixed in the pattern response
+        voice_leading: bool (Default value = True)
+            If True, the voice leading will be applied in the pattern response
+        melody: bool (Default value = False)
+            Do you want to extract a melody or an accompaniment pattern
+        instruments: list[str] (Default value = None)
+            List of instruments to use for the pattern
+        voicing: list[Note] or None (Default value = None)
+            Voicing to use for the pattern, otherwise extract the good one
+        add_metadata: bool (Default value = True)
+            If True, add metadata and features to the pattern
+        Returns
+        -------
+        score_pattern: Chord
+            Patternized chord or score
+        pattern: dict
+            Pattern data of the score
+
+        """
+        from musiclang.analyze.pattern_analyzer import PatternExtractor
+        if self.duration > max_duration:
+            raise Exception(f'Patternize only works on chords with duration <= {max_duration} increase the max_duration parameter if you want to use it on longer chords')
+
+        dict_pattern = PatternExtractor(
+                 nb_excluded_instruments=nb_excluded_instruments,
+                 fixed_bass=fixed_bass,
+                 voice_leading=voice_leading,
+                 melody=melody,
+                 instruments=instruments,
+                 voicing=voicing
+                 ).extract(self)
+
+        pattern = dict_pattern['orchestra']['pattern']
+        if add_metadata:
+            from musiclang.analyze.pattern_analyzer import PatternFeatureExtractor
+            dict_pattern = PatternFeatureExtractor().extract(dict_pattern,
+                                                             self,
+                                                             melody=melody,
+                                                             nb_excluded_instruments=nb_excluded_instruments,
+                                                             )
+        return dict_pattern, pattern
+
+    def project_pattern(self, score, restart_each_chord=False):
+        return self.to_score().project_pattern(score, restart_each_chord=restart_each_chord)
+
     def o(self, octave):
         """Chord up or down the amount of octave in parameter, it will change the chord octave, not the melody
 
         Parameters
         ----------
         octave :
             return:
@@ -935,20 +1098,26 @@
                 key_obj, number = key_obj[0], key_obj[1]
                 number = int(number)
 
             if (isinstance(named_melodies[key], list)):
                 for idx, melody in enumerate(named_melodies[key]):
                     mel = melody.to_melody()
                     if key_obj.startswith('drums'):
-                        mel = Melody([n.convert_to_drum_note(self) for n in mel.notes])
+                        new_mel = None
+                        for n in mel.notes:
+                            new_mel += n.convert_to_drum_note(self)
+                        mel = new_mel
                     named_melodies_result[key_obj + '__' + str(number + idx)] = mel
             else:
                 mel = named_melodies[key].to_melody()
                 if key_obj.startswith('drums'):
-                    mel = Melody([n.convert_to_drum_note(self) for n in mel.notes])
+                    new_mel = None
+                    for n in mel.notes:
+                        new_mel += n.convert_to_drum_note(self)
+                    mel = new_mel
                 named_melodies_result[key_obj + '__' + str(number)] = mel
 
         return named_melodies_result
 
     def items(self):
         return self.score.items()
 
@@ -965,14 +1134,16 @@
             return self(silence)
         else:
             return self(**{part: melody.augment(duration) for part, melody in self.score.items()}, tags=self.tags)
 
     def set_duration(self, duration):
         from musiclang import Silence
         if self.empty_score:
+            if isinstance(duration, float):
+                duration = frac(duration).limit_denominator(8)
             silence = Silence(duration)
             return self(silence)
         else:
             return self(**{part: melody.set_duration(duration) for part, melody in self.score.items()}, tags=self.tags)
 
     def __getattr__(self, item):
         if item in STR_TO_DURATION.keys() and self.empty_score:
@@ -1047,49 +1218,89 @@
 
         """
         return '\n' + ', \n'.join([f"\t{k}=" + str(melody) for k, melody in self.score.items()])
 
     def __repr__(self):
         return f"{self.to_code()}({self.melody_to_str()})"
 
+    @property
+    def full_octave(self):
+        return self.octave + self.tonality.octave
+
+    def replace_instruments(self, **instruments_dict):
+        """
+        Replace any instrument with another (use full part name (eg: piano__0)
+
+        Parameters
+        ----------
+        instruments_dict: dict[str, str]
+            Dictionary of parts name to replace
+
+        Returns
+        -------
+        chord: Chord
+
+        """
+        instruments_dict = {key: instruments_dict[key] if key in instruments_dict.keys() else key for key in self.parts}
+        new_chord_dict = {}
+        for ins_name, new_ins_name in instruments_dict.items():
+            if ins_name in self.score.keys():
+                new_chord_dict[new_ins_name] = self.score[ins_name]
+
+        return self(**new_chord_dict)
+
 
     def normalize_extension(self):
         extension, replacements, additions, removals = self.get_extension_properties()
         replacements = ''.join([f'({r})' for r in replacements])
         additions = ''.join([f'[{a}]' for a in additions])
         removals = ''.join(['{' + r + '}' for r in removals])
         return extension + replacements + additions + removals
 
     def get_extension_properties(self):
-        replacements = sorted(re.findall(r'\((.*?)\)', self.extension))
-        additions = sorted(re.findall(r'\[(.*?)\]', self.extension))
-        removals = sorted(re.findall(r'\{(.*?)\}', self.extension))
-        extension = self.extension.split('(')[0].split('[')[0].split('{')[0]
+        extension = self.extension.split('|')[0]
+        replacements = sorted(re.findall(r'\((.*?)\)', extension))
+        additions = sorted(re.findall(r'\[(.*?)\]', extension))
+        removals = sorted(re.findall(r'\{(.*?)\}', extension))
+        ext = extension
+        for r in replacements + additions + removals:
+            ext = ext.replace(r, '')
+        ext = ext.replace('()', '').replace('[]', '').replace('{}', '')
+        extension = ext
         return extension, replacements, additions, removals
 
 
     def _chord_notes_calc(self, extension, replacements, additions, removals):
         from .library import BASE_EXTENSION_DICT, \
             DICT_REPLACEMENT, DICT_ADDITION, DICT_REMOVAL
         notes = BASE_EXTENSION_DICT[extension][:]
         notes_without_octave = [n.o(-n.octave) for n in notes]
+
+        dict_replaced = {}
+        for replacement in replacements:
+            note_replaced, new_note = DICT_REPLACEMENT[replacement]
+            if note_replaced not in notes_without_octave:
+                additions.append(replacement)
+            else:
+                idx = notes_without_octave.index(note_replaced)
+                notes[idx] = new_note.o(notes[idx].octave)
+                notes_without_octave[idx] = new_note.o(-new_note.octave)
+                dict_replaced[note_replaced] = notes_without_octave[idx]
+
         for addition in additions:
             note_after, new_note = DICT_ADDITION[addition]
-            idx = notes_without_octave.index(note_after) + 1
+            if note_after in dict_replaced.keys():
+                query_note = dict_replaced[note_after]
+            else:
+                query_note = note_after
+            idx = notes_without_octave.index(query_note) + 1
             new_note = new_note.o(note_after.octave)
             notes.insert(idx, new_note)
             notes_without_octave.insert(idx, new_note.o(-new_note.octave))
 
-        for replacement in replacements:
-            note_replaced, new_note = DICT_REPLACEMENT[replacement]
-            idx = notes_without_octave.index(note_replaced)
-            notes[idx] = new_note.o(notes[idx].octave)
-            notes_without_octave[idx] = new_note.o(-new_note.octave)
-
-
         for removal in removals:
             note_removed = DICT_REMOVAL[removal]
             idx = len(notes) - notes_without_octave[::-1].index(note_removed) - 1
             notes.pop(idx)
             notes_without_octave.pop(idx)
         # Sort per pitch
         notes = list(sorted(notes, key=lambda x: self.to_pitch(x)))
```

### Comparing `musiclang-0.8.1/musiclang/write/constants.py` & `musiclang-0.8.2/musiclang/write/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,14 +649,16 @@
 PITCH = 0
 OFFSET = 1
 DURATION = 2
 VELOCITY = 3
 TRACK = 4
 SILENCE = 5
 CONTINUATION = 6
+TEMPO = 7
+PEDAL = 8
 
 DRUMS_DICT = {
     (0, -2):  'bd',
     (1, -2): 'rs',
     (2, -2): 'sn',
     (3, -2): 'cp',
     (4, -2): 'sn2',
```

### Comparing `musiclang-0.8.1/musiclang/write/element.py` & `musiclang-0.8.2/musiclang/write/element.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/library.py` & `musiclang-0.8.2/musiclang/write/library.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,59 @@
 II = ii = Element(1)
 III = iii = Element(2)
 IV = iv = Element(3)
 V = v = Element(4)
 VI = vi = Element(5)
 VII = vii = Element(6)
 Atonal = (I % I.M)
+NC = (I % I.M)
 r = Silence(1)
 l = Continuation(1)
 
 # Chord scale
-c0 = Note('c', 0, 0, 1)  # b0 represents the first note in the chord.extension_notes
+c0 = Note('c', 0, 0, 1)  # c0 represents the first note in the chord.chord_notes
 c1 = Note('c', 1, 0, 1)
 c2 = Note('c', 2, 0, 1)
 c3 = Note('c', 3, 0, 1)
 c4 = Note('c', 4, 0, 1)
 c5 = Note('c', 5, 0, 1)
 c6 = Note('c', 6, 0, 1)
 c7 = Note('c', 7, 0, 1)
 c8 = Note('c', 8, 0, 1)
 c9 = Note('c', 9, 0, 1)
 c10 = Note('c', 10, 0, 1)
 c11 = Note('c', 11, 0, 1)
 
+cu0 = Note('cu', 0, 0, 1)
+cu1 = Note('cu', 1, 0, 1)
+cu2 = Note('cu', 2, 0, 1)
+cu3 = Note('cu', 3, 0, 1)
+cu4 = Note('cu', 4, 0, 1)
+cu5 = Note('cu', 5, 0, 1)
+cu6 = Note('cu', 6, 0, 1)
+cu7 = Note('cu', 7, 0, 1)
+cu8 = Note('cu', 8, 0, 1)
+cu9 = Note('cu', 9, 0, 1)
+cu10 = Note('cu', 10, 0, 1)
+cu11 = Note('cu', 11, 0, 1)
+
+cd0 = Note('cd', 0, 0, 1)
+cd1 = Note('cd', 1, 0, 1)
+cd2 = Note('cd', 2, 0, 1)
+cd3 = Note('cd', 3, 0, 1)
+cd4 = Note('cd', 4, 0, 1)
+cd5 = Note('cd', 5, 0, 1)
+cd6 = Note('cd', 6, 0, 1)
+cd7 = Note('cd', 7, 0, 1)
+cd8 = Note('cd', 8, 0, 1)
+cd9 = Note('cd', 9, 0, 1)
+cd10 = Note('cd', 10, 0, 1)
+cd11 = Note('cd', 11, 0, 1)
+
+
 # Scale
 s0 = Note('s', 0, 0, 1)
 s1 = Note('s', 1, 0, 1)
 s2 = Note('s', 2, 0, 1)
 s3 = Note('s', 3, 0, 1)
 s4 = Note('s', 4, 0, 1)
 s5 = Note('s', 5, 0, 1)
@@ -55,14 +83,41 @@
 b6 = Note('b', 6, 0, 1)
 b7 = Note('b', 7, 0, 1)
 b8 = Note('b', 8, 0, 1)
 b9 = Note('b', 9, 0, 1)
 b10 = Note('b', 10, 0, 1)
 b11 = Note('b', 11, 0, 1)
 
+bu0 = Note('bu', 0, 0, 1)  # b0 represents the first note in the chord.extension_notes
+bu1 = Note('bu', 1, 0, 1)  # b1 represents the second note in the chord.extension_notes
+bu2 = Note('bu', 2, 0, 1)
+bu3 = Note('bu', 3, 0, 1)
+bu4 = Note('bu', 4, 0, 1)
+bu5 = Note('bu', 5, 0, 1)
+bu6 = Note('bu', 6, 0, 1)
+bu7 = Note('bu', 7, 0, 1)
+bu8 = Note('bu', 8, 0, 1)
+bu9 = Note('bu', 9, 0, 1)
+bu10 = Note('bu', 10, 0, 1)
+bu11 = Note('bu', 11, 0, 1)
+
+bd0 = Note('bd', 0, 0, 1)  # b0 represents the first note in the chord.extension_notes
+bd1 = Note('bd', 1, 0, 1)  # b1 represents the second note in the chord.extension_notes
+bd2 = Note('bd', 2, 0, 1)
+bd3 = Note('bd', 3, 0, 1)
+bd4 = Note('bd', 4, 0, 1)
+bd5 = Note('bd', 5, 0, 1)
+bd6 = Note('bd', 6, 0, 1)
+bd7 = Note('bd', 7, 0, 1)
+bd8 = Note('bd', 8, 0, 1)
+bd9 = Note('bd', 9, 0, 1)
+bd10 = Note('bd', 10, 0, 1)
+bd11 = Note('bd', 11, 0, 1)
+
+
 
 # Absolute notes
 a0 = Note('a', 0, 0, 1)
 a1 = Note('a', 1, 0, 1)
 a2 = Note('a', 2, 0, 1)
 a3 = Note('a', 3, 0, 1)
 a4 = Note('a', 4, 0, 1)
@@ -102,19 +157,19 @@
 hh = Note('d', 6, -2, 1)  # Bass tom
 lt = Note('d', 7, -2, 1)  # Low tom
 ch = Note('d', 8, -2, 1)  # Closed hat
 mt = Note('d', 9, -2, 1)  # Medium tom
 oh = Note('d', 10, -2, 1)  # Open hat
 ht = Note('d', 11, -2, 1)  # High tom
 
-dr000 = Note('d', 0, -1, 1)
-dr010 = Note('d', 1, -1, 1)
-dr020 = Note('d', 2, -1, 1)
-dr030 = Note('d', 3, -1, 1)
-dr040 = Note('d', 4, -1, 1)
+hht = Note('d', 0, -1, 1)
+crash = Note('d', 1, -1, 1)
+other_hht = Note('d', 2, -1, 1)
+ride = Note('d', 3, -1, 1)
+ride_hard = Note('d', 4, -1, 1)
 dr050 = Note('d', 5, -1, 1)
 dr060 = Note('d', 6, -1, 1)
 dr070 = Note('d', 7, -1, 1)
 dr080 = Note('d', 8, -1, 1)
 dr090 = Note('d', 9, -1, 1)
 dr100 = Note('d', 10, -1, 1)
 dr110 = Note('d', 11, -1, 1)
@@ -468,14 +523,15 @@
     "sus2": (s2, s1),
     "sus4": (s2, s3),
     "+": (s4, h8),
     "b5": (s4, h6),
     "m3": (s2, h3),
     "M3": (s2, h4),
     "m6": (s5, h8),
+    "M2": (s2, h2),
     "M6": (s5, h9),
     "m7": (s6, h10),
     "M7": (s6, h11),
     "m9": (s1, h1),
     "M9": (s1, h2),
     "#11": (s3, h6),
     "m13": (s5, h8),
@@ -491,14 +547,15 @@
     "-11": s3
 }
 
 DICT_ADDITION = {
     "add2": (s0, s1),
     "add4": (s2, s3),
     "add6": (s4, s5),
+    "add7": (s4, s6),
     "add9": (s0, s1.o(1)),
     "add11": (s2, s3.o(1)),
     "add13": (s4, s5.o(1)),
     "+": (s4, h8),
     "m2": (s0, h1),
     "M2": (s0, h2),
     "m3": (s2, h3),
@@ -508,10 +565,11 @@
     "m7": (s4, h10),
     "M7": (s4, h11),
     "m9": (s0, h1.o(1)),
     "M9": (s0, h3.o(1)),
     "m10": (s2, h3.o(1)),
     "M10": (s2, h4.o(1)),
     "#11": (s4, h6.o(1)),
+    "#4": (s4, h6),
     "m13": (s4, s5.o(1)),
     "M13": (s4, s5.o(1))
 }
```

### Comparing `musiclang-0.8.1/musiclang/write/note.py` & `musiclang-0.8.2/musiclang/write/note.py`

 * *Files 15% similar despite different names*

```diff
@@ -79,14 +79,25 @@
     Accident
     ---------
 
     You can force an accident on a note choosing between : ['min', 'maj', 'dim', 'aug', 'natural']
     It is used to force a specific interval that is robust to transposition, but keeping a diatonic value.
     It is advised to be used in replacement of h-type notes because it is in general more compatible with transformations.
 
+    Tempo
+    -----
+
+    You can set a new tempo when this note is played, it will be played
+
+
+    Pedal
+    -----
+
+    You can set the pedal on or off when this note is played, it will be applied to the whole instrument, not a single part
+
     Examples
     --------
     >>> from musiclang.library import s0, s1, s2, I
 
     You can learn what pitch is associated to a note in the context of a chord :
 
     >>> chord = (I % I.M) # C major chord (first degree of first major tonality relative to C)
@@ -106,25 +117,28 @@
     3
 
     In minor s2 is eb (=3)
 
 
 
     """
+    DEFAULT_AMP = 66
 
-    def __init__(self, type, val, octave, duration, mode=None, accident=None, amp=66, tags=None):
+    def __init__(self, type, val, octave, duration, mode=None, accident=None, amp=DEFAULT_AMP, tags=None, pedal=None, tempo=None):
         self.type = type
         self.val = val
         self.octave = octave
         self.duration = duration
         self.amp = amp
         self.accident = accident
         self.mode = mode
         self.properties = self.init_properties()
         self.tags = tags if tags is not None else set()
+        self.pedal = pedal
+        self.tempo = tempo
 
     def has_tag(self, tag):
         """
         Check if the tag exists for this note
         Returns a copy of the object
         Parameters
         ----------
@@ -167,14 +181,131 @@
         note: Note
 
         """
         cp = self.copy()
         cp.tags = cp.tags.union(set(tags))
         return cp
 
+    @property
+    def interpolate(self):
+        return self.add_tag('interpolate')
+
+    @property
+    def accent(self):
+        return self.add_tag('accent')
+
+    @property
+    def mordant(self):
+        return self.add_tag('mordant')
+
+    @property
+    def chroma_mordant(self):
+        return self.add_tag('chroma_mordant')
+
+    @property
+    def inv_chroma_mordant(self):
+        return self.add_tag('inv_chroma_mordant')
+
+
+    @property
+    def inv_mordant(self):
+        return self.add_tag('inv_mordant')
+
+    @property
+    def grupetto(self):
+        return self.add_tag('grupetto')
+
+    @property
+    def inv_grupetto(self):
+        return self.add_tag('inv_grupetto')
+
+    @property
+    def chroma_grupetto(self):
+        return self.add_tag('chroma_grupetto')
+
+    @property
+    def inv_chroma_grupetto(self):
+        return self.add_tag('inv_chroma_grupetto')
+
+    @property
+    def roll(self):
+        return self.add_tag('roll')
+
+    @property
+    def roll_fast(self):
+        return self.add_tag('roll_fast')
+
+    @property
+    def suspension_prev(self):
+        return self.add_tag('suspension_prev')
+
+    @property
+    def suspension_prev_repeat(self):
+        return self.add_tag('suspension_prev_repeat')
+
+    @property
+    def retarded(self):
+        return self.add_tag('retarded')
+
+    def realize_tags(self, last_note=None, next_note=None):
+        from .ornementation import realize_tags
+
+        return realize_tags(self, last_note, next_note)
+
+
+
+
+    def set_tempo(self, tempo):
+        new_note = self.copy()
+        new_note.tempo = tempo
+        return new_note
+
+    @property
+    def pedal_on(self):
+        new_note = self.copy()
+        new_note.pedal = True
+        return new_note
+
+    @property
+    def pedal_off(self):
+        new_note = self.copy()
+        new_note.pedal = False
+        return new_note
+
+    def remove_effects(self):
+        """
+        Remove pedals and tempo change
+        Returns
+        -------
+        """
+        new_note = self.copy()
+        new_note.tempo = None
+        new_note.pedal = None
+        return new_note
+
+    def remove_tempo(self):
+        """
+        Remove tempo change
+        Returns
+        -------
+        """
+        new_note = self.copy()
+        new_note.tempo = None
+        return new_note
+
+    def remove_pedal(self):
+        """
+        Remove pedal
+        Returns
+        -------
+        """
+        new_note = self.copy()
+        new_note.pedal = None
+        return new_note
+
     def remove_tags(self, tags):
         """
         Remove several tags from the object.
         Returns a copy of the object
 
         Parameters
         ----------
@@ -186,14 +317,16 @@
 
 
         """
         cp = self.copy()
         cp.tags = cp.tags - set(tags)
         return cp
 
+    def clear_note_tags(self):
+        return self.clear_tags()
 
     def remove_tag(self, tag):
         """
         Remove a tag from this object
         Returns a copy of the object
         Parameters
         ----------
@@ -230,15 +363,15 @@
         """
 
         If the note has a mode
 
         Parameters
         ----------
         chord :
-            
+
 
         Returns
         -------
 
         """
         new_chord = chord.copy()
         if self.mode is None:
@@ -302,72 +435,92 @@
     def init_properties(self):
         """ """
         from .properties.note_properties import NoteProperties
         return NoteProperties(self)
 
     def copy(self):
         """ """
-        return Note(self.type, self.val, self.octave, self.duration, mode=self.mode, accident=self.accident, amp=self.amp, tags=set(self.tags))
+        return Note(self.type, self.val, self.octave, self.duration, mode=self.mode, accident=self.accident,
+                    amp=self.amp, tags=set(self.tags),
+                    tempo=self.tempo,
+                    pedal=self.pedal
+                    )
+
+    def set_amp(self, amp):
+        new_note = self.copy()
+        if isinstance(amp, float):
+            amp = int(amp)
+        if isinstance(amp, int):
+            new_note.amp = amp
+        elif isinstance(amp, str):
+            return self.__getattr__(amp)
+
+        return new_note
 
     def set_val(self, val):
         note = self.copy()
         note.val = val
         return note
 
     def set_duration(self, value):
         """
         Set the duration of a note
         Parameters
         ----------
         value :
-            
+
 
         Returns
         -------
 
         """
+        if isinstance(value, float):
+            value = frac(value).limit_denominator(8)
         result = self.copy()
         result.duration = value
         return result
 
     def augment(self, value):
         """
         Returns a copy with augmented duration (multiply current duration by the value)
 
         Parameters
         ----------
         value : fractions.Fraction
                 Fraction on which to multiply the current duration
-            
+
 
         Returns
         -------
         note: Note
               New note with increased duration
 
         Examples
         --------
 
         >>> from musiclang.library import s0
         >>> from fractions import Fraction
-        >>> s0.augment(Fraction(8, 9))
-        s0.augment(frac(8, 9))
+        >>> s0.augment(Fraction(8, 7))
+        s0.augment(frac(8, 7))
 
         """
+        if isinstance(value, float):
+            value = frac(value).limit_denominator(8)
+
         result = self.copy()
         result.duration *= value
         return result
 
     def change_type(self, new_type):
         """
 
         Parameters
         ----------
         new_type :
-            
+
 
         Returns
         -------
 
         """
         c = self.copy()
         c.type = new_type
@@ -375,15 +528,15 @@
 
     def add_interval(self, note):
         """
 
         Parameters
         ----------
         note :
-            
+
 
         Returns
         -------
 
         """
         if note.type[1] not in ['u', 'd']:
             raise Exception('note argument must be a relative type (*u, *d)')
@@ -393,17 +546,17 @@
 
     def add_value(self, val, octave):
         """
 
         Parameters
         ----------
         val :
-            
+
         octave :
-            
+
 
         Returns
         -------
 
         """
         if self.type[0] in ['s', 'h', 'c']:
             if self.type[0] == 's':
@@ -427,15 +580,15 @@
 
     def oabs(self, octave):
         """
 
         Parameters
         ----------
         octave :
-            
+
 
         Returns
         -------
 
         """
         note = self.copy()
         note.octave += octave
@@ -453,36 +606,74 @@
 
         Returns
         -------
         note: Note
             It will return a new note transposed
 
         """
-        if self.type in ['s', 'h', 'c', 'b']:
+        if self.type in ['s', 'h', 'c', 'b', 'a', 'x']:
             return self.oabs(octave)
         return self.copy()
 
+    def __or__(self, other):
+        return self.to_melody() | other
+
+
     def duration_to_str(self):
         """ """
         return DURATION_TO_STR[self.duration]
 
 
     def to_drum(self):
         note = self.copy()
-        note.type = 'd'
+        if not note.is_silence and not note.is_continuation:
+            note.type = 'd'
         return note
 
     @property
     def base_octave(self):
         return 5
 
     @property
     def is_drum(self):
         return self.type == 'd'
 
+    def replace(self, to_replace, new_note, octave=False, amp=False, add_octave=True):
+        """
+        Replace a note by another note
+
+        Parameters
+        ----------
+        to_replace :
+
+        new_note :
+
+
+        Returns
+        -------
+
+        """
+
+        note = self
+        to_add = note.copy()
+        test = note.val == to_replace.val and note.type == to_replace.type
+        test &= (note.octave == to_replace.octave) or not octave
+        if test:
+            to_add.type = new_note.type
+            to_add.val = new_note.val
+            to_add.octave = new_note.octave
+            if not octave:
+                to_add.octave += note.octave
+            to_add.mode = new_note.mode
+            to_add.accident = new_note.accident
+            if amp:
+                to_add.amp = note.amp
+
+        return to_add
+
     def to_code(self):
         """
         Represent a note as valid python code using standard musiclang library
 
         Parameters
         ----------
 
@@ -493,37 +684,45 @@
 
         """
 
         if self.is_note:
             result = f"{self.type}{self.val}"
         elif self.is_drum:
             result = DRUMS_DICT.get((self.val, self.octave), 'r')
+        elif self.type == 'x':
+            result = f"{self.type}{self.val}"
         else:
             result = f"{self.type}"
 
         if self.duration != Q:
             if self.duration in DURATION_TO_STR:
                 duration = DURATION_TO_STR[self.duration]
                 result += f".{duration}"
             else:
                 if isinstance(self.duration, int):
                     result += f".augment({self.duration}))"
                 else:
                     result += f".augment(frac({self.duration.numerator}, {self.duration.denominator}))"
 
         if self.octave != 0 and self.is_note:
-            result += f".o({self.octave})"
+            if not self.is_relative:
+                result += f".o({self.octave})"
+            else:
+                result += f".oabs({self.octave})"
+
         if self.mode is not None and self.is_note:
             result += f".{self.mode}"
         if self.accident is not None and self.is_note:
             result += f".{self.accident}"
-        if self.is_note:
+        if self.is_note or self.type == "x":
             amp_figure = self.amp_figure
             if amp_figure != 'mf':
                 result += f".{self.amp_figure}"
+        if len(self.tags) > 0:
+            result += f".add_tags({self.tags})"
 
         return result
 
 
     def remove_accidents(self):
         new_note = self.copy()
         new_note.accident = None
@@ -541,15 +740,15 @@
         Transform in a list of [(start_time, end_time, pitch, self)]
 
         Parameters
         ----------
         chord : Chord
             Chord on which the note will be played
 
-            
+
         inst : str
             Instrument on which the note will be played
 
         Returns
         -------
         A List of list with one element
 
@@ -571,14 +770,16 @@
     def repr_mode(self):
         """ """
         if self.mode is not None:
             return f".{self.mode}"
 
         return ""
 
+
+
     def __repr__(self):
         return self.to_code()
 
     def __len__(self):
         return 1
 
     def __add__(self, other):
@@ -617,15 +818,15 @@
         Examples
         --------
 
         >>> from musiclang.library import *
         >>> s0 & 2
         s2
         """
-        if self.type in ['s', 'c', 'h']:
+        if self.type in ['s', 'h']:
             return self.add_value(n, 0)
         elif self.type in ['h']:
             return self.add_value((12 * n) // 7, 0)
         else:
             return self.copy()
 
     def __matmul__(self, other):
@@ -662,14 +863,84 @@
         new_note = self.copy()
         new_note.type = 'd'
         pitch = chord.to_pitch(self)
         new_note.val = pitch % 12
         new_note.octave = pitch // 12
         return new_note
 
+    def to_standard_note(self, chord):
+        if self.type in ['b', 'c']:
+            if self.is_bass_note:
+                candidates = chord.extension_notes
+            elif self.is_chord_note:
+                candidates = chord.chord_notes
+            else:
+                raise Exception('Not existing type')
+            val = self.val
+            octave = self.octave
+            new_note = candidates[val % len(candidates)].o((val // len(candidates)) + octave)
+            new_note = new_note.set_duration(self.duration)
+            new_note.amp = self.amp
+            return new_note
+
+        elif self.type in ['a']:
+            new_note = self.copy()
+            base_note = chord.parse(chord.to_pitch(self))
+            new_note.type = base_note.type
+            new_note.val = base_note.val
+            new_note.octave = base_note.octave
+            return new_note
+        else:
+            return self
+
+    def to_absolute_note(self, chord):
+        if not self.is_note:
+            return self.copy()
+        pitch = chord.to_pitch(self)
+        new_note = self.copy()
+        new_note.type = 'a'
+        new_note.val = pitch % 12
+        new_note.octave = pitch // 12
+
+        return new_note
+
+    def as_key(self, octave=False, duration=False, amp=False):
+        oct = self.octave if octave else 0
+        duration = self.duration if duration else 1
+        amp = self.amp if amp else 66
+        return Note(self.type, self.val, oct, duration, mode=self.mode, amp=amp, accident=self.accident)
+
+
+    def to_extension_note(self, chord):
+        candidates = chord.extension_notes
+        candidates_without_octave = [c.o(-c.octave) for c in candidates]
+        try:
+            idx = candidates_without_octave.index(self.as_key())
+            note = candidates[idx]
+            to_return = self.copy()
+            to_return.type = 'b'
+            to_return.val = idx
+            to_return.octave -= note.octave
+            return to_return
+        except:
+            return self.copy()
+
+    def to_chord_note(self, chord):
+        candidates = chord.chord_notes
+        candidates_without_octave = [c.o(-c.octave) for c in candidates]
+        try:
+            idx = candidates_without_octave.index(self.as_key())
+            note = candidates[idx]
+            to_return = self.copy()
+            to_return.type = 'c'
+            to_return.val = idx
+            to_return.octave -= note.octave
+            return to_return
+        except:
+            return self.copy()
 
 
     def __hash__(self):
         return hash(self.__repr__())
 
     def __eq__(self, other):
         """
@@ -741,28 +1012,28 @@
 class Silence(Note):
     """
     Represents a silence in MusicLang.
 
     Only takes a duration as a parameter
     """
 
-    def __init__(self, duration, tags=None):
-        super().__init__("r", 0, 0, duration, tags=tags)
+    def __init__(self, duration, tags=None, tempo=None, pedal=None):
+        super().__init__("r", 0, 0, duration, tags=tags, tempo=tempo, pedal=pedal)
 
     def copy(self):
         """ """
-        return Silence(self.duration, tags=set(self.tags))
+        return Silence(self.duration, tempo=self.tempo, pedal=self.pedal, tags=set(self.tags))
 
 
 class Continuation(Note):
     """
     Represents a continuation in MusicLang.
 
     Only takes a duration as a parameter
     """
 
-    def __init__(self, duration, tags=None):
-        super().__init__("l", 0, 0, duration, tags=tags)
+    def __init__(self, duration, tags=None, tempo=None, pedal=None):
+        super().__init__("l", 0, 0, duration, tempo=tempo, pedal=pedal, tags=tags)
 
     def copy(self):
         """ """
-        return Continuation(self.duration, tags=set(self.tags))
+        return Continuation(self.duration, pedal=self.pedal, tags=set(self.tags))
```

### Comparing `musiclang-0.8.1/musiclang/write/note_pitch.py` & `musiclang-0.8.2/musiclang/write/note_pitch.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 class NotePitch:
     """ """
 
-    def __init__(self, pitch, offset=0, duration=1, velocity=120, track=0, silence=0, continuation=0):
+    def __init__(self, pitch, offset=0, duration=1, velocity=120, track=0, silence=0, continuation=0,
+                 tempo=None, pedal=None
+                 ):
         self.pitch = pitch
         self.offset = offset
         self.duration = duration
         self.velocity = velocity
         self.track = track
         self.silence = silence
         self.continuation = continuation
+        self.tempo = tempo
+        self.pedal = pedal
 
 
     def is_note(self):
         """ """
         return not (self.silence or self.continuation)
 
     def to_midi_note(self):
         """ """
-        return [self.pitch, self.offset, self.duration, self.velocity, self.track, self.silence, self.continuation]
+        return [self.pitch, self.offset, self.duration, self.velocity, self.track, self.silence, self.continuation,
+                self.tempo, self.pedal
+                ]
```

### Comparing `musiclang-0.8.1/musiclang/write/out/constants.py` & `musiclang-0.8.2/musiclang/write/out/constants.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/out/midi_utils.py` & `musiclang-0.8.2/musiclang/write/out/midi_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,32 @@
     -------
 
     """
     instrument_of_voice = instruments.get(voice, 0)
     return instrument_list.index(instrument_of_voice)
 
 
-def matrix_to_mid(matrix, output_file=None, ticks_per_beat=480, tempo=120, instruments={}, instrument_names=None, **kwargs):
+
+def matrix_to_events(matrix, 
+                     output_file=None, 
+                     ticks_per_beat=480, 
+                     tempo=120, 
+                     instruments={}, 
+                     time_signature=(4, 4),
+                     instrument_names=None):
+    matrix = np.asarray(matrix)
+    events = [] # [(time, instrument, duration, message)]
+    for el in matrix:
+        pitch, offset, duration, velocity, track, silence, continuation, tempo, pedal = el
+        # Add note on, note off for each track
+
+    return events
+
+def matrix_to_mid(matrix, output_file=None, ticks_per_beat=480, tempo=120, instruments={}, time_signature=(4, 4),
+                  instrument_names=None, **kwargs):
     """
 
     Parameters
     ----------
     matrix :
         
     output_file :
@@ -49,20 +66,19 @@
     Returns
     -------
 
     """
     if instrument_names is None:
         instrument_names = []
     from mido import MidiFile, MidiTrack, Message, MetaMessage
-    from ..constants import SILENCE, CONTINUATION, PITCH, TRACK, OFFSET, VELOCITY, DURATION
+    from ..constants import SILENCE, CONTINUATION, PITCH, TRACK, OFFSET, VELOCITY, DURATION, TEMPO, PEDAL
     from .constants import OCTAVES
     import os
 
     matrix = np.asarray(matrix)
-
     def number_to_channel(n):
         """
 
         Parameters
         ----------
         n :
             
@@ -105,47 +121,71 @@
         mid.tracks.append(track)
 
     if isinstance(output_file, str):
         mid.tracks[0].append(MetaMessage("track_name", name=os.path.split(output_file)[1], time=int(0)))
     else:
         mid.tracks[0].append(MetaMessage("track_name", name='track', time=int(0)))
     mid.tracks[0].append(MetaMessage("set_tempo", tempo=(480000 * 120) // tempo, time=int(0)))
-    mid.tracks[0].append(MetaMessage("time_signature", numerator=4, denominator=4, time=int(0)))
+    mid.tracks[0].append(MetaMessage("time_signature", numerator=time_signature[0], denominator=time_signature[1], time=int(0)))
+
+
 
     sort_events = []
     last_silence = True
     for row in matrix:
         pitch = row[PITCH] + 60 + 12 * OCTAVES.get(instruments.get(row[TRACK], 0), 0)
         row = row.tolist()
         if row[SILENCE]:
             last_silence = True
+            sort_events.append([0, 2, row[OFFSET], row[TEMPO], row[PEDAL], row[TRACK]])
             continue
+
+        if row[CONTINUATION]:
+            sort_events.append([0, 2, row[OFFSET], row[TEMPO], row[PEDAL], row[TRACK]])
+
         if row[CONTINUATION] == 0:
             sort_events.append([pitch,
-                                1, row[OFFSET], row[VELOCITY], row[TRACK]])
+                                1, row[OFFSET], row[VELOCITY], row[TRACK], row[TEMPO], row[PEDAL]])
 
         if not (row[CONTINUATION] and last_silence):
-            sort_events.append([pitch, 0, (row[OFFSET] + row[DURATION]), row[TRACK], row[CONTINUATION]])
+            sort_events.append([pitch, 0, (row[OFFSET] + row[DURATION]), row[TRACK], row[CONTINUATION],
+                                row[TEMPO], row[PEDAL]
+                                ])
             last_silence = False
 
     sort_events.sort(key=lambda tup: tup[2])
     from fractions import Fraction as frac
-
+    current_tempo = tempo
+    current_pedal = None
     lapso = {idx: 0 for idx in range(nb_tracks + 1)}
     prev_pitch = {idx: 0 for idx in range(nb_tracks + 1)}
     for evt in sort_events:
         if evt[1] == 1:
             vel = int(evt[3])
             track_nb = int(evt[4])
             track = mid.tracks[track_nb]
             if evt[0] > 100 or evt[0] < 10:
                 evt[0] = 0
                 vel = 0
+
+            real_time = int((evt[2] - lapso[track_nb]) * ticks_per_beat)
+
             track.append(Message('note_on', note=int(evt[0]), channel=channels[track_nb],
-                                 velocity=vel, time=int((evt[2] - lapso[track_nb]) * ticks_per_beat)))
+                                 velocity=vel, time=real_time))
+
+            if evt[5] is not None and evt[5] != current_tempo:
+                real_tempo =(480000 * 120) // evt[5]
+                track.append(MetaMessage("set_tempo", tempo=real_tempo, time=int(0)))
+                current_tempo = evt[5]
+
+            if evt[6] is not None and evt[6]:
+                track.append(Message('control_change', value=127, channel=channels[track_nb], control=4, time=int(0)))
+
+            if evt[6] is not None and not evt[6]:
+                track.append(Message('control_change', value=0, channel=channels[track_nb], control=4, time=int(0)))
 
             lapso[track_nb] = evt[2]
             prev_pitch[track_nb] = int(evt[0])
         elif evt[1] == 0:
             track_nb = int(evt[3])
             track = mid.tracks[track_nb]
             if evt[0] > 100 or evt[0] < 10:
@@ -156,14 +196,32 @@
 
 
             else:
                 track.append(Message('note_off', note=int(evt[0]), channel=channels[track_nb],
                                      velocity=0, time=int((evt[2] - lapso[track_nb]) * ticks_per_beat)))
             lapso[track_nb] = evt[2]
 
+        elif evt[1] == 2:
+            track_nb = int(evt[5])
+            track = mid.tracks[track_nb]
+            tempo_change = evt[3]
+            pedal_change = evt[4]
+
+            if tempo_change is not None and tempo_change != current_tempo:
+                real_tempo = (480000 * 120) // tempo_change
+                track.append(MetaMessage("set_tempo", tempo=real_tempo, time=int(0)))
+                current_tempo = tempo_change
+
+            if pedal_change is not None and pedal_change:
+                track.append(Message('control_change', value=127, channel=channels[track_nb], control=4, time=int(0)))
+
+            if pedal_change is not None and not pedal_change:
+                track.append(Message('control_change', value=0, channel=channels[track_nb], control=4, time=int(0)))
+
+
     if output_file is not None:
         for track in mid.tracks:
             track.append(MetaMessage('end_of_track', time=(int(0))))
         if isinstance(output_file, str):
             mid.save(output_file)
         else:
             mid.save(file=output_file)
```

### Comparing `musiclang-0.8.1/musiclang/write/out/to_code.py` & `musiclang-0.8.2/musiclang/write/out/to_code.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/out/to_mxl.py` & `musiclang-0.8.2/musiclang/write/out/to_mxl.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     2: ['D', 'E', 'F#', 'G', 'A', 'B', 'C#'],
     3: ['Eb', 'F', 'G', 'Ab', 'Bb', 'C', 'D'],
     4: ['E', 'F#', 'G#', 'A', 'B', 'C#', 'D#'],
     5: ['F', 'G', 'A', 'Bb', 'C', 'D', 'E'],
     6: ['Gb', 'Ab', 'Bb', 'Cb', 'Db', 'Eb', 'F'],
     7: ['G', 'A', 'B', 'C', 'D', 'E', 'F#'],
     8: ['Ab', 'Bb', 'C', 'Db', 'Eb', 'F', 'G'],
-    9: ['A', 'B', 'C#', 'D#', 'E', 'F#', 'G#'],
+    9: ['A', 'B', 'C#', 'D', 'E', 'F#', 'G#'],
     10: ['Bb', 'C', 'D', 'Eb', 'F', 'G', 'A'],
     11: ['B', 'C#', 'D#', 'E', 'F#', 'G#', 'A#']
 }
 
 
 SCALES_MINOR = {
     0: ['C', 'D', 'Eb', 'F', 'G', 'Ab', 'B'],
@@ -35,16 +35,32 @@
     7: ['G', 'A', 'Bb', 'C', 'D', 'Eb', 'F#'],
     8: ['G#', 'A#', 'B', 'C#', 'D#', 'E', 'F##'],
     9: ['A', 'B', 'C', 'D', 'E', 'F', 'G#'],
     10: ['Bb', 'C', 'Db', 'Eb', 'F', 'Gb', 'A'],
     11: ['B', 'C#', 'D', 'E', 'F#', 'G', 'A#']
 }
 
+SCALES_MELODIC_MINOR = {
+    0: ['C', 'D', 'Eb', 'F', 'G', 'A', 'B'],
+    1: ['C#', 'D#', 'E', 'F#', 'G#', 'A#', 'B#'],
+    2: ['D', 'E', 'F', 'G', 'A', 'B', 'C#'],
+    3: ['Eb', 'F', 'Gb', 'Ab', 'Bb', 'C', 'D'],
+    4: ['E', 'F#', 'G', 'A', 'B', 'C#', 'D#'],
+    5: ['F', 'G', 'Ab', 'Bb', 'C', 'D', 'E'],
+    6: ['F#', 'G#', 'A', 'B', 'C#', 'D#', 'E#'],
+    7: ['G', 'A', 'Bb', 'C', 'D', 'E', 'F#'],
+    8: ['G#', 'A#', 'B', 'C#', 'D#', 'E#', 'F##'],
+    9: ['A', 'B', 'C', 'D', 'E', 'F#', 'G#'],
+    10: ['Bb', 'C', 'Db', 'Eb', 'F', 'G', 'A'],
+    11: ['B', 'C#', 'D', 'E', 'F#', 'G#', 'A#']
+}
+
 SCALES = {
     'm': SCALES_MINOR,
+    'mm': SCALES_MELODIC_MINOR,
     'M': SCALES_MAJOR
 }
 
 
 def get_note_spelling(note, chord, last_pitch=None):
     from .to_midi import note_to_pitch_result
     degree = chord.degree
@@ -55,14 +71,16 @@
     if (pitch % 12) in tonality_scale_pitches:
         idx = tonality_scale_pitches.index(pitch % 12)
         note_spelling = SCALES[mode][tonality_degree][idx]
         # Correct octave
         octave = (pitch + 48) // 12
         if note_spelling in ['B#']:
             octave -= 1
+        elif note_spelling in ['Cb']:
+            octave += 1
         note_spelling = note_spelling + str(octave)
         new_note = music21.note.Note(note_spelling)
         new_note.duration = music21.duration.Duration(note.duration)
     else:
         new_note = music21.note.Note(pitch % 12)
         new_note.octave = (pitch + 48) // 12
         new_note.duration = music21.duration.Duration(note.duration)
@@ -136,15 +154,15 @@
             part.append(instr)
 
         part = parts_dict[ins]
         parts_dict_names[part_name] = part
 
     return parts_dict_names, parts_dict
 
-def score_instrument_to_notes(score, part_name, voice, voice_idx):
+def score_instrument_to_notes(score, part_name, voice, voice_idx, no_repeat=False):
     """
     Given a score and a part name, returns the music21 voice with all the notes
 
     Parameters
     ----------
     score: Score
     part_name: str
@@ -152,17 +170,27 @@
     voice_idx: int
 
     Returns
     -------
     voice: music21.Voice
 
     """
+    last_spelling = None
+    last_pitch = None
+    last_is_silence = True
+    curr_dynamic = 'mf'
     for chord in score.chords:
-        voice = chord_instrument_to_notes(chord, voice, part_name, voice_idx)
-
+        voice, last_spelling, curr_dynamic, last_pitch, last_is_silence = chord_instrument_to_notes(chord, voice, part_name,
+                                                                       voice_idx,
+                                                                       last_spelling=last_spelling,
+                                                                       curr_dynamic=curr_dynamic,
+                                                                       no_repeat=no_repeat,
+                                                                       last_pitch=last_pitch,
+                                                                       last_is_silence=last_is_silence
+                                                                       )
     return voice
 
 
 def chord_to_musescore_lyric(chord: Chord):
     """
     Create the chord scale symbol on the score
 
@@ -174,57 +202,83 @@
     -------
     result: str
         Chord scale symbol
     """
     return "{} /{}".format(chord.element_to_str(), chord.tonality_to_str()).replace('%', '')
 
 
-def chord_instrument_to_notes(chord, voice, part_name, ins_idx):
+def chord_instrument_to_notes(chord, voice, part_name, ins_idx, last_spelling=None, curr_dynamic='mf', no_repeat=False,
+                              last_pitch=None, last_is_silence=True):
     """
     Given a chord, get spellings
 
     Returns
     -------
     """
 
     # Enharmonic
-
-    last_pitch = None
-    last_spelling = None
-    curr_dynamic = 0
+    old_last_is_silence = last_is_silence
+    last_is_silence = False
+    FIGURES = ['n', 'ppp', 'pp', 'p', 'mp', 'mf', 'f', 'ff', 'fff']
     if part_name in chord.score.keys():
         part = chord.score[part_name]
-
         for idx_note, n in enumerate(part.notes):
             if n.is_note:
+                old_last_pitch = last_pitch
                 new_note, last_pitch = get_note_spelling(n, chord, last_pitch=last_pitch)
                 last_spelling = new_note.nameWithOctave
                 if idx_note == 0 and ins_idx == 0:
                     new_note.addLyric(chord_to_musescore_lyric(chord))
-                if n.amp != curr_dynamic:
-                    dyn = dynamics.Dynamic(n.amp / 120)
+                if n.amp_figure != curr_dynamic:
+                    dyn = dynamics.Dynamic(n.amp_figure)
                     voice.append(dyn)
-                    curr_dynamic = n.amp
-                voice.append(new_note)
+                    curr_dynamic = n.amp_figure
+                if (last_pitch != old_last_pitch) or (not no_repeat):
+                    voice.append(new_note)
+                else:
+                    try:
+                        if last_spelling is not None and not last_is_silence:
+                            new_note = note.Note(last_spelling)
+                            new_note.duration = music21.duration.Duration(n.duration)
+                            voice[-1].tie = tie.Tie('start')
+                            new_note.tie = tie.Tie('stop')
+                            voice.append(new_note)
+                        else:
+                            voice.append(note.Rest(n.duration))
+                            last_is_silence = True
+                    except:
+                        voice.append(note.Rest(n.duration))
+                        last_is_silence = True
             elif n.is_silence:
                 voice.append(note.Rest(n.duration))
+                last_is_silence = True
             elif n.is_continuation:
-                new_note = note.Note(last_spelling)
-                new_note.duration = music21.duration.Duration(n.duration)
-                voice[-1].tie = tie.Tie('start')
-                new_note.tie = tie.Tie('stop')
-                voice.append(new_note)
+                if old_last_is_silence:
+                    last_is_silence = True
+                try:
+                    if last_spelling is not None and not last_is_silence:
+                        new_note = note.Note(last_spelling)
+                        new_note.duration = music21.duration.Duration(n.duration)
+                        voice[-1].tie = tie.Tie('start')
+                        new_note.tie = tie.Tie('stop')
+                        voice.append(new_note)
+                    else:
+                        voice.append(note.Rest(n.duration))
+                        last_is_silence = True
+                except:
+                    voice.append(note.Rest(n.duration))
+                    last_is_silence = True
 
     else:
         voice.append(note.Rest(chord.duration))
 
-    return voice
+    return voice, last_spelling, curr_dynamic, last_pitch, last_is_silence
 
 
-def score_to_music_21(score, signature=(4, 4), tempo=50, tonality=None, title='MusicLang score', composer='MusicLang', **kwargs):
+def score_to_music_21(score, signature=(4, 4), tempo=50, tonality=None, title='MusicLang score', composer='MusicLang', no_repeat=False, **kwargs):
     """
     Transform a musiclang score into a Music21 score
     Parameters
     ----------
     score: Score
             MusicLang score to transform
     signature: tuple (nom, den)
@@ -261,29 +315,29 @@
         idx += 1
 
     # Create voices
     idx = 0
     for part_name, part in parts.items():
         # Add notes for each chord if first add lyrics ...
         voice = stream.Voice(number=idx + 1)
-        voice = score_instrument_to_notes(score, part_name, voice, idx)
+        voice = score_instrument_to_notes(score, part_name, voice, idx, no_repeat=no_repeat)
 
         part.insert(0, voice)
         idx += 1
 
     m21_score = stream.Score()
     meta = metadata.Metadata(title=title, composer=composer)
     m21_score.insert(0, meta)
     for part_name, part in instruments.items():
         m21_score.insert(0, part)
     # Iterate over chord for each instrument
     return m21_score
 
 
-def score_to_mxl(score, filepath, signature=(4, 4), tempo=50, tonality=None, **kwargs):
+def score_to_mxl(score, filepath, signature=(4, 4), tempo=50, tonality=None, no_repeat=False, **kwargs):
     """
     Transform a musiclang score into a musicxml file, readable by all the main notation software (musescore, finale ...)
 
     Parameters
     ----------
     score: Score
             MusicLang score to transform
@@ -296,10 +350,10 @@
     tonality: Tonality
             Tonality of the piece if applicable
     title: str
         Title of the piece
 
     """
     # Find tonality
-    m21_score = score_to_music_21(score, signature=signature, tempo=tempo, tonality=tonality, **kwargs)
+    m21_score = score_to_music_21(score, signature=signature, tempo=tempo, tonality=tonality, no_repeat=no_repeat, **kwargs)
     m21_score.write('mxl', filepath)
```

### Comparing `musiclang-0.8.1/musiclang/write/pitches/pitches_utils.py` & `musiclang-0.8.2/musiclang/write/pitches/pitches_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 All rights reserved.
 
 This source code is licensed under the BSD-style license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 import numpy as np
-
 def relative_scale_up_value(delta, last_pitch, scale_pitches):
     """
 
     Parameters
     ----------
     note : Note
     last_pitch : int
@@ -24,15 +23,15 @@
 
     """
     scale_mod = list(sorted([i % 12 for i in scale_pitches]))
     # Get scale index
     if delta == 0:
         new_pitch = last_pitch
     else:
-        whole_scale = [s + octave * 12 for octave in range(-5, 5) for s in scale_mod]
+        whole_scale = [s + octave * 12 for octave in range(-7, 7) for s in scale_mod]
         dists = np.asarray(whole_scale) - last_pitch
         dists = dists[dists >= 0] + last_pitch
         new_pitch = dists[delta - 1 * (last_pitch not in whole_scale)]
 
     return new_pitch
 
 
@@ -52,15 +51,15 @@
 
     """
     scale_mod = list(sorted([i % 12 for i in scale_pitches]))
     # Get scale index
     if delta == 0:
         new_pitch = last_pitch
     else:
-        whole_scale = [s + octave * 12 for octave in range(-5, 5) for s in scale_mod]
+        whole_scale = [s + octave * 12 for octave in range(-7, 7) for s in scale_mod]
         dists = np.asarray(whole_scale) - last_pitch
         dists = dists[dists <= 0] + last_pitch
         new_pitch = dists[-(delta + 1) + 1 * (last_pitch not in whole_scale)]
     return new_pitch
 
 
 def get_relative_scale_value(note, last_pitch, scale_pitches):
@@ -73,18 +72,21 @@
     scale_pitches : list[int]
 
 
     Returns
     -------
     pitch: int
     """
-    if note.is_up:
-        return relative_scale_up_value(note.val + 7 * note.octave, last_pitch, scale_pitches)
-    elif note.is_down:
-        return relative_scale_down_value(note.val + 7 * note.octave, last_pitch, scale_pitches)
+    total_val = note.val + len(scale_pitches) * note.octave
+    if note.is_down:
+        total_val = - total_val
+    if total_val >= 0:
+        return relative_scale_up_value(total_val, last_pitch, scale_pitches)
+    elif total_val < 0:
+        return relative_scale_down_value(-total_val, last_pitch, scale_pitches)
     else:
         raise Exception(f'This relative note {note} is nor up or down')
 
 
 def get_value_to_scale_note_with_accident(note, chord):
     """
     Get the value of the note if there is an accident
@@ -96,15 +98,15 @@
     Returns
     -------
     pitch: int
 
     """
     from musiclang.write.constants import ACCIDENTS_TO_NOTE
     tonic = chord.scale_pitches[0]
-    return tonic + ACCIDENTS_TO_NOTE[(note.val, note.accident)] + 12 * note.octave
+    return tonic + ACCIDENTS_TO_NOTE[(note.val, note.accident)] + 12 * (note.octave)
 
 def get_value_to_scale_note(value, scale_pitches):
     """
     Transform an absolute value and a scale pitches to an unique pitch
 
     Parameters
     ----------
@@ -147,15 +149,14 @@
             if note.has_accident:
                 pitch_result = get_value_to_scale_note_with_accident(note, real_chord)
             else:
                 pitch_result = get_value_to_scale_note(note.val + 7 * note.octave, scale_pitches)
         elif note.is_chord_note:
             scale_chord = chord.chord_pitches
             pitch_result = get_value_to_scale_note(note.val + len(scale_chord) * note.octave, scale_chord)
-            pass
         elif note.is_bass_note:
             scale_chord = chord.chord_extension_pitches
             pitch_result = get_value_to_scale_note(note.val + len(scale_chord) * note.octave, scale_chord)
         elif note.is_absolute_note:
             chromatic_pitches = list(range(12))
             pitch_result = get_value_to_scale_note(note.val + 12 * note.octave, chromatic_pitches)
         elif note.is_chromatic_note:
@@ -166,16 +167,22 @@
             pitch_result = get_value_to_scale_note(note.val + 12 * note.octave, chromatic_pitches)
 
     elif note.is_relative:
         if note.is_scale_note:
             pitch_result = get_relative_scale_value(note, last_pitch, scale_pitches)
             pass
         elif note.is_chord_note:
-            raise Exception('Relative chord notes parsing are not implemented yet')
+            scale_chord = chord.chord_pitches
+            pitch_result = get_relative_scale_value(note, last_pitch, scale_chord)
+            pass
+        elif note.is_bass_note:
+            scale_chord = chord.chord_extension_pitches
+            pitch_result = get_relative_scale_value(note, last_pitch, scale_chord)
             pass
         elif note.is_chromatic_note:
-            raise Exception('Relative chromatic notes parsing are not implemented yet')
+            chromatic_pitches = chord.chromatic_pitches
+            pitch_result = get_relative_scale_value(note, last_pitch, chromatic_pitches)
             pass
         else:
             raise Exception('This kind of note is not supported or has no pitch : {}'.format(note.type))
 
     return pitch_result
```

### Comparing `musiclang-0.8.1/musiclang/write/properties/note_properties.py` & `musiclang-0.8.2/musiclang/write/properties/note_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,24 +183,24 @@
     def is_scale_note(self):
         """ """
         return self.note.type in ["s", "su", "sd"]
 
     @property
     def is_chord_note(self):
         """ """
-        return self.note.type == "c"
+        return self.note.type in ['c', 'cu', 'cd']
 
     @property
     def is_absolute_note(self):
-        return self.note.type == "a"
+        return self.note.type in ['a', 'au', 'ad']
 
     @property
     def is_bass_note(self):
         """ """
-        return self.note.type == "b"
+        return self.note.type in ['b', 'bu', 'bd']
 
     @property
     def is_continuation(self):
         """ """
         return self.note.type == "l"
 
     @property
```

### Comparing `musiclang-0.8.1/musiclang/write/rhythm/metric.py` & `musiclang-0.8.2/musiclang/write/rhythm/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,29 +44,36 @@
         return self.nb_bars * nom * frac(4, den)
 
     @property
     def bar_duration(self):
         nom, den = self.signature
         return nom * frac(4, den)
 
-    def get_beat_durations(self):
-        first_has_note = self.array[0] == 1
+    def get_beat_durations(self, array=None):
+        if array is None:
+            array = self.array
+        first_has_note = array[0] == 1
         result = []
         curr_dur = self.tatum
         is_note = first_has_note
-        for b in self.array[1:]:
+        for b in array[1:]:
             if b == 0:
                 curr_dur += self.tatum
-            else:
+            elif b == 1:
                 result.append((is_note, curr_dur))
                 curr_dur = self.tatum
                 is_note = True
+            else:
+                result.append((is_note, curr_dur))
+                curr_dur = self.tatum
+                is_note = False
+
         result.append((is_note, curr_dur))
 
-        return result
+        return result, first_has_note
 
     def beat_type(self, time):
         """
         Return "STRONG" if the beat is a strong beat
         "WEAK" if weak beat and "SYNCOPATION" otherwise
 
         Parameters
@@ -92,14 +99,15 @@
         elif self.signature in [(3, 4), (3, 8)]:
             return Metric.STRONG if time == 0 else Metric.WEAK
         elif self.signature in [(3, 8), (2, 8), (1, 8)]:
             return Metric.WEAK
         elif self.signature in [(6, 8), (9, 8), (12, 8)]:
             return Metric.STRONG if (time % frac(3, 2)) == 0 else Metric.WEAK
 
+
     @classmethod
     def Euclidian(cls, pulses, signature, tatum, nb_bars=1):
         """
         Following this paper : The Euclidean Algorithm Generates Traditional Musical Rhythms
         http://cgm.cs.mcgill.ca/~godfried/publications/banff.pdf
 
         Parameters
@@ -113,14 +121,17 @@
         metric: Metric
                 Resulting metric of the song
         """
 
         steps = cls._nb_steps(signature, tatum, nb_bars)
         return Metric(bjorklund_algorithm(steps, pulses), signature, tatum, nb_bars=nb_bars)
 
+
+
+
     @classmethod
     def _nb_steps(self, signature, tatum, nb_bars):
         nb_base, den = signature
         base = frac(4, den)
         duration = nb_base * base
         steps = int(nb_bars * frac(duration, tatum))
         return steps
@@ -182,15 +193,38 @@
 
         steps = cls._nb_steps(signature, tatum, nb_bars)
         return Metric([1 if (a % n) == 0 else 0 for a in range(steps)], signature, tatum, nb_bars=nb_bars)
 
     def alternating(self, n):
         return Metric.Alternating(n, signature=self.signature, tatum=self.tatum, nb_bars=self.nb_bars)
 
-    def apply_to_melody(self, melody, expand=True):
+    def apply_to_score(self, score):
+        """
+        Apply the rythm to a given score
+        Parameters
+        ----------
+        score
+
+        Returns
+        -------
+
+        """
+        pass
+
+
+    def get_array_between(self, start, end):
+        if start is None:
+            start = 0
+        if end is None:
+            end = self.duration
+        idx_start = start // self.tatum
+        idx_end = end // self.tatum
+        return [self.array[idx % len(self.array)] for idx in range(idx_start, idx_end)], start, end
+
+    def apply_to_melody(self, melody, expand=True, start=None, end=None):
         """
         Apply the metric to a given melody.
         If expand is True, the notes of the melody will be used circularly until metric duration is satisfied
         Else if the melody has not enough notes it will add silences
 
         Parameters
         ----------
@@ -206,30 +240,46 @@
         if isinstance(melody, Note):
             notes = [melody.copy()]
         elif isinstance(melody, (list, tuple)):
             notes = melody
         else:
             notes = melody.notes
 
-        if not expand and len(notes) < sum(self.array):
-            notes += [Silence(1)] * (sum(self.array) - len(notes))
+        array, start, end = self.get_array_between(start, end)
+        if not expand and len(notes) < sum(array):
+            notes += [Silence(1)] * (sum(array) - len(notes))
+
+        beat_durations, first_has_note = self.get_beat_durations(array)
+        result = self._apply_durations_to_melody(notes, beat_durations, first_has_note=first_has_note, expand=expand)
+        if result.duration > (end - start):
+            # It means the duration of the chord is not divisible by tatum, must shorter the last note
+            delta_tatum = (end - start) % self.tatum
+            before = result.copy()
+            result.notes[-1] = result.notes[-1].set_duration(result.notes[-1].duration - delta_tatum)
+            assert result.duration == (end - start), f'{result.duration} {end - start} {delta_tatum} {result} {before}'
+
+        elif result.duration < (end - start):
+            delta_tatum = (end - start) % self.tatum
+            result.notes[-1] = result.notes[-1].set_duration(result.notes[-1].duration + delta_tatum)
 
-        beat_durations = self.get_beat_durations()
-        return self._apply_durations_to_melody(notes, beat_durations, expand=expand)
+        return result
 
     @classmethod
-    def _apply_durations_to_melody(cls, notes, beat_durations, expand=True):
-        from musiclang import Silence
+    def _apply_durations_to_melody(cls, notes, beat_durations, first_has_note=True, expand=True):
+        from musiclang import Silence, Continuation
         melody = None
-        if not beat_durations[0]:
-            notes = [Silence(1)] + notes
         for idx, (has_note, beat) in enumerate(beat_durations):
-            if not expand and idx > len(notes):
+            if idx == 0 and not first_has_note:
+                melody += Continuation(1).set_duration(beat)
+            elif not expand and idx > len(notes):
                 break
-            melody += notes[idx % len(notes)].set_duration(beat)
+            elif has_note:
+                melody += notes[idx % len(notes)].set_duration(beat)
+            else:
+                melody += Silence(1).set_duration(beat)
 
         return melody
 
     def complementary(self):
         """
         Get the complementary rhythm of a given rhythm
         eg : Complementary of [1, 0, 0, 0] = [0, 1, 1, 1]
@@ -259,15 +309,15 @@
         eg : circular_shift(2) of [1, 0, 0, 0] = [0, 0, 1, 0]
         Keep the same tatum, nb_bars and signature
 
         Returns
         -------
         metric: Metric
         """
-        return Metric(self.array[(n % len(self.array)):] + self.array[:(n % len(self.array))],
+        return Metric(self.array[(-n % len(self.array)):] + self.array[:(-n % len(self.array))],
                       signature=self.signature, tatum=self.tatum, nb_bars=self.nb_bars)
 
     def canon(self, n):
         """
         Get the shifted rhythm of a given rhythm by tatum value, cut the end to fit the metric.
         eg : canon(2) of [1, 0, 0, 0] = [0, 0, 1, 0]
         Keep the same tatum, nb_bars and signature
@@ -277,14 +327,39 @@
         metric: Metric
         """
         array_mask = ([0] * n) + ([1] * (len(self.array) - n))
         return Metric(self.array[(n % len(self.array)):] + self.array[:(n % len(self.array))],
                       signature=self.signature, tatum=self.tatum, nb_bars=self.nb_bars).masked(array_mask)
 
     @classmethod
+    def FromArray(cls, array, signature=(4, 4), tatum=None, nb_bars=1):
+        """
+        Get a metric from a binary array, if several bar we only support constant tatum
+        between bar at the time being
+        Parameters
+        ----------
+        array: list[int]
+            List of binary
+        signature
+        tatum
+        nb_bars
+
+        Returns
+        -------
+
+        """
+        if tatum is None:
+            nb_notes = len(array)
+            nom, den = signature
+            duration = nb_bars * nom * frac(4, den)
+            tatum = duration / nb_notes
+        return Metric(array, signature=signature, tatum=tatum, nb_bars=nb_bars)
+
+
+    @classmethod
     def FromMelody(cls, melody, signature=(4, 4), tatum=None, nb_bars=1):
         # Get tatum
         if tatum is None:
             tatum = min([note.duration for note in melody.notes])
         array = []
         for note in melody.notes:
             nb_tatums = note.duration / tatum
@@ -381,15 +456,15 @@
         from musiclang import Note, Melody, Silence
         if isinstance(melody, Note):
             melody = Melody([melody.copy()])
         elif isinstance(melody, (list, tuple)):
             melody = Melody(melody).copy()
 
         notes = melody.notes
-        durations = sum([m.get_beat_durations() for m in self.metrics], [])
+        durations = sum([m.get_beat_durations()[0] for m in self.metrics], [])
         return Metric.apply_durations_to_melody(notes, durations, expand=expand)
 
     def masked(self, masks):
         if isinstance(masks, Metric):
             masks = []
         return CompositeMetric([metric.masked(mask) for mask, metric in zip(masks, self.metrics)])
```

### Comparing `musiclang-0.8.1/musiclang/write/rhythm/utils_metric.py` & `musiclang-0.8.2/musiclang/write/rhythm/utils_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/score.py` & `musiclang-0.8.2/musiclang/write/score.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     """
     def __init__(self, chords=None, config=None, tags=None):
         self.chords = chords
         self.config = config
         if self.chords is None:
             self.chords = []
         if self.config is None:
-            self.config = {'annotation': "", "tempo": 120}
+            self.config = {'annotation': "",
+                           "tempo": 120,
+                           "pickup": 0,
+                           "time_signature": (4, 4)
+                           }
 
         self.tags = set(tags) if tags is not None else set()
 
     def has_tag(self, tag):
         """
         Check if the tag exists for this object
         Returns a copy of the object
@@ -202,14 +206,105 @@
         -------
         chord: Chord
         """
         cp = self.copy()
         cp.tags = set()
         return cp
 
+
+    def set_amp(self, amp):
+        """
+        Set the velocity of the notes in the score (between 0 and 120)
+        Parameters
+        ----------
+        amp: int
+
+        Returns
+        -------
+
+        """
+        return Score([c.set_amp(amp) for c in self.chords], tags=set(self.tags))
+
+
+    def normalize_instruments(self):
+        """
+        Get a score with the same instruments on all chords,
+        if an instrument is missing on one chord add it with a silence lasting for the chord duration.
+
+        Returns
+        -------
+        score: Score
+        Normalize score
+        """
+        from musiclang import Silence
+        score = None
+        instruments = set(self.instruments)
+        for chord_raw in self.chords:
+            chord = chord_raw.copy()
+            missing_instruments = set(instruments) - set(chord.instruments)
+            chord_score = chord.score
+            for instrument in missing_instruments:
+                chord_score[instrument] = Silence(chord.duration)
+            score += chord(**chord_score)
+        return score
+
+    def remove_silenced_instruments(self):
+        """
+        Inverse operation of :func:`~Score.normalize_instruments`
+        For each chord remove all instruments that are silenced
+        Returns
+        -------
+        score: Score
+        """
+
+        score = None
+        for chord_raw in self.chords:
+            chord = chord_raw.copy()
+            chord_score = chord.score
+
+            for instrument in list(chord_score.keys()):
+                if all([n.type == 'r' for n in chord_score[instrument]]):
+                    del chord_score[instrument]
+
+            score += chord(**chord_score)
+
+        return score
+
+    def replace_instruments(self, **instruments_dict):
+        """
+        Replace any instrument with another (use full part name (eg: piano__0)
+
+        Parameters
+        ----------
+        instruments_dict: dict[str, str]
+            Dictionary of parts name to replace
+
+        Returns
+        -------
+        score: Score
+
+        """
+        score = None
+        instruments_dict = {key: instruments_dict[key] if key in instruments_dict.keys() else key for key in self.parts}
+        for chord in self.chords:
+            new_chord_dict = {}
+            for ins_name, new_ins_name in instruments_dict.items():
+                if ins_name in chord.score.keys():
+                    new_chord_dict[new_ins_name] = chord.score[ins_name]
+            score += chord(**new_chord_dict)
+
+        return score
+
+
+    def clean(self):
+        return self.to_drum().decompose_duration()
+
+    def to_drum(self):
+        return Score([chord.to_drum() for chord in self.chords], tags=set(self.tags))
+
     def to_chords(self):
         """ """
         res = [chord.to_chord() for chord in self.chords]
         return res
 
     def copy(self):
         """
@@ -267,14 +362,18 @@
         if isinstance(other, int):
             return Score([c & other for c in self.chords], tags=self.tags)
         else:
             raise Exception(f'Not compatible type with & {other.__class__}')
 
 
     @property
+    def parts(self):
+        return self.instruments
+
+    @property
     def instruments(self):
         """
 
         Parameters
         ----------
 
         Returns
@@ -312,14 +411,32 @@
         """
         score = None
         for chord in self:
             score += chord(**{instrument: melody.o(instruments_octaves.get(instrument, 0)) for instrument, melody in chord.items()})
 
         return score
 
+    def to_events(self, tempo=120, **kwargs):
+        from musiclang.write.out import score_to_events
+        events = score_to_events(self, tempo=tempo, **kwargs)
+        return events
+
+    def to_events_pickle(self, filepath, tempo=120, **kwargs):
+        from musiclang.write.out import score_to_events
+        import pickle
+        events = score_to_events(self, tempo=tempo, **kwargs)
+        with open(filepath, 'wb') as f:
+            pickle.dump(events, f)
+
+    def apply(self, keep_durations=True, **melodies):
+        if keep_durations:
+            return Score([c(**melodies).augment(c.duration) for c in self.chords])
+        else:
+            return Score([c(**melodies) for c in self.chords])
+
     def to_voicing(self, nb_voices=4, instruments=None):
         """Convert score to a four voice voicing using the extensions provided in the chord.
 
         It will remove the existing scores of each chord and create the associated voicings
 
         Parameters
         ----------
@@ -358,14 +475,17 @@
         import tempfile
         import os
         with tempfile.TemporaryDirectory() as di:
             m21_score = self.to_music21(**kwargs)
             return m21_score.show(*args)
 
 
+    def __setitem__(self, key, value):
+        return self.chords.__setitem__(key, value)
+
     def __getitem__(self, item):
         """
         If str return a score with only this voice
         else returns item getter of the list of chords and convert it back to a score
         """
         from .note import Silence
         from .chord import Chord
@@ -418,45 +538,235 @@
         >>> score.put_on_same_chord()
         (I % I.m)(piano__0=s0 + s2)
 
         """
         from .time_utils import put_on_same_chord
         return put_on_same_chord(self)
 
-    def project_on_score(self, score2, keep_score=False):
-        """Project harmonically the current score onto the score2
+    @classmethod
+    def json_file_to_score(cls, filepath):
+        """
+        Load a score from an orchestrated json file
+        Parameters
+        ----------
+        filepath
+
+        Returns
+        -------
+
+        """
+        import json
+        with open(filepath, 'r') as f:
+            data = json.load(f)
+
+        return cls.dict_to_score(data)
+
+    @classmethod
+    def from_file(cls, filepath):
+        """
+        Load a score from a musiclang text file
+        Parameters
+        ----------
+        filepath
+
+        Returns
+        -------
+
+        """
+        with open(filepath, 'r') as f:
+            data = f.read()
+        return cls.from_str(data)
+
+    def to_pickle(self, filepath, create_dir=False):
+        """
+        Save the score into a pickle file
+
+        Parameters
+        ----------
+        filepath : str
+                   Filepath on which to save the score
+        create_dir : bool (Default value = False)
+                    Create the directory if it does not exist
+        """
+        import pickle
+        import os
+        directory = os.path.dirname(filepath)
+        if create_dir and not os.path.exists(directory):
+            os.makedirs(directory)
+        with open(filepath, 'wb') as f:
+            pickle.dump(self, f)
+
+    def predict_score(self):
+        """
+        Predict the continuation of the score given the current score
+        Currently it takes no argument.
+        Please note that this method is still very experimental as we are
+        currently improving our musiclang language model.
+
+        Returns
+        -------
+        predicted_score: Score
+            The predicted score
+
+        """
+        from musiclang.predict.predictors import predict_score_from_hugginface
+        score_str = predict_score_from_hugginface(str(self))
+        return Score.from_str(score_str)
+
+    def to_text_file(self, filepath, create_dir=False):
+        """
+        Save as a musiclang txt file
+        Parameters
+        ----------
+        filepath
+        create_dir: bool (Default value = False)
+            Create the directory if it does not exist
+        Returns
+        -------
+
+        """
+        import os
+        directory = os.path.dirname(filepath)
+        if create_dir and not os.path.exists(directory):
+            os.makedirs(directory)
+        with open(filepath, 'w') as f:
+            f.write(str(self))
+    @classmethod
+    def dict_to_score(cls, data):
+        """
+        Load a score from an orchestrated json file
+        Parameters
+        ----------
+        data
+
+        Returns
+        -------
+
+        """
+        from musiclang import PartComposer
+        score = PartComposer.compose(data)
+        return score
+
+
+
+
+    def get_patterns(self, nb_excluded_instruments=0, **kwargs):
+        metadata_base = {
+            "tempo": self.config['tempo']
+        }
+        metadata_base = {**metadata_base, **kwargs}
+        data = []
+        patterns = []
+        for chord_idx, chord in enumerate(self.chords):
+            if len(chord.parts) <= nb_excluded_instruments:
+                continue
+            try:
+                dict_pattern, pattern = chord.patternize(nb_excluded_instruments=nb_excluded_instruments, **kwargs)
+                dict_pattern['metadata'] = {**dict_pattern['metadata'], **metadata_base}
+                dict_pattern['metadata']['chord_idx'] = chord_idx
+                data.append(dict_pattern)
+                patterns.append(pattern)
+            except Exception as e:
+                print("Error with chord: ", chord)
+                print(e)
+        return data, patterns
+
+    def project_pattern(self, score, restart_each_chord=False):
+        """
+
+        Parameters
+        ----------
+        score: Score or list[Note]
+            - If score : Score on which the pattern will be projected
+            - If list : List of notes on which the pattern will be projected (It will replace the adequate "xi")
+
+        Returns
+        -------
+        score: Score
+            Score with the pattern projected on it
+        """
+        from musiclang.transform.composing import Patternator
+        if isinstance(score, list):
+            voicing = score
+            parts = self.parts
+            score = NC(**{part: Score.from_str(voicing[idx]).set_duration(self.duration)
+                          for idx, part in enumerate(parts)})
+        else:
+            pass
+
+        score_patterned = Patternator(restart_each_chord=restart_each_chord)(self, score)
+        return score_patterned
+
+    def project_on_score(self, score2, keep_pitch=False, voice_leading=True, keep_score=False,
+                         repeat_to_duration=False, allow_override=False):
+        """Project harmonically the current score onto the score2.
+        The score2 notes will disappear, only keeping the current score with the harmony of score2
+        Can either project by complete diatonic transposition or trying to move as little as possible the notes
+        (voice_leading=True)
+
         Algorithm : For each chord of score2 : get chords that belongs to score1 and reproject on chord of score2
 
         Parameters
         ----------
         score : Score
                 Score to project on the chords of score2
         score2 : Score
             Score that contains the harmony
-        keep_score : Score (Default value = False)
-            Keep the voices of score2 ? (Default value = False)
-
+        voice_leading: boolean (default=True)
+            If true, we try to move the notes as little as possible
+        voice_leading : boolean (default=True)
+            If True try to move the notes as little as possible (Default value = True)
+        repeat_to_duration: boolean (default=False)
+            If True then Repeat the score to fit the duration of score2
+        allow_override: boolean (default=False)
+            In case keep_score is True should we allow existence of intersection of voices between self and score2 ?
+            If True score2 parts that exists in self will be replaced by projected parts of self. Otherwise raise an Exception
         Returns
         -------
         new_score: Score
                   The score projected on score2 chord progression. It will fit the minimal duration of both scores
 
         Examples
         --------
 
         >>> from musiclang.library import *
         >>> score1 = (I % I.m)(piano__0=s0.e) + (V % I.m)(piano__0=s2.e)
         >>> score2 = (II % III.m)(piano__0=s0.e + s0.e)
-        >>> score1.project_on_score(score2, keep_score=False)
+        >>> score1.project_on_score(score2, voice_leading=False)
         (II % III.m)(piano__0=s0.e + s2.e)
 
         """
         # Algo : For each chord of score2 : get chords that belongs to score1 and reproject on chord of score2
         from .time_utils import project_on_score
-        return project_on_score(self.to_score(), score2.to_score(), keep_score=keep_score)
+        from musiclang.transform.composing import project_on_score_keep_notes
+
+        if repeat_to_duration and self.duration < score2.duration:
+            diff_duration = (score2.duration // self.duration) + 1
+            to_project = self * diff_duration
+        else:
+            to_project = self
+
+        if keep_pitch:
+            to_project = self.to_absolute_note()
+
+        if voice_leading:
+            result_score = project_on_score_keep_notes(to_project.to_score(), score2.to_score())
+        else:
+            result_score = project_on_score(to_project.to_score(), score2.to_score(), keep_score=False)
+
+        if keep_score:
+            if not allow_override and len(set(result_score.parts).intersection(score2.parts)) != 0:
+                raise Exception('If keep_score flag is True, parts should be differents between the scores')
+
+            result_score = sum([c1(**{**c2.score, **c1.score}) for c1, c2 in zip(result_score.chords, score2.chords)], None)
+
+        return result_score
+
+    def to_absolute_note(self):
+        return Score([chord.to_absolute_note() for chord in self.chords], tags=self.tags)
 
 
     def get_chord_between(self, chord, start, end):
         """
 
         Parameters
         ----------
@@ -470,14 +780,31 @@
         Returns
         -------
 
         """
         from .time_utils import get_chord_between
         return get_chord_between(chord, start, end)
 
+    @property
+    def pedal_each_chord(self):
+        return Score([c.pedal for c in self.chords], tags=set(self.tags))
+
+    def doubling(self, **args):
+        new_score = None
+        for chord in self.chords:
+            score = chord.copy().score
+            for part, new_parts in args.items():
+                if isinstance(new_parts, str):
+                    new_parts = [new_parts]
+                for new_part in new_parts:
+                    if part in score.keys():
+                        score[new_part] = score[part].copy()
+            new_score += chord(**score)
+
+        return new_score
 
     def get_score_between(self, start=None, end=None):
         """
         Get the score between start and end time.
 
         Parameters
         ----------
@@ -523,52 +850,61 @@
             cello__0=s0,
             violin__0=s4)
 
         """
         from .arrange_utils import reduce
         return reduce(self, n_voices=n_voices, start_low=start_low, instruments=instruments)
 
-    def to_pickle(self, filepath):
-        """
-        Save the score into a pickle file
 
-        Parameters
-        ----------
-        filepath : str
-                   Filepath on which to save the score
 
-        """
-        import pickle
-        with open(filepath, 'wb') as f:
-            pickle.dump(self, f)
+    @classmethod
+    def from_annotation_file(cls, file):
+        with open(file, 'r') as f:
+            text = f.read()
+        return Score.from_annotation(text)
+
+    @classmethod
+    def from_annotation(cls, text):
+        from musiclang.analyze import ScoreFormatter
+        return ScoreFormatter(text).parse()
+
 
     @classmethod
     def from_midi(cls, filename):
         """
         Load a midi score into musiclang
 
         .. warning:: This step can take some time depending on the length of the file
 
         Parameters
         ----------
         filename : str
                    Filepath of the file
-            
 
         Returns
         -------
         score: Score
                The loaded score
 
         """
         from musiclang.analyze import parse_to_musiclang
         score, config = parse_to_musiclang(filename)
         score.config = config
         return score
 
+    def to_extension_note(self):
+        return Score([chord.to_extension_note() for chord in self.chords], tags=set(self.tags))
+
+    def to_chord_note(self):
+        return Score([chord.to_chord_note() for chord in self.chords], tags=set(self.tags))
+
+    def to_standard_note(self):
+        return Score([chord.to_standard_note() for chord in self.chords], tags=set(self.tags))
+
+
     @classmethod
     def from_xml(cls, filename):
         """
         Load a musicxml score into musiclang
 
         .. warning:: This step can take some time depending on the length of the file
 
@@ -584,39 +920,36 @@
 
         score: Score
                The loaded score
 
         """
         from musiclang.analyze import parse_to_musiclang
         score, config = parse_to_musiclang(filename)
-        score.config = config
+        score.config.update(config)
         return score
 
     def decompose_duration(self):
         """
         Decompose the duration in a note + continuations. It recursively call
         :func:`~Note.decompose_duration()`
         """
         return Score([chord.decompose_duration() for chord in self.chords], tags=self.tags)
 
-    def to_score(self):
+    def to_score(self, copy=True):
         """ """
-        return self.copy()
+        if not copy:
+            return self
+        else:
+            return self.copy()
 
 
     @classmethod
     def from_str(cls, s):
-        from musiclang.library import I, II, III, IV, V, VI, VII
-        from musiclang.library import s0, s1, s2, s3, s4, s5, s6
-        from musiclang.library import h0, h1, h2, h3, h4, h5, h6, h7, h8, h9, h10, h11
-        from musiclang.library import su0, su1, su2, su3, su4, su5, su6
-        from musiclang.library import hu0, hu1, hu2, hu3, hu4, hu5, hu6, hu7, hu8, hu9, hu10, hu11
-        from musiclang.library import sd0, sd1, sd2, sd3, sd4, sd5, sd6
-        from musiclang.library import hd0, hd1, hd2, hd3, hd4, hd5, hd6, hd7, hd8, hd9, hd10, hd11
-        return eval(s.replace('\n', ''))
+
+        return eval(str(s).replace('\n', ''))
 
     @classmethod
     def from_sequence(cls, sequence, **kwargs):
         """
 
         Parameters
         ----------
@@ -753,15 +1086,15 @@
         -------
 
         """
         code = self.to_code(**kwargs)
         with open(filepath, 'w') as f:
             f.write(code)
 
-    def to_musicxml(self, filepath, signature=(4, 4), tonality=None, tempo=120, **kwargs):
+    def to_musicxml(self, filepath, signature=(4, 4), tonality=None, tempo=120, no_repeat=False, **kwargs):
         """
         Transform a musiclang score into a musicxml file, readable by all the main notation software (musescore, finale ...)
 
         Parameters
         ----------
         score: Score
                 MusicLang score to transform
@@ -776,15 +1109,15 @@
         title: str
             Title of the piece
 
         """
         # Convert score to midi
         from .out.to_mxl import score_to_mxl
 
-        return score_to_mxl(self, filepath, signature=signature, tonality=tonality, tempo=tempo, **kwargs)
+        return score_to_mxl(self, filepath, signature=signature, tonality=tonality, tempo=tempo, no_repeat=no_repeat, **kwargs)
 
     def to_music21(self, signature=(4, 4), tonality=None, tempo=120, **kwargs):
         """
         Transform a musiclang score into a Music21 score
         Parameters
         ----------
         score: Score
```

### Comparing `musiclang-0.8.1/musiclang/write/sequence/sequence.py` & `musiclang-0.8.2/musiclang/write/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/sequence/sequence_utils.py` & `musiclang-0.8.2/musiclang/write/sequence/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/time_utils/time_utils.py` & `musiclang-0.8.2/musiclang/write/time_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/musiclang/write/tonality.py` & `musiclang-0.8.2/musiclang/write/tonality.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,29 @@
         """
         self.degree = degree
         self.mode = mode
         self.octave = octave
         self.tags = set(tags) if tags is not None else set()
 
 
+    @classmethod
+    def from_str(cls, text):
+        tab = 'CDEFGAB'
+        notes = [0, 2, 4, 5, 7, 9, 11]
+        note = text.replace(':', '').replace('#', '').replace('b', '').replace('-', '')
+        tone = notes[tab.index(note.upper())]
+        mode = 'M' if note.upper() == note else 'm'
+
+        tone += text.count('#')
+        tone += text.count('s')
+        tone -= text.count('b')
+        tone -= text.count('-')
+
+        return cls(tone, mode)
+
     def __hash__(self):
         return hash(self.__repr__())
 
 
     def has_tag(self, tag):
         """
         Check if the tag exists for this object
```

### Comparing `musiclang-0.8.1/musiclang.egg-info/SOURCES.txt` & `musiclang-0.8.2/musiclang.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,32 +6,46 @@
 musiclang/library.py
 musiclang.egg-info/PKG-INFO
 musiclang.egg-info/SOURCES.txt
 musiclang.egg-info/dependency_links.txt
 musiclang.egg-info/requires.txt
 musiclang.egg-info/top_level.txt
 musiclang/analyze/__init__.py
+musiclang/analyze/constants.py
 musiclang/analyze/item.py
 musiclang/analyze/midi_parser.py
 musiclang/analyze/parser.py
+musiclang/analyze/pattern_analyzer.py
+musiclang/analyze/pattern_sampler.py
+musiclang/analyze/roman_parser.py
+musiclang/analyze/score_formatter.py
+musiclang/analyze/score_formatter_elements.py
 musiclang/analyze/to_musiclang.py
 musiclang/analyze/voice_separation.py
 musiclang/analyze/augmented_net/__init__.py
 musiclang/analyze/augmented_net/cache.py
 musiclang/analyze/augmented_net/chord_vocabulary.py
 musiclang/analyze/augmented_net/feature_representation.py
 musiclang/analyze/augmented_net/inference.py
 musiclang/analyze/augmented_net/input_representations.py
 musiclang/analyze/augmented_net/keydistance.py
 musiclang/analyze/augmented_net/models.py
 musiclang/analyze/augmented_net/output_representations.py
 musiclang/analyze/augmented_net/score_parser.py
 musiclang/analyze/augmented_net/utils.py
 musiclang/predict/__init__.py
+musiclang/predict/arranger/__init__.py
+musiclang/predict/arranger/arranger.py
+musiclang/predict/arranger/arranger_trainer.py
+musiclang/predict/composer/__init__.py
+musiclang/predict/composer/auto_composer.py
+musiclang/predict/composer/composer.py
+musiclang/predict/composer/harmony.py
 musiclang/predict/predictors/__init__.py
+musiclang/predict/predictors/huggin.py
 musiclang/predict/predictors/windowed.py
 musiclang/predict/tokenizers/__init__.py
 musiclang/predict/tokenizers/chord_tokenizer.py
 musiclang/transform/__init__.py
 musiclang/transform/base_transformer.py
 musiclang/transform/graph.py
 musiclang/transform/library.py
@@ -40,78 +54,110 @@
 musiclang/transform/pipeline.py
 musiclang/transform/transformer.py
 musiclang/transform/utils_random.py
 musiclang/transform/chord/__init__.py
 musiclang/transform/chord/basics.py
 musiclang/transform/composing/__init__.py
 musiclang/transform/composing/arrange.py
+musiclang/transform/composing/constants.py
 musiclang/transform/composing/counterpoint.py
+musiclang/transform/composing/layer.py
+musiclang/transform/composing/pattern.py
+musiclang/transform/composing/patternator.py
 musiclang/transform/composing/project.py
+musiclang/transform/composing/voice_leading.py
+musiclang/transform/dynamics/__init__.py
+musiclang/transform/dynamics/dynamizer.py
 musiclang/transform/features/__init__.py
 musiclang/transform/features/basics.py
 musiclang/transform/generators/__init__.py
 musiclang/transform/generators/rythm_generator.py
 musiclang/transform/melody/__init__.py
 musiclang/transform/melody/basics.py
+musiclang/transform/melody/continuation.py
+musiclang/transform/melody/filler.py
 musiclang/transform/note/__init__.py
 musiclang/transform/note/basics.py
+musiclang/transform/orchestrations/__init__.py
+musiclang/transform/orchestrations/epic.py
+musiclang/transform/orchestrations/nocturne.py
 musiclang/transform/score/__init__.py
 musiclang/transform/score/basics.py
 musiclang/transform/score_merger/__init__.py
 musiclang/transform/score_merger/basics.py
 musiclang/transform/structure_graphs/__init__.py
 musiclang/transform/structure_graphs/forms.py
 musiclang/write/__init__.py
 musiclang/write/chord.py
 musiclang/write/constants.py
 musiclang/write/element.py
 musiclang/write/library.py
 musiclang/write/melody.py
 musiclang/write/note.py
 musiclang/write/note_pitch.py
+musiclang/write/ornementation.py
 musiclang/write/score.py
 musiclang/write/tonality.py
 musiclang/write/arrange_utils/__init__.py
 musiclang/write/arrange_utils/arrange_utils.py
 musiclang/write/arrange_utils/skyline_algorithm.py
+musiclang/write/elements/__init__.py
+musiclang/write/elements/bar.py
+musiclang/write/elements/beat.py
+musiclang/write/elements/chord.py
+musiclang/write/elements/counterpoint.py
+musiclang/write/elements/element.py
+musiclang/write/elements/free_text.py
+musiclang/write/elements/instruments.py
+musiclang/write/elements/rhythm.py
+musiclang/write/elements/time_signature.py
+musiclang/write/elements/tonality.py
+musiclang/write/elements/voice_leading.py
+musiclang/write/elements/voicing.py
 musiclang/write/out/__init__.py
 musiclang/write/out/constants.py
 musiclang/write/out/midi_utils.py
 musiclang/write/out/to_code.py
 musiclang/write/out/to_midi.py
 musiclang/write/out/to_mxl.py
 musiclang/write/pitches/__init__.py
 musiclang/write/pitches/pitches_utils.py
 musiclang/write/properties/__init__.py
 musiclang/write/properties/note_properties.py
 musiclang/write/rhythm/__init__.py
 musiclang/write/rhythm/metric.py
+musiclang/write/rhythm/score_rythm.py
 musiclang/write/rhythm/utils_metric.py
 musiclang/write/sequence/__init__.py
 musiclang/write/sequence/sequence.py
 musiclang/write/sequence/sequence_utils.py
 musiclang/write/time_utils/__init__.py
 musiclang/write/time_utils/time_utils.py
 tests/__init__.py
 tests/analyze/__init__.py
 tests/analyze/test_analyze.py
+tests/analyze/test_score_formatter.py
 tests/composing/__init__.py
 tests/composing/test_counterpoint.py
 tests/composing/test_project.py
+tests/composing/test_voice_leading.py
+tests/predict/__init__.py
+tests/predict/test_auto_composer.py
 tests/transform/__init__.py
 tests/transform/test_mask.py
 tests/transform/test_pipeline.py
 tests/transform/test_transform.py
 tests/transform/test_transform_graph.py
 tests/transform/test_transforms.py
 tests/write/__init__.py
 tests/write/test_absolute_note.py
 tests/write/test_bass_notes.py
 tests/write/test_chord.py
 tests/write/test_chord_notes.py
+tests/write/test_chromatic_notes.py
 tests/write/test_drum_notes.py
 tests/write/test_extensions.py
 tests/write/test_melody.py
 tests/write/test_note.py
 tests/write/test_score.py
 tests/write/test_tonality.py
 tests/write/out/__init__.py
```

### Comparing `musiclang-0.8.1/pyproject.toml` & `musiclang-0.8.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "musiclang"
-version = "0.8.1"
+version = "0.8.2"
 description = "A python package for music notation and generation"
 readme = "README.md"
 authors = [{ name = "Florian GARDIN", email = "fgardin.pro@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `musiclang-0.8.1/setup.py` & `musiclang-0.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="musiclang",
-    version="0.8.1",
+    version="0.8.2",
     author="Florian GARDIN",
     author_email="fgardin.pro@gmail.com",
     description=("A python package for music notation and generation"
                 ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
```

### Comparing `musiclang-0.8.1/tests/composing/test_project.py` & `musiclang-0.8.2/tests/composing/test_project.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/transform/test_mask.py` & `musiclang-0.8.2/tests/transform/test_mask.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/transform/test_pipeline.py` & `musiclang-0.8.2/tests/transform/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/transform/test_transforms.py` & `musiclang-0.8.2/tests/transform/test_transforms.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/out/test_to_midi.py` & `musiclang-0.8.2/tests/write/out/test_to_midi.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,69 +5,69 @@
 def test_note_to_pitch_down():
     from musiclang import Chord, Tonality, Element
 
     note = Note("sd", 1, 0, 1)
     last_pitch = [12]
     chord = Element(3) % Tonality(2, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [10, 12, 1, 66, 0, 0, 0]
+    res = [10, 12, 1, 66, 0, 0, 0, None, None]
     assert result == (res, res)
 
 
 def test_note_to_pitch_up():
     note = Note("su", 1, 0, 1)
     last_pitch = [12]
     chord = Element(3) % Tonality(1, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [13, 12, 1, 66, 0, 0, 0]
+    res = [13, 12, 1, 66, 0, 0, 0, None, None]
     assert result == (res, res)
 
 
 def test_note_to_pitch_abs():
     from musiclang import Chord, Tonality, Element
 
     note = Note("s", 1, -1, 1)
     last_pitch = [12]
     chord = Element(3) % Tonality(2, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [-15, 12, 1, 66, 0, 0, 0]
+    res = [-15, 12, 1, 66, 0, 0, 0, None, None]
     assert result == (res, res)
 
 
 def test_note_to_pitch_abs_octave_tonality():
     from musiclang import Chord, Tonality, Element
 
     note = Note("s", 1, -1, 1)
     last_pitch = [12]
     chord = Element(3).o(1) % Tonality(2, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [-3, 12, 1, 66, 0, 0, 0]
+    res = [-3, 12, 1, 66, 0, 0, 0, None, None]
     assert result == (res, res)
 
 
 def test_note_to_pitch_silence():
     note = Silence(1)
     last_pitch = [12]
     chord = Element(3) % Tonality(1, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [0, 12, 1, 66, 0, 1, 0]
+    res = [0, 12, 1, 66, 0, 1, 0, None, None]
     assert result == (res, last_pitch)
 
 
 def test_note_to_pitch_continuation():
     note = Continuation(1)
     last_pitch = [12]
     chord = Element(3) % Tonality(1, mode="m", octave=-1)
     result = note_to_pitch(note, chord, 0, 12, last_pitch)
-    res = [0, 12, 1, 66, 0, 0, 1]
+    res = [0, 12, 1, 66, 0, 0, 1, None, None]
     assert result == (res, last_pitch)
 
 
 def test_to_midi():
-    notes = [[0, 12, 1, 66, 0, 0, 0], [0, 12, 1, 66, 0, 0, 0]]
+    notes = [[0, 12, 1, 66, 0, 0, 0, None, None], [0, 12, 1, 66, 0, 0, 0, None, None]]
     res = to_midi(notes, output_file=None)
     assert res is not None
 
 
 def test_score_to_midi():
     from musiclang.write.library import s0, s1, s2, I
     score = I(piano__0=s0 + s1 + s2)
@@ -94,14 +94,14 @@
 def test_create_melody_for_track():
     from musiclang.write.library import s0, s1, s2, I, V
     chord1 = I(piano__0=s0 + s1 + s2, piano__1=s0 + s1 + s2, violin__0=s0 + s1 + s2)
     chord2 = V(piano__0=s0 + s1 + s2, oboe__0=s0 + s1 + s2, violin__0=s0 + s1 + s2)
     score = chord1 + chord2
 
     res = create_melody_for_track(score, 0, 'piano__0')
-    expected_res = [[0, 0, 1, 66, 0, 0, 0],
-                    [2, 1, 1, 66, 0, 0, 0],
-                    [4, 2, 1, 66, 0, 0, 0],
-                    [7, 3, 1, 66, 0, 0, 0],
-                    [9, 4, 1, 66, 0, 0, 0],
-                    [11, 5, 1, 66, 0, 0, 0]]
+    expected_res = [[0, 0, 1, 66, 0, 0, 0, None, None],
+                    [2, 1, 1, 66, 0, 0, 0, None, None],
+                    [4, 2, 1, 66, 0, 0, 0, None, None],
+                    [7, 3, 1, 66, 0, 0, 0, None, None],
+                    [9, 4, 1, 66, 0, 0, 0, None, None],
+                    [11, 5, 1, 66, 0, 0, 0, None, None]]
     assert res == expected_res
```

### Comparing `musiclang-0.8.1/tests/write/pitches/test_pitches_utils.py` & `musiclang-0.8.2/tests/write/pitches/test_pitches_utils.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/properties/test_note_properties.py` & `musiclang-0.8.2/tests/write/properties/test_note_properties.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/rythm/test_metric.py` & `musiclang-0.8.2/tests/write/rythm/test_metric.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/test_chord_notes.py` & `musiclang-0.8.2/tests/write/test_chord_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/test_drum_notes.py` & `musiclang-0.8.2/tests/write/test_drum_notes.py`

 * *Files identical despite different names*

### Comparing `musiclang-0.8.1/tests/write/test_extensions.py` & `musiclang-0.8.2/tests/write/test_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     assert chord.extension_notes == [s0, s1, h3, s4, s6, s1.o(1), h6.o(1)]
 
 
 def test_very_complicated_chord2():
     chord = (I % I.M)['2[add4][M6](M3)(+)']
     assert chord.extension_notes == [s6.o(-1), s0, h4, s3, h8, h9]
 
+def test_replacement_become_addition():
+    chord = (I % I.M)['(M7)']
+    assert chord.extension_notes == [s0, s2, s4, h11]
+
 
 def test_replace_b9():
     chord = (I % I.M)['9(m9)']
     assert chord.extension_notes == [s0, s2, s4, s6, h1.o(1)]
 
 
 def test_addition_and_replacement():
```

### Comparing `musiclang-0.8.1/tests/write/test_tonality.py` & `musiclang-0.8.2/tests/write/test_tonality.py`

 * *Files identical despite different names*


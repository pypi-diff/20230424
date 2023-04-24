# Comparing `tmp/adaseq-0.6.2.tar.gz` & `tmp/adaseq-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adaseq-0.6.2.tar", last modified: Tue Feb 21 08:22:50 2023, max compression
+gzip compressed data, was "dist/adaseq-0.6.3.tar", last modified: Mon Apr 24 06:03:35 2023, max compression
```

## Comparing `adaseq-0.6.2.tar` & `adaseq-0.6.3.tar`

### file list

```diff
@@ -1,127 +1,132 @@
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:22.000000 adaseq-0.6.2/
--rw-r--r--   0 pangda   (1345362) users      (100)    11416 2022-12-14 08:58:36.000000 adaseq-0.6.2/LICENSE
--rw-r--r--   0 pangda   (1345362) users      (100)     5689 2023-02-21 08:26:22.000000 adaseq-0.6.2/PKG-INFO
--rw-r--r--   0 pangda   (1345362) users      (100)     5311 2023-02-21 08:24:32.000000 adaseq-0.6.2/README.md
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:13.000000 adaseq-0.6.2/adaseq/
--rw-r--r--   0 pangda   (1345362) users      (100)      272 2023-01-10 12:12:52.000000 adaseq-0.6.2/adaseq/__init__.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:13.000000 adaseq-0.6.2/adaseq/commands/
--rw-r--r--   0 pangda   (1345362) users      (100)      844 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/commands/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4674 2023-02-16 06:14:41.000000 adaseq-0.6.2/adaseq/commands/pretrain.py
--rw-r--r--   0 pangda   (1345362) users      (100)      360 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/commands/subcommand.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3448 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/commands/test.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8196 2023-02-21 08:24:32.000000 adaseq-0.6.2/adaseq/commands/train.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:14.000000 adaseq-0.6.2/adaseq/data/
--rw-r--r--   0 pangda   (1345362) users      (100)      155 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/data/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1969 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/batch.py
--rw-r--r--   0 pangda   (1345362) users      (100)      284 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/data/constant.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:14.000000 adaseq-0.6.2/adaseq/data/data_collators/
--rw-r--r--   0 pangda   (1345362) users      (100)      539 2023-01-12 08:59:17.000000 adaseq-0.6.2/adaseq/data/data_collators/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5403 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/data_collators/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1777 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)      645 2023-01-12 08:59:17.000000 adaseq-0.6.2/adaseq/data/data_collators/pretraining_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)      703 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1275 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1651 2023-02-20 09:45:46.000000 adaseq-0.6.2/adaseq/data/data_collators/twostage_data_collator_with_padding.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:15.000000 adaseq-0.6.2/adaseq/data/dataset_builders/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.2/adaseq/data/dataset_builders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4771 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/dataset_builders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4079 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/data/dataset_builders/entity_typing_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7721 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9605 2023-01-10 11:56:59.000000 adaseq-0.6.2/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4485 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:17.000000 adaseq-0.6.2/adaseq/data/dataset_dumpers/
--rw-r--r--   0 pangda   (1345362) users      (100)      139 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/data/dataset_dumpers/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1143 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/dataset_dumpers/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3234 2022-12-21 02:38:01.000000 adaseq-0.6.2/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9864 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/dataset_manager.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:18.000000 adaseq-0.6.2/adaseq/data/preprocessors/
--rw-r--r--   0 pangda   (1345362) users      (100)      602 2023-02-16 06:13:38.000000 adaseq-0.6.2/adaseq/data/preprocessors/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7010 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/preprocessors/multilabel_typing_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)    10258 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/data/preprocessors/nlp_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5000 2023-01-12 08:59:17.000000 adaseq-0.6.2/adaseq/data/preprocessors/pretraining_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1439 2023-01-11 09:41:17.000000 adaseq-0.6.2/adaseq/data/preprocessors/relation_extraction_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3828 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/data/preprocessors/sequence_labeling_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1483 2023-01-11 09:41:17.000000 adaseq-0.6.2/adaseq/data/preprocessors/span_extraction_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3744 2023-02-20 09:45:46.000000 adaseq-0.6.2/adaseq/data/preprocessors/twostage_preprocessor.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2650 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/data/span_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)      948 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/data/tokenizer.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1678 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/data/utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)      327 2022-12-14 08:58:36.000000 adaseq-0.6.2/adaseq/main.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4004 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/metainfo.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:18.000000 adaseq-0.6.2/adaseq/metrics/
--rw-r--r--   0 pangda   (1345362) users      (100)      352 2023-02-16 06:13:38.000000 adaseq-0.6.2/adaseq/metrics/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9133 2023-02-16 06:16:11.000000 adaseq-0.6.2/adaseq/metrics/pretraining_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3188 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/metrics/relation_extraction_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4339 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/metrics/sequence_labeling_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4468 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/metrics/span_extraction_metric.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8629 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/metrics/typing_metric.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:19.000000 adaseq-0.6.2/adaseq/models/
--rw-r--r--   0 pangda   (1345362) users      (100)      515 2023-02-16 06:13:38.000000 adaseq-0.6.2/adaseq/models/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9570 2023-02-20 09:45:46.000000 adaseq-0.6.2/adaseq/models/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6735 2023-02-20 09:45:46.000000 adaseq-0.6.2/adaseq/models/biaffine_ner_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9185 2023-02-20 09:45:46.000000 adaseq-0.6.2/adaseq/models/global_pointer_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)    18041 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/models/multilabel_typing_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8812 2023-02-16 07:59:33.000000 adaseq-0.6.2/adaseq/models/pretraining_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4045 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/models/relation_extraction_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8045 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/models/sequence_labeling_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)    11244 2023-02-21 07:28:13.000000 adaseq-0.6.2/adaseq/models/twostage_ner_model.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2304 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/models/utils.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:19.000000 adaseq-0.6.2/adaseq/modules/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.2/adaseq/modules/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2018 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/biaffine.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:20.000000 adaseq-0.6.2/adaseq/modules/decoders/
--rw-r--r--   0 pangda   (1345362) users      (100)      250 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/modules/decoders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4237 2022-12-14 08:58:37.000000 adaseq-0.6.2/adaseq/modules/decoders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)    46589 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/modules/decoders/crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1959 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/modules/decoders/mlm_head.py
--rw-r--r--   0 pangda   (1345362) users      (100)    12649 2022-12-14 08:58:37.000000 adaseq-0.6.2/adaseq/modules/decoders/pairwise_crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6471 2022-12-14 08:58:37.000000 adaseq-0.6.2/adaseq/modules/decoders/partial_crf.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1190 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/dropouts.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:20.000000 adaseq-0.6.2/adaseq/modules/embedders/
--rw-r--r--   0 pangda   (1345362) users      (100)      191 2023-01-10 11:56:59.000000 adaseq-0.6.2/adaseq/modules/embedders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2227 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/embedders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5482 2023-02-08 11:54:02.000000 adaseq-0.6.2/adaseq/modules/embedders/embedding.py
--rw-r--r--   0 pangda   (1345362) users      (100)    17440 2023-02-16 07:59:33.000000 adaseq-0.6.2/adaseq/modules/embedders/transformer_embedder.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:20.000000 adaseq-0.6.2/adaseq/modules/encoders/
--rw-r--r--   0 pangda   (1345362) users      (100)      208 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/encoders/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1854 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/encoders/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     5109 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/encoders/pytorch_rnn_encoder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3070 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/encoders/span_encoder.py
--rw-r--r--   0 pangda   (1345362) users      (100)     7663 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/modules/losses.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4024 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/modules/scalar_mix.py
--rw-r--r--   0 pangda   (1345362) users      (100)     9730 2022-12-30 08:44:17.000000 adaseq-0.6.2/adaseq/modules/util.py
--rw-r--r--   0 pangda   (1345362) users      (100)      547 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/ms_patch.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:21.000000 adaseq-0.6.2/adaseq/pipelines/
--rw-r--r--   0 pangda   (1345362) users      (100)      173 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/pipelines/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1728 2023-01-11 07:11:36.000000 adaseq-0.6.2/adaseq/pipelines/base.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2413 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/pipelines/sequence_labeling_pipeline.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1760 2023-01-10 12:12:52.000000 adaseq-0.6.2/adaseq/pipelines/span_based_ner_pipeline.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:21.000000 adaseq-0.6.2/adaseq/training/
--rw-r--r--   0 pangda   (1345362) users      (100)      207 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/training/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)      621 2023-02-16 06:22:26.000000 adaseq-0.6.2/adaseq/training/default_config.py
--rw-r--r--   0 pangda   (1345362) users      (100)     6339 2023-02-13 12:10:14.000000 adaseq-0.6.2/adaseq/training/default_trainer.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:21.000000 adaseq-0.6.2/adaseq/training/hooks/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.2/adaseq/training/hooks/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)     2987 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/training/hooks/text_logger_hook.py
--rw-r--r--   0 pangda   (1345362) users      (100)      961 2023-01-12 08:59:18.000000 adaseq-0.6.2/adaseq/training/lr_scheduler.py
--rw-r--r--   0 pangda   (1345362) users      (100)     8422 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/training/optimizer.py
--rw-r--r--   0 pangda   (1345362) users      (100)     3282 2023-02-16 06:13:36.000000 adaseq-0.6.2/adaseq/training/typing_trainer.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:22.000000 adaseq-0.6.2/adaseq/utils/
--rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.2/adaseq/utils/__init__.py
--rw-r--r--   0 pangda   (1345362) users      (100)      710 2022-12-14 08:58:37.000000 adaseq-0.6.2/adaseq/utils/checks.py
--rw-r--r--   0 pangda   (1345362) users      (100)     1006 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/utils/common_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)       87 2023-02-21 08:24:32.000000 adaseq-0.6.2/adaseq/utils/constant.py
--rw-r--r--   0 pangda   (1345362) users      (100)      214 2022-12-21 02:38:02.000000 adaseq-0.6.2/adaseq/utils/file_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)      667 2023-02-16 06:13:37.000000 adaseq-0.6.2/adaseq/utils/hub_utils.py
--rw-r--r--   0 pangda   (1345362) users      (100)     4888 2023-01-31 06:40:19.000000 adaseq-0.6.2/adaseq/utils/logging.py
--rw-r--r--   0 pangda   (1345362) users      (100)       72 2023-02-21 08:24:36.000000 adaseq-0.6.2/adaseq/version.py
-drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-02-21 08:26:13.000000 adaseq-0.6.2/adaseq.egg-info/
--rw-r--r--   0 pangda   (1345362) users      (100)     5689 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/PKG-INFO
--rw-r--r--   0 pangda   (1345362) users      (100)     3818 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/SOURCES.txt
--rw-r--r--   0 pangda   (1345362) users      (100)        1 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/dependency_links.txt
--rw-r--r--   0 pangda   (1345362) users      (100)       43 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/entry_points.txt
--rw-r--r--   0 pangda   (1345362) users      (100)      121 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/requires.txt
--rw-r--r--   0 pangda   (1345362) users      (100)        7 2023-02-21 08:26:11.000000 adaseq-0.6.2/adaseq.egg-info/top_level.txt
--rw-r--r--   0 pangda   (1345362) users      (100)      412 2022-12-14 08:58:38.000000 adaseq-0.6.2/pyproject.toml
--rw-r--r--   0 pangda   (1345362) users      (100)       38 2023-02-21 08:26:22.000000 adaseq-0.6.2/setup.cfg
--rw-r--r--   0 pangda   (1345362) users      (100)     4724 2022-12-22 15:49:06.000000 adaseq-0.6.2/setup.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/
+-rw-r--r--   0 pangda   (1345362) users      (100)    11416 2022-12-14 08:58:36.000000 adaseq-0.6.3/LICENSE
+-rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-04-24 06:07:40.000000 adaseq-0.6.3/PKG-INFO
+-rw-r--r--   0 pangda   (1345362) users      (100)     5526 2023-04-24 03:08:57.000000 adaseq-0.6.3/README.md
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/
+-rw-r--r--   0 pangda   (1345362) users      (100)      283 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/__init__.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/commands/
+-rw-r--r--   0 pangda   (1345362) users      (100)      844 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/commands/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4674 2023-02-16 06:14:41.000000 adaseq-0.6.3/adaseq/commands/pretrain.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      360 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/commands/subcommand.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3448 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/commands/test.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9019 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/commands/train.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/data/
+-rw-r--r--   0 pangda   (1345362) users      (100)      155 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1969 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/batch.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      284 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/constant.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq/data/data_collators/
+-rw-r--r--   0 pangda   (1345362) users      (100)      539 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/data/data_collators/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5403 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/data_collators/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1777 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      645 2023-01-12 08:59:17.000000 adaseq-0.6.3/adaseq/data/data_collators/pretraining_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      703 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1275 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1651 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/data/data_collators/twostage_data_collator_with_padding.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/dataset_builders/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/data/dataset_builders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4771 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_builders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4079 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_builders/entity_typing_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7721 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    10006 2023-04-24 04:01:26.000000 adaseq-0.6.3/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4485 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/
+-rw-r--r--   0 pangda   (1345362) users      (100)      139 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1143 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3234 2022-12-21 02:38:01.000000 adaseq-0.6.3/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9864 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/dataset_manager.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/data/preprocessors/
+-rw-r--r--   0 pangda   (1345362) users      (100)      602 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/data/preprocessors/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7010 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/preprocessors/multilabel_typing_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    10258 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/preprocessors/nlp_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5000 2023-01-12 08:59:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/pretraining_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1439 2023-01-11 09:41:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/relation_extraction_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3828 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/data/preprocessors/sequence_labeling_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1483 2023-01-11 09:41:17.000000 adaseq-0.6.3/adaseq/data/preprocessors/span_extraction_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3744 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/data/preprocessors/twostage_preprocessor.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2650 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/data/span_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      948 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/data/tokenizer.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1678 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/data/utils.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/exporters/
+-rw-r--r--   0 pangda   (1345362) users      (100)       76 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      605 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1886 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/exporters/sequence_labeling_model_exporter.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      327 2022-12-14 08:58:36.000000 adaseq-0.6.3/adaseq/main.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4004 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/metainfo.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/metrics/
+-rw-r--r--   0 pangda   (1345362) users      (100)      352 2023-02-16 06:13:38.000000 adaseq-0.6.3/adaseq/metrics/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9133 2023-02-16 06:16:11.000000 adaseq-0.6.3/adaseq/metrics/pretraining_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3188 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/relation_extraction_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4339 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/sequence_labeling_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4468 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/span_extraction_metric.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8629 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/metrics/typing_metric.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:39.000000 adaseq-0.6.3/adaseq/models/
+-rw-r--r--   0 pangda   (1345362) users      (100)      515 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9420 2023-04-24 03:48:13.000000 adaseq-0.6.3/adaseq/models/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6735 2023-02-20 09:45:46.000000 adaseq-0.6.3/adaseq/models/biaffine_ner_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9185 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/global_pointer_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    18041 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/models/multilabel_typing_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8812 2023-02-16 07:59:33.000000 adaseq-0.6.3/adaseq/models/pretraining_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4045 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/models/relation_extraction_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8045 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/models/sequence_labeling_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    11244 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/models/twostage_ner_model.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2304 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/models/utils.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/modules/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2018 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/biaffine.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/decoders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      250 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4237 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    46589 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1959 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/decoders/mlm_head.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    12649 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/pairwise_crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6471 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/modules/decoders/partial_crf.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1190 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/dropouts.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/embedders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      191 2023-01-10 11:56:59.000000 adaseq-0.6.3/adaseq/modules/embedders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2227 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/embedders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5482 2023-02-08 11:54:02.000000 adaseq-0.6.3/adaseq/modules/embedders/embedding.py
+-rw-r--r--   0 pangda   (1345362) users      (100)    17440 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/modules/embedders/transformer_embedder.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/modules/encoders/
+-rw-r--r--   0 pangda   (1345362) users      (100)      208 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1854 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     5109 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/pytorch_rnn_encoder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3070 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/encoders/span_encoder.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     7663 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/modules/losses.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4024 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/modules/scalar_mix.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     9730 2022-12-30 08:44:17.000000 adaseq-0.6.3/adaseq/modules/util.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      547 2023-03-16 03:16:27.000000 adaseq-0.6.3/adaseq/ms_patch.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/pipelines/
+-rw-r--r--   0 pangda   (1345362) users      (100)      173 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/pipelines/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1728 2023-01-11 07:11:36.000000 adaseq-0.6.3/adaseq/pipelines/base.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2413 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/pipelines/sequence_labeling_pipeline.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1760 2023-01-10 12:12:52.000000 adaseq-0.6.3/adaseq/pipelines/span_based_ner_pipeline.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/training/
+-rw-r--r--   0 pangda   (1345362) users      (100)      207 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/training/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      621 2023-02-16 06:22:26.000000 adaseq-0.6.3/adaseq/training/default_config.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     6339 2023-02-13 12:10:14.000000 adaseq-0.6.3/adaseq/training/default_trainer.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/training/hooks/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/training/hooks/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     2987 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/training/hooks/text_logger_hook.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      961 2023-01-12 08:59:18.000000 adaseq-0.6.3/adaseq/training/lr_scheduler.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     8422 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/training/optimizer.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3282 2023-02-16 06:13:36.000000 adaseq-0.6.3/adaseq/training/typing_trainer.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:40.000000 adaseq-0.6.3/adaseq/utils/
+-rw-r--r--   0 pangda   (1345362) users      (100)        0 2023-01-10 07:40:59.000000 adaseq-0.6.3/adaseq/utils/__init__.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      710 2022-12-14 08:58:37.000000 adaseq-0.6.3/adaseq/utils/checks.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     1006 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/utils/common_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)       87 2023-03-07 07:57:58.000000 adaseq-0.6.3/adaseq/utils/constant.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      214 2022-12-21 02:38:02.000000 adaseq-0.6.3/adaseq/utils/file_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)      667 2023-02-16 06:13:37.000000 adaseq-0.6.3/adaseq/utils/hub_utils.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     4888 2023-01-31 06:40:19.000000 adaseq-0.6.3/adaseq/utils/logging.py
+-rw-r--r--   0 pangda   (1345362) users      (100)     3478 2023-03-16 03:51:12.000000 adaseq-0.6.3/adaseq/utils/yaml.py
+-rw-r--r--   0 pangda   (1345362) users      (100)       72 2023-04-24 04:00:39.000000 adaseq-0.6.3/adaseq/version.py
+drwxr-xr-x   0 pangda   (1345362) users      (100)        0 2023-04-24 06:07:38.000000 adaseq-0.6.3/adaseq.egg-info/
+-rw-r--r--   0 pangda   (1345362) users      (100)     5906 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/PKG-INFO
+-rw-r--r--   0 pangda   (1345362) users      (100)     3946 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/SOURCES.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)        1 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/dependency_links.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)       44 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/entry_points.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)      114 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/requires.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)        7 2023-04-24 06:07:37.000000 adaseq-0.6.3/adaseq.egg-info/top_level.txt
+-rw-r--r--   0 pangda   (1345362) users      (100)      412 2022-12-14 08:58:38.000000 adaseq-0.6.3/pyproject.toml
+-rw-r--r--   0 pangda   (1345362) users      (100)       38 2023-04-24 06:07:40.000000 adaseq-0.6.3/setup.cfg
+-rw-r--r--   0 pangda   (1345362) users      (100)     4724 2022-12-22 15:49:06.000000 adaseq-0.6.3/setup.py
```

### Comparing `adaseq-0.6.2/LICENSE` & `adaseq-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/PKG-INFO` & `adaseq-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: adaseq
-Version: 0.6.2
+Version: 0.6.3
 Summary: AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 Home-page: https://github.com/modelscope/adaseq
 Author: Alibaba Damo Academy NLP foundation team
 License: Apache License 2.0
 Platform: any
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 
 <div align="center">
 
 [![license](https://img.shields.io/github/license/modelscope/adaseq.svg)](./LICENSE)
-[![modelscope](https://img.shields.io/badge/modelscope->=1.2.0-624aff.svg)](https://modelscope.cn/)
+[![modelscope](https://img.shields.io/badge/modelscope->=1.4.0-624aff.svg)](https://modelscope.cn/)
 ![version](https://img.shields.io/github/tag/modelscope/adaseq.svg)
 [![issues](https://img.shields.io/github/issues/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/issues)
 [![stars](https://img.shields.io/github/stars/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/stargazers)
 [![downloads](https://static.pepy.tech/personalized-badge/adaseq?period=total&left_color=grey&right_color=yellowgreen&left_text=downloads)](https://pypi.org/project/adaseq)
 [![contribution](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](./CONTRIBUTING.md)
 
 </div>
@@ -55,14 +55,15 @@
   It's easy to register a module, or build a customized sequence understanding model by assembling the predefined modules.
 
 </details>
 
 ⚠️**Notice:** This project is under quick development. This means some interfaces could be changed in the future.
 
 ## 📢 What's New
+- 2022-03: [SemEval 2023] Our U-RaNER Won ***1st place in 9 tracks*** at [SemEval 2023 Task2: Multilingual Complex Named Entity Recognition](https://multiconer.github.io/results)! Source code will be released soon.
 - 2022-12: [[EMNLP 2022] Retrieval-augmented Multimodal Entity Understanding Model (MoRe)](./examples/MoRe)
 - 2022-11: [[EMNLP 2022] Ultra-Fine Entity Typing Model (NPCRF)](./examples/NPCRF)
 - 2022-11: [[EMNLP 2022] Unsupervised Boundary-Aware Language Model (BABERT)](./examples/babert)
 
 ## ⚡ Quick Experience
 You can try out our models via online demos built on ModelScope:
 [[English NER]](https://modelscope.cn/models/damo/nlp_raner_named-entity-recognition_english-large-news/summary)
@@ -126,7 +127,9 @@
   - [TODO] Serving with AdaLA
 
 ## 📝 Contributing
 All contributions are welcome to improve AdaSeq. Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for the contributing guideline.
 
 ## 📄 License
 This project is licensed under the Apache License (Version 2.0).
+
+
```

### Comparing `adaseq-0.6.2/README.md` & `adaseq-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 
 <div align="center">
 
 [![license](https://img.shields.io/github/license/modelscope/adaseq.svg)](./LICENSE)
-[![modelscope](https://img.shields.io/badge/modelscope->=1.2.0-624aff.svg)](https://modelscope.cn/)
+[![modelscope](https://img.shields.io/badge/modelscope->=1.4.0-624aff.svg)](https://modelscope.cn/)
 ![version](https://img.shields.io/github/tag/modelscope/adaseq.svg)
 [![issues](https://img.shields.io/github/issues/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/issues)
 [![stars](https://img.shields.io/github/stars/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/stargazers)
 [![downloads](https://static.pepy.tech/personalized-badge/adaseq?period=total&left_color=grey&right_color=yellowgreen&left_text=downloads)](https://pypi.org/project/adaseq)
 [![contribution](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](./CONTRIBUTING.md)
 
 </div>
@@ -43,14 +43,15 @@
   It's easy to register a module, or build a customized sequence understanding model by assembling the predefined modules.
 
 </details>
 
 ⚠️**Notice:** This project is under quick development. This means some interfaces could be changed in the future.
 
 ## 📢 What's New
+- 2022-03: [SemEval 2023] Our U-RaNER Won ***1st place in 9 tracks*** at [SemEval 2023 Task2: Multilingual Complex Named Entity Recognition](https://multiconer.github.io/results)! Source code will be released soon.
 - 2022-12: [[EMNLP 2022] Retrieval-augmented Multimodal Entity Understanding Model (MoRe)](./examples/MoRe)
 - 2022-11: [[EMNLP 2022] Ultra-Fine Entity Typing Model (NPCRF)](./examples/NPCRF)
 - 2022-11: [[EMNLP 2022] Unsupervised Boundary-Aware Language Model (BABERT)](./examples/babert)
 
 ## ⚡ Quick Experience
 You can try out our models via online demos built on ModelScope:
 [[English NER]](https://modelscope.cn/models/damo/nlp_raner_named-entity-recognition_english-large-news/summary)
```

### Comparing `adaseq-0.6.2/adaseq/commands/__init__.py` & `adaseq-0.6.3/adaseq/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/commands/pretrain.py` & `adaseq-0.6.3/adaseq/commands/pretrain.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/commands/test.py` & `adaseq-0.6.3/adaseq/commands/test.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/commands/train.py` & `adaseq-0.6.3/adaseq/commands/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,37 +16,39 @@
 from adaseq.metainfo import Trainers
 from adaseq.training import build_trainer
 from adaseq.utils.checks import ConfigurationError
 from adaseq.utils.common_utils import create_datetime_str, has_keys
 from adaseq.utils.constant import DEMO_CONFIG
 from adaseq.utils.file_utils import is_empty_dir
 from adaseq.utils.logging import prepare_logging
+from adaseq.utils.yaml import read_yaml
 
 
 class Train(Subcommand):
     """
-    usage: adaseq train [-h] -c CONFIG_PATH [-w WORK_DIR] [-n RUN_NAME]
-                        [-d DEVICE] [-f FORCE] [-ckpt CHECKPOINT_PATH]
-                        [--seed SEED] [--local_rank LOCAL_RANK]
+    usage: adaseq train [-h] -c CONFIG_PATH [-w WORK_DIR] [-n RUN_NAME] [-f FORCE]
+                        [-ckpt CHECKPOINT_PATH] [--seed SEED] [-d DEVICE]
+                        [--use_fp16] [--local_rank LOCAL_RANK]
 
     optional arguments:
       -h, --help            show this help message and exit
       -c CONFIG_PATH, --config_path CONFIG_PATH
                             configuration YAML file
       -w WORK_DIR, --work_dir WORK_DIR
                             directory to save experiment logs and checkpoints
       -n RUN_NAME, --run_name RUN_NAME
                             trial name
-      -d DEVICE, --device DEVICE
-                            device name
       -f FORCE, --force FORCE
                             overwrite the output directory if it exists.
       -ckpt CHECKPOINT_PATH, --checkpoint_path CHECKPOINT_PATH
-                            model checkpoint
+                            model checkpoint to load
       --seed SEED           random seed for everything
+      -d DEVICE, --device DEVICE
+                            device name
+      --use_fp16            whether to use mixed precision
       --local_rank LOCAL_RANK
     """
 
     @classmethod
     def add_subparser(cls, parser: argparse._SubParsersAction) -> argparse.ArgumentParser:
         """Add training arguments parser"""
         subparser = parser.add_parser('train', help='train a model')
@@ -57,46 +59,53 @@
             '-w',
             '--work_dir',
             type=str,
             default=None,
             help='directory to save experiment logs and checkpoints',
         )
         subparser.add_argument('-n', '--run_name', type=str, default=None, help='trial name')
-        subparser.add_argument('-d', '--device', type=str, default='gpu', help='device name')
         subparser.add_argument(
             '-f', '--force', default=None, help='overwrite the output directory if it exists.'
         )
-        subparser.add_argument('-ckpt', '--checkpoint_path', default=None, help='model checkpoint')
+        subparser.add_argument(
+            '-ckpt', '--checkpoint_path', default=None, help='model checkpoint to load'
+        )
         subparser.add_argument('--seed', type=int, default=None, help='random seed for everything')
+        subparser.add_argument('-d', '--device', type=str, default='gpu', help='device name')
+        subparser.add_argument(
+            '--use_fp16', action='store_true', help='whether to use mixed precision'
+        )
         subparser.add_argument('--local_rank', type=str, default='0')
 
         subparser.set_defaults(func=train_model_from_args)
         return subparser
 
 
 def train_model_from_args(args: argparse.Namespace):  # noqa: D103
     train_model(
         config_path_or_dict=args.config_path,
         work_dir=args.work_dir,
         run_name=args.run_name,
-        seed=args.seed,
         force=args.force,
+        seed=args.seed,
         device=args.device,
+        use_fp16=args.use_fp16,
         local_rank=args.local_rank,
         checkpoint_path=args.checkpoint_path,
     )
 
 
 def train_model(
     config_path_or_dict: Union[str, dict],
     work_dir: Optional[str] = None,
     run_name: Optional[str] = None,
-    seed: Optional[int] = None,
     force: bool = False,
+    seed: Optional[int] = None,
     device: str = 'gpu',
+    use_fp16: bool = False,
     local_rank: str = '0',
     checkpoint_path: Optional[str] = None,
 ) -> None:
     """
     Train a model from config file or dict.
     You can manually call this function in a python script for debugging.
     """
@@ -130,19 +139,30 @@
         seed = config.safe_get('experiment.seed', 42)  # 42 by default
         if seed < 0:
             raise ConfigurationError(f'random seed must be greater than 0, got: {seed}')
     else:
         config['experiment']['seed'] = seed
     set_random_seed(seed)
 
+    # A stupid implementation to reload config with `envyaml`
+    new_config_path = os.path.join(work_dir, 'config.yaml')
+    with open(new_config_path, mode='w', encoding='utf8') as file:
+        yaml.dump(config.to_dict(), file, allow_unicode=True)
+
+    parsed = read_yaml(new_config_path)
+    with open(new_config_path, mode='w', encoding='utf8') as file:
+        yaml.dump(parsed, file, allow_unicode=True)
+    config = Config.from_file(new_config_path)
+
     trainer = build_trainer_from_partial_objects(
         config,
         work_dir=work_dir,
         seed=seed,
         device=device,
+        use_fp16=use_fp16,
         local_rank=local_rank,
     )
     trainer.train(checkpoint_path)
     trainer.test()
 
 
 def build_trainer_from_partial_objects(config, work_dir, **kwargs):
```

### Comparing `adaseq-0.6.2/adaseq/data/batch.py` & `adaseq-0.6.3/adaseq/data/batch.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/__init__.py` & `adaseq-0.6.3/adaseq/data/data_collators/__init__.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/base.py` & `adaseq-0.6.3/adaseq/data/data_collators/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py` & `adaseq-0.6.3/adaseq/data/data_collators/multilabel_typing_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/pretraining_data_collator_with_padding.py` & `adaseq-0.6.3/adaseq/data/data_collators/pretraining_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py` & `adaseq-0.6.3/adaseq/data/data_collators/sequence_labeling_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py` & `adaseq-0.6.3/adaseq/data/data_collators/span_extraction_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/data_collators/twostage_data_collator_with_padding.py` & `adaseq-0.6.3/adaseq/data/data_collators/twostage_data_collator_with_padding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_builders/base.py` & `adaseq-0.6.3/adaseq/data/dataset_builders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_builders/entity_typing_dataset_builder.py` & `adaseq-0.6.3/adaseq/data/dataset_builders/entity_typing_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py` & `adaseq-0.6.3/adaseq/data/dataset_builders/mcce_entity_typing_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py` & `adaseq-0.6.3/adaseq/data/dataset_builders/named_entity_recognition_dataset_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 
+import ast
 import json
 from typing import Dict
 
 import datasets
 from datasets import Features, Value
 
 from adaseq.data.constant import PAD_LABEL
@@ -171,36 +172,44 @@
         is_end_included = corpus_config.get('is_end_included', False)
 
         with open(filepath, encoding='utf-8') as f:
             guid = 0
             for line in f:
                 if line.strip() == '':
                     continue
-                example = json.loads(line)
-                text = example[text_key]
-                if isinstance(text, list):
-                    tokens = text
-                elif isinstance(text, str):
-                    if tokenizer == 'char':
-                        tokens = list(text)
-                    elif tokenizer == 'blank':
-                        tokens = text.split(' ')
+                try:
+                    try:
+                        example = json.loads(line)
+                    except:
+                        example = ast.literal_eval(line)
+                    text = example[text_key]
+                    if isinstance(text, list):
+                        tokens = text
+                    elif isinstance(text, str):
+                        if tokenizer == 'char':
+                            tokens = list(text)
+                        elif tokenizer == 'blank':
+                            tokens = text.split(' ')
+                        else:
+                            raise RuntimeError
                     else:
-                        raise RuntimeError
-                else:
-                    raise ValueError('Unsupported text input.')
-                spans = []
-                for span in example[spans_key]:
-                    if is_end_included:
-                        span['end'] += 1
-                    if 'word' in span:
-                        del span['word']
-                    spans.append(span)
-                mask = [True] * len(tokens)
-                yield guid, {'id': str(guid), 'tokens': tokens, 'spans': spans, 'mask': mask}
+                        raise ValueError('Unsupported text input.')
+                    spans = []
+                    for span in example[spans_key]:
+                        if is_end_included:
+                            span['end'] += 1
+                        if 'word' in span:
+                            del span['word']
+                        if isinstance(span['type'], list):
+                            span['type'] = span['type'][0]
+                        spans.append(span)
+                    mask = [True] * len(tokens)
+                    yield guid, {'id': str(guid), 'tokens': tokens, 'spans': spans, 'mask': mask}
+                except:
+                    pass
                 guid += 1
 
     @classmethod
     def _load_cluener_file(cls, filepath, corpus_config):
         is_end_included = corpus_config.get('is_end_included', False)
 
         with open(filepath, encoding='utf-8') as f:
```

### Comparing `adaseq-0.6.2/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py` & `adaseq-0.6.3/adaseq/data/dataset_builders/relation_extraction_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_dumpers/base.py` & `adaseq-0.6.3/adaseq/data/dataset_dumpers/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py` & `adaseq-0.6.3/adaseq/data/dataset_dumpers/named_entity_recognition_dataset_dumper.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/dataset_manager.py` & `adaseq-0.6.3/adaseq/data/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/__init__.py` & `adaseq-0.6.3/adaseq/data/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/multilabel_typing_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/multilabel_typing_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/nlp_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/nlp_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/pretraining_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/pretraining_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/relation_extraction_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/relation_extraction_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/sequence_labeling_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/sequence_labeling_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/span_extraction_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/span_extraction_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/preprocessors/twostage_preprocessor.py` & `adaseq-0.6.3/adaseq/data/preprocessors/twostage_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/span_utils.py` & `adaseq-0.6.3/adaseq/data/span_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/tokenizer.py` & `adaseq-0.6.3/adaseq/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/data/utils.py` & `adaseq-0.6.3/adaseq/data/utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metainfo.py` & `adaseq-0.6.3/adaseq/metainfo.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metrics/pretraining_metric.py` & `adaseq-0.6.3/adaseq/metrics/pretraining_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metrics/relation_extraction_metric.py` & `adaseq-0.6.3/adaseq/metrics/relation_extraction_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metrics/sequence_labeling_metric.py` & `adaseq-0.6.3/adaseq/metrics/sequence_labeling_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metrics/span_extraction_metric.py` & `adaseq-0.6.3/adaseq/metrics/span_extraction_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/metrics/typing_metric.py` & `adaseq-0.6.3/adaseq/metrics/typing_metric.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/__init__.py` & `adaseq-0.6.3/adaseq/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/base.py` & `adaseq-0.6.3/adaseq/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,18 +155,14 @@
         if config is not None:
             # config modification
             config['plugins'] = ['adaseq']
 
             if self.pipeline is not None:
                 config['pipeline'] = {'type': self.pipeline}
 
-            for field in ['experiment', 'dataset', 'train', 'evaluation']:
-                if field in config:
-                    del config[field]
-
             if (
                 'preprocessor' in config
                 and 'label_to_id' not in config['preprocessor']
                 and 'model' in config
                 and 'id_to_label' in config['model']
             ):
                 config['preprocessor']['label_to_id'] = {
```

### Comparing `adaseq-0.6.2/adaseq/models/biaffine_ner_model.py` & `adaseq-0.6.3/adaseq/models/biaffine_ner_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/global_pointer_model.py` & `adaseq-0.6.3/adaseq/models/global_pointer_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/multilabel_typing_model.py` & `adaseq-0.6.3/adaseq/models/multilabel_typing_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/pretraining_model.py` & `adaseq-0.6.3/adaseq/models/pretraining_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/relation_extraction_model.py` & `adaseq-0.6.3/adaseq/models/relation_extraction_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/sequence_labeling_model.py` & `adaseq-0.6.3/adaseq/models/sequence_labeling_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/twostage_ner_model.py` & `adaseq-0.6.3/adaseq/models/twostage_ner_model.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/models/utils.py` & `adaseq-0.6.3/adaseq/models/utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/biaffine.py` & `adaseq-0.6.3/adaseq/modules/biaffine.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/decoders/base.py` & `adaseq-0.6.3/adaseq/modules/decoders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/decoders/crf.py` & `adaseq-0.6.3/adaseq/modules/decoders/crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/decoders/mlm_head.py` & `adaseq-0.6.3/adaseq/modules/decoders/mlm_head.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/decoders/pairwise_crf.py` & `adaseq-0.6.3/adaseq/modules/decoders/pairwise_crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/decoders/partial_crf.py` & `adaseq-0.6.3/adaseq/modules/decoders/partial_crf.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/dropouts.py` & `adaseq-0.6.3/adaseq/modules/dropouts.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/embedders/base.py` & `adaseq-0.6.3/adaseq/modules/embedders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/embedders/embedding.py` & `adaseq-0.6.3/adaseq/modules/embedders/embedding.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/embedders/transformer_embedder.py` & `adaseq-0.6.3/adaseq/modules/embedders/transformer_embedder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/encoders/base.py` & `adaseq-0.6.3/adaseq/modules/encoders/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/encoders/pytorch_rnn_encoder.py` & `adaseq-0.6.3/adaseq/modules/encoders/pytorch_rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/encoders/span_encoder.py` & `adaseq-0.6.3/adaseq/modules/encoders/span_encoder.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/losses.py` & `adaseq-0.6.3/adaseq/modules/losses.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/scalar_mix.py` & `adaseq-0.6.3/adaseq/modules/scalar_mix.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/modules/util.py` & `adaseq-0.6.3/adaseq/modules/util.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/ms_patch.py` & `adaseq-0.6.3/adaseq/ms_patch.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/pipelines/base.py` & `adaseq-0.6.3/adaseq/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/pipelines/sequence_labeling_pipeline.py` & `adaseq-0.6.3/adaseq/pipelines/sequence_labeling_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/pipelines/span_based_ner_pipeline.py` & `adaseq-0.6.3/adaseq/pipelines/span_based_ner_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/default_config.py` & `adaseq-0.6.3/adaseq/training/default_config.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/default_trainer.py` & `adaseq-0.6.3/adaseq/training/default_trainer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/hooks/text_logger_hook.py` & `adaseq-0.6.3/adaseq/training/hooks/text_logger_hook.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/lr_scheduler.py` & `adaseq-0.6.3/adaseq/training/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/optimizer.py` & `adaseq-0.6.3/adaseq/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/training/typing_trainer.py` & `adaseq-0.6.3/adaseq/training/typing_trainer.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/utils/checks.py` & `adaseq-0.6.3/adaseq/utils/checks.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/utils/common_utils.py` & `adaseq-0.6.3/adaseq/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/utils/hub_utils.py` & `adaseq-0.6.3/adaseq/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq/utils/logging.py` & `adaseq-0.6.3/adaseq/utils/logging.py`

 * *Files identical despite different names*

### Comparing `adaseq-0.6.2/adaseq.egg-info/PKG-INFO` & `adaseq-0.6.3/adaseq.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: adaseq
-Version: 0.6.2
+Version: 0.6.3
 Summary: AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 Home-page: https://github.com/modelscope/adaseq
 Author: Alibaba Damo Academy NLP foundation team
 License: Apache License 2.0
 Platform: any
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models
 
 <div align="center">
 
 [![license](https://img.shields.io/github/license/modelscope/adaseq.svg)](./LICENSE)
-[![modelscope](https://img.shields.io/badge/modelscope->=1.2.0-624aff.svg)](https://modelscope.cn/)
+[![modelscope](https://img.shields.io/badge/modelscope->=1.4.0-624aff.svg)](https://modelscope.cn/)
 ![version](https://img.shields.io/github/tag/modelscope/adaseq.svg)
 [![issues](https://img.shields.io/github/issues/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/issues)
 [![stars](https://img.shields.io/github/stars/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/stargazers)
 [![downloads](https://static.pepy.tech/personalized-badge/adaseq?period=total&left_color=grey&right_color=yellowgreen&left_text=downloads)](https://pypi.org/project/adaseq)
 [![contribution](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](./CONTRIBUTING.md)
 
 </div>
@@ -55,14 +55,15 @@
   It's easy to register a module, or build a customized sequence understanding model by assembling the predefined modules.
 
 </details>
 
 ⚠️**Notice:** This project is under quick development. This means some interfaces could be changed in the future.
 
 ## 📢 What's New
+- 2022-03: [SemEval 2023] Our U-RaNER Won ***1st place in 9 tracks*** at [SemEval 2023 Task2: Multilingual Complex Named Entity Recognition](https://multiconer.github.io/results)! Source code will be released soon.
 - 2022-12: [[EMNLP 2022] Retrieval-augmented Multimodal Entity Understanding Model (MoRe)](./examples/MoRe)
 - 2022-11: [[EMNLP 2022] Ultra-Fine Entity Typing Model (NPCRF)](./examples/NPCRF)
 - 2022-11: [[EMNLP 2022] Unsupervised Boundary-Aware Language Model (BABERT)](./examples/babert)
 
 ## ⚡ Quick Experience
 You can try out our models via online demos built on ModelScope:
 [[English NER]](https://modelscope.cn/models/damo/nlp_raner_named-entity-recognition_english-large-news/summary)
@@ -126,7 +127,9 @@
   - [TODO] Serving with AdaLA
 
 ## 📝 Contributing
 All contributions are welcome to improve AdaSeq. Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for the contributing guideline.
 
 ## 📄 License
 This project is licensed under the Apache License (Version 2.0).
+
+
```

### Comparing `adaseq-0.6.2/adaseq.egg-info/SOURCES.txt` & `adaseq-0.6.3/adaseq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 adaseq/data/preprocessors/multilabel_typing_preprocessor.py
 adaseq/data/preprocessors/nlp_preprocessor.py
 adaseq/data/preprocessors/pretraining_preprocessor.py
 adaseq/data/preprocessors/relation_extraction_preprocessor.py
 adaseq/data/preprocessors/sequence_labeling_preprocessor.py
 adaseq/data/preprocessors/span_extraction_preprocessor.py
 adaseq/data/preprocessors/twostage_preprocessor.py
+adaseq/exporters/__init__.py
+adaseq/exporters/base.py
+adaseq/exporters/sequence_labeling_model_exporter.py
 adaseq/metrics/__init__.py
 adaseq/metrics/pretraining_metric.py
 adaseq/metrics/relation_extraction_metric.py
 adaseq/metrics/sequence_labeling_metric.py
 adaseq/metrics/span_extraction_metric.py
 adaseq/metrics/typing_metric.py
 adaseq/models/__init__.py
@@ -99,8 +102,9 @@
 adaseq/training/hooks/text_logger_hook.py
 adaseq/utils/__init__.py
 adaseq/utils/checks.py
 adaseq/utils/common_utils.py
 adaseq/utils/constant.py
 adaseq/utils/file_utils.py
 adaseq/utils/hub_utils.py
-adaseq/utils/logging.py
+adaseq/utils/logging.py
+adaseq/utils/yaml.py
```

### Comparing `adaseq-0.6.2/setup.py` & `adaseq-0.6.3/setup.py`

 * *Files identical despite different names*


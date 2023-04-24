# Comparing `tmp/monai-1.2.0rc4-202304121831-py3-none-any.whl.zip` & `tmp/monai-1.2.0rc5-202304241345-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,366 +1,367 @@
-Zip file size: 1243555 bytes, number of entries: 364
--rw-r--r--  2.0 unx     2276 b- defN 23-Apr-12 18:31 monai/__init__.py
--rw-r--r--  2.0 unx      500 b- defN 23-Apr-12 18:33 monai/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 18:31 monai/py.typed
--rw-r--r--  2.0 unx      642 b- defN 23-Apr-12 18:31 monai/_extensions/__init__.py
--rw-r--r--  2.0 unx     3643 b- defN 23-Apr-12 18:31 monai/_extensions/loader.py
--rw-r--r--  2.0 unx     2931 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm.cpp
--rw-r--r--  2.0 unx     1760 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm.h
--rw-r--r--  2.0 unx     1118 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--  2.0 unx    16213 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--  2.0 unx     3520 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--  2.0 unx      908 b- defN 23-Apr-12 18:31 monai/apps/__init__.py
--rw-r--r--  2.0 unx    34560 b- defN 23-Apr-12 18:31 monai/apps/datasets.py
--rw-r--r--  2.0 unx    13505 b- defN 23-Apr-12 18:31 monai/apps/utils.py
--rw-r--r--  2.0 unx      952 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/__init__.py
--rw-r--r--  2.0 unx     1349 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/__main__.py
--rw-r--r--  2.0 unx    36092 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/auto_runner.py
--rw-r--r--  2.0 unx    23164 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--  2.0 unx    17319 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--  2.0 unx    11249 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--  2.0 unx    17523 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/transforms.py
--rw-r--r--  2.0 unx     2765 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/deepedit/__init__.py
--rw-r--r--  2.0 unx     4501 b- defN 23-Apr-12 18:31 monai/apps/deepedit/interaction.py
--rw-r--r--  2.0 unx    37435 b- defN 23-Apr-12 18:31 monai/apps/deepedit/transforms.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/__init__.py
--rw-r--r--  2.0 unx    10054 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/dataset.py
--rw-r--r--  2.0 unx     3739 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/interaction.py
--rw-r--r--  2.0 unx    42011 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/transforms.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/__init__.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/__init__.py
--rw-r--r--  2.0 unx    26617 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/coco.py
--rw-r--r--  2.0 unx    17161 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/matching.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/__init__.py
--rw-r--r--  2.0 unx    51663 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--  2.0 unx    17604 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/retinanet_network.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/__init__.py
--rw-r--r--  2.0 unx    24519 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/array.py
--rw-r--r--  2.0 unx    17970 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/box_ops.py
--rw-r--r--  2.0 unx    68979 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/dictionary.py
--rw-r--r--  2.0 unx    13531 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/__init__.py
--rw-r--r--  2.0 unx    18681 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/anchor_utils.py
--rw-r--r--  2.0 unx    11120 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/box_coder.py
--rw-r--r--  2.0 unx     9031 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/box_selector.py
--rw-r--r--  2.0 unx    10306 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/detector_utils.py
--rw-r--r--  2.0 unx    13890 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--  2.0 unx     5627 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/predict_utils.py
--rw-r--r--  2.0 unx      726 b- defN 23-Apr-12 18:31 monai/apps/mmars/__init__.py
--rw-r--r--  2.0 unx    13115 b- defN 23-Apr-12 18:31 monai/apps/mmars/mmars.py
--rw-r--r--  2.0 unx     9996 b- defN 23-Apr-12 18:31 monai/apps/mmars/model_desc.py
--rw-r--r--  2.0 unx      745 b- defN 23-Apr-12 18:31 monai/apps/nnunet/__init__.py
--rw-r--r--  2.0 unx     2975 b- defN 23-Apr-12 18:31 monai/apps/nnunet/__main__.py
--rw-r--r--  2.0 unx    38587 b- defN 23-Apr-12 18:31 monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--  2.0 unx     6791 b- defN 23-Apr-12 18:31 monai/apps/nnunet/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/nuclick/__init__.py
--rw-r--r--  2.0 unx    24948 b- defN 23-Apr-12 18:31 monai/apps/nuclick/transforms.py
--rw-r--r--  2.0 unx     1030 b- defN 23-Apr-12 18:31 monai/apps/pathology/__init__.py
--rw-r--r--  2.0 unx     2860 b- defN 23-Apr-12 18:31 monai/apps/pathology/utils.py
--rw-r--r--  2.0 unx      650 b- defN 23-Apr-12 18:31 monai/apps/pathology/engines/__init__.py
--rw-r--r--  2.0 unx     2397 b- defN 23-Apr-12 18:31 monai/apps/pathology/engines/utils.py
--rw-r--r--  2.0 unx      609 b- defN 23-Apr-12 18:31 monai/apps/pathology/handlers/__init__.py
--rw-r--r--  2.0 unx     2315 b- defN 23-Apr-12 18:31 monai/apps/pathology/handlers/utils.py
--rw-r--r--  2.0 unx      660 b- defN 23-Apr-12 18:31 monai/apps/pathology/inferers/__init__.py
--rw-r--r--  2.0 unx     9148 b- defN 23-Apr-12 18:31 monai/apps/pathology/inferers/inferer.py
--rw-r--r--  2.0 unx      650 b- defN 23-Apr-12 18:31 monai/apps/pathology/losses/__init__.py
--rw-r--r--  2.0 unx     7293 b- defN 23-Apr-12 18:31 monai/apps/pathology/losses/hovernet_loss.py
--rw-r--r--  2.0 unx      646 b- defN 23-Apr-12 18:31 monai/apps/pathology/metrics/__init__.py
--rw-r--r--  2.0 unx     7225 b- defN 23-Apr-12 18:31 monai/apps/pathology/metrics/lesion_froc.py
--rw-r--r--  2.0 unx     2243 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/__init__.py
--rw-r--r--  2.0 unx     1995 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--  2.0 unx    37322 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/array.py
--rw-r--r--  2.0 unx    25992 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/dictionary.py
--rw-r--r--  2.0 unx      836 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--  2.0 unx     8366 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/array.py
--rw-r--r--  2.0 unx     4761 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/__init__.py
--rw-r--r--  2.0 unx     8393 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/complex_utils.py
--rw-r--r--  2.0 unx     3644 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--  2.0 unx     2000 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/mri_utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/__init__.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--  2.0 unx     4183 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/blocks/varnetblock.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--  2.0 unx     6215 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--  2.0 unx     4775 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--  2.0 unx    11377 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--  2.0 unx     3831 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/varnet.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/array.py
--rw-r--r--  2.0 unx    15844 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/dictionary.py
--rw-r--r--  2.0 unx      765 b- defN 23-Apr-12 18:31 monai/apps/tcia/__init__.py
--rw-r--r--  2.0 unx     1582 b- defN 23-Apr-12 18:31 monai/apps/tcia/label_desc.py
--rw-r--r--  2.0 unx     6152 b- defN 23-Apr-12 18:31 monai/apps/tcia/utils.py
--rw-r--r--  2.0 unx     1164 b- defN 23-Apr-12 18:31 monai/auto3dseg/__init__.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Apr-12 18:31 monai/auto3dseg/algo_gen.py
--rw-r--r--  2.0 unx    41223 b- defN 23-Apr-12 18:31 monai/auto3dseg/analyzer.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Apr-12 18:31 monai/auto3dseg/operations.py
--rw-r--r--  2.0 unx     8725 b- defN 23-Apr-12 18:31 monai/auto3dseg/seg_summarizer.py
--rw-r--r--  2.0 unx    12193 b- defN 23-Apr-12 18:31 monai/auto3dseg/utils.py
--rw-r--r--  2.0 unx     1341 b- defN 23-Apr-12 18:31 monai/bundle/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-12 18:31 monai/bundle/__main__.py
--rw-r--r--  2.0 unx    16035 b- defN 23-Apr-12 18:31 monai/bundle/config_item.py
--rw-r--r--  2.0 unx    22410 b- defN 23-Apr-12 18:31 monai/bundle/config_parser.py
--rw-r--r--  2.0 unx     8628 b- defN 23-Apr-12 18:31 monai/bundle/properties.py
--rw-r--r--  2.0 unx    14353 b- defN 23-Apr-12 18:31 monai/bundle/reference_resolver.py
--rw-r--r--  2.0 unx    63733 b- defN 23-Apr-12 18:31 monai/bundle/scripts.py
--rw-r--r--  2.0 unx     8911 b- defN 23-Apr-12 18:31 monai/bundle/utils.py
--rw-r--r--  2.0 unx    16520 b- defN 23-Apr-12 18:31 monai/bundle/workflows.py
--rw-r--r--  2.0 unx     1048 b- defN 23-Apr-12 18:31 monai/config/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 23-Apr-12 18:31 monai/config/deviceconfig.py
--rw-r--r--  2.0 unx     3485 b- defN 23-Apr-12 18:31 monai/config/type_definitions.py
--rw-r--r--  2.0 unx     5087 b- defN 23-Apr-12 18:31 monai/data/__init__.py
--rw-r--r--  2.0 unx    50102 b- defN 23-Apr-12 18:31 monai/data/box_utils.py
--rw-r--r--  2.0 unx     4952 b- defN 23-Apr-12 18:31 monai/data/csv_saver.py
--rw-r--r--  2.0 unx     3835 b- defN 23-Apr-12 18:31 monai/data/dataloader.py
--rw-r--r--  2.0 unx    68927 b- defN 23-Apr-12 18:31 monai/data/dataset.py
--rw-r--r--  2.0 unx    10216 b- defN 23-Apr-12 18:31 monai/data/dataset_summary.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Apr-12 18:31 monai/data/decathlon_datalist.py
--rw-r--r--  2.0 unx     4448 b- defN 23-Apr-12 18:31 monai/data/fft_utils.py
--rw-r--r--  2.0 unx     6344 b- defN 23-Apr-12 18:31 monai/data/folder_layout.py
--rw-r--r--  2.0 unx    12484 b- defN 23-Apr-12 18:31 monai/data/grid_dataset.py
--rw-r--r--  2.0 unx     7008 b- defN 23-Apr-12 18:31 monai/data/image_dataset.py
--rw-r--r--  2.0 unx    60619 b- defN 23-Apr-12 18:31 monai/data/image_reader.py
--rw-r--r--  2.0 unx    39872 b- defN 23-Apr-12 18:31 monai/data/image_writer.py
--rw-r--r--  2.0 unx    13309 b- defN 23-Apr-12 18:31 monai/data/iterable_dataset.py
--rw-r--r--  2.0 unx    14097 b- defN 23-Apr-12 18:31 monai/data/itk_torch_bridge.py
--rw-r--r--  2.0 unx     8800 b- defN 23-Apr-12 18:31 monai/data/meta_obj.py
--rw-r--r--  2.0 unx    27321 b- defN 23-Apr-12 18:31 monai/data/meta_tensor.py
--rw-r--r--  2.0 unx     5268 b- defN 23-Apr-12 18:31 monai/data/samplers.py
--rw-r--r--  2.0 unx     7375 b- defN 23-Apr-12 18:31 monai/data/synthetic.py
--rw-r--r--  2.0 unx     9780 b- defN 23-Apr-12 18:31 monai/data/test_time_augmentation.py
--rw-r--r--  2.0 unx     8840 b- defN 23-Apr-12 18:31 monai/data/thread_buffer.py
--rw-r--r--  2.0 unx     5500 b- defN 23-Apr-12 18:31 monai/data/torchscript_utils.py
--rw-r--r--  2.0 unx    64795 b- defN 23-Apr-12 18:31 monai/data/utils.py
--rw-r--r--  2.0 unx     9059 b- defN 23-Apr-12 18:31 monai/data/video_dataset.py
--rw-r--r--  2.0 unx    18631 b- defN 23-Apr-12 18:31 monai/data/wsi_datasets.py
--rw-r--r--  2.0 unx    49442 b- defN 23-Apr-12 18:31 monai/data/wsi_reader.py
--rw-r--r--  2.0 unx     1133 b- defN 23-Apr-12 18:31 monai/engines/__init__.py
--rw-r--r--  2.0 unx    24568 b- defN 23-Apr-12 18:31 monai/engines/evaluator.py
--rw-r--r--  2.0 unx     7278 b- defN 23-Apr-12 18:31 monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--  2.0 unx    21347 b- defN 23-Apr-12 18:31 monai/engines/trainer.py
--rw-r--r--  2.0 unx    11631 b- defN 23-Apr-12 18:31 monai/engines/utils.py
--rw-r--r--  2.0 unx    15250 b- defN 23-Apr-12 18:31 monai/engines/workflow.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/fl/__init__.py
--rw-r--r--  2.0 unx      725 b- defN 23-Apr-12 18:31 monai/fl/client/__init__.py
--rw-r--r--  2.0 unx     5097 b- defN 23-Apr-12 18:31 monai/fl/client/client_algo.py
--rw-r--r--  2.0 unx    32635 b- defN 23-Apr-12 18:31 monai/fl/client/monai_algo.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/fl/utils/__init__.py
--rw-r--r--  2.0 unx     2091 b- defN 23-Apr-12 18:31 monai/fl/utils/constants.py
--rw-r--r--  2.0 unx     3527 b- defN 23-Apr-12 18:31 monai/fl/utils/exchange_object.py
--rw-r--r--  2.0 unx     1628 b- defN 23-Apr-12 18:31 monai/fl/utils/filters.py
--rw-r--r--  2.0 unx     2351 b- defN 23-Apr-12 18:31 monai/handlers/__init__.py
--rw-r--r--  2.0 unx     6798 b- defN 23-Apr-12 18:31 monai/handlers/checkpoint_loader.py
--rw-r--r--  2.0 unx    16071 b- defN 23-Apr-12 18:31 monai/handlers/checkpoint_saver.py
--rw-r--r--  2.0 unx     7606 b- defN 23-Apr-12 18:31 monai/handlers/classification_saver.py
--rw-r--r--  2.0 unx     7506 b- defN 23-Apr-12 18:31 monai/handlers/clearml_handlers.py
--rw-r--r--  2.0 unx     3989 b- defN 23-Apr-12 18:31 monai/handlers/confusion_matrix.py
--rw-r--r--  2.0 unx     4425 b- defN 23-Apr-12 18:31 monai/handlers/decollate_batch.py
--rw-r--r--  2.0 unx     4381 b- defN 23-Apr-12 18:31 monai/handlers/earlystop_handler.py
--rw-r--r--  2.0 unx     3338 b- defN 23-Apr-12 18:31 monai/handlers/garbage_collector.py
--rw-r--r--  2.0 unx     3580 b- defN 23-Apr-12 18:31 monai/handlers/hausdorff_distance.py
--rw-r--r--  2.0 unx     5578 b- defN 23-Apr-12 18:31 monai/handlers/ignite_metric.py
--rw-r--r--  2.0 unx     3931 b- defN 23-Apr-12 18:31 monai/handlers/logfile_handler.py
--rw-r--r--  2.0 unx     3575 b- defN 23-Apr-12 18:31 monai/handlers/lr_schedule_handler.py
--rw-r--r--  2.0 unx     2832 b- defN 23-Apr-12 18:31 monai/handlers/mean_dice.py
--rw-r--r--  2.0 unx     2831 b- defN 23-Apr-12 18:31 monai/handlers/mean_iou.py
--rw-r--r--  2.0 unx     5477 b- defN 23-Apr-12 18:31 monai/handlers/metric_logger.py
--rw-r--r--  2.0 unx     6168 b- defN 23-Apr-12 18:31 monai/handlers/metrics_reloaded_handler.py
--rw-r--r--  2.0 unx     8560 b- defN 23-Apr-12 18:31 monai/handlers/metrics_saver.py
--rw-r--r--  2.0 unx    16326 b- defN 23-Apr-12 18:31 monai/handlers/mlflow_handler.py
--rw-r--r--  2.0 unx     6819 b- defN 23-Apr-12 18:31 monai/handlers/nvtx_handlers.py
--rw-r--r--  2.0 unx     3637 b- defN 23-Apr-12 18:31 monai/handlers/panoptic_quality.py
--rw-r--r--  2.0 unx     7119 b- defN 23-Apr-12 18:31 monai/handlers/parameter_scheduler.py
--rw-r--r--  2.0 unx     3285 b- defN 23-Apr-12 18:31 monai/handlers/postprocessing.py
--rw-r--r--  2.0 unx     5336 b- defN 23-Apr-12 18:31 monai/handlers/probability_maps.py
--rw-r--r--  2.0 unx     8422 b- defN 23-Apr-12 18:31 monai/handlers/regression_metrics.py
--rw-r--r--  2.0 unx     2730 b- defN 23-Apr-12 18:31 monai/handlers/roc_auc.py
--rw-r--r--  2.0 unx     3051 b- defN 23-Apr-12 18:31 monai/handlers/smartcache_handler.py
--rw-r--r--  2.0 unx    14251 b- defN 23-Apr-12 18:31 monai/handlers/stats_handler.py
--rw-r--r--  2.0 unx     3313 b- defN 23-Apr-12 18:31 monai/handlers/surface_distance.py
--rw-r--r--  2.0 unx    23325 b- defN 23-Apr-12 18:31 monai/handlers/tensorboard_handlers.py
--rw-r--r--  2.0 unx     9855 b- defN 23-Apr-12 18:31 monai/handlers/utils.py
--rw-r--r--  2.0 unx     3269 b- defN 23-Apr-12 18:31 monai/handlers/validation_handler.py
--rw-r--r--  2.0 unx      857 b- defN 23-Apr-12 18:31 monai/inferers/__init__.py
--rw-r--r--  2.0 unx    27881 b- defN 23-Apr-12 18:31 monai/inferers/inferer.py
--rw-r--r--  2.0 unx     6393 b- defN 23-Apr-12 18:31 monai/inferers/merger.py
--rw-r--r--  2.0 unx     9397 b- defN 23-Apr-12 18:31 monai/inferers/splitter.py
--rw-r--r--  2.0 unx    20036 b- defN 23-Apr-12 18:31 monai/inferers/utils.py
--rw-r--r--  2.0 unx     1409 b- defN 23-Apr-12 18:31 monai/losses/__init__.py
--rw-r--r--  2.0 unx     3430 b- defN 23-Apr-12 18:31 monai/losses/contrastive.py
--rw-r--r--  2.0 unx     4979 b- defN 23-Apr-12 18:31 monai/losses/deform.py
--rw-r--r--  2.0 unx    46326 b- defN 23-Apr-12 18:31 monai/losses/dice.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Apr-12 18:31 monai/losses/ds_loss.py
--rw-r--r--  2.0 unx     9490 b- defN 23-Apr-12 18:31 monai/losses/focal_loss.py
--rw-r--r--  2.0 unx     2795 b- defN 23-Apr-12 18:31 monai/losses/giou_loss.py
--rw-r--r--  2.0 unx    15492 b- defN 23-Apr-12 18:31 monai/losses/image_dissimilarity.py
--rw-r--r--  2.0 unx     3636 b- defN 23-Apr-12 18:31 monai/losses/multi_scale.py
--rw-r--r--  2.0 unx     2942 b- defN 23-Apr-12 18:31 monai/losses/spatial_mask.py
--rw-r--r--  2.0 unx     4292 b- defN 23-Apr-12 18:31 monai/losses/ssim_loss.py
--rw-r--r--  2.0 unx     6645 b- defN 23-Apr-12 18:31 monai/losses/tversky.py
--rw-r--r--  2.0 unx    10224 b- defN 23-Apr-12 18:31 monai/losses/unified_focal_loss.py
--rw-r--r--  2.0 unx     1977 b- defN 23-Apr-12 18:31 monai/metrics/__init__.py
--rw-r--r--  2.0 unx     8211 b- defN 23-Apr-12 18:31 monai/metrics/active_learning_metrics.py
--rw-r--r--  2.0 unx    15101 b- defN 23-Apr-12 18:31 monai/metrics/confusion_matrix.py
--rw-r--r--  2.0 unx     5578 b- defN 23-Apr-12 18:31 monai/metrics/cumulative_average.py
--rw-r--r--  2.0 unx     4026 b- defN 23-Apr-12 18:31 monai/metrics/f_beta_score.py
--rw-r--r--  2.0 unx     6157 b- defN 23-Apr-12 18:31 monai/metrics/froc.py
--rw-r--r--  2.0 unx     8262 b- defN 23-Apr-12 18:31 monai/metrics/generalized_dice.py
--rw-r--r--  2.0 unx    11470 b- defN 23-Apr-12 18:31 monai/metrics/hausdorff_distance.py
--rw-r--r--  2.0 unx     4907 b- defN 23-Apr-12 18:31 monai/metrics/loss_metric.py
--rw-r--r--  2.0 unx    10937 b- defN 23-Apr-12 18:31 monai/metrics/meandice.py
--rw-r--r--  2.0 unx     7209 b- defN 23-Apr-12 18:31 monai/metrics/meaniou.py
--rw-r--r--  2.0 unx    15140 b- defN 23-Apr-12 18:31 monai/metrics/metric.py
--rw-r--r--  2.0 unx    13679 b- defN 23-Apr-12 18:31 monai/metrics/panoptic_quality.py
--rw-r--r--  2.0 unx    18235 b- defN 23-Apr-12 18:31 monai/metrics/regression.py
--rw-r--r--  2.0 unx     8038 b- defN 23-Apr-12 18:31 monai/metrics/rocauc.py
--rw-r--r--  2.0 unx    14415 b- defN 23-Apr-12 18:31 monai/metrics/surface_dice.py
--rw-r--r--  2.0 unx    10186 b- defN 23-Apr-12 18:31 monai/metrics/surface_distance.py
--rw-r--r--  2.0 unx    15100 b- defN 23-Apr-12 18:31 monai/metrics/utils.py
--rw-r--r--  2.0 unx    11772 b- defN 23-Apr-12 18:31 monai/metrics/wrapper.py
--rw-r--r--  2.0 unx     1020 b- defN 23-Apr-12 18:31 monai/networks/__init__.py
--rw-r--r--  2.0 unx    46286 b- defN 23-Apr-12 18:31 monai/networks/utils.py
--rw-r--r--  2.0 unx     2134 b- defN 23-Apr-12 18:31 monai/networks/blocks/__init__.py
--rw-r--r--  2.0 unx     4275 b- defN 23-Apr-12 18:31 monai/networks/blocks/acti_norm.py
--rw-r--r--  2.0 unx     5839 b- defN 23-Apr-12 18:31 monai/networks/blocks/activation.py
--rw-r--r--  2.0 unx     4380 b- defN 23-Apr-12 18:31 monai/networks/blocks/aspp.py
--rw-r--r--  2.0 unx     7490 b- defN 23-Apr-12 18:31 monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--  2.0 unx    11686 b- defN 23-Apr-12 18:31 monai/networks/blocks/convolutions.py
--rw-r--r--  2.0 unx     5009 b- defN 23-Apr-12 18:31 monai/networks/blocks/crf.py
--rw-r--r--  2.0 unx     4740 b- defN 23-Apr-12 18:31 monai/networks/blocks/denseblock.py
--rw-r--r--  2.0 unx     9255 b- defN 23-Apr-12 18:31 monai/networks/blocks/dints_block.py
--rw-r--r--  2.0 unx     2413 b- defN 23-Apr-12 18:31 monai/networks/blocks/downsample.py
--rw-r--r--  2.0 unx    11062 b- defN 23-Apr-12 18:31 monai/networks/blocks/dynunet_block.py
--rw-r--r--  2.0 unx     3669 b- defN 23-Apr-12 18:31 monai/networks/blocks/encoder.py
--rw-r--r--  2.0 unx     9024 b- defN 23-Apr-12 18:31 monai/networks/blocks/fcn.py
--rw-r--r--  2.0 unx    10586 b- defN 23-Apr-12 18:31 monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--  2.0 unx     8263 b- defN 23-Apr-12 18:31 monai/networks/blocks/fft_utils_t.py
--rw-r--r--  2.0 unx    11454 b- defN 23-Apr-12 18:31 monai/networks/blocks/localnet_block.py
--rw-r--r--  2.0 unx     2813 b- defN 23-Apr-12 18:31 monai/networks/blocks/mlp.py
--rw-r--r--  2.0 unx     7987 b- defN 23-Apr-12 18:31 monai/networks/blocks/patchembedding.py
--rw-r--r--  2.0 unx     8825 b- defN 23-Apr-12 18:31 monai/networks/blocks/regunet_block.py
--rw-r--r--  2.0 unx     3245 b- defN 23-Apr-12 18:31 monai/networks/blocks/segresnet_block.py
--rw-r--r--  2.0 unx     3099 b- defN 23-Apr-12 18:31 monai/networks/blocks/selfattention.py
--rw-r--r--  2.0 unx    12752 b- defN 23-Apr-12 18:31 monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--  2.0 unx     2322 b- defN 23-Apr-12 18:31 monai/networks/blocks/transformerblock.py
--rw-r--r--  2.0 unx     9049 b- defN 23-Apr-12 18:31 monai/networks/blocks/unetr_block.py
--rw-r--r--  2.0 unx    13312 b- defN 23-Apr-12 18:31 monai/networks/blocks/upsample.py
--rw-r--r--  2.0 unx     6656 b- defN 23-Apr-12 18:31 monai/networks/blocks/warp.py
--rw-r--r--  2.0 unx     1562 b- defN 23-Apr-12 18:31 monai/networks/layers/__init__.py
--rw-r--r--  2.0 unx     8288 b- defN 23-Apr-12 18:31 monai/networks/layers/convutils.py
--rw-r--r--  2.0 unx     1802 b- defN 23-Apr-12 18:31 monai/networks/layers/drop_path.py
--rw-r--r--  2.0 unx    12620 b- defN 23-Apr-12 18:31 monai/networks/layers/factories.py
--rw-r--r--  2.0 unx    17992 b- defN 23-Apr-12 18:31 monai/networks/layers/filtering.py
--rw-r--r--  2.0 unx     3324 b- defN 23-Apr-12 18:31 monai/networks/layers/gmm.py
--rw-r--r--  2.0 unx    28470 b- defN 23-Apr-12 18:31 monai/networks/layers/simplelayers.py
--rw-r--r--  2.0 unx    25576 b- defN 23-Apr-12 18:31 monai/networks/layers/spatial_transforms.py
--rw-r--r--  2.0 unx     4296 b- defN 23-Apr-12 18:31 monai/networks/layers/utils.py
--rw-r--r--  2.0 unx     2253 b- defN 23-Apr-12 18:31 monai/networks/layers/weight_init.py
--rw-r--r--  2.0 unx     3141 b- defN 23-Apr-12 18:31 monai/networks/nets/__init__.py
--rw-r--r--  2.0 unx    21533 b- defN 23-Apr-12 18:31 monai/networks/nets/ahnet.py
--rw-r--r--  2.0 unx     9202 b- defN 23-Apr-12 18:31 monai/networks/nets/attentionunet.py
--rw-r--r--  2.0 unx    12089 b- defN 23-Apr-12 18:31 monai/networks/nets/autoencoder.py
--rw-r--r--  2.0 unx    10950 b- defN 23-Apr-12 18:31 monai/networks/nets/basic_unet.py
--rw-r--r--  2.0 unx     7960 b- defN 23-Apr-12 18:31 monai/networks/nets/basic_unetplusplus.py
--rw-r--r--  2.0 unx     6293 b- defN 23-Apr-12 18:31 monai/networks/nets/classifier.py
--rw-r--r--  2.0 unx    15820 b- defN 23-Apr-12 18:31 monai/networks/nets/densenet.py
--rw-r--r--  2.0 unx    44771 b- defN 23-Apr-12 18:31 monai/networks/nets/dints.py
--rw-r--r--  2.0 unx    18210 b- defN 23-Apr-12 18:31 monai/networks/nets/dynunet.py
--rw-r--r--  2.0 unx    40643 b- defN 23-Apr-12 18:31 monai/networks/nets/efficientnet.py
--rw-r--r--  2.0 unx    14147 b- defN 23-Apr-12 18:31 monai/networks/nets/flexible_unet.py
--rw-r--r--  2.0 unx     7212 b- defN 23-Apr-12 18:31 monai/networks/nets/fullyconnectednet.py
--rw-r--r--  2.0 unx     6581 b- defN 23-Apr-12 18:31 monai/networks/nets/generator.py
--rw-r--r--  2.0 unx     8882 b- defN 23-Apr-12 18:31 monai/networks/nets/highresnet.py
--rw-r--r--  2.0 unx    28678 b- defN 23-Apr-12 18:31 monai/networks/nets/hovernet.py
--rw-r--r--  2.0 unx     9812 b- defN 23-Apr-12 18:31 monai/networks/nets/milmodel.py
--rw-r--r--  2.0 unx     6102 b- defN 23-Apr-12 18:31 monai/networks/nets/netadapter.py
--rw-r--r--  2.0 unx     6488 b- defN 23-Apr-12 18:31 monai/networks/nets/regressor.py
--rw-r--r--  2.0 unx    17189 b- defN 23-Apr-12 18:31 monai/networks/nets/regunet.py
--rw-r--r--  2.0 unx    16785 b- defN 23-Apr-12 18:31 monai/networks/nets/resnet.py
--rw-r--r--  2.0 unx    13994 b- defN 23-Apr-12 18:31 monai/networks/nets/segresnet.py
--rw-r--r--  2.0 unx    15667 b- defN 23-Apr-12 18:31 monai/networks/nets/segresnet_ds.py
--rw-r--r--  2.0 unx    19289 b- defN 23-Apr-12 18:31 monai/networks/nets/senet.py
--rw-r--r--  2.0 unx    42000 b- defN 23-Apr-12 18:31 monai/networks/nets/swin_unetr.py
--rw-r--r--  2.0 unx     6248 b- defN 23-Apr-12 18:31 monai/networks/nets/torchvision_fc.py
--rw-r--r--  2.0 unx    16626 b- defN 23-Apr-12 18:31 monai/networks/nets/transchex.py
--rw-r--r--  2.0 unx    13722 b- defN 23-Apr-12 18:31 monai/networks/nets/unet.py
--rw-r--r--  2.0 unx     7943 b- defN 23-Apr-12 18:31 monai/networks/nets/unetr.py
--rw-r--r--  2.0 unx     6285 b- defN 23-Apr-12 18:31 monai/networks/nets/varautoencoder.py
--rw-r--r--  2.0 unx     5655 b- defN 23-Apr-12 18:31 monai/networks/nets/vit.py
--rw-r--r--  2.0 unx     4817 b- defN 23-Apr-12 18:31 monai/networks/nets/vitautoenc.py
--rw-r--r--  2.0 unx    10011 b- defN 23-Apr-12 18:31 monai/networks/nets/vnet.py
--rw-r--r--  2.0 unx      796 b- defN 23-Apr-12 18:31 monai/optimizers/__init__.py
--rw-r--r--  2.0 unx    21948 b- defN 23-Apr-12 18:31 monai/optimizers/lr_finder.py
--rw-r--r--  2.0 unx     3652 b- defN 23-Apr-12 18:31 monai/optimizers/lr_scheduler.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Apr-12 18:31 monai/optimizers/novograd.py
--rw-r--r--  2.0 unx     4131 b- defN 23-Apr-12 18:31 monai/optimizers/utils.py
--rw-r--r--  2.0 unx    15216 b- defN 23-Apr-12 18:31 monai/transforms/__init__.py
--rw-r--r--  2.0 unx     8946 b- defN 23-Apr-12 18:31 monai/transforms/adaptors.py
--rw-r--r--  2.0 unx    40532 b- defN 23-Apr-12 18:31 monai/transforms/compose.py
--rw-r--r--  2.0 unx    17160 b- defN 23-Apr-12 18:31 monai/transforms/inverse.py
--rw-r--r--  2.0 unx     7054 b- defN 23-Apr-12 18:31 monai/transforms/inverse_batch_transform.py
--rw-r--r--  2.0 unx     3386 b- defN 23-Apr-12 18:31 monai/transforms/nvtx.py
--rw-r--r--  2.0 unx     2885 b- defN 23-Apr-12 18:31 monai/transforms/traits.py
--rw-r--r--  2.0 unx    18234 b- defN 23-Apr-12 18:31 monai/transforms/transform.py
--rw-r--r--  2.0 unx    71153 b- defN 23-Apr-12 18:31 monai/transforms/utils.py
--rw-r--r--  2.0 unx    31081 b- defN 23-Apr-12 18:31 monai/transforms/utils_create_transform_ims.py
--rw-r--r--  2.0 unx    18397 b- defN 23-Apr-12 18:31 monai/transforms/utils_pytorch_numpy_unification.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/croppad/__init__.py
--rw-r--r--  2.0 unx    68728 b- defN 23-Apr-12 18:31 monai/transforms/croppad/array.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Apr-12 18:31 monai/transforms/croppad/batch.py
--rw-r--r--  2.0 unx    54071 b- defN 23-Apr-12 18:31 monai/transforms/croppad/dictionary.py
--rw-r--r--  2.0 unx    12673 b- defN 23-Apr-12 18:31 monai/transforms/croppad/functional.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/intensity/__init__.py
--rw-r--r--  2.0 unx    98613 b- defN 23-Apr-12 18:31 monai/transforms/intensity/array.py
--rw-r--r--  2.0 unx    76501 b- defN 23-Apr-12 18:31 monai/transforms/intensity/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/io/__init__.py
--rw-r--r--  2.0 unx    25430 b- defN 23-Apr-12 18:31 monai/transforms/io/array.py
--rw-r--r--  2.0 unx    17821 b- defN 23-Apr-12 18:31 monai/transforms/io/dictionary.py
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-12 18:31 monai/transforms/lazy/__init__.py
--rw-r--r--  2.0 unx     5552 b- defN 23-Apr-12 18:31 monai/transforms/lazy/functional.py
--rw-r--r--  2.0 unx     9739 b- defN 23-Apr-12 18:31 monai/transforms/lazy/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/meta_utility/__init__.py
--rw-r--r--  2.0 unx     4896 b- defN 23-Apr-12 18:31 monai/transforms/meta_utility/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/post/__init__.py
--rw-r--r--  2.0 unx    40858 b- defN 23-Apr-12 18:31 monai/transforms/post/array.py
--rw-r--r--  2.0 unx    39905 b- defN 23-Apr-12 18:31 monai/transforms/post/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/signal/__init__.py
--rw-r--r--  2.0 unx    16378 b- defN 23-Apr-12 18:31 monai/transforms/signal/array.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/__init__.py
--rw-r--r--  2.0 unx    17833 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/array.py
--rw-r--r--  2.0 unx    11194 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/spatial/__init__.py
--rw-r--r--  2.0 unx   168618 b- defN 23-Apr-12 18:31 monai/transforms/spatial/array.py
--rw-r--r--  2.0 unx   107151 b- defN 23-Apr-12 18:31 monai/transforms/spatial/dictionary.py
--rw-r--r--  2.0 unx    31494 b- defN 23-Apr-12 18:31 monai/transforms/spatial/functional.py
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/utility/__init__.py
--rw-r--r--  2.0 unx    70325 b- defN 23-Apr-12 18:31 monai/transforms/utility/array.py
--rw-r--r--  2.0 unx    75816 b- defN 23-Apr-12 18:31 monai/transforms/utility/dictionary.py
--rw-r--r--  2.0 unx     3366 b- defN 23-Apr-12 18:31 monai/utils/__init__.py
--rw-r--r--  2.0 unx     4099 b- defN 23-Apr-12 18:31 monai/utils/aliases.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Apr-12 18:31 monai/utils/decorators.py
--rw-r--r--  2.0 unx    14759 b- defN 23-Apr-12 18:31 monai/utils/deprecate_utils.py
--rw-r--r--  2.0 unx     8526 b- defN 23-Apr-12 18:31 monai/utils/dist.py
--rw-r--r--  2.0 unx    16807 b- defN 23-Apr-12 18:31 monai/utils/enums.py
--rw-r--r--  2.0 unx    15637 b- defN 23-Apr-12 18:31 monai/utils/jupyter_utils.py
--rw-r--r--  2.0 unx    27512 b- defN 23-Apr-12 18:31 monai/utils/misc.py
--rw-r--r--  2.0 unx    23631 b- defN 23-Apr-12 18:31 monai/utils/module.py
--rw-r--r--  2.0 unx     6876 b- defN 23-Apr-12 18:31 monai/utils/nvtx.py
--rw-r--r--  2.0 unx    15936 b- defN 23-Apr-12 18:31 monai/utils/profiling.py
--rw-r--r--  2.0 unx     5955 b- defN 23-Apr-12 18:31 monai/utils/state_cacher.py
--rw-r--r--  2.0 unx    21147 b- defN 23-Apr-12 18:31 monai/utils/type_conversion.py
--rw-r--r--  2.0 unx     1038 b- defN 23-Apr-12 18:31 monai/visualize/__init__.py
--rw-r--r--  2.0 unx    16156 b- defN 23-Apr-12 18:31 monai/visualize/class_activation_maps.py
--rw-r--r--  2.0 unx     6277 b- defN 23-Apr-12 18:31 monai/visualize/gradient_based.py
--rw-r--r--  2.0 unx     9200 b- defN 23-Apr-12 18:31 monai/visualize/img2tensorboard.py
--rw-r--r--  2.0 unx    18816 b- defN 23-Apr-12 18:31 monai/visualize/occlusion_sensitivity.py
--rw-r--r--  2.0 unx     9966 b- defN 23-Apr-12 18:31 monai/visualize/utils.py
--rw-r--r--  2.0 unx     1377 b- defN 23-Apr-12 18:31 monai/visualize/visualizer.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/LICENSE
--rw-r--r--  2.0 unx    10172 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    32603 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/RECORD
-364 files, 4707907 bytes uncompressed, 1192237 bytes compressed:  74.7%
+Zip file size: 1253120 bytes, number of entries: 365
+-rw-r--r--  2.0 unx     2276 b- defN 23-Apr-24 13:45 monai/__init__.py
+-rw-r--r--  2.0 unx      500 b- defN 23-Apr-24 13:47 monai/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-24 13:45 monai/py.typed
+-rw-r--r--  2.0 unx      642 b- defN 23-Apr-24 13:45 monai/_extensions/__init__.py
+-rw-r--r--  2.0 unx     3643 b- defN 23-Apr-24 13:45 monai/_extensions/loader.py
+-rw-r--r--  2.0 unx     2931 b- defN 23-Apr-24 13:45 monai/_extensions/gmm/gmm.cpp
+-rw-r--r--  2.0 unx     1760 b- defN 23-Apr-24 13:45 monai/_extensions/gmm/gmm.h
+-rw-r--r--  2.0 unx     1118 b- defN 23-Apr-24 13:45 monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--  2.0 unx    16213 b- defN 23-Apr-24 13:45 monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--  2.0 unx     3520 b- defN 23-Apr-24 13:45 monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--  2.0 unx      908 b- defN 23-Apr-24 13:45 monai/apps/__init__.py
+-rw-r--r--  2.0 unx    34568 b- defN 23-Apr-24 13:45 monai/apps/datasets.py
+-rw-r--r--  2.0 unx    13505 b- defN 23-Apr-24 13:45 monai/apps/utils.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/__init__.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/__main__.py
+-rw-r--r--  2.0 unx    37585 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--  2.0 unx    26014 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--  2.0 unx    17319 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--  2.0 unx    24328 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--  2.0 unx    17523 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/transforms.py
+-rw-r--r--  2.0 unx     2917 b- defN 23-Apr-24 13:45 monai/apps/auto3dseg/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/deepedit/__init__.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-Apr-24 13:45 monai/apps/deepedit/interaction.py
+-rw-r--r--  2.0 unx    37435 b- defN 23-Apr-24 13:45 monai/apps/deepedit/transforms.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/deepgrow/__init__.py
+-rw-r--r--  2.0 unx    10054 b- defN 23-Apr-24 13:45 monai/apps/deepgrow/dataset.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-Apr-24 13:45 monai/apps/deepgrow/interaction.py
+-rw-r--r--  2.0 unx    42011 b- defN 23-Apr-24 13:45 monai/apps/deepgrow/transforms.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/detection/__init__.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/detection/metrics/__init__.py
+-rw-r--r--  2.0 unx    26617 b- defN 23-Apr-24 13:45 monai/apps/detection/metrics/coco.py
+-rw-r--r--  2.0 unx    17161 b- defN 23-Apr-24 13:45 monai/apps/detection/metrics/matching.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/detection/networks/__init__.py
+-rw-r--r--  2.0 unx    53221 b- defN 23-Apr-24 13:45 monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--  2.0 unx    18850 b- defN 23-Apr-24 13:45 monai/apps/detection/networks/retinanet_network.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/detection/transforms/__init__.py
+-rw-r--r--  2.0 unx    24519 b- defN 23-Apr-24 13:45 monai/apps/detection/transforms/array.py
+-rw-r--r--  2.0 unx    17916 b- defN 23-Apr-24 13:45 monai/apps/detection/transforms/box_ops.py
+-rw-r--r--  2.0 unx    68979 b- defN 23-Apr-24 13:45 monai/apps/detection/transforms/dictionary.py
+-rw-r--r--  2.0 unx    13531 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/__init__.py
+-rw-r--r--  2.0 unx    18681 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--  2.0 unx    11120 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/box_coder.py
+-rw-r--r--  2.0 unx     9031 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/box_selector.py
+-rw-r--r--  2.0 unx    10306 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/detector_utils.py
+-rw-r--r--  2.0 unx    13890 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--  2.0 unx     5818 b- defN 23-Apr-24 13:45 monai/apps/detection/utils/predict_utils.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-24 13:45 monai/apps/mmars/__init__.py
+-rw-r--r--  2.0 unx    13115 b- defN 23-Apr-24 13:45 monai/apps/mmars/mmars.py
+-rw-r--r--  2.0 unx     9996 b- defN 23-Apr-24 13:45 monai/apps/mmars/model_desc.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-24 13:45 monai/apps/nnunet/__init__.py
+-rw-r--r--  2.0 unx     2975 b- defN 23-Apr-24 13:45 monai/apps/nnunet/__main__.py
+-rw-r--r--  2.0 unx    38587 b- defN 23-Apr-24 13:45 monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--  2.0 unx     6791 b- defN 23-Apr-24 13:45 monai/apps/nnunet/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/nuclick/__init__.py
+-rw-r--r--  2.0 unx    24948 b- defN 23-Apr-24 13:45 monai/apps/nuclick/transforms.py
+-rw-r--r--  2.0 unx     1030 b- defN 23-Apr-24 13:45 monai/apps/pathology/__init__.py
+-rw-r--r--  2.0 unx     2860 b- defN 23-Apr-24 13:45 monai/apps/pathology/utils.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Apr-24 13:45 monai/apps/pathology/engines/__init__.py
+-rw-r--r--  2.0 unx     2397 b- defN 23-Apr-24 13:45 monai/apps/pathology/engines/utils.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-24 13:45 monai/apps/pathology/handlers/__init__.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Apr-24 13:45 monai/apps/pathology/handlers/utils.py
+-rw-r--r--  2.0 unx      660 b- defN 23-Apr-24 13:45 monai/apps/pathology/inferers/__init__.py
+-rw-r--r--  2.0 unx     9148 b- defN 23-Apr-24 13:45 monai/apps/pathology/inferers/inferer.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Apr-24 13:45 monai/apps/pathology/losses/__init__.py
+-rw-r--r--  2.0 unx     7293 b- defN 23-Apr-24 13:45 monai/apps/pathology/losses/hovernet_loss.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Apr-24 13:45 monai/apps/pathology/metrics/__init__.py
+-rw-r--r--  2.0 unx     7225 b- defN 23-Apr-24 13:45 monai/apps/pathology/metrics/lesion_froc.py
+-rw-r--r--  2.0 unx     2243 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/__init__.py
+-rw-r--r--  2.0 unx     1995 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--  2.0 unx    37322 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/post/array.py
+-rw-r--r--  2.0 unx    25928 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/post/dictionary.py
+-rw-r--r--  2.0 unx      836 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--  2.0 unx     8366 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--  2.0 unx     4761 b- defN 23-Apr-24 13:45 monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/__init__.py
+-rw-r--r--  2.0 unx     8393 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/complex_utils.py
+-rw-r--r--  2.0 unx     3644 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--  2.0 unx     2000 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/mri_utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/__init__.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--  2.0 unx     4183 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/blocks/varnetblock.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--  2.0 unx     6215 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--  2.0 unx     4775 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--  2.0 unx    11377 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--  2.0 unx     3831 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/networks/nets/varnet.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/transforms/array.py
+-rw-r--r--  2.0 unx    15844 b- defN 23-Apr-24 13:45 monai/apps/reconstruction/transforms/dictionary.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Apr-24 13:45 monai/apps/tcia/__init__.py
+-rw-r--r--  2.0 unx     1582 b- defN 23-Apr-24 13:45 monai/apps/tcia/label_desc.py
+-rw-r--r--  2.0 unx     6152 b- defN 23-Apr-24 13:45 monai/apps/tcia/utils.py
+-rw-r--r--  2.0 unx     1164 b- defN 23-Apr-24 13:45 monai/auto3dseg/__init__.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Apr-24 13:45 monai/auto3dseg/algo_gen.py
+-rw-r--r--  2.0 unx    41223 b- defN 23-Apr-24 13:45 monai/auto3dseg/analyzer.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Apr-24 13:45 monai/auto3dseg/operations.py
+-rw-r--r--  2.0 unx     8725 b- defN 23-Apr-24 13:45 monai/auto3dseg/seg_summarizer.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-Apr-24 13:45 monai/auto3dseg/utils.py
+-rw-r--r--  2.0 unx     1341 b- defN 23-Apr-24 13:45 monai/bundle/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-24 13:45 monai/bundle/__main__.py
+-rw-r--r--  2.0 unx    16035 b- defN 23-Apr-24 13:45 monai/bundle/config_item.py
+-rw-r--r--  2.0 unx    22410 b- defN 23-Apr-24 13:45 monai/bundle/config_parser.py
+-rw-r--r--  2.0 unx     8811 b- defN 23-Apr-24 13:45 monai/bundle/properties.py
+-rw-r--r--  2.0 unx    14353 b- defN 23-Apr-24 13:45 monai/bundle/reference_resolver.py
+-rw-r--r--  2.0 unx    63940 b- defN 23-Apr-24 13:45 monai/bundle/scripts.py
+-rw-r--r--  2.0 unx     8911 b- defN 23-Apr-24 13:45 monai/bundle/utils.py
+-rw-r--r--  2.0 unx    17082 b- defN 23-Apr-24 13:45 monai/bundle/workflows.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-Apr-24 13:45 monai/config/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 23-Apr-24 13:45 monai/config/deviceconfig.py
+-rw-r--r--  2.0 unx     3485 b- defN 23-Apr-24 13:45 monai/config/type_definitions.py
+-rw-r--r--  2.0 unx     5087 b- defN 23-Apr-24 13:45 monai/data/__init__.py
+-rw-r--r--  2.0 unx    50102 b- defN 23-Apr-24 13:45 monai/data/box_utils.py
+-rw-r--r--  2.0 unx     4952 b- defN 23-Apr-24 13:45 monai/data/csv_saver.py
+-rw-r--r--  2.0 unx     3835 b- defN 23-Apr-24 13:45 monai/data/dataloader.py
+-rw-r--r--  2.0 unx    68927 b- defN 23-Apr-24 13:45 monai/data/dataset.py
+-rw-r--r--  2.0 unx    10216 b- defN 23-Apr-24 13:45 monai/data/dataset_summary.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Apr-24 13:45 monai/data/decathlon_datalist.py
+-rw-r--r--  2.0 unx     4448 b- defN 23-Apr-24 13:45 monai/data/fft_utils.py
+-rw-r--r--  2.0 unx     6344 b- defN 23-Apr-24 13:45 monai/data/folder_layout.py
+-rw-r--r--  2.0 unx    12484 b- defN 23-Apr-24 13:45 monai/data/grid_dataset.py
+-rw-r--r--  2.0 unx     7008 b- defN 23-Apr-24 13:45 monai/data/image_dataset.py
+-rw-r--r--  2.0 unx    60619 b- defN 23-Apr-24 13:45 monai/data/image_reader.py
+-rw-r--r--  2.0 unx    39872 b- defN 23-Apr-24 13:45 monai/data/image_writer.py
+-rw-r--r--  2.0 unx    13309 b- defN 23-Apr-24 13:45 monai/data/iterable_dataset.py
+-rw-r--r--  2.0 unx    14097 b- defN 23-Apr-24 13:45 monai/data/itk_torch_bridge.py
+-rw-r--r--  2.0 unx     8800 b- defN 23-Apr-24 13:45 monai/data/meta_obj.py
+-rw-r--r--  2.0 unx    27321 b- defN 23-Apr-24 13:45 monai/data/meta_tensor.py
+-rw-r--r--  2.0 unx     5268 b- defN 23-Apr-24 13:45 monai/data/samplers.py
+-rw-r--r--  2.0 unx     7375 b- defN 23-Apr-24 13:45 monai/data/synthetic.py
+-rw-r--r--  2.0 unx     9780 b- defN 23-Apr-24 13:45 monai/data/test_time_augmentation.py
+-rw-r--r--  2.0 unx     8840 b- defN 23-Apr-24 13:45 monai/data/thread_buffer.py
+-rw-r--r--  2.0 unx     5500 b- defN 23-Apr-24 13:45 monai/data/torchscript_utils.py
+-rw-r--r--  2.0 unx    64795 b- defN 23-Apr-24 13:45 monai/data/utils.py
+-rw-r--r--  2.0 unx     9059 b- defN 23-Apr-24 13:45 monai/data/video_dataset.py
+-rw-r--r--  2.0 unx    18619 b- defN 23-Apr-24 13:45 monai/data/wsi_datasets.py
+-rw-r--r--  2.0 unx    49442 b- defN 23-Apr-24 13:45 monai/data/wsi_reader.py
+-rw-r--r--  2.0 unx     1133 b- defN 23-Apr-24 13:45 monai/engines/__init__.py
+-rw-r--r--  2.0 unx    24568 b- defN 23-Apr-24 13:45 monai/engines/evaluator.py
+-rw-r--r--  2.0 unx     7278 b- defN 23-Apr-24 13:45 monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--  2.0 unx    21347 b- defN 23-Apr-24 13:45 monai/engines/trainer.py
+-rw-r--r--  2.0 unx    11631 b- defN 23-Apr-24 13:45 monai/engines/utils.py
+-rw-r--r--  2.0 unx    15250 b- defN 23-Apr-24 13:45 monai/engines/workflow.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/fl/__init__.py
+-rw-r--r--  2.0 unx      725 b- defN 23-Apr-24 13:45 monai/fl/client/__init__.py
+-rw-r--r--  2.0 unx     5097 b- defN 23-Apr-24 13:45 monai/fl/client/client_algo.py
+-rw-r--r--  2.0 unx    33232 b- defN 23-Apr-24 13:45 monai/fl/client/monai_algo.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/fl/utils/__init__.py
+-rw-r--r--  2.0 unx     1713 b- defN 23-Apr-24 13:45 monai/fl/utils/constants.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-Apr-24 13:45 monai/fl/utils/exchange_object.py
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-24 13:45 monai/fl/utils/filters.py
+-rw-r--r--  2.0 unx     2351 b- defN 23-Apr-24 13:45 monai/handlers/__init__.py
+-rw-r--r--  2.0 unx     6798 b- defN 23-Apr-24 13:45 monai/handlers/checkpoint_loader.py
+-rw-r--r--  2.0 unx    16071 b- defN 23-Apr-24 13:45 monai/handlers/checkpoint_saver.py
+-rw-r--r--  2.0 unx     7606 b- defN 23-Apr-24 13:45 monai/handlers/classification_saver.py
+-rw-r--r--  2.0 unx     7506 b- defN 23-Apr-24 13:45 monai/handlers/clearml_handlers.py
+-rw-r--r--  2.0 unx     3989 b- defN 23-Apr-24 13:45 monai/handlers/confusion_matrix.py
+-rw-r--r--  2.0 unx     4425 b- defN 23-Apr-24 13:45 monai/handlers/decollate_batch.py
+-rw-r--r--  2.0 unx     4381 b- defN 23-Apr-24 13:45 monai/handlers/earlystop_handler.py
+-rw-r--r--  2.0 unx     3338 b- defN 23-Apr-24 13:45 monai/handlers/garbage_collector.py
+-rw-r--r--  2.0 unx     3580 b- defN 23-Apr-24 13:45 monai/handlers/hausdorff_distance.py
+-rw-r--r--  2.0 unx     5578 b- defN 23-Apr-24 13:45 monai/handlers/ignite_metric.py
+-rw-r--r--  2.0 unx     3931 b- defN 23-Apr-24 13:45 monai/handlers/logfile_handler.py
+-rw-r--r--  2.0 unx     3575 b- defN 23-Apr-24 13:45 monai/handlers/lr_schedule_handler.py
+-rw-r--r--  2.0 unx     3220 b- defN 23-Apr-24 13:45 monai/handlers/mean_dice.py
+-rw-r--r--  2.0 unx     2831 b- defN 23-Apr-24 13:45 monai/handlers/mean_iou.py
+-rw-r--r--  2.0 unx     5477 b- defN 23-Apr-24 13:45 monai/handlers/metric_logger.py
+-rw-r--r--  2.0 unx     6168 b- defN 23-Apr-24 13:45 monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--  2.0 unx     8560 b- defN 23-Apr-24 13:45 monai/handlers/metrics_saver.py
+-rw-r--r--  2.0 unx    16326 b- defN 23-Apr-24 13:45 monai/handlers/mlflow_handler.py
+-rw-r--r--  2.0 unx     6819 b- defN 23-Apr-24 13:45 monai/handlers/nvtx_handlers.py
+-rw-r--r--  2.0 unx     3637 b- defN 23-Apr-24 13:45 monai/handlers/panoptic_quality.py
+-rw-r--r--  2.0 unx     7119 b- defN 23-Apr-24 13:45 monai/handlers/parameter_scheduler.py
+-rw-r--r--  2.0 unx     3285 b- defN 23-Apr-24 13:45 monai/handlers/postprocessing.py
+-rw-r--r--  2.0 unx     5336 b- defN 23-Apr-24 13:45 monai/handlers/probability_maps.py
+-rw-r--r--  2.0 unx     8422 b- defN 23-Apr-24 13:45 monai/handlers/regression_metrics.py
+-rw-r--r--  2.0 unx     2730 b- defN 23-Apr-24 13:45 monai/handlers/roc_auc.py
+-rw-r--r--  2.0 unx     3051 b- defN 23-Apr-24 13:45 monai/handlers/smartcache_handler.py
+-rw-r--r--  2.0 unx    14251 b- defN 23-Apr-24 13:45 monai/handlers/stats_handler.py
+-rw-r--r--  2.0 unx     3313 b- defN 23-Apr-24 13:45 monai/handlers/surface_distance.py
+-rw-r--r--  2.0 unx    23325 b- defN 23-Apr-24 13:45 monai/handlers/tensorboard_handlers.py
+-rw-r--r--  2.0 unx     9855 b- defN 23-Apr-24 13:45 monai/handlers/utils.py
+-rw-r--r--  2.0 unx     3269 b- defN 23-Apr-24 13:45 monai/handlers/validation_handler.py
+-rw-r--r--  2.0 unx      917 b- defN 23-Apr-24 13:45 monai/inferers/__init__.py
+-rw-r--r--  2.0 unx    32038 b- defN 23-Apr-24 13:45 monai/inferers/inferer.py
+-rw-r--r--  2.0 unx     6393 b- defN 23-Apr-24 13:45 monai/inferers/merger.py
+-rw-r--r--  2.0 unx     9397 b- defN 23-Apr-24 13:45 monai/inferers/splitter.py
+-rw-r--r--  2.0 unx    20017 b- defN 23-Apr-24 13:45 monai/inferers/utils.py
+-rw-r--r--  2.0 unx     1409 b- defN 23-Apr-24 13:45 monai/losses/__init__.py
+-rw-r--r--  2.0 unx     3430 b- defN 23-Apr-24 13:45 monai/losses/contrastive.py
+-rw-r--r--  2.0 unx     4979 b- defN 23-Apr-24 13:45 monai/losses/deform.py
+-rw-r--r--  2.0 unx    46326 b- defN 23-Apr-24 13:45 monai/losses/dice.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-Apr-24 13:45 monai/losses/ds_loss.py
+-rw-r--r--  2.0 unx     9490 b- defN 23-Apr-24 13:45 monai/losses/focal_loss.py
+-rw-r--r--  2.0 unx     2795 b- defN 23-Apr-24 13:45 monai/losses/giou_loss.py
+-rw-r--r--  2.0 unx    15492 b- defN 23-Apr-24 13:45 monai/losses/image_dissimilarity.py
+-rw-r--r--  2.0 unx     3636 b- defN 23-Apr-24 13:45 monai/losses/multi_scale.py
+-rw-r--r--  2.0 unx     2942 b- defN 23-Apr-24 13:45 monai/losses/spatial_mask.py
+-rw-r--r--  2.0 unx     4825 b- defN 23-Apr-24 13:45 monai/losses/ssim_loss.py
+-rw-r--r--  2.0 unx     6645 b- defN 23-Apr-24 13:45 monai/losses/tversky.py
+-rw-r--r--  2.0 unx    10224 b- defN 23-Apr-24 13:45 monai/losses/unified_focal_loss.py
+-rw-r--r--  2.0 unx     1977 b- defN 23-Apr-24 13:45 monai/metrics/__init__.py
+-rw-r--r--  2.0 unx     8211 b- defN 23-Apr-24 13:45 monai/metrics/active_learning_metrics.py
+-rw-r--r--  2.0 unx    15101 b- defN 23-Apr-24 13:45 monai/metrics/confusion_matrix.py
+-rw-r--r--  2.0 unx     5578 b- defN 23-Apr-24 13:45 monai/metrics/cumulative_average.py
+-rw-r--r--  2.0 unx     4026 b- defN 23-Apr-24 13:45 monai/metrics/f_beta_score.py
+-rw-r--r--  2.0 unx     6157 b- defN 23-Apr-24 13:45 monai/metrics/froc.py
+-rw-r--r--  2.0 unx     8262 b- defN 23-Apr-24 13:45 monai/metrics/generalized_dice.py
+-rw-r--r--  2.0 unx    11470 b- defN 23-Apr-24 13:45 monai/metrics/hausdorff_distance.py
+-rw-r--r--  2.0 unx     4907 b- defN 23-Apr-24 13:45 monai/metrics/loss_metric.py
+-rw-r--r--  2.0 unx    12472 b- defN 23-Apr-24 13:45 monai/metrics/meandice.py
+-rw-r--r--  2.0 unx     7209 b- defN 23-Apr-24 13:45 monai/metrics/meaniou.py
+-rw-r--r--  2.0 unx    15140 b- defN 23-Apr-24 13:45 monai/metrics/metric.py
+-rw-r--r--  2.0 unx    13679 b- defN 23-Apr-24 13:45 monai/metrics/panoptic_quality.py
+-rw-r--r--  2.0 unx    19719 b- defN 23-Apr-24 13:45 monai/metrics/regression.py
+-rw-r--r--  2.0 unx     8038 b- defN 23-Apr-24 13:45 monai/metrics/rocauc.py
+-rw-r--r--  2.0 unx    14415 b- defN 23-Apr-24 13:45 monai/metrics/surface_dice.py
+-rw-r--r--  2.0 unx    10186 b- defN 23-Apr-24 13:45 monai/metrics/surface_distance.py
+-rw-r--r--  2.0 unx    15094 b- defN 23-Apr-24 13:45 monai/metrics/utils.py
+-rw-r--r--  2.0 unx    11772 b- defN 23-Apr-24 13:45 monai/metrics/wrapper.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Apr-24 13:45 monai/networks/__init__.py
+-rw-r--r--  2.0 unx    46938 b- defN 23-Apr-24 13:45 monai/networks/utils.py
+-rw-r--r--  2.0 unx     2134 b- defN 23-Apr-24 13:45 monai/networks/blocks/__init__.py
+-rw-r--r--  2.0 unx     4275 b- defN 23-Apr-24 13:45 monai/networks/blocks/acti_norm.py
+-rw-r--r--  2.0 unx     5839 b- defN 23-Apr-24 13:45 monai/networks/blocks/activation.py
+-rw-r--r--  2.0 unx     4380 b- defN 23-Apr-24 13:45 monai/networks/blocks/aspp.py
+-rw-r--r--  2.0 unx     7488 b- defN 23-Apr-24 13:45 monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--  2.0 unx    11686 b- defN 23-Apr-24 13:45 monai/networks/blocks/convolutions.py
+-rw-r--r--  2.0 unx     5009 b- defN 23-Apr-24 13:45 monai/networks/blocks/crf.py
+-rw-r--r--  2.0 unx     4740 b- defN 23-Apr-24 13:45 monai/networks/blocks/denseblock.py
+-rw-r--r--  2.0 unx     9255 b- defN 23-Apr-24 13:45 monai/networks/blocks/dints_block.py
+-rw-r--r--  2.0 unx     2413 b- defN 23-Apr-24 13:45 monai/networks/blocks/downsample.py
+-rw-r--r--  2.0 unx    11062 b- defN 23-Apr-24 13:45 monai/networks/blocks/dynunet_block.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-Apr-24 13:45 monai/networks/blocks/encoder.py
+-rw-r--r--  2.0 unx     9024 b- defN 23-Apr-24 13:45 monai/networks/blocks/fcn.py
+-rw-r--r--  2.0 unx    10586 b- defN 23-Apr-24 13:45 monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--  2.0 unx     8263 b- defN 23-Apr-24 13:45 monai/networks/blocks/fft_utils_t.py
+-rw-r--r--  2.0 unx    11454 b- defN 23-Apr-24 13:45 monai/networks/blocks/localnet_block.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Apr-24 13:45 monai/networks/blocks/mlp.py
+-rw-r--r--  2.0 unx     7987 b- defN 23-Apr-24 13:45 monai/networks/blocks/patchembedding.py
+-rw-r--r--  2.0 unx     8825 b- defN 23-Apr-24 13:45 monai/networks/blocks/regunet_block.py
+-rw-r--r--  2.0 unx     3245 b- defN 23-Apr-24 13:45 monai/networks/blocks/segresnet_block.py
+-rw-r--r--  2.0 unx     3099 b- defN 23-Apr-24 13:45 monai/networks/blocks/selfattention.py
+-rw-r--r--  2.0 unx    12752 b- defN 23-Apr-24 13:45 monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--  2.0 unx     3811 b- defN 23-Apr-24 13:45 monai/networks/blocks/text_embedding.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Apr-24 13:45 monai/networks/blocks/transformerblock.py
+-rw-r--r--  2.0 unx     9049 b- defN 23-Apr-24 13:45 monai/networks/blocks/unetr_block.py
+-rw-r--r--  2.0 unx    13312 b- defN 23-Apr-24 13:45 monai/networks/blocks/upsample.py
+-rw-r--r--  2.0 unx     6656 b- defN 23-Apr-24 13:45 monai/networks/blocks/warp.py
+-rw-r--r--  2.0 unx     1562 b- defN 23-Apr-24 13:45 monai/networks/layers/__init__.py
+-rw-r--r--  2.0 unx     8288 b- defN 23-Apr-24 13:45 monai/networks/layers/convutils.py
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-24 13:45 monai/networks/layers/drop_path.py
+-rw-r--r--  2.0 unx    12638 b- defN 23-Apr-24 13:45 monai/networks/layers/factories.py
+-rw-r--r--  2.0 unx    17992 b- defN 23-Apr-24 13:45 monai/networks/layers/filtering.py
+-rw-r--r--  2.0 unx     3324 b- defN 23-Apr-24 13:45 monai/networks/layers/gmm.py
+-rw-r--r--  2.0 unx    28470 b- defN 23-Apr-24 13:45 monai/networks/layers/simplelayers.py
+-rw-r--r--  2.0 unx    25576 b- defN 23-Apr-24 13:45 monai/networks/layers/spatial_transforms.py
+-rw-r--r--  2.0 unx     4296 b- defN 23-Apr-24 13:45 monai/networks/layers/utils.py
+-rw-r--r--  2.0 unx     2253 b- defN 23-Apr-24 13:45 monai/networks/layers/weight_init.py
+-rw-r--r--  2.0 unx     3141 b- defN 23-Apr-24 13:45 monai/networks/nets/__init__.py
+-rw-r--r--  2.0 unx    21533 b- defN 23-Apr-24 13:45 monai/networks/nets/ahnet.py
+-rw-r--r--  2.0 unx     9202 b- defN 23-Apr-24 13:45 monai/networks/nets/attentionunet.py
+-rw-r--r--  2.0 unx    12089 b- defN 23-Apr-24 13:45 monai/networks/nets/autoencoder.py
+-rw-r--r--  2.0 unx    10950 b- defN 23-Apr-24 13:45 monai/networks/nets/basic_unet.py
+-rw-r--r--  2.0 unx     7960 b- defN 23-Apr-24 13:45 monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--  2.0 unx     6293 b- defN 23-Apr-24 13:45 monai/networks/nets/classifier.py
+-rw-r--r--  2.0 unx    15820 b- defN 23-Apr-24 13:45 monai/networks/nets/densenet.py
+-rw-r--r--  2.0 unx    44771 b- defN 23-Apr-24 13:45 monai/networks/nets/dints.py
+-rw-r--r--  2.0 unx    18210 b- defN 23-Apr-24 13:45 monai/networks/nets/dynunet.py
+-rw-r--r--  2.0 unx    40643 b- defN 23-Apr-24 13:45 monai/networks/nets/efficientnet.py
+-rw-r--r--  2.0 unx    14147 b- defN 23-Apr-24 13:45 monai/networks/nets/flexible_unet.py
+-rw-r--r--  2.0 unx     7212 b- defN 23-Apr-24 13:45 monai/networks/nets/fullyconnectednet.py
+-rw-r--r--  2.0 unx     6581 b- defN 23-Apr-24 13:45 monai/networks/nets/generator.py
+-rw-r--r--  2.0 unx     8882 b- defN 23-Apr-24 13:45 monai/networks/nets/highresnet.py
+-rw-r--r--  2.0 unx    28678 b- defN 23-Apr-24 13:45 monai/networks/nets/hovernet.py
+-rw-r--r--  2.0 unx     9812 b- defN 23-Apr-24 13:45 monai/networks/nets/milmodel.py
+-rw-r--r--  2.0 unx     6102 b- defN 23-Apr-24 13:45 monai/networks/nets/netadapter.py
+-rw-r--r--  2.0 unx     6488 b- defN 23-Apr-24 13:45 monai/networks/nets/regressor.py
+-rw-r--r--  2.0 unx    17189 b- defN 23-Apr-24 13:45 monai/networks/nets/regunet.py
+-rw-r--r--  2.0 unx    16785 b- defN 23-Apr-24 13:45 monai/networks/nets/resnet.py
+-rw-r--r--  2.0 unx    13994 b- defN 23-Apr-24 13:45 monai/networks/nets/segresnet.py
+-rw-r--r--  2.0 unx    15667 b- defN 23-Apr-24 13:45 monai/networks/nets/segresnet_ds.py
+-rw-r--r--  2.0 unx    19289 b- defN 23-Apr-24 13:45 monai/networks/nets/senet.py
+-rw-r--r--  2.0 unx    42000 b- defN 23-Apr-24 13:45 monai/networks/nets/swin_unetr.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Apr-24 13:45 monai/networks/nets/torchvision_fc.py
+-rw-r--r--  2.0 unx    16626 b- defN 23-Apr-24 13:45 monai/networks/nets/transchex.py
+-rw-r--r--  2.0 unx    13722 b- defN 23-Apr-24 13:45 monai/networks/nets/unet.py
+-rw-r--r--  2.0 unx     7943 b- defN 23-Apr-24 13:45 monai/networks/nets/unetr.py
+-rw-r--r--  2.0 unx     6285 b- defN 23-Apr-24 13:45 monai/networks/nets/varautoencoder.py
+-rw-r--r--  2.0 unx     5655 b- defN 23-Apr-24 13:45 monai/networks/nets/vit.py
+-rw-r--r--  2.0 unx     4817 b- defN 23-Apr-24 13:45 monai/networks/nets/vitautoenc.py
+-rw-r--r--  2.0 unx    10011 b- defN 23-Apr-24 13:45 monai/networks/nets/vnet.py
+-rw-r--r--  2.0 unx      796 b- defN 23-Apr-24 13:45 monai/optimizers/__init__.py
+-rw-r--r--  2.0 unx    21952 b- defN 23-Apr-24 13:45 monai/optimizers/lr_finder.py
+-rw-r--r--  2.0 unx     3652 b- defN 23-Apr-24 13:45 monai/optimizers/lr_scheduler.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Apr-24 13:45 monai/optimizers/novograd.py
+-rw-r--r--  2.0 unx     4131 b- defN 23-Apr-24 13:45 monai/optimizers/utils.py
+-rw-r--r--  2.0 unx    15248 b- defN 23-Apr-24 13:45 monai/transforms/__init__.py
+-rw-r--r--  2.0 unx     8946 b- defN 23-Apr-24 13:45 monai/transforms/adaptors.py
+-rw-r--r--  2.0 unx    40812 b- defN 23-Apr-24 13:45 monai/transforms/compose.py
+-rw-r--r--  2.0 unx    18000 b- defN 23-Apr-24 13:45 monai/transforms/inverse.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-Apr-24 13:45 monai/transforms/inverse_batch_transform.py
+-rw-r--r--  2.0 unx     3386 b- defN 23-Apr-24 13:45 monai/transforms/nvtx.py
+-rw-r--r--  2.0 unx     2885 b- defN 23-Apr-24 13:45 monai/transforms/traits.py
+-rw-r--r--  2.0 unx    18234 b- defN 23-Apr-24 13:45 monai/transforms/transform.py
+-rw-r--r--  2.0 unx    72516 b- defN 23-Apr-24 13:45 monai/transforms/utils.py
+-rw-r--r--  2.0 unx    31081 b- defN 23-Apr-24 13:45 monai/transforms/utils_create_transform_ims.py
+-rw-r--r--  2.0 unx    18397 b- defN 23-Apr-24 13:45 monai/transforms/utils_pytorch_numpy_unification.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/croppad/__init__.py
+-rw-r--r--  2.0 unx    68231 b- defN 23-Apr-24 13:45 monai/transforms/croppad/array.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-Apr-24 13:45 monai/transforms/croppad/batch.py
+-rw-r--r--  2.0 unx    54071 b- defN 23-Apr-24 13:45 monai/transforms/croppad/dictionary.py
+-rw-r--r--  2.0 unx    12673 b- defN 23-Apr-24 13:45 monai/transforms/croppad/functional.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/intensity/__init__.py
+-rw-r--r--  2.0 unx    98613 b- defN 23-Apr-24 13:45 monai/transforms/intensity/array.py
+-rw-r--r--  2.0 unx    76501 b- defN 23-Apr-24 13:45 monai/transforms/intensity/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/io/__init__.py
+-rw-r--r--  2.0 unx    25430 b- defN 23-Apr-24 13:45 monai/transforms/io/array.py
+-rw-r--r--  2.0 unx    17821 b- defN 23-Apr-24 13:45 monai/transforms/io/dictionary.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-24 13:45 monai/transforms/lazy/__init__.py
+-rw-r--r--  2.0 unx     5552 b- defN 23-Apr-24 13:45 monai/transforms/lazy/functional.py
+-rw-r--r--  2.0 unx     9851 b- defN 23-Apr-24 13:45 monai/transforms/lazy/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/meta_utility/__init__.py
+-rw-r--r--  2.0 unx     4896 b- defN 23-Apr-24 13:45 monai/transforms/meta_utility/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/post/__init__.py
+-rw-r--r--  2.0 unx    40858 b- defN 23-Apr-24 13:45 monai/transforms/post/array.py
+-rw-r--r--  2.0 unx    39905 b- defN 23-Apr-24 13:45 monai/transforms/post/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/signal/__init__.py
+-rw-r--r--  2.0 unx    16378 b- defN 23-Apr-24 13:45 monai/transforms/signal/array.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/smooth_field/__init__.py
+-rw-r--r--  2.0 unx    17833 b- defN 23-Apr-24 13:45 monai/transforms/smooth_field/array.py
+-rw-r--r--  2.0 unx    11194 b- defN 23-Apr-24 13:45 monai/transforms/smooth_field/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/spatial/__init__.py
+-rw-r--r--  2.0 unx   168618 b- defN 23-Apr-24 13:45 monai/transforms/spatial/array.py
+-rw-r--r--  2.0 unx   107151 b- defN 23-Apr-24 13:45 monai/transforms/spatial/dictionary.py
+-rw-r--r--  2.0 unx    31494 b- defN 23-Apr-24 13:45 monai/transforms/spatial/functional.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-24 13:45 monai/transforms/utility/__init__.py
+-rw-r--r--  2.0 unx    70839 b- defN 23-Apr-24 13:45 monai/transforms/utility/array.py
+-rw-r--r--  2.0 unx    76330 b- defN 23-Apr-24 13:45 monai/transforms/utility/dictionary.py
+-rw-r--r--  2.0 unx     3380 b- defN 23-Apr-24 13:45 monai/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Apr-24 13:45 monai/utils/aliases.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-Apr-24 13:45 monai/utils/decorators.py
+-rw-r--r--  2.0 unx    14759 b- defN 23-Apr-24 13:45 monai/utils/deprecate_utils.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-Apr-24 13:45 monai/utils/dist.py
+-rw-r--r--  2.0 unx    16807 b- defN 23-Apr-24 13:45 monai/utils/enums.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-Apr-24 13:45 monai/utils/jupyter_utils.py
+-rw-r--r--  2.0 unx    28185 b- defN 23-Apr-24 13:45 monai/utils/misc.py
+-rw-r--r--  2.0 unx    23631 b- defN 23-Apr-24 13:45 monai/utils/module.py
+-rw-r--r--  2.0 unx     6876 b- defN 23-Apr-24 13:45 monai/utils/nvtx.py
+-rw-r--r--  2.0 unx    15936 b- defN 23-Apr-24 13:45 monai/utils/profiling.py
+-rw-r--r--  2.0 unx     5955 b- defN 23-Apr-24 13:45 monai/utils/state_cacher.py
+-rw-r--r--  2.0 unx    21147 b- defN 23-Apr-24 13:45 monai/utils/type_conversion.py
+-rw-r--r--  2.0 unx     1038 b- defN 23-Apr-24 13:45 monai/visualize/__init__.py
+-rw-r--r--  2.0 unx    16156 b- defN 23-Apr-24 13:45 monai/visualize/class_activation_maps.py
+-rw-r--r--  2.0 unx     6277 b- defN 23-Apr-24 13:45 monai/visualize/gradient_based.py
+-rw-r--r--  2.0 unx     9200 b- defN 23-Apr-24 13:45 monai/visualize/img2tensorboard.py
+-rw-r--r--  2.0 unx    18816 b- defN 23-Apr-24 13:45 monai/visualize/occlusion_sensitivity.py
+-rw-r--r--  2.0 unx     9966 b- defN 23-Apr-24 13:45 monai/visualize/utils.py
+-rw-r--r--  2.0 unx     1377 b- defN 23-Apr-24 13:45 monai/visualize/visualizer.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-24 13:47 monai-1.2.0rc5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10172 b- defN 23-Apr-24 13:47 monai-1.2.0rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-Apr-24 13:47 monai-1.2.0rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-24 13:47 monai-1.2.0rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    32699 b- defN 23-Apr-24 13:47 monai-1.2.0rc5.dist-info/RECORD
+365 files, 4746247 bytes uncompressed, 1201648 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -729,14 +729,17 @@
 
 Filename: monai/networks/blocks/selfattention.py
 Comment: 
 
 Filename: monai/networks/blocks/squeeze_and_excitation.py
 Comment: 
 
+Filename: monai/networks/blocks/text_embedding.py
+Comment: 
+
 Filename: monai/networks/blocks/transformerblock.py
 Comment: 
 
 Filename: monai/networks/blocks/unetr_block.py
 Comment: 
 
 Filename: monai/networks/blocks/upsample.py
@@ -1071,23 +1074,23 @@
 
 Filename: monai/visualize/utils.py
 Comment: 
 
 Filename: monai/visualize/visualizer.py
 Comment: 
 
-Filename: monai-1.2.0rc4.dist-info/LICENSE
+Filename: monai-1.2.0rc5.dist-info/LICENSE
 Comment: 
 
-Filename: monai-1.2.0rc4.dist-info/METADATA
+Filename: monai-1.2.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: monai-1.2.0rc4.dist-info/WHEEL
+Filename: monai-1.2.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: monai-1.2.0rc4.dist-info/top_level.txt
+Filename: monai-1.2.0rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: monai-1.2.0rc4.dist-info/RECORD
+Filename: monai-1.2.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-04-12T19:27:56+0100",
+ "date": "2023-04-23T21:17:43+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "1a55ba5423d04d2ef7ac19356ccabc4c7906f577",
- "version": "1.2.0rc4"
+ "full-revisionid": "9c9777751ab4f96e059a6597b9aa7ac6e7ca3b92",
+ "version": "1.2.0rc5"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/apps/datasets.py

```diff
@@ -582,15 +582,15 @@
         First of all, download a series from TCIA according to `series_uid`.
         Then find all referenced series and download.
         """
         seg_first_dir = os.path.join(download_dir, "raw", series_uid)
         download_tcia_series_instance(
             series_uid=series_uid, download_dir=download_dir, output_dir=seg_first_dir, check_md5=False
         )
-        dicom_files = [f for f in os.listdir(seg_first_dir) if f.endswith(".dcm")]
+        dicom_files = [f for f in sorted(os.listdir(seg_first_dir)) if f.endswith(".dcm")]
         # achieve series number and patient id from the first dicom file
         dcm_path = os.path.join(seg_first_dir, dicom_files[0])
         ds = PydicomReader(stop_before_pixels=True, specific_tags=self.load_tags).read(dcm_path)
         # (0x0010,0x0020) and (0x0010,0x0010), better to be contained in `specific_tags`
         patient_id = ds.PatientID if ds.PatientID else ds.PatientName
         if not patient_id:
             warnings.warn(f"unable to find patient name of dicom file: {dcm_path}, use 'patient' instead.")
```

## monai/apps/auto3dseg/__init__.py

```diff
@@ -10,10 +10,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from .auto_runner import AutoRunner
 from .bundle_gen import BundleAlgo, BundleGen
 from .data_analyzer import DataAnalyzer
-from .ensemble_builder import AlgoEnsemble, AlgoEnsembleBestByFold, AlgoEnsembleBestN, AlgoEnsembleBuilder
+from .ensemble_builder import (
+    AlgoEnsemble,
+    AlgoEnsembleBestByFold,
+    AlgoEnsembleBestN,
+    AlgoEnsembleBuilder,
+    EnsembleRunner,
+)
 from .hpo_gen import NNIGen, OptunaGen
 from .utils import export_bundle_algo_history, import_bundle_algo_history
```

## monai/apps/auto3dseg/__main__.py

```diff
@@ -10,25 +10,26 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from monai.apps.auto3dseg.auto_runner import AutoRunner
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo, BundleGen
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
-from monai.apps.auto3dseg.ensemble_builder import AlgoEnsembleBuilder
+from monai.apps.auto3dseg.ensemble_builder import AlgoEnsembleBuilder, EnsembleRunner
 from monai.apps.auto3dseg.hpo_gen import NNIGen, OptunaGen
 
 if __name__ == "__main__":
     from monai.utils import optional_import
 
     fire, _ = optional_import("fire")
     fire.Fire(
         {
             "DataAnalyzer": DataAnalyzer,
             "BundleGen": BundleGen,
             "BundleAlgo": BundleAlgo,
             "AlgoEnsembleBuilder": AlgoEnsembleBuilder,
+            "EnsembleRunner": EnsembleRunner,
             "AutoRunner": AutoRunner,
             "NNIGen": NNIGen,
             "OptunaGen": OptunaGen,
         }
     )
```

## monai/apps/auto3dseg/auto_runner.py

```diff
@@ -15,33 +15,27 @@
 import shutil
 import subprocess
 import warnings
 from copy import deepcopy
 from time import sleep
 from typing import Any, cast
 
-import numpy as np
 import torch
 
 from monai.apps.auto3dseg.bundle_gen import BundleGen
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
-from monai.apps.auto3dseg.ensemble_builder import (
-    AlgoEnsemble,
-    AlgoEnsembleBestByFold,
-    AlgoEnsembleBestN,
-    AlgoEnsembleBuilder,
-)
+from monai.apps.auto3dseg.ensemble_builder import EnsembleRunner
 from monai.apps.auto3dseg.hpo_gen import NNIGen
 from monai.apps.auto3dseg.utils import export_bundle_algo_history, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle import ConfigParser
 from monai.transforms import SaveImage
-from monai.utils.enums import AlgoKeys
-from monai.utils.module import look_up_option, optional_import
+from monai.utils import AlgoKeys, has_option, look_up_option, optional_import
+from monai.utils.misc import check_kwargs_exist_in_class_init
 
 logger = get_logger(module_name=__name__)
 
 nni, has_nni = optional_import("nni")
 
 
 class AutoRunner:
@@ -84,14 +78,16 @@
             is supported
         ensemble: on/off switch to run model ensemble and use the ensemble to predict outputs in testing
             datasets.
         not_use_cache: if the value is True, it will ignore all cached results in data analysis,
             algorithm generation, or training, and start the pipeline from scratch.
         templates_path_or_url: the folder with the algorithm templates or a url. If None provided, the default template
             zip url will be downloaded and extracted into the work_dir.
+        allow_skip: a switch passed to BundleGen process which determines if some Algo in the default templates
+            can be skipped based on the analysis on the dataset from Auto3DSeg DataAnalyzer.
         kwargs: image writing parameters for the ensemble inference. The kwargs format follows the SaveImage
             transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage.
 
 
     Examples:
         - User can use the one-liner to start the Auto3Dseg workflow
 
@@ -218,24 +214,27 @@
         algo_gen: bool | None = None,
         train: bool | None = None,
         hpo: bool = False,
         hpo_backend: str = "nni",
         ensemble: bool = True,
         not_use_cache: bool = False,
         templates_path_or_url: str | None = None,
+        allow_skip: bool = True,
         **kwargs: Any,
     ):
         logger.info(f"AutoRunner using work directory {work_dir}")
         os.makedirs(work_dir, exist_ok=True)
 
         self.work_dir = os.path.abspath(work_dir)
         self.data_src_cfg = dict()
         self.data_src_cfg_name = os.path.join(self.work_dir, "input.yaml")
         self.algos = algos
         self.templates_path_or_url = templates_path_or_url
+        self.allow_skip = allow_skip
+        self.kwargs = deepcopy(kwargs)
 
         if input is None and os.path.isfile(self.data_src_cfg_name):
             input = self.data_src_cfg_name
             logger.info(f"Input config is not provided, using the default {input}")
 
         if isinstance(input, dict):
             self.data_src_cfg = input
@@ -281,24 +280,19 @@
         # determine if we need to analyze, algo_gen or train from cache, unless manually provided
         self.analyze = not self.cache["analyze"] if analyze is None else analyze
         self.algo_gen = not self.cache["algo_gen"] if algo_gen is None else algo_gen
         self.train = train
         self.ensemble = ensemble  # last step, no need to check
 
         self.set_training_params()
+        self.set_device_info()
         self.set_prediction_params()
         self.set_analyze_params()
-
-        self.save_image = self.set_image_save_transform(kwargs)
-
-        self.ensemble_method: AlgoEnsemble
-        self.ensemble_method_name: str | None = None
-
+        self.set_ensemble_method()
         self.set_num_fold(num_fold=num_fold)
-        self.set_ensemble_method("AlgoEnsembleBestByFold")
 
         self.gpu_customization = False
         self.gpu_customization_specs: dict[str, Any] = {}
 
         # hpo
         if hpo_backend.lower() != "nni":
             raise NotImplementedError("HPOGen backend only supports NNI")
@@ -457,26 +451,19 @@
 
     def set_num_fold(self, num_fold: int = 5) -> None:
         """
         Set the number of cross validation folds for all algos.
 
         Args:
             num_fold: a positive integer to define the number of folds.
-
-        Notes:
-            If the ensemble method is ``AlgoEnsembleBestByFold``, this function automatically updates the ``n_fold``
-            parameter in the ``ensemble_method`` to avoid inconsistency between the training and the ensemble.
         """
 
         if num_fold <= 0:
             raise ValueError(f"num_fold is expected to be an integer greater than zero. Now it gets {num_fold}")
-
         self.num_fold = num_fold
-        if self.ensemble_method_name == "AlgoEnsembleBestByFold":
-            self.ensemble_method.n_fold = self.num_fold  # type: ignore
 
     def set_training_params(self, params: dict[str, Any] | None = None) -> None:
         """
         Set the training params for all algos.
 
         Args:
             params: a dict that defines the overriding key-value pairs during training. The overriding method
@@ -484,14 +471,110 @@
 
         Examples:
             For BundleAlgo objects, the training parameter to shorten the training time to a few epochs can be
                 {"num_iterations": 8, "num_iterations_per_validation": 4}
 
         """
         self.train_params = deepcopy(params) if params is not None else {}
+        if "CUDA_VISIBLE_DEVICES" in self.train_params:
+            warnings.warn(
+                "CUDA_VISIBLE_DEVICES is deprecated from 'set_training_params'. Use 'set_device_info' intead.",
+                DeprecationWarning,
+            )
+
+    def set_device_info(
+        self,
+        cuda_visible_devices: list[int] | str | None = None,
+        num_nodes: int | None = None,
+        mn_start_method: str | None = None,
+        cmd_prefix: str | None = None,
+    ) -> None:
+        """
+        Set the device related info
+
+        Args:
+            cuda_visible_device: define GPU ids for data analyzer, training, and ensembling.
+                List of GPU ids [0,1,2,3] or a string "0,1,2,3".
+                Default using env "CUDA_VISIBLE_DEVICES" or all devices available.
+            num_nodes: number of nodes for training and ensembling.
+                Default using env "NUM_NODES" or 1 if "NUM_NODES" is unset.
+            mn_start_method: multi-node start method. Autorunner will use the method to start multi-node processes.
+                Default using env "MN_START_METHOD" or 'bcprun' if "MN_START_METHOD" is unset.
+            cmd_prefix: command line prefix for subprocess running in BundleAlgo and EnsembleRunner.
+                Default using env "CMD_PREFIX" or None, examples are:
+
+                    - single GPU/CPU or multinode bcprun: "python " or "/opt/conda/bin/python3.8 ",
+                    - single node multi-GPU running "torchrun --nnodes=1 --nproc_per_node=2 "
+
+                If user define this prefix, please make sure --nproc_per_node matches cuda_visible_device or
+                os.env['CUDA_VISIBLE_DEVICES]. Also always set --nnodes=1. Set num_nodes for multi-node.
+        """
+        self.device_setting: dict[str, Any] = {}
+        if cuda_visible_devices is None:
+            cuda_visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES")
+        if cuda_visible_devices is None:  # still None after reading the environ
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in range(torch.cuda.device_count())])
+            self.device_setting["n_devices"] = torch.cuda.device_count()
+        elif isinstance(cuda_visible_devices, str):
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = cuda_visible_devices
+            self.device_setting["n_devices"] = len(cuda_visible_devices.split(","))
+        elif isinstance(cuda_visible_devices, (list, tuple)):
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in cuda_visible_devices])
+            self.device_setting["n_devices"] = len(cuda_visible_devices)
+        else:
+            logger.warn(f"Wrong format of cuda_visible_devices {cuda_visible_devices}, devices not set")
+
+        if num_nodes is None:
+            num_nodes = int(os.environ.get("NUM_NODES", 1))
+        self.device_setting["NUM_NODES"] = num_nodes
+
+        if mn_start_method is None:
+            mn_start_method = os.environ.get("MN_START_METHOD", "bcprun")
+        self.device_setting["MN_START_METHOD"] = mn_start_method
+
+        if cmd_prefix is None:
+            cmd_prefix = os.environ.get("CMD_PREFIX")
+        self.device_setting["CMD_PREFIX"] = cmd_prefix
+
+        if cmd_prefix is not None:
+            logger.info(f"Using user defined command running prefix {cmd_prefix}, will overide other settings")
+
+    def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
+        """
+        Set the bundle ensemble method name and parameters for save image transform parameters.
+
+        Args:
+            params: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
+                and "AlgoEnsembleBestByFold".
+            kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
+                ``AlgoEnsembleBestN`` is supported.
+        """
+        self.ensemble_method_name = look_up_option(
+            ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
+        )
+        self.kwargs.update(kwargs)
+
+    def set_image_save_transform(self, **kwargs: Any) -> None:
+        """
+        Set the ensemble output transform.
+
+        Args:
+            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
+                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage.
+
+        """
+
+        are_all_args_present, missing_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
+        if are_all_args_present:
+            self.kwargs.update(kwargs)
+        else:
+            raise ValueError(
+                f"{missing_args} are not supported in monai.transforms.SaveImage,"
+                "Check https://docs.monai.io/en/stable/transforms.html#saveimage for more information."
+            )
 
     def set_prediction_params(self, params: dict[str, Any] | None = None) -> None:
         """
         Set the prediction params for all algos.
 
         Args:
             params: a dict that defines the overriding key-value pairs during prediction. The overriding method
@@ -543,18 +626,15 @@
             params: a dict that defines the overriding key-value pairs during instantiation of the algo. For
                 BundleAlgo, it will override the template config filling.
 
         Notes:
             Users can set ``nni_dry_run`` to ``True`` in the ``params`` to enable the dry-run mode for the NNI backend.
 
         """
-        if params is None:
-            self.hpo_params = self.train_params
-        else:
-            self.hpo_params = params
+        self.hpo_params = self.train_params if params is None else params
 
     def set_nni_search_space(self, search_space):
         """
         Set the search space for NNI parameter search.
 
         Args:
             search_space: hyper parameter search space in the form of dict. For more information, please check
@@ -565,66 +645,14 @@
             if "_value" not in v:
                 raise ValueError(f"{search_space} key {k} value {v} has not _value")
             value_combinations *= len(v["_value"])
 
         self.search_space = search_space
         self.hpo_tasks = value_combinations
 
-    def set_image_save_transform(self, kwargs):
-        """
-        Set the ensemble output transform.
-
-        Args:
-            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
-                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
-
-        """
-
-        if "output_dir" in kwargs:
-            output_dir = kwargs.pop("output_dir")
-        else:
-            output_dir = os.path.join(self.work_dir, "ensemble_output")
-            logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions")
-
-        if not os.path.isdir(output_dir):
-            os.makedirs(output_dir)
-            logger.info(f"Directory {output_dir} is created to save ensemble predictions")
-
-        self.output_dir = output_dir
-        output_postfix = kwargs.pop("output_postfix", "ensemble")
-        output_dtype = kwargs.pop("output_dtype", np.uint8)
-        resample = kwargs.pop("resample", False)
-
-        return SaveImage(
-            output_dir=output_dir, output_postfix=output_postfix, output_dtype=output_dtype, resample=resample, **kwargs
-        )
-
-    def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
-        """
-        Set the bundle ensemble method
-
-        Args:
-            ensemble_method_name: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
-                and "AlgoEnsembleBestByFold".
-            kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
-                ``AlgoEnsembleBestN`` is supported.
-
-        """
-        self.ensemble_method_name = look_up_option(
-            ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
-        )
-        if self.ensemble_method_name == "AlgoEnsembleBestN":
-            n_best = kwargs.pop("n_best", False)
-            n_best = 2 if not n_best else n_best
-            self.ensemble_method = AlgoEnsembleBestN(n_best=n_best)
-        elif self.ensemble_method_name == "AlgoEnsembleBestByFold":
-            self.ensemble_method = AlgoEnsembleBestByFold(n_fold=self.num_fold)
-        else:
-            raise NotImplementedError(f"Ensemble method {self.ensemble_method_name} is not implemented.")
-
     def _train_algo_in_sequence(self, history: list[dict[str, Any]]) -> None:
         """
         Train the Algos in a sequential scheme. The order of training is randomized.
 
         Args:
             history: the history of generated Algos. It is a list of dicts. Each element has the task name
                 (e.g. "dints_0" for dints network in fold 0) as the key and the algo object as the value.
@@ -633,15 +661,18 @@
         Note:
             The final results of the model training will be written to all the generated algorithm's output
             folders under the working directory. The results include the model checkpoints, a
             progress.yaml, accuracies in CSV and a pickle file of the Algo object.
         """
         for algo_dict in history:
             algo = algo_dict[AlgoKeys.ALGO]
-            algo.train(self.train_params)
+            if has_option(algo.train, "device_setting"):
+                algo.train(self.train_params, self.device_setting)
+            else:
+                algo.train(self.train_params)
             acc = algo.get_score()
 
             algo_meta_data = {str(AlgoKeys.SCORE): acc}
             algo_to_pickle(algo, template_path=algo.template_path, **algo_meta_data)
 
     def _train_algo_in_nni(self, history: list[dict[str, Any]]) -> None:
         """
@@ -747,17 +778,18 @@
 
             if self.gpu_customization:
                 bundle_generator.generate(
                     self.work_dir,
                     num_fold=self.num_fold,
                     gpu_customization=self.gpu_customization,
                     gpu_customization_specs=self.gpu_customization_specs,
+                    allow_skip=self.allow_skip,
                 )
             else:
-                bundle_generator.generate(self.work_dir, num_fold=self.num_fold)
+                bundle_generator.generate(self.work_dir, num_fold=self.num_fold, allow_skip=self.allow_skip)
             history = bundle_generator.get_history()
             export_bundle_algo_history(history)
             self.export_cache(algo_gen=True)
         else:
             logger.info("Skipping algorithm generation...")
 
         # step 3: algo training
@@ -769,15 +801,15 @@
                 raise ValueError(
                     f"Could not find training scripts in {self.work_dir}. "
                     "Possibly the required algorithms generation step was not completed."
                 )
 
             if auto_train_choice:
                 skip_algos = [h[AlgoKeys.ID] for h in history if h[AlgoKeys.IS_TRAINED]]
-                if len(skip_algos) > 0:
+                if skip_algos:
                     logger.info(
                         f"Skipping already trained algos {skip_algos}."
                         "Set option train=True to always retrain all algos."
                     )
                     history = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
 
             if len(history) > 0:
@@ -788,38 +820,18 @@
 
             self.export_cache(train=True)
         else:
             logger.info("Skipping algorithm training...")
 
         # step 4: model ensemble and write the prediction to disks.
         if self.ensemble:
-            history = import_bundle_algo_history(self.work_dir, only_trained=False)
-
-            history_untrained = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
-            if len(history_untrained) > 0:
-                warnings.warn(
-                    f"Ensembling step will skip {[h['name'] for h in history_untrained]} untrained algos."
-                    "Generally it means these algos did not complete training."
-                )
-                history = [h for h in history if h[AlgoKeys.IS_TRAINED]]
-
-            if len(history) == 0:
-                raise ValueError(
-                    f"Could not find any trained algos in {self.work_dir}. "
-                    "Possibly the required training step was not completed."
-                )
-
-            builder = AlgoEnsembleBuilder(history, self.data_src_cfg_name)
-            builder.set_ensemble_method(self.ensemble_method)
-
-            ensembler = builder.get_ensemble()
-            preds = ensembler(pred_param=self.pred_params)
-            if len(preds) > 0:
-                logger.info("Auto3Dseg picked the following networks to ensemble:")
-                for algo in ensembler.get_algo_ensemble():
-                    logger.info(algo[AlgoKeys.ID])
-
-                for pred in preds:
-                    self.save_image(pred)
-                logger.info(f"Auto3Dseg ensemble prediction outputs are saved in {self.output_dir}.")
-
+            ensemble_runner = EnsembleRunner(
+                data_src_cfg_name=self.data_src_cfg_name,
+                work_dir=self.work_dir,
+                num_fold=self.num_fold,
+                ensemble_method_name=self.ensemble_method_name,
+                mgpu=int(self.device_setting["n_devices"]) > 1,
+                **self.kwargs,  # for set_image_save_transform
+                **self.pred_params,
+            )  # for inference
+            ensemble_runner.run(self.device_setting)
         logger.info("Auto3Dseg pipeline is completed successfully.")
```

## monai/apps/auto3dseg/bundle_gen.py

```diff
@@ -32,15 +32,15 @@
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.utils import ensure_tuple
 from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
-ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "b37ed82")
+ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "23ea143")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
 
 class BundleAlgo(Algo):
     """
     An algorithm represented by a set of bundle configurations and scripts.
@@ -76,14 +76,22 @@
         self.data_stats_files = ""
         self.data_list_file = ""
         self.output_path = ""
         self.name = ""
         self.best_metric = None
         # track records when filling template config: {"<config name>": {"<placeholder key>": value, ...}, ...}
         self.fill_records: dict = {}
+        # device_setting set default value and sanity check, in case device_setting not from autorunner
+        self.device_setting: dict[str, int | str] = {
+            "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
+            "n_devices": int(torch.cuda.device_count()),
+            "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
+            "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
+            "CMD_PREFIX": os.environ.get("CMD_PREFIX"),  # type: ignore
+        }
 
     def pre_check_skip_algo(self, skip_bundlegen: bool = False, skip_info: str = "") -> tuple[bool, str]:
         """
         Analyse the data analysis report and check if the algorithm needs to be skipped.
         This function is overriden within algo.
         Args:
             skip_bundlegen: skip generating bundles for this algo if true.
@@ -146,79 +154,120 @@
             if os.path.isdir(self.output_path):
                 shutil.rmtree(self.output_path)
             shutil.copytree(self.template_path, self.output_path)
         else:
             self.output_path = self.template_path
         if kwargs.pop("fill_template", True):
             self.fill_records = self.fill_template_config(self.data_stats_files, self.output_path, **kwargs)
-        logger.info(self.output_path)
+        logger.info(f"Generated:{self.output_path}")
 
-    def _create_cmd(self, train_params=None):
+    def _create_cmd(self, train_params: None | dict = None) -> tuple[str, str]:
         """
         Create the command to execute training.
 
         """
-        if train_params is not None:
-            params = deepcopy(train_params)
+        if train_params is None:
+            train_params = {}
+        params = deepcopy(train_params)
 
         train_py = os.path.join(self.output_path, "scripts", "train.py")
         config_dir = os.path.join(self.output_path, "configs")
 
         if os.path.isdir(config_dir):
             base_cmd = ""
-            for file in os.listdir(config_dir):
+            for file in sorted(os.listdir(config_dir)):
                 if not (file.endswith("yaml") or file.endswith("json")):
                     continue
-                if len(base_cmd) == 0:
-                    base_cmd += f"{train_py} run --config_file="
-                else:
-                    base_cmd += ","  # Python Fire does not accept space
+                base_cmd += f"{train_py} run --config_file=" if len(base_cmd) == 0 else ","
                 # Python Fire may be confused by single-quoted WindowsPath
                 config_yaml = Path(os.path.join(config_dir, file)).as_posix()
                 base_cmd += f"'{config_yaml}'"
-
-        if "CUDA_VISIBLE_DEVICES" in params:
-            devices = params.pop("CUDA_VISIBLE_DEVICES")
-            n_devices, devices_info = len(devices), ",".join([str(x) for x in devices])
-        else:
-            n_devices, devices_info = torch.cuda.device_count(), ""
-        if n_devices > 1:
-            cmd = f"torchrun --nnodes={1:d} --nproc_per_node={n_devices:d} "
+        cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
+        # make sure cmd end with a space
+        if cmd is not None and not cmd.endswith(" "):
+            cmd += " "
+        if (int(self.device_setting["NUM_NODES"]) > 1 and self.device_setting["MN_START_METHOD"] == "bcprun") or (
+            int(self.device_setting["NUM_NODES"]) <= 1 and int(self.device_setting["n_devices"]) <= 1
+        ):
+            cmd = "python " if cmd is None else cmd
+        elif int(self.device_setting["NUM_NODES"]) > 1:
+            raise NotImplementedError(
+                f"{self.device_setting['MN_START_METHOD']} is not supported yet."
+                "Try modify BundleAlgo._create_cmd for your cluster."
+            )
         else:
-            cmd = "python "  # TODO: which system python?
+            if cmd is None:
+                cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
         cmd += base_cmd
         if params and isinstance(params, Mapping):
             for k, v in params.items():
                 cmd += f" --{k}={v}"
-        return cmd, devices_info
+        return cmd, ""
 
-    def _run_cmd(self, cmd: str, devices_info: str) -> subprocess.CompletedProcess:
+    def _run_cmd(self, cmd: str, devices_info: str = "") -> subprocess.CompletedProcess:
         """
         Execute the training command with target devices information.
 
         """
+        if devices_info:
+            warnings.warn(f"input devices_info {devices_info} is deprecated and ignored.")
 
-        logger.info(f"Launching: {cmd}")
         ps_environ = os.environ.copy()
-        if devices_info:
-            ps_environ["CUDA_VISIBLE_DEVICES"] = devices_info
-        normal_out = subprocess.run(cmd.split(), env=ps_environ, check=True)
+        ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
+        if int(self.device_setting["NUM_NODES"]) > 1:
+            if self.device_setting["MN_START_METHOD"] == "bcprun":
+                cmd_list = [
+                    "bcprun",
+                    "-n",
+                    str(self.device_setting["NUM_NODES"]),
+                    "-p",
+                    str(self.device_setting["n_devices"]),
+                    "-c",
+                    cmd,
+                ]
+            else:
+                raise NotImplementedError(
+                    f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
+                    "Try modify BundleAlgo._run_cmd for your cluster."
+                )
+        else:
+            cmd_list = cmd.split()
+
+        _idx = 0
+        for _idx, c in enumerate(cmd_list):
+            if "=" not in c:  # remove variable assignments before the command such as "OMP_NUM_THREADS=1"
+                break
+        cmd_list = cmd_list[_idx:]
+
+        logger.info(f"Launching: {' '.join(cmd_list)}")
 
-        return normal_out
+        return subprocess.run(cmd_list, env=ps_environ, check=True)
 
-    def train(self, train_params=None):
+    def train(
+        self, train_params: None | dict = None, device_setting: None | dict = None
+    ) -> subprocess.CompletedProcess:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
 
         Args:
-            train_params:  to specify the devices using a list of integers: ``{"CUDA_VISIBLE_DEVICES": [1,2,3]}``.
-        """
-        cmd, devices_info = self._create_cmd(train_params)
-        return self._run_cmd(cmd, devices_info)
+            train_params:  training parameters
+            device_settings: device related settings, should follow the device_setting in auto_runner.set_device_info.
+            'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
+        """
+        if device_setting is not None:
+            self.device_setting.update(device_setting)
+            self.device_setting["n_devices"] = len(str(self.device_setting["CUDA_VISIBLE_DEVICES"]).split(","))
+
+        if train_params is not None and "CUDA_VISIBLE_DEVICES" in train_params:
+            warnings.warn("CUDA_VISIBLE_DEVICES is deprecated from train_params!")
+            train_params.pop("CUDA_VISIBLE_DEVICES")
+
+        cmd, _unused_return = self._create_cmd(train_params)
+        return self._run_cmd(cmd)
 
     def get_score(self, *args, **kwargs):
         """
         Returns validation scores of the model trained by the current Algo.
         """
         config_yaml = os.path.join(self.output_path, "configs", "hyper_parameters.yaml")
         parser = ConfigParser()
@@ -272,19 +321,15 @@
         Use the trained model to predict the outputs with a given input image.
 
         Args:
             predict_files: a list of paths to files to run inference on ["path_to_image_1", "path_to_image_2"]
             predict_params: a dict to override the parameters in the bundle config (including the files to predict).
 
         """
-        if predict_params is None:
-            params = {}
-        else:
-            params = deepcopy(predict_params)
-
+        params = {} if predict_params is None else deepcopy(predict_params)
         inferer = self.get_inferer(**params)
         return [inferer.infer(f) for f in ensure_tuple(predict_files)]
 
     def get_output_path(self):
         """Returns the algo output paths to find the algo scripts and configs."""
         return self.output_path
 
@@ -351,15 +396,15 @@
 
     algos_all = {}
     for name in os.listdir(at_path):
         if os.path.exists(os.path.join(folder, name, "scripts", "algo.py")):
             algos_all[name] = dict(
                 _target_=f"{name}.scripts.algo.{name.capitalize()}Algo", template_path=os.path.join(at_path, name)
             )
-            logger.info(f"{name} -- {algos_all[name]}")
+            logger.info(f"Copying template: {name} -- {algos_all[name]}")
     if not algos_all:
         raise ValueError(f"Unable to find any algos in {folder}")
 
     return algos_all
 
 
 class BundleGen(AlgoGen):
@@ -369,19 +414,18 @@
     Args:
         algo_path: the directory path to save the algorithm templates. Default is the current working dir.
         algos: If dictionary, it outlines the algorithm to use. If a list or a string, defines a subset of names of
             the algorithms to use, e.g. ('segresnet', 'dints') out of the full set of algorithm templates provided
             by templates_path_or_url. Defaults to None - to use all available algorithms.
         templates_path_or_url: the folder with the algorithm templates or a url. If None provided, the default template
             zip url will be downloaded and extracted into the algo_path. The current default options are released at:
-            https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg
-        data_stats_filename: the path to the data stats file (generated by DataAnalyzer)
+            https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg.
+        data_stats_filename: the path to the data stats file (generated by DataAnalyzer).
         data_src_cfg_name: the path to the data source config YAML file. The config will be in a form of
-            {"modality": "ct", "datalist": "path_to_json_datalist", "dataroot": "path_dir_data"}
-
+                           {"modality": "ct", "datalist": "path_to_json_datalist", "dataroot": "path_dir_data"}.
     .. code-block:: bash
 
         python -m monai.apps.auto3dseg BundleGen generate --data_stats_filename="../algorithms/datastats.yaml"
     """
 
     def __init__(
         self,
@@ -476,27 +520,30 @@
 
     def generate(
         self,
         output_folder: str = ".",
         num_fold: int = 5,
         gpu_customization: bool = False,
         gpu_customization_specs: dict[str, Any] | None = None,
+        allow_skip: bool = True,
     ) -> None:
         """
         Generate the bundle scripts/configs for each bundleAlgo
 
         Args:
             output_folder: the output folder to save each algorithm.
             num_fold: the number of cross validation fold.
             gpu_customization: the switch to determine automatically customize/optimize bundle script/config
                 parameters for each bundleAlgo based on gpus. Custom parameters are obtained through dummy
                 training to simulate the actual model training process and hyperparameter optimization (HPO)
                 experiments.
             gpu_customization_specs (optinal): the dictionary to enable users overwrite the HPO settings. user can
                 overwrite part of variables as follows or all of them. The structure is as follows.
+            allow_skip: a switch to determine if some Algo in the default templates can be skipped based on the
+                analysis on the dataset from Auto3DSeg DataAnalyzer.
 
                 .. code-block:: python
 
                     gpu_customization_specs = {
                         'ALOG': {
                             'num_trials': 6,
                             'range_num_images_per_batch': [1, 20],
@@ -518,18 +565,21 @@
             for f_id in ensure_tuple(fold_idx):
                 data_stats = self.get_data_stats()
                 data_src_cfg = self.get_data_src()
                 gen_algo = deepcopy(algo)
                 gen_algo.set_data_stats(data_stats)
                 gen_algo.set_data_source(data_src_cfg)
                 name = f"{gen_algo.name}_{f_id}"
-                skip_bundlegen, skip_info = gen_algo.pre_check_skip_algo()
-                if skip_bundlegen:
-                    logger.info(f"{name} is skipped! {skip_info}")
-                    continue
+
+                if allow_skip:
+                    skip_bundlegen, skip_info = gen_algo.pre_check_skip_algo()
+                    if skip_bundlegen:
+                        logger.info(f"{name} is skipped! {skip_info}")
+                        continue
+
                 if gpu_customization:
                     gen_algo.export_to_disk(
                         output_folder,
                         name,
                         fold=f_id,
                         gpu_customization=True,
                         gpu_customization_specs=gpu_customization_specs,
```

## monai/apps/auto3dseg/ensemble_builder.py

```diff
@@ -8,32 +8,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
+import subprocess
 from abc import ABC, abstractmethod
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from copy import deepcopy
 from typing import Any, cast
 from warnings import warn
 
 import numpy as np
 import torch
+import torch.distributed as dist
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
+from monai.apps.auto3dseg.utils import import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg import concat_val_to_np
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import ConfigParser
-from monai.transforms import MeanEnsemble, VoteEnsemble
+from monai.data import partition_dataset
+from monai.transforms import MeanEnsemble, SaveImage, VoteEnsemble
 from monai.utils.enums import AlgoKeys
-from monai.utils.misc import prob2class
-from monai.utils.module import look_up_option
+from monai.utils.misc import check_kwargs_exist_in_class_init, prob2class
+from monai.utils.module import look_up_option, optional_import
+
+tqdm, has_tqdm = optional_import("tqdm", name="tqdm")
 
 logger = get_logger(module_name=__name__)
 
 
 class AlgoEnsemble(ABC):
     """
     The base class of Ensemble methods
@@ -84,15 +90,15 @@
 
         if isinstance(data_list_or_path, list):
             self.infer_files = data_list_or_path
         elif isinstance(data_list_or_path, str):
             datalist = ConfigParser.load_config_file(data_list_or_path)
             if data_key in datalist:
                 self.infer_files, _ = datafold_read(datalist=datalist, basedir=dataroot, fold=-1, key=data_key)
-            else:
+            elif hasattr(self, "rank") and self.rank == 0:
                 logger.info(f"Datalist file has no testing key - {data_key}. No data for inference is specified")
 
         else:
             raise ValueError("Unsupported parameter type")
 
     def ensemble_pred(self, preds, sigmoid=False):
         """
@@ -103,25 +109,28 @@
             sigmoid: use the sigmoid function to threshold probability one-hot map,
                 otherwise argmax is used. Defaults to False
 
         Returns:
             a tensor which is the ensembled prediction.
         """
 
+        if any(not p.is_cuda for p in preds):
+            preds = [p.cpu() for p in preds]  # ensure CPU if at least one is on CPU
+
         if self.mode == "mean":
             prob = MeanEnsemble()(preds)
             return prob2class(cast(torch.Tensor, prob), dim=0, keepdim=True, sigmoid=sigmoid)
         elif self.mode == "vote":
             classes = [prob2class(p, dim=0, keepdim=True, sigmoid=sigmoid) for p in preds]
             if sigmoid:
                 return VoteEnsemble()(classes)  # do not specify num_classes for one-hot encoding
             else:
                 return VoteEnsemble(num_classes=preds[0].shape[0])(classes)
 
-    def __call__(self, pred_param: dict[str, Any] | None = None) -> list[torch.Tensor]:
+    def __call__(self, pred_param: dict | None = None) -> list:
         """
         Use the ensembled model to predict result.
 
         Args:
             pred_param: prediction parameter dictionary. The key has two groups: the first one will be consumed
                 in this function, and the second group will be passed to the `InferClass` to override the
                 parameters of the class functions.
@@ -131,19 +140,15 @@
                 'mode': ensemble mode. Currently "mean" and "vote" (majority voting) schemes are supported.
                 'sigmoid': use the sigmoid function (e.g. x>0.5) to convert the prediction probability map to
                     the label class prediction, otherwise argmax(x) is used.
 
         Returns:
             A list of tensors.
         """
-        if pred_param is None:
-            param = {}
-        else:
-            param = deepcopy(pred_param)
-
+        param = {} if pred_param is None else deepcopy(pred_param)
         files = self.infer_files
 
         if "infer_files" in param:
             files = param.pop("infer_files")
 
         if "files_slices" in param:
             slices = param.pop("files_slices")
@@ -151,23 +156,44 @@
 
         if "mode" in param:
             mode = param.pop("mode")
             self.mode = look_up_option(mode, supported=["mean", "vote"])
 
         sigmoid = param.pop("sigmoid", False)
 
+        if "image_save_func" in param:
+            img_saver = ConfigParser(param["image_save_func"]).get_parsed_content()
+
         outputs = []
-        for i, file in enumerate(files):
-            print(i)
+        for _, file in (
+            enumerate(tqdm(files, desc="Ensembling (rank 0)..."))
+            if has_tqdm and pred_param and pred_param.get("rank", 0) == 0
+            else enumerate(files)
+        ):
             preds = []
             for algo in self.algo_ensemble:
                 infer_instance = algo[AlgoKeys.ALGO]
                 pred = infer_instance.predict(predict_files=[file], predict_params=param)
                 preds.append(pred[0])
-            outputs.append(self.ensemble_pred(preds, sigmoid=sigmoid))
+            if "image_save_func" in param:
+                try:
+                    ensemble_preds = self.ensemble_pred(preds, sigmoid=sigmoid)
+                except BaseException:
+                    ensemble_preds = self.ensemble_pred([_.to("cpu") for _ in preds], sigmoid=sigmoid)
+                res = img_saver(ensemble_preds)
+                # res is the path to the saved results
+                if hasattr(res, "meta") and "saved_to" in res.meta.keys():
+                    res = res.meta["saved_to"]
+                else:
+                    warn("Image save path not returned.")
+                    res = None
+            else:
+                warn("Prediction returned in list instead of disk, provide image_save_func to avoid out of memory.")
+                res = self.ensemble_pred(preds, sigmoid=sigmoid)
+            outputs.append(res)
         return outputs
 
     @abstractmethod
     def collect_algos(self, *args, **kwargs):
         raise NotImplementedError
 
 
@@ -323,7 +349,268 @@
 
         self.ensemble = ensemble
 
     def get_ensemble(self):
         """Get the ensemble"""
 
         return self.ensemble
+
+
+class EnsembleRunner:
+    """
+    The Runner for ensembler
+
+    Args:
+        work_dir: working directory to save the intermediate and final results.
+        data_src_cfg_name: filename of the data source.
+        num_fold: number of fold.
+        ensemble_method_name: method to ensemble predictions from different model.
+                              Suported methods: ["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"].
+        mgpu: if using multi-gpu.
+        kwargs: additional image writing, ensembling parameters and prediction parameters for the ensemble inference.
+    Examples:
+
+        .. code-block:: python
+
+            ensemble_runner = EnsembleRunner(data_src_cfg_name,
+                                             work_dir,
+                                             ensemble_method_name,
+                                             mgpu=device_setting['n_devices']>1,
+                                             **kwargs,
+                                             **pred_params)
+            ensemble_runner.run(device_setting)
+
+    """
+
+    def __init__(
+        self,
+        data_src_cfg_name: str = "./work_dir/input.yaml",
+        work_dir: str = "./work_dir",
+        num_fold: int = 5,
+        ensemble_method_name: str = "AlgoEnsembleBestByFold",
+        mgpu: bool = True,
+        **kwargs: Any,
+    ) -> None:
+        self.data_src_cfg_name = data_src_cfg_name
+        self.work_dir = work_dir
+        self.num_fold = num_fold
+        self.ensemble_method_name = ensemble_method_name
+        self.mgpu = mgpu
+        self.kwargs = deepcopy(kwargs)
+        self.rank = 0
+        self.world_size = 1
+        self.device_setting: dict[str, int | str] = {
+            "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
+            "n_devices": torch.cuda.device_count(),
+            "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
+            "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
+            "CMD_PREFIX": os.environ.get("CMD_PREFIX"),  # type: ignore
+        }
+
+        # self.kwargs needs to pop out args for set_image_save_transform
+        self.save_image: dict[str, Any] = self._pop_kwargs_to_get_image_save_transform(**self.kwargs)
+
+    def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
+        """
+        Set the bundle ensemble method
+
+        Args:
+            ensemble_method_name: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
+                and "AlgoEnsembleBestByFold".
+            kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
+                ``AlgoEnsembleBestN`` is supported.
+
+        """
+        self.ensemble_method_name = look_up_option(
+            ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
+        )
+        if self.ensemble_method_name == "AlgoEnsembleBestN":
+            n_best = kwargs.pop("n_best", False) or 2
+            self.ensemble_method = AlgoEnsembleBestN(n_best=n_best)
+        elif self.ensemble_method_name == "AlgoEnsembleBestByFold":
+            self.ensemble_method = AlgoEnsembleBestByFold(n_fold=self.num_fold)  # type: ignore
+        else:
+            raise NotImplementedError(f"Ensemble method {self.ensemble_method_name} is not implemented.")
+
+    def _pop_kwargs_to_get_image_save_transform(self, **kwargs):
+        """
+        Pop the kwargs used to define ImageSave class for the ensemble output.
+
+        Args:
+            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
+                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
+
+        Returns:
+            save_image: a dictionary that can be used to instantiate a SaveImage class in ConfigParser.
+        """
+
+        output_dir = kwargs.pop("output_dir", None)
+
+        if output_dir is None:
+            output_dir = os.path.join(self.work_dir, "ensemble_output")
+            logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions.")
+
+        if not os.path.isdir(output_dir):
+            os.makedirs(output_dir, exist_ok=True)
+            logger.info(f"Directory {output_dir} is created to save ensemble predictions")
+
+        save_image = {
+            "_target_": "SaveImage",
+            "output_dir": output_dir,
+            "output_postfix": kwargs.pop("output_postfix", "ensemble"),
+            "output_dtype": kwargs.pop("output_dtype", "$np.uint8"),
+            "resample": kwargs.pop("resample", False),
+            "print_log": False,
+            "savepath_in_metadict": True,
+        }
+
+        are_all_args_save_image, extra_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
+        if are_all_args_save_image:
+            save_image.update(kwargs)
+        else:
+            # kwargs has extra values for other purposes, for example, pred_params
+            for args in list(kwargs):
+                if args not in extra_args:
+                    save_image.update({args: kwargs.pop(args)})
+
+        return save_image
+
+    def set_image_save_transform(self, **kwargs):
+        """
+        Set the ensemble output transform.
+
+        Args:
+            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
+                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
+
+        """
+        kwargs_copy = deepcopy(kwargs)
+        self.save_image = self._pop_kwargs_to_get_image_save_transform(**kwargs_copy)
+
+    def set_num_fold(self, num_fold: int = 5) -> None:
+        """
+        Set the number of cross validation folds for all algos.
+
+        Args:
+            num_fold: a positive integer to define the number of folds.
+        """
+
+        if num_fold <= 0:
+            raise ValueError(f"num_fold is expected to be an integer greater than zero. Now it gets {num_fold}")
+        self.num_fold = num_fold
+
+    def ensemble(self):
+        if self.mgpu:  # torch.cuda.device_count() is not used because env is not set by autorruner
+            # init multiprocessing and update infer_files
+            dist.init_process_group(backend="nccl", init_method="env://")
+            self.world_size = dist.get_world_size()
+            self.rank = dist.get_rank()
+        # set params after init_process_group to know the rank
+        self.set_num_fold(num_fold=self.num_fold)
+        self.set_ensemble_method(self.ensemble_method_name, **self.kwargs)
+
+        history = import_bundle_algo_history(self.work_dir, only_trained=False)
+        history_untrained = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
+        if history_untrained:
+            if self.rank == 0:
+                warn(
+                    f"Ensembling step will skip {[h[AlgoKeys.ID] for h in history_untrained]} untrained algos."
+                    "Generally it means these algos did not complete training."
+                )
+            history = [h for h in history if h[AlgoKeys.IS_TRAINED]]
+        if len(history) == 0:
+            raise ValueError(
+                f"Could not find the trained results in {self.work_dir}. "
+                "Possibly the required training step was not completed."
+            )
+
+        builder = AlgoEnsembleBuilder(history, self.data_src_cfg_name)
+        builder.set_ensemble_method(self.ensemble_method)
+        self.ensembler = builder.get_ensemble()
+        infer_files = self.ensembler.infer_files
+        infer_files = partition_dataset(
+            data=infer_files, shuffle=False, num_partitions=self.world_size, even_divisible=True
+        )[self.rank]
+        # TO DO: Add some function in ensembler for infer_files update?
+        self.ensembler.infer_files = infer_files
+        # add rank to pred_params
+        self.kwargs["rank"] = self.rank
+        self.kwargs["image_save_func"] = self.save_image
+        if self.rank == 0:
+            logger.info("Auto3Dseg picked the following networks to ensemble:")
+            for algo in self.ensembler.get_algo_ensemble():
+                logger.info(algo[AlgoKeys.ID])
+            output_dir = self.save_image["output_dir"]
+            logger.info(f"Auto3Dseg ensemble prediction outputs will be saved in {output_dir}.")
+        self.ensembler(pred_param=self.kwargs)
+
+        if self.mgpu:
+            dist.destroy_process_group()
+
+    def run(self, device_setting: dict | None = None) -> None:
+        """
+        Load the run function in the training script of each model. Training parameter is predefined by the
+        algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
+
+        Args:
+            train_params:  training parameters
+            device_settings: device related settings, should follow the device_setting in auto_runner.set_device_info.
+            'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
+        """
+        # device_setting set default value and sanity check, in case device_setting not from autorunner
+        if device_setting is not None:
+            self.device_setting.update(device_setting)
+            self.device_setting["n_devices"] = len(str(self.device_setting["CUDA_VISIBLE_DEVICES"]).split(","))
+        self._create_cmd()
+
+    def _create_cmd(self) -> None:
+        if int(self.device_setting["NUM_NODES"]) <= 1 and int(self.device_setting["n_devices"]) <= 1:
+            # if single GPU
+            logger.info("Ensembling using single GPU!")
+            self.ensemble()
+            return
+
+        # define base cmd for subprocess
+        base_cmd = f"monai.apps.auto3dseg EnsembleRunner ensemble \
+                --data_src_cfg_name {self.data_src_cfg_name} \
+                --work_dir {self.work_dir} \
+                --num_fold {self.num_fold} \
+                --ensemble_method_name {self.ensemble_method_name} \
+                --mgpu True"
+
+        if self.kwargs and isinstance(self.kwargs, Mapping):
+            for k, v in self.kwargs.items():
+                base_cmd += f" --{k}={v}"
+        # define env for subprocess
+        ps_environ = os.environ.copy()
+        ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
+        cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
+        if cmd is not None and not str(cmd).endswith(" "):
+            cmd += " "
+        if int(self.device_setting["NUM_NODES"]) > 1:
+            if self.device_setting["MN_START_METHOD"] != "bcprun":
+                raise NotImplementedError(
+                    f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
+                    "Try modify EnsembleRunner._create_cmd for your cluster."
+                )
+            logger.info(f"Ensembling on {self.device_setting['NUM_NODES']} nodes!")
+            cmd = "python " if cmd is None else cmd
+            cmd = f"{cmd} -m {base_cmd}"
+            cmd_list = [
+                "bcprun",
+                "-n",
+                str(self.device_setting["NUM_NODES"]),
+                "-p",
+                str(self.device_setting["n_devices"]),
+                "-c",
+                cmd,
+            ]
+
+        else:
+            logger.info(f"Ensembling using {self.device_setting['n_devices']} GPU!")
+            if cmd is None:
+                cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
+            cmd = f"{cmd} -m {base_cmd}"
+            cmd_list = cmd.split()
+
+        _ = subprocess.run(cmd_list, env=ps_environ, check=True)
+        return
```

## monai/apps/auto3dseg/utils.py

```diff
@@ -46,14 +46,20 @@
 
         algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
         if isinstance(algo, BundleAlgo):  # algo's template path needs override
             algo.template_path = algo_meta_data["template_path"]
 
         best_metric = algo_meta_data.get(AlgoKeys.SCORE, None)
+        if best_metric is None:
+            try:
+                best_metric = algo.get_score()
+            except BaseException:
+                pass
+
         is_trained = best_metric is not None
 
         if (only_trained and is_trained) or not only_trained:
             history.append(
                 {AlgoKeys.ID: name, AlgoKeys.ALGO: algo, AlgoKeys.SCORE: best_metric, AlgoKeys.IS_TRAINED: is_trained}
             )
```

## monai/apps/detection/networks/retinanet_detector.py

```diff
@@ -118,27 +118,31 @@
             - size_divisible (int or Sequence[int]) is the expectation on the input image shape.
               The network needs the input spatial_size to be divisible by size_divisible, length should be 2 or 3.
             - cls_key (str) is the key to represent classification in the output dict.
             - box_reg_key (str) is the key to represent box regression in the output dict.
             - num_anchors (int) is the number of anchor shapes at each location. it should equal to
               ``self.anchor_generator.num_anchors_per_location()[0]``.
 
+            If network does not have these attributes, user needs to provide them for the detector.
+
         2. Its input should be an image Tensor sized (B, C, H, W) or (B, C, H, W, D).
 
-        3. About its output ``head_outputs``:
+        3. About its output ``head_outputs``, it should be either a list of tensors or a dictionary of str: List[Tensor]:
 
-            - It should be a dictionary with at least two keys:
-              ``network.cls_key`` and ``network.box_reg_key``.
-            - ``head_outputs[network.cls_key]`` should be List[Tensor] or Tensor. Each Tensor represents
+            - If it is a dictionary, it needs to have at least two keys:
+              ``network.cls_key`` and ``network.box_reg_key``, representing predicted classification maps and box regression maps.
+              ``head_outputs[network.cls_key]`` should be List[Tensor] or Tensor. Each Tensor represents
               classification logits map at one resolution level,
               sized (B, num_classes*num_anchors, H_i, W_i) or (B, num_classes*num_anchors, H_i, W_i, D_i).
-            - ``head_outputs[network.box_reg_key]`` should be List[Tensor] or Tensor. Each Tensor represents
+              ``head_outputs[network.box_reg_key]`` should be List[Tensor] or Tensor. Each Tensor represents
               box regression map at one resolution level,
               sized (B, 2*spatial_dims*num_anchors, H_i, W_i)or (B, 2*spatial_dims*num_anchors, H_i, W_i, D_i).
-            - ``len(head_outputs[network.cls_key]) == len(head_outputs[network.box_reg_key])``.
+              ``len(head_outputs[network.cls_key]) == len(head_outputs[network.box_reg_key])``.
+            - If it is a list of 2N tensors, the first N tensors should be the predicted classification maps,
+              and the second N tensors should be the predicted box regression maps.
 
     Example:
 
         .. code-block:: python
 
             # define a naive network
             import torch
@@ -180,42 +184,41 @@
     """
 
     def __init__(
         self,
         network: nn.Module,
         anchor_generator: AnchorGenerator,
         box_overlap_metric: Callable = box_iou,
+        spatial_dims: int | None = None,  # used only when network.spatial_dims does not exist
+        num_classes: int | None = None,  # used only when network.num_classes does not exist
+        size_divisible: Sequence[int] | int = 1,  # used only when network.size_divisible does not exist
+        cls_key: str = "classification",  # used only when network.cls_key does not exist
+        box_reg_key: str = "box_regression",  # used only when network.box_reg_key does not exist
         debug: bool = False,
     ):
         super().__init__()
 
-        if not all(
-            hasattr(network, attr)
-            for attr in ["spatial_dims", "num_classes", "cls_key", "box_reg_key", "num_anchors", "size_divisible"]
-        ):
-            raise AttributeError(
-                "network should have attributes, including: "
-                "'spatial_dims', 'num_classes', 'cls_key', 'box_reg_key', 'num_anchors', 'size_divisible'."
-            )
-
         self.network = network
-        self.spatial_dims: int = self.network.spatial_dims  # type: ignore[assignment]
-        self.num_classes = self.network.num_classes
-        self.size_divisible = ensure_tuple_rep(self.network.size_divisible, self.spatial_dims)
+        # network attribute
+        self.spatial_dims = self.get_attribute_from_network("spatial_dims", default_value=spatial_dims)
+        self.num_classes = self.get_attribute_from_network("num_classes", default_value=num_classes)
+
+        self.size_divisible = self.get_attribute_from_network("size_divisible", default_value=size_divisible)
+        self.size_divisible = ensure_tuple_rep(self.size_divisible, self.spatial_dims)
         # keys for the network output
-        self.cls_key: str = self.network.cls_key  # type: ignore[assignment]
-        self.box_reg_key: str = self.network.box_reg_key  # type: ignore[assignment]
+        self.cls_key = self.get_attribute_from_network("cls_key", default_value=cls_key)
+        self.box_reg_key = self.get_attribute_from_network("box_reg_key", default_value=box_reg_key)
 
         # check if anchor_generator matches with network
         self.anchor_generator = anchor_generator
-
         self.num_anchors_per_loc = self.anchor_generator.num_anchors_per_location()[0]
-        if self.num_anchors_per_loc != self.network.num_anchors:
+        network_num_anchors = self.get_attribute_from_network("num_anchors", default_value=self.num_anchors_per_loc)
+        if self.num_anchors_per_loc != network_num_anchors:
             raise ValueError(
-                f"Number of feature map channels ({self.network.num_anchors}) "
+                f"Number of feature map channels ({network_num_anchors}) "
                 f"should match with number of anchors at each location ({self.num_anchors_per_loc})."
             )
         # if new coming input images has same shape with
         # self.previous_image_shape, there is no need to generate new anchors.
         self.anchors: list[Tensor] | None = None
         self.previous_image_shape: Any | None = None
 
@@ -248,14 +251,22 @@
             score_thresh=0.05,
             topk_candidates_per_level=1000,
             nms_thresh=0.5,
             detections_per_img=300,
             apply_sigmoid=True,
         )
 
+    def get_attribute_from_network(self, attr_name, default_value=None):
+        if hasattr(self.network, attr_name):
+            return getattr(self.network, attr_name)
+        elif default_value is not None:
+            return default_value
+        else:
+            raise ValueError(f"network does not have attribute {attr_name}, please provide it in the detector.")
+
     def set_box_coder_weights(self, weights: tuple[float]) -> None:
         """
         Set the weights for box coder.
 
         Args:
             weights: a list/tuple with length of 2*self.spatial_dims
 
@@ -493,15 +504,22 @@
         # 2. Pad list of images to a single Tensor `images` with spatial size divisible by self.size_divisible.
         # image_sizes stores the original spatial_size of each image before padding.
         images, image_sizes = preprocess_images(input_images, self.spatial_dims, self.size_divisible)
 
         # 3. Generate network outputs. Use inferer only in evaluation mode.
         if self.training or (not use_inferer):
             head_outputs = self.network(images)
-            ensure_dict_value_to_list_(head_outputs)  # ensure head_outputs is Dict[str, List[Tensor]]
+            if isinstance(head_outputs, (tuple, list)):
+                tmp_dict = {}
+                tmp_dict[self.cls_key] = head_outputs[: len(head_outputs) // 2]
+                tmp_dict[self.box_reg_key] = head_outputs[len(head_outputs) // 2 :]
+                head_outputs = tmp_dict
+            else:
+                # ensure head_outputs is Dict[str, List[Tensor]]
+                ensure_dict_value_to_list_(head_outputs)
         else:
             if self.inferer is None:
                 raise ValueError(
                     "`self.inferer` is not defined." "Please refer to function self.set_sliding_window_inferer(*)."
                 )
             head_outputs = predict_with_inferer(
                 images, self.network, keys=[self.cls_key, self.box_reg_key], inferer=self.inferer
```

## monai/apps/detection/networks/retinanet_network.py

```diff
@@ -37,15 +37,15 @@
 https://github.com/pytorch/vision/blob/main/torchvision/models/detection/retinanet.py
 """
 
 from __future__ import annotations
 
 import math
 from collections.abc import Callable, Sequence
-from typing import Dict
+from typing import Any, Dict
 
 import torch
 from torch import Tensor, nn
 
 from monai.networks.blocks.backbone_fpn_utils import BackboneWithFPN, _resnet_fpn_extractor
 from monai.networks.layers.factories import Conv
 from monai.networks.nets import resnet
@@ -199,28 +199,35 @@
         return box_regression_maps
 
 
 class RetinaNet(nn.Module):
     """
     The network used in RetinaNet.
 
-    It takes an image tensor as inputs, and outputs a dictionary ``head_outputs``.
+    It takes an image tensor as inputs, and outputs either 1) a dictionary ``head_outputs``.
     ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
     ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+    or 2) a list of 2N tensors ``head_outputs``, with first N tensors being the predicted
+    classification maps and second N tensors being the predicted box regression maps.
 
     Args:
         spatial_dims: number of spatial dimensions of the images. We support both 2D and 3D images.
         num_classes: number of output classes of the model (excluding the background).
         num_anchors: number of anchors at each location.
         feature_extractor: a network that outputs feature maps from the input images,
             each feature map corresponds to a different resolution.
             Its output can have a format of Tensor, Dict[Any, Tensor], or Sequence[Tensor].
             It can be the output of ``resnet_fpn_feature_extractor(*args, **kwargs)``.
         size_divisible: the spatial size of the network input should be divisible by size_divisible,
             decided by the feature_extractor.
+        use_list_output: default False. If False, the network outputs a dictionary ``head_outputs``,
+            ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
+            ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+            If True, the network outputs a list of 2N tensors ``head_outputs``, with first N tensors being
+            the predicted classification maps and second N tensors being the predicted box regression maps.
 
     Example:
 
         .. code-block:: python
 
             from monai.networks.nets import resnet
             spatial_dims = 3  # 3D network
@@ -251,31 +258,33 @@
                 spatial_dims = spatial_dims,
                 num_classes = 5,
                 num_anchors = 6,
                 feature_extractor=feature_extractor,
                 size_divisible = size_divisible,
             ).to(device)
             result = model(torch.rand(2, 1, 128,128,128))
-            cls_logits_maps = result["cls_logits"]  # a list of len(returned_layers)+1 Tensor
+            cls_logits_maps = result["classification"]  # a list of len(returned_layers)+1 Tensor
             box_regression_maps = result["box_regression"]  # a list of len(returned_layers)+1 Tensor
     """
 
     def __init__(
         self,
         spatial_dims: int,
         num_classes: int,
         num_anchors: int,
         feature_extractor: nn.Module,
         size_divisible: Sequence[int] | int = 1,
+        use_list_output: bool = False,
     ):
         super().__init__()
 
         self.spatial_dims = look_up_option(spatial_dims, supported=[1, 2, 3])
         self.num_classes = num_classes
         self.size_divisible = ensure_tuple_rep(size_divisible, self.spatial_dims)
+        self.use_list_output = use_list_output
 
         if not hasattr(feature_extractor, "out_channels"):
             raise ValueError(
                 "feature_extractor should contain an attribute out_channels "
                 "specifying the number of output channels (assumed to be the "
                 "same for all the levels)"
             )
@@ -289,27 +298,29 @@
         self.regression_head = RetinaNetRegressionHead(
             self.feature_map_channels, self.num_anchors, spatial_dims=self.spatial_dims
         )
 
         self.cls_key: str = "classification"
         self.box_reg_key: str = "box_regression"
 
-    def forward(self, images: Tensor) -> dict[str, list[Tensor]]:
+    def forward(self, images: Tensor) -> Any:
         """
-        It takes an image tensor as inputs, and outputs a dictionary ``head_outputs``.
-        ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
-        ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+        It takes an image tensor as inputs, and outputs predicted classification maps
+        and predicted box regression maps in ``head_outputs``.
 
         Args:
             images: input images, sized (B, img_channels, H, W) or (B, img_channels, H, W, D).
 
         Return:
-            a dictionary ``head_outputs`` with keys including self.cls_key and self.box_reg_key.
+            1) If self.use_list_output is False, output a dictionary ``head_outputs`` with
+            keys including self.cls_key and self.box_reg_key.
             ``head_outputs[self.cls_key]`` is the predicted classification maps, a list of Tensor.
             ``head_outputs[self.box_reg_key]`` is the predicted box regression maps, a list of Tensor.
+            2) if self.use_list_output is True, outputs a list of 2N tensors ``head_outputs``, with first N tensors being
+            the predicted classification maps and second N tensors being the predicted box regression maps.
 
         """
         # compute features maps list from the input images.
         features = self.feature_extractor(images)
         if isinstance(features, Tensor):
             feature_maps = [features]
         elif torch.jit.isinstance(features, Dict[str, Tensor]):
@@ -319,18 +330,23 @@
 
         if not isinstance(feature_maps[0], Tensor):
             raise ValueError("feature_extractor output format must be Tensor, Dict[str, Tensor], or Sequence[Tensor].")
 
         # compute classification and box regression maps from the feature maps
         # expandable for mask prediction in the future
 
-        head_outputs: dict[str, list[Tensor]] = {self.cls_key: self.classification_head(feature_maps)}
-        head_outputs[self.box_reg_key] = self.regression_head(feature_maps)
-
-        return head_outputs
+        if not self.use_list_output:
+            # output dict
+            head_outputs = {self.cls_key: self.classification_head(feature_maps)}
+            head_outputs[self.box_reg_key] = self.regression_head(feature_maps)
+            return head_outputs
+        else:
+            # output list of tensor, first half is classification, second half is box regression
+            head_outputs_sequence = self.classification_head(feature_maps) + self.regression_head(feature_maps)
+            return head_outputs_sequence
 
 
 def resnet_fpn_feature_extractor(
     backbone: resnet.ResNet,
     spatial_dims: int,
     pretrained_backbone: bool = False,
     returned_layers: Sequence[int] = (1, 2, 3),
```

## monai/apps/detection/transforms/box_ops.py

```diff
@@ -17,20 +17,18 @@
 import numpy as np
 import torch
 
 from monai.config.type_definitions import DtypeLike, NdarrayOrTensor, NdarrayTensor
 from monai.data.box_utils import COMPUTE_DTYPE, TO_REMOVE, get_spatial_dims
 from monai.transforms import Resize
 from monai.transforms.utils import create_scale
-from monai.utils import look_up_option, optional_import
+from monai.utils import look_up_option
 from monai.utils.misc import ensure_tuple, ensure_tuple_rep
 from monai.utils.type_conversion import convert_data_type, convert_to_dst_type
 
-scipy, _ = optional_import("scipy")
-
 
 def _apply_affine_to_points(points: torch.Tensor, affine: torch.Tensor, include_shift: bool = True) -> torch.Tensor:
     """
     This internal function applies affine matrices to the point coordinate
 
     Args:
         points: point coordinates, Nx2 or Nx3 torch tensor or ndarray, representing [x, y] or [x, y, z]
```

## monai/apps/detection/utils/predict_utils.py

```diff
@@ -69,14 +69,20 @@
         keys: the keys in the network output whose values will be output in this func.
             If not provided, will use all keys.
 
     Return:
         network output values concat to a single List[Tensor]
     """
     head_outputs = network(images)
+
+    # if head_outputs is already a sequence of tensors, directly output it
+    if isinstance(head_outputs, (tuple, list)):
+        return list(head_outputs)
+
+    # if head_outputs is a dict
     ensure_dict_value_to_list_(head_outputs, keys)
     if keys is None:
         keys = list(head_outputs.keys())
     check_dict_values_same_length(head_outputs, keys)
     head_outputs_sequence = []
     for k in keys:
         head_outputs_sequence += list(head_outputs[k])
```

## monai/apps/pathology/transforms/post/dictionary.py

```diff
@@ -31,15 +31,14 @@
 )
 from monai.config.type_definitions import DtypeLike, KeysCollection, NdarrayOrTensor
 from monai.transforms.transform import MapTransform, Transform
 from monai.utils import optional_import
 from monai.utils.enums import HoVerNetBranch
 
 find_contours, _ = optional_import("skimage.measure", name="find_contours")
-moments, _ = optional_import("skimage.measure", name="moments")
 
 __all__ = [
     "WatershedD",
     "WatershedDict",
     "Watershedd",
     "GenerateWatershedMaskD",
     "GenerateWatershedMaskDict",
```

## monai/bundle/properties.py

```diff
@@ -155,14 +155,19 @@
         BundlePropertyConfig.ID: "bundle_root",
     },
     "device": {
         BundleProperty.DESC: "target device to execute the bundle workflow.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "device",
     },
+    "evaluator": {
+        BundleProperty.DESC: "inference / evaluation workflow engine.",
+        BundleProperty.REQUIRED: True,
+        BundlePropertyConfig.ID: "evaluator",
+    },
     "network_def": {
         BundleProperty.DESC: "network module for the inference.",
         BundleProperty.REQUIRED: True,
         BundlePropertyConfig.ID: "network_def",
     },
     "inferer": {
         BundleProperty.DESC: "MONAI Inferer object to execute the model computation in inference.",
```

## monai/bundle/scripts.py

```diff
@@ -621,16 +621,19 @@
 
         # Set default args of `run` in a JSON / YAML file, help to record and simplify the command line.
         # Other args still can override the default args at runtime:
         python -m monai.bundle run --args_file "/workspace/data/args.json" --config_file <config path>
 
     Args:
         run_id: ID name of the expected config expression to run, default to "run".
+            to run the config, the target config must contain this ID.
         init_id: ID name of the expected config expression to initialize before running, default to "initialize".
+            it's optional for both configs and this `run` function.
         final_id: ID name of the expected config expression to finalize after running, default to "finalize".
+            it's optional for both configs and this `run` function.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
             Default to "configs/metadata.json", which is commonly used for bundles in MONAI model zoo.
         config_file: filepath of the config file, if `None`, must be provided in `args_file`.
             if it is a list of file paths, the content of them will be merged.
         logging_file: config file for `logging` module in the program. for more details:
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
```

## monai/bundle/workflows.py

```diff
@@ -40,23 +40,26 @@
         workflow: specifies the workflow type: "train" or "training" for a training workflow,
             or "infer", "inference", "eval", "evaluation" for a inference workflow,
             other unsupported string will raise a ValueError.
             default to `None` for common workflow.
 
     """
 
+    supported_train_type: tuple = ("train", "training")
+    supported_infer_type: tuple = ("infer", "inference", "eval", "evaluation")
+
     def __init__(self, workflow: str | None = None):
         if workflow is None:
             self.properties = None
             self.workflow = None
             return
-        if workflow.lower() in ("train", "training"):
+        if workflow.lower() in self.supported_train_type:
             self.properties = TrainProperties
             self.workflow = "train"
-        elif workflow.lower() in ("infer", "inference", "eval", "evaluation"):
+        elif workflow.lower() in self.supported_infer_type:
             self.properties = InferProperties
             self.workflow = "infer"
         else:
             raise ValueError(f"Unsupported workflow type: '{workflow}'.")
 
     @abstractmethod
     def initialize(self, *args: Any, **kwargs: Any) -> Any:
@@ -141,16 +144,19 @@
     """
     Specification for the config-based bundle workflow.
     Standardized the `initialize`, `run`, `finalize` behavior in a config-based training, evaluation, or inference.
     For more information: https://docs.monai.io/en/latest/mb_specification.html.
 
     Args:
         run_id: ID name of the expected config expression to run, default to "run".
+            to run the config, the target config must contain this ID.
         init_id: ID name of the expected config expression to initialize before running, default to "initialize".
+            allow a config to have no `initialize` logic and the ID.
         final_id: ID name of the expected config expression to finalize after running, default to "finalize".
+            allow a config to have no `finalize` logic and the ID.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
             Default to "configs/metadata.json", which is commonly used for bundles in MONAI model zoo.
         config_file: filepath of the config file, if it is a list of file paths, the content of them will be merged.
         logging_file: config file for `logging` module in the program. for more details:
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
         tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
@@ -175,15 +181,15 @@
         meta_file: str | Sequence[str] | None = "configs/metadata.json",
         logging_file: str | None = "configs/logging.conf",
         init_id: str = "initialize",
         run_id: str = "run",
         final_id: str = "finalize",
         tracking: str | dict | None = None,
         workflow: str | None = None,
-        **override: dict,
+        **override: Any,
     ) -> None:
         super().__init__(workflow=workflow)
         if logging_file is not None:
             if not os.path.exists(logging_file):
                 if logging_file == "configs/logging.conf":
                     warnings.warn("Default logging file in 'configs/logging.conf' does not exist, skipping logging.")
                 else:
@@ -211,29 +217,33 @@
         # set tracking configs for experiment management
         if tracking is not None:
             if isinstance(tracking, str) and tracking in DEFAULT_EXP_MGMT_SETTINGS:
                 settings_ = DEFAULT_EXP_MGMT_SETTINGS[tracking]
             else:
                 settings_ = ConfigParser.load_config_files(tracking)
             self.patch_bundle_tracking(parser=self.parser, settings=settings_)
+        self._is_initialized: bool = False
 
     def initialize(self) -> Any:
         """
         Initialize the bundle workflow before running.
 
         """
         # reset the "reference_resolver" buffer at initialization stage
         self.parser.parse(reset=True)
+        self._is_initialized = True
         return self._run_expr(id=self.init_id)
 
     def run(self) -> Any:
         """
         Run the bundle workflow, it can be a training, evaluation or inference.
 
         """
+        if self.run_id not in self.parser:
+            raise ValueError(f"run ID '{self.run_id}' doesn't exist in the config file.")
         return self._run_expr(id=self.run_id)
 
     def finalize(self) -> Any:
         """
         Finalize step after the running of bundle workflow.
 
         """
@@ -280,15 +290,15 @@
         With specified property name and information, get the parsed property value from config.
 
         Args:
             name: the name of target property.
             property: other information for the target property, defined in `TrainProperties` or `InferProperties`.
 
         """
-        if not self.parser.ref_resolver.is_resolved():
+        if not self._is_initialized:
             raise RuntimeError("Please execute 'initialize' before getting any parsed content.")
         prop_id = self._get_prop_id(name, property)
         return self.parser.get_parsed_content(id=prop_id) if prop_id is not None else None
 
     def _set_property(self, name: str, property: dict, value: Any) -> None:
         """
         With specified property name and information, set value for the expected property.
@@ -299,14 +309,15 @@
             value: value to set for the property.
 
         """
         prop_id = self._get_prop_id(name, property)
         if prop_id is not None:
             self.parser[prop_id] = value
             # must parse the config again after changing the content
+            self._is_initialized = False
             self.parser.ref_resolver.reset()
 
     def _check_optional_id(self, name: str, property: dict) -> bool:
         """
         If an optional property has reference in the config, check whether the property is existing.
         If `ValidationHandler` is defined for a training workflow, will check whether the optional properties
         "evaluator" and "val_interval" are existing.
```

## monai/data/wsi_datasets.py

```diff
@@ -56,16 +56,16 @@
 
     Note:
         The input data has the following form as an example:
 
         .. code-block:: python
 
             [
-                {"image": "path/to/image1.tiff", "patch_location": [200, 500], "label": 0},
-                {"image": "path/to/image2.tiff", "patch_location": [100, 700], "patch_size": [20, 20], "patch_level": 2, "label": 1}
+                {"image": "path/to/image1.tiff", "location": [200, 500], "label": 0},
+                {"image": "path/to/image2.tiff", "location": [100, 700], "patch_size": [20, 20], "patch_level": 2, "label": 1}
             ]
 
     """
 
     def __init__(
         self,
         data: Sequence,
```

## monai/fl/client/monai_algo.py

```diff
@@ -7,39 +7,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import logging
 import os
+import time
 from collections.abc import Mapping, MutableMapping
 from typing import Any, cast
 
 import torch
 import torch.distributed as dist
 
-import monai
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
 from monai.apps.utils import get_logger
 from monai.auto3dseg import SegSummarizer
-from monai.bundle import DEFAULT_EXP_MGMT_SETTINGS, ConfigComponent, ConfigItem, ConfigParser, ConfigWorkflow
-from monai.engines import SupervisedTrainer, Trainer
+from monai.bundle import BundleWorkflow, ConfigComponent, ConfigItem, ConfigParser, ConfigWorkflow
+from monai.engines import SupervisedEvaluator, SupervisedTrainer, Trainer
 from monai.fl.client import ClientAlgo, ClientAlgoStats
-from monai.fl.utils.constants import (
-    BundleKeys,
-    ExtraItems,
-    FiltersType,
-    FlPhase,
-    FlStatistics,
-    ModelType,
-    RequiredBundleKeys,
-    WeightType,
-)
+from monai.fl.utils.constants import ExtraItems, FiltersType, FlPhase, FlStatistics, ModelType, WeightType
 from monai.fl.utils.exchange_object import ExchangeObject
 from monai.networks.utils import copy_model_state, get_state_dict
 from monai.utils import min_version, require_pkg
 from monai.utils.enums import DataStatsKeys
 
 logger = get_logger(__name__)
 
@@ -66,73 +56,78 @@
 def compute_weight_diff(global_weights, local_var_dict):
     if global_weights is None:
         raise ValueError("Cannot compute weight differences if `global_weights` is None!")
     if local_var_dict is None:
         raise ValueError("Cannot compute weight differences if `local_var_dict` is None!")
     # compute delta model, global model has the primary key set
     weight_diff = {}
+    n_diff = 0
     for name in global_weights:
         if name not in local_var_dict:
             continue
         # returned weight diff will be on the cpu
         weight_diff[name] = local_var_dict[name].cpu() - global_weights[name].cpu()
+        n_diff += 1
         if torch.any(torch.isnan(weight_diff[name])):
             raise ValueError(f"Weights for {name} became NaN...")
+    if n_diff == 0:
+        raise RuntimeError("No weight differences computed!")
     return weight_diff
 
 
-def check_bundle_config(parser):
-    for k in RequiredBundleKeys:
-        if parser.get(k, None) is None:
-            raise KeyError(f"Bundle config misses required key `{k}`")
-
-
-def disable_ckpt_loaders(parser):
-    if BundleKeys.VALIDATE_HANDLERS in parser:
-        for h in parser[BundleKeys.VALIDATE_HANDLERS]:
+def disable_ckpt_loaders(parser: ConfigParser) -> None:
+    if "validate#handlers" in parser:
+        for h in parser["validate#handlers"]:
             if ConfigComponent.is_instantiable(h):
                 if "CheckpointLoader" in h["_target_"]:
                     h["_disabled_"] = True
 
 
 class MonaiAlgoStats(ClientAlgoStats):
     """
     Implementation of ``ClientAlgoStats`` to allow federated learning with MONAI bundle configurations.
 
     Args:
-        bundle_root: path of bundle.
+        bundle_root: directory path of the bundle.
         config_train_filename: bundle training config path relative to bundle_root. Can be a list of files;
-            defaults to "configs/train.json".
+            defaults to "configs/train.json". only useful when `workflow` is None.
         config_filters_filename: filter configuration file. Can be a list of files; defaults to `None`.
+        data_stats_transform_list: transforms to apply for the data stats result.
         histogram_only: whether to only compute histograms. Defaults to False.
+        workflow: the bundle workflow to execute, usually it's training, evaluation or inference.
+            if None, will create an `ConfigWorkflow` internally based on `config_train_filename`.
     """
 
     def __init__(
         self,
         bundle_root: str,
         config_train_filename: str | list | None = "configs/train.json",
         config_filters_filename: str | list | None = None,
-        train_data_key: str | None = BundleKeys.TRAIN_DATA,
-        eval_data_key: str | None = BundleKeys.VALID_DATA,
         data_stats_transform_list: list | None = None,
         histogram_only: bool = False,
+        workflow: BundleWorkflow | None = None,
     ):
         self.logger = logger
         self.bundle_root = bundle_root
         self.config_train_filename = config_train_filename
         self.config_filters_filename = config_filters_filename
-        self.train_data_key = train_data_key
-        self.eval_data_key = eval_data_key
+        self.train_data_key = "train"
+        self.eval_data_key = "eval"
         self.data_stats_transform_list = data_stats_transform_list
         self.histogram_only = histogram_only
+        self.workflow = None
+        if workflow is not None:
+            if not isinstance(workflow, BundleWorkflow):
+                raise ValueError("workflow must be a subclass of BundleWorkflow.")
+            if workflow.get_workflow_type() is None:
+                raise ValueError("workflow doesn't specify the type.")
+            self.workflow = workflow
 
         self.client_name: str | None = None
         self.app_root: str = ""
-        self.train_parser: ConfigParser | None = None
-        self.filter_parser: ConfigParser | None = None
         self.post_statistics_filters: Any = None
         self.phase = FlPhase.IDLE
         self.dataset_root: Any = None
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
@@ -145,43 +140,34 @@
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
         self.logger.info(f"Initializing {self.client_name} ...")
 
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
-
-        # Read bundle config files
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
-        config_train_files = self._add_config_files(self.config_train_filename)
-        config_filter_files = self._add_config_files(self.config_filters_filename)
+        if self.workflow is None:
+            config_train_files = self._add_config_files(self.config_train_filename)
+            self.workflow = ConfigWorkflow(
+                config_file=config_train_files, meta_file=None, logging_file=None, workflow="train"
+            )
+        self.workflow.initialize()
+        self.workflow.bundle_root = self.bundle_root
+        # initialize the workflow as the content changed
+        self.workflow.initialize()
 
-        # Parse
-        self.train_parser = ConfigParser()
-        self.filter_parser = ConfigParser()
-        if len(config_train_files) > 0:
-            self.train_parser.read_config(config_train_files)
-            check_bundle_config(self.train_parser)
+        config_filter_files = self._add_config_files(self.config_filters_filename)
+        filter_parser = ConfigParser()
         if len(config_filter_files) > 0:
-            self.filter_parser.read_config(config_filter_files)
-
-        # override some config items
-        self.train_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-
-        # Get data location
-        self.dataset_root = self.train_parser.get_parsed_content(
-            BundleKeys.DATASET_DIR, default=ConfigItem(None, BundleKeys.DATASET_DIR)
-        )
-
-        # Get filters
-        self.post_statistics_filters = self.filter_parser.get_parsed_content(
-            FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
-        )
-
+            filter_parser.read_config(config_filter_files)
+            # Get filters
+            self.post_statistics_filters = filter_parser.get_parsed_content(
+                FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
+            )
         self.logger.info(f"Initialized {self.client_name}.")
 
     def get_data_stats(self, extra: dict | None = None) -> ExchangeObject:
         """
         Returns summary statistics about the local data.
 
         Args:
@@ -191,49 +177,54 @@
         Returns:
             stats: ExchangeObject with summary statistics.
 
         """
         if extra is None:
             raise ValueError("`extra` has to be set")
 
-        if self.dataset_root:
+        if self.workflow.dataset_dir:  # type: ignore
             self.phase = FlPhase.GET_DATA_STATS
-            self.logger.info(f"Computing statistics on {self.dataset_root}")
+            self.logger.info(f"Computing statistics on {self.workflow.dataset_dir}")  # type: ignore
 
             if FlStatistics.HIST_BINS not in extra:
                 raise ValueError("FlStatistics.NUM_OF_BINS not specified in `extra`")
             else:
                 hist_bins = extra[FlStatistics.HIST_BINS]
             if FlStatistics.HIST_RANGE not in extra:
                 raise ValueError("FlStatistics.HIST_RANGE not specified in `extra`")
             else:
                 hist_range = extra[FlStatistics.HIST_RANGE]
 
             stats_dict = {}
 
             # train data stats
             train_summary_stats, train_case_stats = self._get_data_key_stats(
-                parser=self.train_parser,
+                data=self.workflow.train_dataset_data,  # type: ignore
                 data_key=self.train_data_key,
                 hist_bins=hist_bins,
                 hist_range=hist_range,
                 output_path=os.path.join(self.app_root, "train_data_stats.yaml"),
             )
             if train_case_stats:
                 # Only return summary statistics to FL server
                 stats_dict.update({self.train_data_key: train_summary_stats})
 
             # eval data stats
-            eval_summary_stats, eval_case_stats = self._get_data_key_stats(
-                parser=self.train_parser,
-                data_key=self.eval_data_key,
-                hist_bins=hist_bins,
-                hist_range=hist_range,
-                output_path=os.path.join(self.app_root, "eval_data_stats.yaml"),
-            )
+            eval_summary_stats = None
+            eval_case_stats = None
+            if self.workflow.val_dataset_data is not None:  # type: ignore
+                eval_summary_stats, eval_case_stats = self._get_data_key_stats(
+                    data=self.workflow.val_dataset_data,  # type: ignore
+                    data_key=self.eval_data_key,
+                    hist_bins=hist_bins,
+                    hist_range=hist_range,
+                    output_path=os.path.join(self.app_root, "eval_data_stats.yaml"),
+                )
+            else:
+                self.logger.warning("the datalist doesn't contain validation section.")
             if eval_summary_stats:
                 # Only return summary statistics to FL server
                 stats_dict.update({self.eval_data_key: eval_summary_stats})
 
             # total stats
             if train_case_stats and eval_case_stats:
                 # Compute total summary
@@ -248,25 +239,18 @@
                 for _filter in self.post_statistics_filters:
                     stats = _filter(stats, extra)
 
             return stats
         else:
             raise ValueError("data_root not set!")
 
-    def _get_data_key_stats(self, parser, data_key, hist_bins, hist_range, output_path=None):
-        if data_key not in parser:
-            self.logger.warning(f"Data key {data_key} not available in bundle configs.")
-            return None, None
-        data = parser.get_parsed_content(data_key)
-
-        datalist = {data_key: data}
-
+    def _get_data_key_stats(self, data, data_key, hist_bins, hist_range, output_path=None):
         analyzer = DataAnalyzer(
-            datalist=datalist,
-            dataroot=self.dataset_root,
+            datalist={data_key: data},
+            dataroot=self.workflow.dataset_dir,  # type: ignore
             hist_bins=hist_bins,
             hist_range=hist_range,
             output_path=output_path,
             histogram_only=self.histogram_only,
         )
 
         self.logger.info(f"{self.client_name} compute data statistics on {data_key}...")
@@ -321,227 +305,205 @@
         return files
 
 
 @require_pkg(pkg_name="ignite", version="0.4.10", version_checker=min_version)
 class MonaiAlgo(ClientAlgo, MonaiAlgoStats):
     """
     Implementation of ``ClientAlgo`` to allow federated learning with MONAI bundle configurations.
-    FIXME: reimplement this class based on the bundle "ConfigWorkflow".
 
     Args:
-        bundle_root: path of bundle.
+        bundle_root: directory path of the bundle.
         local_epochs: number of local epochs to execute during each round of local training; defaults to 1.
         send_weight_diff: whether to send weight differences rather than full weights; defaults to `True`.
-        config_train_filename: bundle training config path relative to bundle_root. Can be a list of files;
-            defaults to "configs/train.json".
-        config_evaluate_filename: bundle evaluation config path relative to bundle_root. Can be a list of files.
-            If "default", config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"] will be used;
+        config_train_filename: bundle training config path relative to bundle_root. can be a list of files.
+            defaults to "configs/train.json". only useful when `train_workflow` is None.
+        train_kwargs: other args of the `ConfigWorkflow` of train, except for `config_file`, `meta_file`,
+            `logging_file`, `workflow`. only useful when `train_workflow` is None.
+        config_evaluate_filename: bundle evaluation config path relative to bundle_root. can be a list of files.
+            if "default", ["configs/train.json", "configs/evaluate.json"] will be used.
+            this arg is only useful when `eval_workflow` is None.
+        eval_kwargs: other args of the `ConfigWorkflow` of evaluation, except for `config_file`, `meta_file`,
+            `logging_file`, `workflow`. only useful when `eval_workflow` is None.
         config_filters_filename: filter configuration file. Can be a list of files; defaults to `None`.
         disable_ckpt_loading: do not use any CheckpointLoader if defined in train/evaluate configs; defaults to `True`.
         best_model_filepath: location of best model checkpoint; defaults "models/model.pt" relative to `bundle_root`.
         final_model_filepath: location of final model checkpoint; defaults "models/model_final.pt" relative to `bundle_root`.
         save_dict_key: If a model checkpoint contains several state dicts,
             the one defined by `save_dict_key` will be returned by `get_weights`; defaults to "model".
             If all state dicts should be returned, set `save_dict_key` to None.
-        seed: set random seed for modules to enable or disable deterministic training; defaults to `None`,
-            i.e., non-deterministic training.
-        benchmark: set benchmark to `False` for full deterministic behavior in cuDNN components.
-            Note, full determinism in federated learning depends also on deterministic behavior of other FL components,
-            e.g., the aggregator, which is not controlled by this class.
-        multi_gpu: whether to run MonaiAlgo in a multi-GPU setting; defaults to `False`.
-        backend: backend to use for torch.distributed; defaults to "nccl".
-        init_method: init_method for torch.distributed; defaults to "env://".
-        tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
-            if "mlflow", will add `MLFlowHandler` to the parsed bundle with default tracking settings,
-            if other string, treat it as file path to load the tracking settings.
-            if `dict`, treat it as tracking settings.
-            will patch the target config content with `tracking handlers` and the top-level items of `configs`.
-            for detailed usage examples, plesae check the tutorial:
-            https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
+        data_stats_transform_list: transforms to apply for the data stats result.
+        eval_workflow_name: the workflow name corresponding to the "config_evaluate_filename", default to "train"
+            as the default "config_evaluate_filename" overrides the train workflow config.
+            this arg is only useful when `eval_workflow` is None.
+        train_workflow: the bundle workflow to execute training, if None, will create a `ConfigWorkflow` internally
+            based on `config_train_filename` and `train_kwargs`.
+        eval_workflow: the bundle workflow to execute evaluation, if None, will create a `ConfigWorkflow` internally
+            based on `config_evaluate_filename`, `eval_kwargs`, `eval_workflow_name`.
 
     """
 
     def __init__(
         self,
         bundle_root: str,
         local_epochs: int = 1,
         send_weight_diff: bool = True,
         config_train_filename: str | list | None = "configs/train.json",
+        train_kwargs: dict | None = None,
         config_evaluate_filename: str | list | None = "default",
+        eval_kwargs: dict | None = None,
         config_filters_filename: str | list | None = None,
         disable_ckpt_loading: bool = True,
         best_model_filepath: str | None = "models/model.pt",
         final_model_filepath: str | None = "models/model_final.pt",
         save_dict_key: str | None = "model",
-        seed: int | None = None,
-        benchmark: bool = True,
-        multi_gpu: bool = False,
-        backend: str = "nccl",
-        init_method: str = "env://",
-        train_data_key: str | None = BundleKeys.TRAIN_DATA,
-        eval_data_key: str | None = BundleKeys.VALID_DATA,
         data_stats_transform_list: list | None = None,
-        tracking: str | dict | None = None,
+        eval_workflow_name: str = "train",
+        train_workflow: BundleWorkflow | None = None,
+        eval_workflow: BundleWorkflow | None = None,
     ):
         self.logger = logger
-        if config_evaluate_filename == "default":
-            # by default, evaluator needs both training and evaluate to be instantiated.
-            config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"]
         self.bundle_root = bundle_root
         self.local_epochs = local_epochs
         self.send_weight_diff = send_weight_diff
         self.config_train_filename = config_train_filename
+        self.train_kwargs = {} if train_kwargs is None else train_kwargs
+        if config_evaluate_filename == "default":
+            # by default, evaluator needs both training and evaluate to be instantiated
+            config_evaluate_filename = ["configs/train.json", "configs/evaluate.json"]
         self.config_evaluate_filename = config_evaluate_filename
+        self.eval_kwargs = {} if eval_kwargs is None else eval_kwargs
         self.config_filters_filename = config_filters_filename
         self.disable_ckpt_loading = disable_ckpt_loading
         self.model_filepaths = {ModelType.BEST_MODEL: best_model_filepath, ModelType.FINAL_MODEL: final_model_filepath}
         self.save_dict_key = save_dict_key
-        self.seed = seed
-        self.benchmark = benchmark
-        self.multi_gpu = multi_gpu
-        self.backend = backend
-        self.init_method = init_method
-        self.train_data_key = train_data_key
-        self.eval_data_key = eval_data_key
         self.data_stats_transform_list = data_stats_transform_list
-        self.tracking = tracking
+        self.eval_workflow_name = eval_workflow_name
+        self.train_workflow = None
+        self.eval_workflow = None
+        if train_workflow is not None:
+            if not isinstance(train_workflow, BundleWorkflow) or train_workflow.get_workflow_type() != "train":
+                raise ValueError(
+                    f"train workflow must be BundleWorkflow and set type in {BundleWorkflow.supported_train_type}."
+                )
+            self.train_workflow = train_workflow
+        if eval_workflow is not None:
+            # evaluation workflow can be "train" type or "infer" type
+            if not isinstance(eval_workflow, BundleWorkflow) or eval_workflow.get_workflow_type() is None:
+                raise ValueError("train workflow must be BundleWorkflow and set type.")
+            self.eval_workflow = eval_workflow
 
         self.app_root = ""
-        self.train_parser: ConfigParser | None = None
-        self.eval_parser: ConfigParser | None = None
         self.filter_parser: ConfigParser | None = None
         self.trainer: SupervisedTrainer | None = None
-        self.evaluator: Any | None = None
+        self.evaluator: SupervisedEvaluator | None = None
         self.pre_filters = None
         self.post_weight_filters = None
         self.post_evaluate_filters = None
         self.iter_of_start_time = 0
         self.global_weights: Mapping | None = None
-        self.rank = 0
 
         self.phase = FlPhase.IDLE
         self.client_name = None
         self.dataset_root = None
 
     def initialize(self, extra=None):
         """
         Initialize routine to parse configuration files and extract main components such as trainer, evaluator, and filters.
 
         Args:
             extra: Dict with additional information that should be provided by FL system,
                 i.e., `ExtraItems.CLIENT_NAME` and `ExtraItems.APP_ROOT`.
 
         """
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         self.client_name = extra.get(ExtraItems.CLIENT_NAME, "noname")
+        timestamp = time.strftime("%Y%m%d_%H%M%S")
         self.logger.info(f"Initializing {self.client_name} ...")
-
-        if self.multi_gpu:
-            dist.init_process_group(backend=self.backend, init_method=self.init_method)
-            self._set_cuda_device()
-            self.logger.info(
-                f"Using multi-gpu training on rank {self.rank} (available devices: {torch.cuda.device_count()})"
-            )
-            if self.rank > 0:
-                self.logger.setLevel(logging.WARNING)
-
-        if self.seed:
-            monai.utils.set_determinism(seed=self.seed)
-        torch.backends.cudnn.benchmark = self.benchmark
-
         # FL platform needs to provide filepath to configuration files
         self.app_root = extra.get(ExtraItems.APP_ROOT, "")
-
-        # Read bundle config files
         self.bundle_root = os.path.join(self.app_root, self.bundle_root)
 
-        config_train_files = self._add_config_files(self.config_train_filename)
-        config_eval_files = self._add_config_files(self.config_evaluate_filename)
-        config_filter_files = self._add_config_files(self.config_filters_filename)
+        if self.train_workflow is None and self.config_train_filename is not None:
+            config_train_files = self._add_config_files(self.config_train_filename)
+            # if enabled experiment tracking, set the run name to the FL client name and timestamp,
+            # expect the tracking settings use "run_name" to define the run name
+            if "run_name" not in self.train_kwargs:
+                self.train_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
+            self.train_workflow = ConfigWorkflow(
+                config_file=config_train_files, meta_file=None, logging_file=None, workflow="train", **self.train_kwargs
+            )
+        if self.train_workflow is not None:
+            self.train_workflow.initialize()
+            self.train_workflow.bundle_root = self.bundle_root
+            self.train_workflow.max_epochs = self.local_epochs
+            if self.disable_ckpt_loading and isinstance(self.train_workflow, ConfigWorkflow):
+                disable_ckpt_loaders(parser=self.train_workflow.parser)
+            # initialize the workflow as the content changed
+            self.train_workflow.initialize()
+            self.trainer = self.train_workflow.trainer
+            if not isinstance(self.trainer, SupervisedTrainer):
+                raise ValueError(f"trainer must be SupervisedTrainer, but got: {type(self.trainer)}.")
+
+        if self.eval_workflow is None and self.config_evaluate_filename is not None:
+            config_eval_files = self._add_config_files(self.config_evaluate_filename)
+            # if enabled experiment tracking, set the run name to the FL client name and timestamp,
+            # expect the tracking settings use "run_name" to define the run name
+            if "run_name" not in self.eval_kwargs:
+                self.eval_kwargs["run_name"] = f"{self.client_name}_{timestamp}"
+            self.eval_workflow = ConfigWorkflow(
+                config_file=config_eval_files,
+                meta_file=None,
+                logging_file=None,
+                workflow=self.eval_workflow_name,
+                **self.eval_kwargs,
+            )
+        if self.eval_workflow is not None:
+            self.eval_workflow.initialize()
+            self.eval_workflow.bundle_root = self.bundle_root
+            if self.disable_ckpt_loading and isinstance(self.eval_workflow, ConfigWorkflow):
+                disable_ckpt_loaders(parser=self.eval_workflow.parser)
+            # initialize the workflow as the content changed
+            self.eval_workflow.initialize()
+            self.evaluator = self.eval_workflow.evaluator
+            if not isinstance(self.evaluator, SupervisedEvaluator):
+                raise ValueError(f"evaluator must be SupervisedEvaluator, but got: {type(self.evaluator)}.")
 
-        # Parse
-        self.train_parser = ConfigParser()
-        self.eval_parser = ConfigParser()
+        config_filter_files = self._add_config_files(self.config_filters_filename)
         self.filter_parser = ConfigParser()
-        if len(config_train_files) > 0:
-            self.train_parser.read_config(config_train_files)
-            check_bundle_config(self.train_parser)
-        if len(config_eval_files) > 0:
-            self.eval_parser.read_config(config_eval_files)
-            check_bundle_config(self.eval_parser)
         if len(config_filter_files) > 0:
             self.filter_parser.read_config(config_filter_files)
 
-        # override some config items
-        self.train_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-        self.eval_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
-        # number of training epochs for each round
-        if BundleKeys.TRAIN_TRAINER_MAX_EPOCHS in self.train_parser:
-            self.train_parser[BundleKeys.TRAIN_TRAINER_MAX_EPOCHS] = self.local_epochs
-
-        # remove checkpoint loaders
-        if self.disable_ckpt_loading:
-            disable_ckpt_loaders(self.train_parser)
-            disable_ckpt_loaders(self.eval_parser)
-
-        # set tracking configs for experiment management
-        if self.tracking is not None:
-            if isinstance(self.tracking, str) and self.tracking in DEFAULT_EXP_MGMT_SETTINGS:
-                settings_ = DEFAULT_EXP_MGMT_SETTINGS[self.tracking]
-            else:
-                settings_ = ConfigParser.load_config_files(self.tracking)
-            ConfigWorkflow.patch_bundle_tracking(parser=self.train_parser, settings=settings_)
-            ConfigWorkflow.patch_bundle_tracking(parser=self.eval_parser, settings=settings_)
-
-        # Get trainer, evaluator
-        self.trainer = self.train_parser.get_parsed_content(
-            BundleKeys.TRAINER, default=ConfigItem(None, BundleKeys.TRAINER)
-        )
-        self.evaluator = self.eval_parser.get_parsed_content(
-            BundleKeys.EVALUATOR, default=ConfigItem(None, BundleKeys.EVALUATOR)
-        )
-
         # Get filters
         self.pre_filters = self.filter_parser.get_parsed_content(
             FiltersType.PRE_FILTERS, default=ConfigItem(None, FiltersType.PRE_FILTERS)
         )
         self.post_weight_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_WEIGHT_FILTERS, default=ConfigItem(None, FiltersType.POST_WEIGHT_FILTERS)
         )
         self.post_evaluate_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_EVALUATE_FILTERS, default=ConfigItem(None, FiltersType.POST_EVALUATE_FILTERS)
         )
         self.post_statistics_filters = self.filter_parser.get_parsed_content(
             FiltersType.POST_STATISTICS_FILTERS, default=ConfigItem(None, FiltersType.POST_STATISTICS_FILTERS)
         )
-
-        # Get data location
-        self.dataset_root = self.train_parser.get_parsed_content(
-            BundleKeys.DATASET_DIR, default=ConfigItem(None, BundleKeys.DATASET_DIR)
-        )
-
-        if self.multi_gpu:
-            if self.rank > 0 and self.trainer:
-                self.trainer.logger.setLevel(logging.WARNING)
-            if self.rank > 0 and self.evaluator:
-                self.evaluator.logger.setLevel(logging.WARNING)
         self.logger.info(f"Initialized {self.client_name}.")
 
     def train(self, data: ExchangeObject, extra: dict | None = None) -> None:
         """
         Train on client's local data.
 
         Args:
             data: `ExchangeObject` containing the current global model weights.
             extra: Dict with additional information that can be provided by the FL system.
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         if not isinstance(data, ExchangeObject):
             raise ValueError(f"expected data to be ExchangeObject but received {type(data)}")
 
         if self.trainer is None:
             raise ValueError("self.trainer should not be None.")
@@ -575,16 +537,16 @@
             extra: Dict with additional information that can be provided by the FL system.
 
         Returns:
             return_weights: `ExchangeObject` containing current weights (default)
                 or load requested model type from disk (`ModelType.BEST_MODEL` or `ModelType.FINAL_MODEL`).
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
 
         # by default return current weights, return best if requested via model type.
         self.phase = FlPhase.GET_WEIGHTS
 
         if ExtraItems.MODEL_TYPE in extra:
@@ -654,16 +616,16 @@
             data: `ExchangeObject` containing the current global model weights.
             extra: Dict with additional information that can be provided by the FL system.
 
         Returns:
             return_metrics: `ExchangeObject` containing evaluation metrics.
 
         """
-        self._set_cuda_device()
 
+        self._set_cuda_device()
         if extra is None:
             extra = {}
         if not isinstance(data, ExchangeObject):
             raise ValueError(f"expected data to be ExchangeObject but received {type(data)}")
 
         if self.evaluator is None:
             raise ValueError("self.evaluator should not be None.")
@@ -717,25 +679,26 @@
         self.logger.info(f"Terminating {self.client_name} during {self.phase} phase.")
         if isinstance(self.trainer, Trainer):
             self.logger.info(f"Terminating {self.client_name} trainer...")
             self.trainer.terminate()
         if isinstance(self.evaluator, Trainer):
             self.logger.info(f"Terminating {self.client_name} evaluator...")
             self.evaluator.terminate()
-
-        if self.multi_gpu:
-            dist.destroy_process_group()
+        if self.train_workflow is not None:
+            self.train_workflow.finalize()
+        if self.eval_workflow is not None:
+            self.eval_workflow.finalize()
 
     def _check_converted(self, global_weights, local_var_dict, n_converted):
         if n_converted == 0:
-            self.logger.warning(
+            raise RuntimeError(
                 f"No global weights converted! Received weight dict keys are {list(global_weights.keys())}"
             )
         else:
             self.logger.info(
                 f"Converted {n_converted} global variables to match {len(local_var_dict)} local variables."
             )
 
     def _set_cuda_device(self):
-        if self.multi_gpu:
+        if dist.is_initialized():
             self.rank = int(os.environ["LOCAL_RANK"])
             torch.cuda.set_device(self.rank)
```

## monai/fl/utils/constants.py

```diff
@@ -47,26 +47,12 @@
     DATA_STATS = "data_stats"
     DATA_COUNT = "data_count"
     FAIL_COUNT = "fail_count"
     TOTAL_DATA = "total_data"
     FEATURE_NAMES = "feature_names"
 
 
-class RequiredBundleKeys(StrEnum):
-    BUNDLE_ROOT = "bundle_root"
-
-
-class BundleKeys(StrEnum):
-    TRAINER = "train#trainer"
-    EVALUATOR = "validate#evaluator"
-    TRAIN_TRAINER_MAX_EPOCHS = "train#trainer#max_epochs"
-    VALIDATE_HANDLERS = "validate#handlers"
-    DATASET_DIR = "dataset_dir"
-    TRAIN_DATA = "train#dataset#data"
-    VALID_DATA = "validate#dataset#data"
-
-
 class FiltersType(StrEnum):
     PRE_FILTERS = "pre_filters"
     POST_WEIGHT_FILTERS = "post_weight_filters"
     POST_EVALUATE_FILTERS = "post_evaluate_filters"
     POST_STATISTICS_FILTERS = "post_statistics_filters"
```

## monai/fl/utils/filters.py

```diff
@@ -34,15 +34,15 @@
         """
 
         raise NotImplementedError
 
 
 class SummaryFilter(Filter):
     """
-    Summary filter to content of ExchangeObject.
+    Summary filter to show content of ExchangeObject.
     """
 
     def __call__(self, data: ExchangeObject, extra: dict | None = None) -> ExchangeObject:
         """
         Example filter that doesn't filter anything but only prints data summary.
 
         Arguments:
```

## monai/handlers/mean_dice.py

```diff
@@ -23,32 +23,36 @@
     Computes Dice score metric from full size Tensor and collects average over batch, class-channels, iterations.
     """
 
     def __init__(
         self,
         include_background: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN,
+        num_classes: int | None = None,
         output_transform: Callable = lambda x: x,
         save_details: bool = True,
     ) -> None:
         """
 
         Args:
             include_background: whether to include dice computation on the first channel of the predicted output.
                 Defaults to True.
             reduction: define the mode to reduce metrics, will only execute reduction on `not-nan` values,
                 available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
                 ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction.
+            num_classes: number of input channels (always including the background). When this is None,
+                ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+                single-channel class indices and the number of classes is not automatically inferred from data.
             output_transform: callable to extract `y_pred` and `y` from `ignite.engine.state.output` then
                 construct `(y_pred, y)` pair, where `y_pred` and `y` can be `batch-first` Tensors or
                 lists of `channel-first` Tensors. the form of `(y_pred, y)` is required by the `update()`.
                 `engine.state` and `output_transform` inherit from the ignite concept:
                 https://pytorch.org/ignite/concepts.html#state, explanation and usage example are in the tutorial:
                 https://github.com/Project-MONAI/tutorials/blob/master/modules/batch_output_transform.ipynb.
             save_details: whether to save metric computation details per image, for example: mean dice of every image.
                 default to True, will save to `engine.state.metric_details` dict with the metric name as key.
 
         See also:
             :py:meth:`monai.metrics.meandice.compute_dice`
         """
-        metric_fn = DiceMetric(include_background=include_background, reduction=reduction)
+        metric_fn = DiceMetric(include_background=include_background, reduction=reduction, num_classes=num_classes)
         super().__init__(metric_fn=metric_fn, output_transform=output_transform, save_details=save_details)
```

## monai/inferers/__init__.py

```diff
@@ -7,11 +7,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .inferer import Inferer, PatchInferer, SaliencyInferer, SimpleInferer, SliceInferer, SlidingWindowInferer
+from .inferer import (
+    Inferer,
+    PatchInferer,
+    SaliencyInferer,
+    SimpleInferer,
+    SliceInferer,
+    SlidingWindowInferer,
+    SlidingWindowInfererAdapt,
+)
 from .merger import AvgMerger, Merger
 from .splitter import SlidingWindowSplitter, Splitter
 from .utils import sliding_window_inference
```

## monai/inferers/inferer.py

```diff
@@ -16,22 +16,33 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from pydoc import locate
 from typing import Any
 
 import torch
 import torch.nn as nn
 
+from monai.apps.utils import get_logger
 from monai.data.meta_tensor import MetaTensor
 from monai.inferers.merger import AvgMerger, Merger
 from monai.inferers.splitter import Splitter
 from monai.inferers.utils import compute_importance_map, sliding_window_inference
 from monai.utils import BlendMode, PatchKeys, PytorchPadMode, ensure_tuple, optional_import
 from monai.visualize import CAM, GradCAM, GradCAMpp
 
-__all__ = ["Inferer", "PatchInferer", "SimpleInferer", "SlidingWindowInferer", "SaliencyInferer", "SliceInferer"]
+logger = get_logger(__name__)
+
+__all__ = [
+    "Inferer",
+    "PatchInferer",
+    "SimpleInferer",
+    "SlidingWindowInferer",
+    "SaliencyInferer",
+    "SliceInferer",
+    "SlidingWindowInfererAdapt",
+]
 
 
 class Inferer(ABC):
     """
     A base class for model inference.
     Extend this class to support operations during inference, e.g. a sliding window method.
 
@@ -444,15 +455,17 @@
             network: target model to execute inference.
                 supports callables such as ``lambda x: my_torch_model(x, additional_config)``
             args: optional args to be passed to ``network``.
             kwargs: optional keyword args to be passed to ``network``.
 
         """
 
-        device = self.device
+        device = kwargs.pop("device", self.device)
+        buffer_steps = kwargs.pop("buffer_steps", self.buffer_steps)
+
         if device is None and self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh:
             device = "cpu"  # stitch in cpu memory if image is too large
 
         return sliding_window_inference(
             inputs,
             self.roi_size,
             self.sw_batch_size,
@@ -463,21 +476,104 @@
             self.padding_mode,
             self.cval,
             self.sw_device,
             device,
             self.progress,
             self.roi_weight_map,
             None,
-            self.buffer_steps,
+            buffer_steps,
             self.buffer_dim,
             *args,
             **kwargs,
         )
 
 
+class SlidingWindowInfererAdapt(SlidingWindowInferer):
+    """
+    SlidingWindowInfererAdapt extends SlidingWindowInferer to automatically switch to buffered and then to CPU stitching,
+    when OOM on GPU. It also records a size of such large images to automatically
+    try CPU stitching for the next large image of a similar size.  If the stitching 'device' input parameter is provided,
+    automatic adaptation won't be attempted, please keep the default option device = None for adaptive behavior.
+    Note: the output might be on CPU (even if the input was on GPU), if the GPU memory was not sufficient.
+
+    """
+
+    def __call__(
+        self,
+        inputs: torch.Tensor,
+        network: Callable[..., torch.Tensor | Sequence[torch.Tensor] | dict[Any, torch.Tensor]],
+        *args: Any,
+        **kwargs: Any,
+    ) -> torch.Tensor | tuple[torch.Tensor, ...] | dict[Any, torch.Tensor]:
+        """
+
+        Args:
+            inputs: model input data for inference.
+            network: target model to execute inference.
+                supports callables such as ``lambda x: my_torch_model(x, additional_config)``
+            args: optional args to be passed to ``network``.
+            kwargs: optional keyword args to be passed to ``network``.
+
+        """
+
+        # if device is provided, use without any adaptations
+        if self.device is not None:
+            return super().__call__(inputs, network, *args, **kwargs)
+
+        skip_buffer = self.buffer_steps is not None and self.buffer_steps <= 0
+        cpu_cond = self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh
+        gpu_stitching = inputs.is_cuda and not cpu_cond
+        buffered_stitching = inputs.is_cuda and cpu_cond and not skip_buffer
+        buffer_steps = max(1, self.buffer_steps) if self.buffer_steps is not None else 1
+
+        for _ in range(10):  # at most 10 trials
+            try:
+                return super().__call__(
+                    inputs,
+                    network,
+                    device=inputs.device if gpu_stitching else torch.device("cpu"),
+                    buffer_steps=buffer_steps if buffered_stitching else None,
+                    *args,
+                    **kwargs,
+                )
+            except RuntimeError as e:
+                if not gpu_stitching and not buffered_stitching or "OutOfMemoryError" not in str(type(e).__name__):
+                    raise e
+
+                logger.info(e)
+
+                if gpu_stitching:  # if failed on gpu
+                    gpu_stitching = False
+                    self.cpu_thresh = inputs.shape[2:].numel() - 1  # update thresh
+
+                    if skip_buffer:
+                        buffered_stitching = False
+                        logger.warning(f"GPU stitching failed, attempting on CPU, image dim {inputs.shape}..")
+
+                    else:
+                        buffered_stitching = True
+                        self.buffer_steps = buffer_steps
+                        logger.warning(
+                            f"GPU stitching failed, attempting with buffer {buffer_steps}, image dim {inputs.shape}.."
+                        )
+                elif buffer_steps > 1:
+                    buffer_steps = max(1, buffer_steps // 2)
+                    self.buffer_steps = buffer_steps
+                    logger.warning(
+                        f"GPU buffered stitching failed, image dim {inputs.shape} reducing buffer to {buffer_steps}"
+                    )
+                else:
+                    buffered_stitching = False
+                    self.buffer_steps = 0  # disable future buffer attempts
+                    logger.warning(f"GPU buffered stitching failed, attempting on CPU, image dim {inputs.shape}")
+        raise RuntimeError(  # not possible to finish after the trials
+            f"SlidingWindowInfererAdapt {skip_buffer} {cpu_cond} {gpu_stitching} {buffered_stitching} {buffer_steps}"
+        )
+
+
 class SaliencyInferer(Inferer):
     """
     SaliencyInferer is inference with activation maps.
 
     Args:
         cam_name: expected CAM method name, should be: "CAM", "GradCAM" or "GradCAMpp".
         target_layers: name of the model layer to generate the feature map.
```

## monai/inferers/utils.py

```diff
@@ -276,15 +276,15 @@
                 if non_blocking:
                     output_image_list[0][o_slice].copy_(sw_device_buffer[0], non_blocking=non_blocking)
                 else:
                     output_image_list[0][o_slice] += sw_device_buffer[0].to(device=device)
             else:
                 sw_device_buffer[ss] *= w_t
                 sw_device_buffer[ss] = sw_device_buffer[ss].to(device)
-                _compute_coords(sw_batch_size, unravel_slice, z_scale, output_image_list[ss], sw_device_buffer[ss])
+                _compute_coords(unravel_slice, z_scale, output_image_list[ss], sw_device_buffer[ss])
         sw_device_buffer = []
         if buffered:
             b_s += 1
 
     if non_blocking:
         torch.cuda.current_stream().synchronize()
 
@@ -338,15 +338,15 @@
         s_s = slices_np[windows_range[_s - 1].stop % len(slices) if _s > 0 else 0, 0]
         s_e = slices_np[(_r.stop - 1) % len(slices), 1]
         b_slices.append((_r.stop, s_s, s_e))  # buffer index, slice start, slice end
     windows_range = itertools.chain(*windows_range)  # type: ignore
     return slices, n_per_batch, b_slices, windows_range
 
 
-def _compute_coords(sw, coords, z_scale, out, patch):
+def _compute_coords(coords, z_scale, out, patch):
     """sliding window batch spatial scaling indexing for multi-resolution outputs."""
     for original_idx, p in zip(coords, patch):
         idx_zm = list(original_idx)  # 4D for 2D image, 5D for 3D image
         if z_scale:
             for axis in range(2, len(idx_zm)):
                 idx_zm[axis] = slice(
                     int(original_idx[axis].start * z_scale[axis - 2]), int(original_idx[axis].stop * z_scale[axis - 2])
```

## monai/losses/ssim_loss.py

```diff
@@ -7,98 +7,119 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from collections.abc import Sequence
+
 import torch
 from torch.nn.modules.loss import _Loss
 
-from monai.metrics.regression import SSIMMetric
+from monai.metrics.regression import KernelType, SSIMMetric
+from monai.utils import LossReduction, ensure_tuple_rep
 
 
 class SSIMLoss(_Loss):
     """
-    Build a Pytorch version of the SSIM loss function based on the original formula of SSIM
-
-    Modified and adopted from:
-        https://github.com/facebookresearch/fastMRI/blob/main/banding_removal/fastmri/ssim_loss_mixin.py
+    Compute the loss function based on the Structural Similarity Index Measure (SSIM) Metric.
 
     For more info, visit
         https://vicuesoft.com/glossary/term/ssim-ms-ssim/
 
     SSIM reference paper:
         Wang, Zhou, et al. "Image quality assessment: from error visibility to structural
         similarity." IEEE transactions on image processing 13.4 (2004): 600-612.
     """
 
-    def __init__(self, win_size: int = 7, k1: float = 0.01, k2: float = 0.03, spatial_dims: int = 2):
+    def __init__(
+        self,
+        spatial_dims: int,
+        data_range: float = 1.0,
+        kernel_type: KernelType | str = KernelType.GAUSSIAN,
+        win_size: int | Sequence[int] = 11,
+        kernel_sigma: float | Sequence[float] = 1.5,
+        k1: float = 0.01,
+        k2: float = 0.03,
+        reduction: LossReduction | str = LossReduction.MEAN,
+    ):
         """
         Args:
-            win_size: gaussian weighting window size
+            spatial_dims: number of spatial dimensions of the input images.
+            data_range: value range of input images. (usually 1.0 or 255)
+            kernel_type: type of kernel, can be "gaussian" or "uniform".
+            win_size: window size of kernel
+            kernel_sigma: standard deviation for Gaussian kernel.
             k1: stability constant used in the luminance denominator
             k2: stability constant used in the contrast denominator
-            spatial_dims: if 2, input shape is expected to be (B,C,H,W). if 3, it is expected to be (B,C,H,W,D)
+            reduction: {``"none"``, ``"mean"``, ``"sum"``}
+                Specifies the reduction to apply to the output. Defaults to ``"mean"``.
+                - ``"none"``: no reduction will be applied.
+                - ``"mean"``: the sum of the output will be divided by the number of elements in the output.
+                - ``"sum"``: the output will be summed.
+
         """
-        super().__init__()
-        self.win_size = win_size
-        self.k1, self.k2 = k1, k2
+        super().__init__(reduction=LossReduction(reduction).value)
         self.spatial_dims = spatial_dims
+        self.data_range = data_range
+        self.kernel_type = kernel_type
 
-    def forward(self, x: torch.Tensor, y: torch.Tensor, data_range: torch.Tensor) -> torch.Tensor:
+        if not isinstance(win_size, Sequence):
+            win_size = ensure_tuple_rep(win_size, spatial_dims)
+        self.kernel_size = win_size
+
+        if not isinstance(kernel_sigma, Sequence):
+            kernel_sigma = ensure_tuple_rep(kernel_sigma, spatial_dims)
+        self.kernel_sigma = kernel_sigma
+
+        self.k1 = k1
+        self.k2 = k2
+
+        self.ssim_metric = SSIMMetric(
+            spatial_dims=self.spatial_dims,
+            data_range=self.data_range,
+            kernel_type=self.kernel_type,
+            win_size=self.kernel_size,
+            kernel_sigma=self.kernel_sigma,
+            k1=self.k1,
+            k2=self.k2,
+        )
+
+    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D and pseudo-3D data,
-                and (B,C,W,H,D) for 3D data,
-            y: second sample (e.g., the reconstructed image). It has similar shape as x.
-            data_range: dynamic range of the data
+            input: batch of predicted images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+            target: batch of target images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
 
         Returns:
-            1-ssim_value (recall this is meant to be a loss function)
+            1 minus the ssim index (recall this is meant to be a loss function)
 
         Example:
             .. code-block:: python
 
                 import torch
 
                 # 2D data
                 x = torch.ones([1,1,10,10])/2
                 y = torch.ones([1,1,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=2)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=2)(x,y))
 
                 # pseudo-3D data
                 x = torch.ones([1,5,10,10])/2  # 5 could represent number of slices
                 y = torch.ones([1,5,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=2)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=2)(x,y))
 
                 # 3D data
                 x = torch.ones([1,1,10,10,10])/2
                 y = torch.ones([1,1,10,10,10])/2
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(1-SSIMLoss(spatial_dims=3)(x,y,data_range))
+                print(1-SSIMLoss(spatial_dims=3)(x,y))
         """
-        if x.shape[0] == 1:
-            ssim_value: torch.Tensor = SSIMMetric(
-                data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-            )._compute_tensor(x, y)
-        elif x.shape[0] > 1:
-            for i in range(x.shape[0]):
-                ssim_val: torch.Tensor = SSIMMetric(
-                    data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-                )._compute_tensor(x[i : i + 1], y[i : i + 1])
-                if i == 0:
-                    ssim_value = ssim_val
-                else:
-                    ssim_value = torch.cat((ssim_value.view(i), ssim_val.view(1)), dim=0)
-
-        else:
-            raise ValueError("Batch size is not nonnegative integer value")
-        # 1- dimensional tensor is only allowed
-        ssim_value = ssim_value.view(-1, 1)
-        loss: torch.Tensor = 1 - ssim_value.mean()
+        ssim_value = self.ssim_metric._compute_tensor(input, target).view(-1, 1)
+        loss: torch.Tensor = 1 - ssim_value
+
+        if self.reduction == LossReduction.MEAN.value:
+            loss = torch.mean(loss)  # the batch average
+        elif self.reduction == LossReduction.SUM.value:
+            loss = torch.sum(loss)  # sum over the batch
+
         return loss
```

## monai/metrics/meandice.py

```diff
@@ -43,35 +43,41 @@
             available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
             ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction.
         get_not_nans: whether to return the `not_nans` count, if True, aggregate() returns (metric, not_nans).
             Here `not_nans` count the number of not nans for the metric, thus its shape equals to the shape of the metric.
         ignore_empty: whether to ignore empty ground truth cases during calculation.
             If `True`, NaN value will be set for empty ground truth cases.
             If `False`, 1 will be set if the predictions of empty ground truth cases are also empty.
+        num_classes: number of input channels (always including the background). When this is None,
+            ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+            single-channel class indices and the number of classes is not automatically inferred from data.
 
     """
 
     def __init__(
         self,
         include_background: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN,
         get_not_nans: bool = False,
         ignore_empty: bool = True,
+        num_classes: int | None = None,
     ) -> None:
         super().__init__()
         self.include_background = include_background
         self.reduction = reduction
         self.get_not_nans = get_not_nans
         self.ignore_empty = ignore_empty
+        self.num_classes = num_classes
         self.dice_helper = DiceHelper(
             include_background=self.include_background,
             reduction=MetricReduction.NONE,
             get_not_nans=False,
             softmax=False,
             ignore_empty=self.ignore_empty,
+            num_classes=self.num_classes,
         )
 
     def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
         """
         Args:
             y_pred: input data to compute, typical segmentation model output.
                 It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
@@ -106,46 +112,53 @@
 
         # do metric reduction
         f, not_nans = do_metric_reduction(data, reduction or self.reduction)
         return (f, not_nans) if self.get_not_nans else f
 
 
 def compute_dice(
-    y_pred: torch.Tensor, y: torch.Tensor, include_background: bool = True, ignore_empty: bool = True
+    y_pred: torch.Tensor,
+    y: torch.Tensor,
+    include_background: bool = True,
+    ignore_empty: bool = True,
+    num_classes: int | None = None,
 ) -> torch.Tensor:
     """Computes Dice score metric for a batch of predictions.
 
     Args:
         y_pred: input data to compute, typical segmentation model output.
-            It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
-            should be binarized.
+            `y_pred` can be single-channel class indices or in the one-hot format.
         y: ground truth to compute mean dice metric. `y` can be single-channel class indices or in the one-hot format.
         include_background: whether to skip Dice computation on the first channel of
             the predicted output. Defaults to True.
         ignore_empty: whether to ignore empty ground truth cases during calculation.
             If `True`, NaN value will be set for empty ground truth cases.
             If `False`, 1 will be set if the predictions of empty ground truth cases are also empty.
+        num_classes: number of input channels (always including the background). When this is None,
+            ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+            single-channel class indices and the number of classes is not automatically inferred from data.
 
     Returns:
         Dice scores per batch and per class, (shape: [batch_size, num_classes]).
 
     """
     return DiceHelper(  # type: ignore
         include_background=include_background,
         reduction=MetricReduction.NONE,
         get_not_nans=False,
         softmax=False,
         ignore_empty=ignore_empty,
+        num_classes=num_classes,
     )(y_pred=y_pred, y=y)
 
 
 class DiceHelper:
     """
     Compute Dice score between two tensors `y_pred` and `y`.
-    `y_pred` must have N channels, `y` can be single-channel class indices or in the one-hot format.
+    `y_pred` and `y` can be single-channel class indices or in the one-hot format.
 
     Example:
 
     .. code-block:: python
 
         import torch
         from monai.metrics import DiceHelper
@@ -166,14 +179,15 @@
         include_background: bool | None = None,
         sigmoid: bool = False,
         softmax: bool | None = None,
         activate: bool = False,
         get_not_nans: bool = True,
         reduction: MetricReduction | str = MetricReduction.MEAN_BATCH,
         ignore_empty: bool = True,
+        num_classes: int | None = None,
     ) -> None:
         """
 
         Args:
             include_background: whether to skip the score on the first channel
                 (default to the value of `sigmoid`, False).
             sigmoid: whether ``y_pred`` are/will be sigmoid activated outputs. If True, thresholding at 0.5
@@ -182,22 +196,26 @@
                 get the discrete prediction. Defaults to the value of ``not sigmoid``.
             activate: whether to apply sigmoid to ``y_pred`` if ``sigmoid`` is True. Defaults to False.
                 This option is only valid when ``sigmoid`` is True.
             get_not_nans: whether to return the number of not-nan values.
             reduction: define mode of reduction to the metrics
             ignore_empty: if `True`, NaN value will be set for empty ground truth cases.
                 If `False`, 1 will be set if the Union of ``y_pred`` and ``y`` is empty.
+            num_classes: number of input channels (always including the background). When this is None,
+                ``y_pred.shape[1]`` will be used. This option is useful when both ``y_pred`` and ``y`` are
+                single-channel class indices and the number of classes is not automatically inferred from data.
         """
         self.sigmoid = sigmoid
         self.reduction = reduction
         self.get_not_nans = get_not_nans
         self.include_background = sigmoid if include_background is None else include_background
         self.softmax = not sigmoid if softmax is None else softmax
         self.activate = activate
         self.ignore_empty = ignore_empty
+        self.num_classes = num_classes
 
     def compute_channel(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """"""
         y_o = torch.sum(y)
         if y_o > 0:
             return (2.0 * torch.sum(torch.masked_select(y, y_pred))) / (y_o + torch.sum(y_pred))
         if self.ignore_empty:
@@ -207,25 +225,31 @@
             return torch.tensor(1.0, device=y_o.device)
         return torch.tensor(0.0, device=y_o.device)
 
     def __call__(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         """
 
         Args:
-            y_pred: input predictions with shape (batch_size, num_classes, spatial_dims...).
-                the number of channels is inferred from ``y_pred.shape[1]``.
+            y_pred: input predictions with shape (batch_size, num_classes or 1, spatial_dims...).
+                the number of channels is inferred from ``y_pred.shape[1]`` when ``num_classes is None``.
             y: ground truth with shape (batch_size, num_classes or 1, spatial_dims...).
         """
-        n_pred_ch = y_pred.shape[1]
+        _softmax, _sigmoid = self.softmax, self.sigmoid
+        if self.num_classes is None:
+            n_pred_ch = y_pred.shape[1]  # y_pred is in one-hot format or multi-channel scores
+        else:
+            n_pred_ch = self.num_classes
+            if y_pred.shape[1] == 1 and self.num_classes > 1:  # y_pred is single-channel class indices
+                _softmax = _sigmoid = False
 
-        if self.softmax:
+        if _softmax:
             if n_pred_ch > 1:
                 y_pred = torch.argmax(y_pred, dim=1, keepdim=True)
 
-        elif self.sigmoid:
+        elif _sigmoid:
             if self.activate:
                 y_pred = torch.sigmoid(y_pred)
             y_pred = y_pred > 0.5
 
         first_ch = 0 if self.include_background else 1
         data = []
         for b in range(y_pred.shape[0]):
```

## monai/metrics/regression.py

```diff
@@ -9,23 +9,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import math
 from abc import abstractmethod
-from collections.abc import Callable
+from collections.abc import Callable, Sequence
 from functools import partial
 from typing import Any
 
 import torch
 import torch.nn.functional as F
 
 from monai.metrics.utils import do_metric_reduction
-from monai.utils import MetricReduction
+from monai.utils import MetricReduction, StrEnum, convert_data_type, ensure_tuple_rep
 from monai.utils.type_conversion import convert_to_dst_type
 
 from .metric import CumulativeIterationMetric
 
 
 class RegressionMetric(CumulativeIterationMetric):
     """
@@ -228,162 +228,216 @@
 def compute_mean_error_metrics(y_pred: torch.Tensor, y: torch.Tensor, func: Callable) -> torch.Tensor:
     # reducing in only channel + spatial dimensions (not batch)
     # reduction of batch handled inside __call__() using do_metric_reduction() in respective calling class
     flt = partial(torch.flatten, start_dim=1)
     return torch.mean(flt(func(y - y_pred)), dim=-1, keepdim=True)
 
 
+class KernelType(StrEnum):
+    GAUSSIAN = "gaussian"
+    UNIFORM = "uniform"
+
+
 class SSIMMetric(RegressionMetric):
     r"""
-    Build a Pytorch version of the SSIM metric based on the original formula of SSIM
+    Computes the Structural Similarity Index Measure (SSIM).
 
     .. math::
         \operatorname {SSIM}(x,y) =\frac {(2 \mu_x \mu_y + c_1)(2 \sigma_{xy} + c_2)}{((\mu_x^2 + \
                 \mu_y^2 + c_1)(\sigma_x^2 + \sigma_y^2 + c_2)}
 
     For more info, visit
         https://vicuesoft.com/glossary/term/ssim-ms-ssim/
 
-    Modified and adopted from:
-        https://github.com/facebookresearch/fastMRI/blob/main/banding_removal/fastmri/ssim_loss_mixin.py
-
     SSIM reference paper:
         Wang, Zhou, et al. "Image quality assessment: from error visibility to structural
         similarity." IEEE transactions on image processing 13.4 (2004): 600-612.
 
     Args:
-        data_range: dynamic range of the data
-        win_size: gaussian weighting window size
+        spatial_dims: number of spatial dimensions of the input images.
+        data_range: value range of input images. (usually 1.0 or 255)
+        kernel_type: type of kernel, can be "gaussian" or "uniform".
+        win_size: window size of kernel
+        kernel_sigma: standard deviation for Gaussian kernel.
         k1: stability constant used in the luminance denominator
         k2: stability constant used in the contrast denominator
-        spatial_dims: if 2, input shape is expected to be (B,C,W,H). if 3, it is expected to be (B,C,W,H,D)
         reduction: define the mode to reduce metrics, will only execute reduction on `not-nan` values,
             available reduction modes: {``"none"``, ``"mean"``, ``"sum"``, ``"mean_batch"``, ``"sum_batch"``,
             ``"mean_channel"``, ``"sum_channel"``}, default to ``"mean"``. if "none", will not do reduction
         get_not_nans: whether to return the `not_nans` count, if True, aggregate() returns (metric, not_nans)
     """
 
     def __init__(
         self,
-        data_range: torch.Tensor,
-        win_size: int = 7,
+        spatial_dims: int,
+        data_range: float = 1.0,
+        kernel_type: KernelType | str = KernelType.GAUSSIAN,
+        win_size: int | Sequence[int] = 11,
+        kernel_sigma: float | Sequence[float] = 1.5,
         k1: float = 0.01,
         k2: float = 0.03,
-        spatial_dims: int = 2,
         reduction: MetricReduction | str = MetricReduction.MEAN,
         get_not_nans: bool = False,
-    ):
+    ) -> None:
         super().__init__(reduction=reduction, get_not_nans=get_not_nans)
-        self.data_range = data_range
-        self.win_size = win_size
-        self.k1, self.k2 = k1, k2
+
         self.spatial_dims = spatial_dims
-        self.cov_norm = (win_size**2) / (win_size**2 - 1)
-        self.w = torch.ones([1, 1] + [win_size for _ in range(spatial_dims)]) / win_size**spatial_dims
+        self.data_range = data_range
+        self.kernel_type = kernel_type
 
-    def _compute_intermediate_statistics(self, x: torch.Tensor, y: torch.Tensor) -> tuple[torch.Tensor, ...]:
-        data_range = self.data_range[(None,) * (self.spatial_dims + 2)]
-        # determine whether to work with 2D convolution or 3D
-        conv = getattr(F, f"conv{self.spatial_dims}d")
-        w = convert_to_dst_type(src=self.w, dst=x)[0]
-
-        c1 = (self.k1 * data_range) ** 2  # stability constant for luminance
-        c2 = (self.k2 * data_range) ** 2  # stability constant for contrast
-        ux = conv(x, w)  # mu_x
-        uy = conv(y, w)  # mu_y
-        uxx = conv(x * x, w)  # mu_x^2
-        uyy = conv(y * y, w)  # mu_y^2
-        uxy = conv(x * y, w)  # mu_xy
-        vx = self.cov_norm * (uxx - ux * ux)  # sigma_x
-        vy = self.cov_norm * (uyy - uy * uy)  # sigma_y
-        vxy = self.cov_norm * (uxy - ux * uy)  # sigma_xy
+        if not isinstance(win_size, Sequence):
+            win_size = ensure_tuple_rep(win_size, spatial_dims)
+        self.kernel_size = win_size
+
+        if not isinstance(kernel_sigma, Sequence):
+            kernel_sigma = ensure_tuple_rep(kernel_sigma, spatial_dims)
+        self.kernel_sigma = kernel_sigma
 
-        return c1, c2, ux, uy, vx, vy, vxy
+        self.k1 = k1
+        self.k2 = k2
 
-    def _compute_metric(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+    def _compute_metric(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """
         Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D data and (B,C,W,H,D) for 3D.
-                A fastMRI sample should use the 2D format with C being the number of slices.
-            y: second sample (e.g., the reconstructed image). It has similar shape as x
-
-        Returns:
-            ssim_value
-
-        Example:
-            .. code-block:: python
-
-                import torch
-                x = torch.ones([1,1,10,10])/2 # ground truth
-                y = torch.ones([1,1,10,10])/2 # prediction
-                data_range = x.max().unsqueeze(0)
-                # the following line should print 1.0 (or 0.9999)
-                print(SSIMMetric(data_range=data_range,spatial_dims=2)._compute_metric(x,y))
+            y_pred: Predicted image.
+                It must be a 2D or 3D batch-first tensor [B,C,H,W] or [B,C,H,W,D].
+            y: Reference image.
+                It must be a 2D or 3D batch-first tensor [B,C,H,W] or [B,C,H,W,D].
+
+        Raises:
+            ValueError: when `y_pred` is not a 2D or 3D image.
         """
-        if x.shape[1] > 1:  # handling multiple channels (C>1)
-            if x.shape[1] != y.shape[1]:
-                raise ValueError(
-                    f"x and y should have the same number of channels, "
-                    f"but x has {x.shape[1]} channels and y has {y.shape[1]} channels."
-                )
-
-            ssim = torch.stack(
-                [
-                    SSIMMetric(self.data_range, self.win_size, self.k1, self.k2, self.spatial_dims)(  # type: ignore[misc]
-                        x[:, i, ...].unsqueeze(1), y[:, i, ...].unsqueeze(1)
-                    )
-                    for i in range(x.shape[1])
-                ]
+        dims = y_pred.ndimension()
+        if self.spatial_dims == 2 and dims != 4:
+            raise ValueError(
+                f"y_pred should have 4 dimensions (batch, channel, height, width) when using {self.spatial_dims} "
+                f"spatial dimensions, got {dims}."
             )
-            channel_wise_ssim = ssim.mean(1).view(-1, 1)
-            return channel_wise_ssim
 
-        c1, c2, ux, uy, vx, vy, vxy = self._compute_intermediate_statistics(x, y)
+        if self.spatial_dims == 3 and dims != 5:
+            raise ValueError(
+                f"y_pred should have 4 dimensions (batch, channel, height, width, depth) when using {self.spatial_dims}"
+                f" spatial dimensions, got {dims}."
+            )
 
-        numerator = (2 * ux * uy + c1) * (2 * vxy + c2)
-        denom = (ux**2 + uy**2 + c1) * (vx + vy + c2)
-        ssim_value = numerator / denom
-        # [B, 1]
-        ssim_per_batch: torch.Tensor = ssim_value.view(ssim_value.shape[1], -1).mean(1, keepdim=True)
+        ssim_value_full_image, _ = compute_ssim_and_cs(
+            y_pred=y_pred,
+            y=y,
+            spatial_dims=self.spatial_dims,
+            data_range=self.data_range,
+            kernel_type=self.kernel_type,
+            kernel_size=self.kernel_size,
+            kernel_sigma=self.kernel_sigma,
+            k1=self.k1,
+            k2=self.k2,
+        )
+
+        ssim_per_batch: torch.Tensor = ssim_value_full_image.view(ssim_value_full_image.shape[0], -1).mean(
+            1, keepdim=True
+        )
 
         return ssim_per_batch
 
-    def _compute_metric_and_contrast(self, x: torch.Tensor, y: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
-        """
-        Args:
-            x: first sample (e.g., the reference image). Its shape is (B,C,W,H) for 2D data and (B,C,W,H,D) for 3D.
-                A fastMRI sample should use the 2D format with C being the number of slices.
-            y: second sample (e.g., the reconstructed image). It has similar shape as x
 
-        Returns:
-            ssim_value, cs_value
+def _gaussian_kernel(
+    spatial_dims: int, num_channels: int, kernel_size: Sequence[int], kernel_sigma: Sequence[float]
+) -> torch.Tensor:
+    """Computes 2D or 3D gaussian kernel.
+
+    Args:
+        spatial_dims: number of spatial dimensions of the input images.
+        num_channels: number of channels in the image
+        kernel_size: size of kernel
+        kernel_sigma: standard deviation for Gaussian kernel.
+    """
+
+    def gaussian_1d(kernel_size: int, sigma: float) -> torch.Tensor:
+        """Computes 1D gaussian kernel.
+
+        Args:
+            kernel_size: size of the gaussian kernel
+            sigma: Standard deviation of the gaussian kernel
         """
-        if x.shape[1] > 1:  # handling multiple channels (C>1)
-            if x.shape[1] != y.shape[1]:
-                raise ValueError(
-                    f"x and y should have the same number of channels, "
-                    f"but x has {x.shape[1]} channels and y has {y.shape[1]} channels."
-                )
-
-            ssim_ls = []
-            cs_ls = []
-            for i in range(x.shape[1]):
-                ssim_val, cs_val = SSIMMetric(
-                    self.data_range, self.win_size, self.k1, self.k2, self.spatial_dims
-                )._compute_metric_and_contrast(x[:, i, ...].unsqueeze(1), y[:, i, ...].unsqueeze(1))
-                ssim_ls.append(ssim_val)
-                cs_ls.append(cs_val)
-            channel_wise_ssim: torch.Tensor = torch.stack(ssim_ls).mean(1).view(-1, 1)
-            channel_wise_cs: torch.Tensor = torch.stack(cs_ls).mean(1).view(-1, 1)
-            return channel_wise_ssim, channel_wise_cs
-
-        c1, c2, ux, uy, vx, vy, vxy = self._compute_intermediate_statistics(x, y)
-
-        numerator = (2 * ux * uy + c1) * (2 * vxy + c2)
-        denom = (ux**2 + uy**2 + c1) * (vx + vy + c2)
-        ssim_value = numerator / denom
-        # [B, 1]
-        ssim_per_batch: torch.Tensor = ssim_value.view(ssim_value.shape[1], -1).mean(1, keepdim=True)
-
-        cs_per_batch: torch.Tensor = (2 * vxy + c2) / (vx + vy + c2)  # contrast sensitivity function
-        cs_per_batch = cs_per_batch.view(cs_per_batch.shape[0], -1).mean(1, keepdim=True)  # [B, 1]
-        return ssim_per_batch, cs_per_batch
+        dist = torch.arange(start=(1 - kernel_size) / 2, end=(1 + kernel_size) / 2, step=1)
+        gauss = torch.exp(-torch.pow(dist / sigma, 2) / 2)
+        return (gauss / gauss.sum()).unsqueeze(dim=0)
+
+    gaussian_kernel_x = gaussian_1d(kernel_size[0], kernel_sigma[0])
+    gaussian_kernel_y = gaussian_1d(kernel_size[1], kernel_sigma[1])
+    kernel = torch.matmul(gaussian_kernel_x.t(), gaussian_kernel_y)  # (kernel_size, 1) * (1, kernel_size)
+
+    kernel_dimensions: tuple[int, ...] = (num_channels, 1, kernel_size[0], kernel_size[1])
+
+    if spatial_dims == 3:
+        gaussian_kernel_z = gaussian_1d(kernel_size[2], kernel_sigma[2])[None,]
+        kernel = torch.mul(
+            kernel.unsqueeze(-1).repeat(1, 1, kernel_size[2]),
+            gaussian_kernel_z.expand(kernel_size[0], kernel_size[1], kernel_size[2]),
+        )
+        kernel_dimensions = (num_channels, 1, kernel_size[0], kernel_size[1], kernel_size[2])
+
+    return kernel.expand(kernel_dimensions)
+
+
+def compute_ssim_and_cs(
+    y_pred: torch.Tensor,
+    y: torch.Tensor,
+    spatial_dims: int,
+    kernel_size: Sequence[int],
+    kernel_sigma: Sequence[float],
+    data_range: float = 1.0,
+    kernel_type: KernelType | str = KernelType.GAUSSIAN,
+    k1: float = 0.01,
+    k2: float = 0.03,
+) -> tuple[torch.Tensor, torch.Tensor]:
+    """
+    Function to compute the Structural Similarity Index Measure (SSIM) and Contrast Sensitivity (CS) for a batch
+    of images.
+
+    Args:
+        y_pred: batch of predicted images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+        y: batch of target images with shape (batch_size, channels, spatial_dim1, spatial_dim2[, spatial_dim3])
+        kernel_size: the size of the kernel to use for the SSIM computation.
+        kernel_sigma: the standard deviation of the kernel to use for the SSIM computation.
+        spatial_dims: number of spatial dimensions of the images (2, 3)
+        data_range: the data range of the images.
+        kernel_type: the type of kernel to use for the SSIM computation. Can be either "gaussian" or "uniform".
+        k1: the first stability constant.
+        k2: the second stability constant.
+
+    Returns:
+        ssim: the Structural Similarity Index Measure score for the batch of images.
+        cs: the Contrast Sensitivity for the batch of images.
+    """
+    if y.shape != y_pred.shape:
+        raise ValueError(f"y_pred and y should have same shapes, got {y_pred.shape} and {y.shape}.")
+
+    y_pred = convert_data_type(y_pred, output_type=torch.Tensor, dtype=torch.float)[0]
+    y = convert_data_type(y, output_type=torch.Tensor, dtype=torch.float)[0]
+
+    num_channels = y_pred.size(1)
+
+    if kernel_type == KernelType.GAUSSIAN:
+        kernel = _gaussian_kernel(spatial_dims, num_channels, kernel_size, kernel_sigma)
+    elif kernel_type == KernelType.UNIFORM:
+        kernel = torch.ones((num_channels, 1, *kernel_size)) / torch.prod(torch.tensor(kernel_size))
+
+    kernel = convert_to_dst_type(src=kernel, dst=y_pred)[0]
+
+    c1 = (k1 * data_range) ** 2  # stability constant for luminance
+    c2 = (k2 * data_range) ** 2  # stability constant for contrast
+
+    conv_fn = getattr(F, f"conv{spatial_dims}d")
+    mu_x = conv_fn(y_pred, kernel, groups=num_channels)
+    mu_y = conv_fn(y, kernel, groups=num_channels)
+    mu_xx = conv_fn(y_pred * y_pred, kernel, groups=num_channels)
+    mu_yy = conv_fn(y * y, kernel, groups=num_channels)
+    mu_xy = conv_fn(y_pred * y, kernel, groups=num_channels)
+
+    sigma_x = mu_xx - mu_x * mu_x
+    sigma_y = mu_yy - mu_y * mu_y
+    sigma_xy = mu_xy - mu_x * mu_y
+
+    contrast_sensitivity = (2 * sigma_xy + c2) / (sigma_x + sigma_y + c2)
+    ssim_value_full_image = ((2 * mu_x * mu_y + c1) / (mu_x**2 + mu_y**2 + c1)) * contrast_sensitivity
+
+    return ssim_value_full_image, contrast_sensitivity
```

## monai/metrics/utils.py

```diff
@@ -305,26 +305,26 @@
     Returns:
         spacing: a sequence with length `batch_size` that includes integers, floats or sequences of length `img_dim`.
     """
     if spacing is None or isinstance(spacing, (int, float)):
         return list([spacing] * batch_size)
     elif isinstance(spacing, (Sequence, np.ndarray)):
         assert all(
-            [isinstance(s, type(spacing[0])) for s in list(spacing)]
+            isinstance(s, type(spacing[0])) for s in list(spacing)
         ), "if `spacing` is a sequence, its elements should be of same type."
 
         if isinstance(spacing[0], (Sequence, np.ndarray)):
             assert (
                 len(spacing) == batch_size
             ), "if `spacing` is a sequence of sequences, the outer sequence should have same length as batch size."
             assert all(
-                [len(s) == img_dim for s in list(spacing)]
+                len(s) == img_dim for s in list(spacing)
             ), "each element of `spacing` list should either have same length as image dim."
             assert all(
-                [isinstance(i, (int, float)) for s in list(spacing) for i in list(s)]
+                isinstance(i, (int, float)) for s in list(spacing) for i in list(s)
             ), "if `spacing` is a sequence of sequences or 2D np.ndarray, the elements should be integers or floats."
             return list(spacing)
         elif isinstance(spacing[0], (int, float)):
             assert (
                 len(spacing) == img_dim
             ), "if `spacing` is a sequence of numbers, it should have same length as image dim."
             return [spacing for _ in range(batch_size)]  # type: ignore
```

## monai/networks/utils.py

```diff
@@ -23,18 +23,18 @@
 from copy import deepcopy
 from typing import Any
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from monai.apps.utils import get_logger, optional_import
+from monai.apps.utils import get_logger
 from monai.config import PathLike
 from monai.utils.misc import ensure_tuple, save_obj, set_determinism
-from monai.utils.module import look_up_option, pytorch_after
+from monai.utils.module import look_up_option, optional_import, pytorch_after
 from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
 
 onnx, _ = optional_import("onnx")
 onnxreference, _ = optional_import("onnx.reference")
 onnxruntime, _ = optional_import("onnxruntime")
 
 __all__ = [
@@ -55,18 +55,41 @@
     "convert_to_trt",
     "meshgrid_ij",
     "meshgrid_xy",
     "replace_modules",
     "replace_modules_temp",
     "look_up_named_module",
     "set_named_module",
+    "has_nvfuser_instance_norm",
 ]
 
 logger = get_logger(module_name=__name__)
 
+_has_nvfuser = None
+
+
+def has_nvfuser_instance_norm():
+    """whether the current environment has InstanceNorm3dNVFuser
+    https://github.com/NVIDIA/apex/blob/23.05-devel/apex/normalization/instance_norm.py#L15-L16
+    """
+    global _has_nvfuser
+    if _has_nvfuser is not None:
+        return _has_nvfuser
+
+    _, _has_nvfuser = optional_import("apex.normalization", name="InstanceNorm3dNVFuser")
+    if not _has_nvfuser:
+        return False
+    try:
+        import importlib
+
+        importlib.import_module("instance_norm_nvfuser_cuda")
+    except ImportError:
+        _has_nvfuser = False
+    return _has_nvfuser
+
 
 def look_up_named_module(name: str, mod, print_all_options=False):
     """
     get the named module in `mod` by the attribute name,
     for example ``look_up_named_module(net, "features.3.1.attn")``
 
     Args:
@@ -886,15 +909,15 @@
 
     if not input_shape:
         raise ValueError("Missing the input shape for model convert.")
 
     if not dynamic_batchsize:
         warnings.warn(f"There is no dynamic batch range. The converted model only takes {input_shape} shape input.")
 
-    if (not (dynamic_batchsize is None)) and (len(dynamic_batchsize) != 3):
+    if (dynamic_batchsize is not None) and (len(dynamic_batchsize) != 3):
         warnings.warn(f"The dynamic batch range sequence should have 3 elements, but got {dynamic_batchsize} elements.")
 
     device = device if device else 0
     target_device = torch.device(f"cuda:{device}") if device else torch.device("cuda:0")
     convert_precision = torch.float32 if precision == "fp32" else torch.half
     inputs = [torch.rand(ensure_tuple(input_shape)).to(target_device)]
```

## monai/networks/blocks/backbone_fpn_utils.py

```diff
@@ -151,15 +151,15 @@
     # select layers that wont be frozen
     if trainable_layers < 0 or trainable_layers > 5:
         raise ValueError(f"Trainable layers should be in the range [0,5], got {trainable_layers}")
     layers_to_train = ["layer4", "layer3", "layer2", "layer1", "conv1"][:trainable_layers]
     if trainable_layers == 5:
         layers_to_train.append("bn1")
     for name, parameter in backbone.named_parameters():
-        if all([not name.startswith(layer) for layer in layers_to_train]):
+        if all(not name.startswith(layer) for layer in layers_to_train):
             parameter.requires_grad_(False)
 
     if extra_blocks is None:
         extra_blocks = LastLevelMaxPool(spatial_dims)
 
     if returned_layers is None:
         returned_layers = [1, 2, 3, 4]
```

## monai/networks/layers/factories.py

```diff
@@ -63,18 +63,17 @@
 
 import warnings
 from collections.abc import Callable
 from typing import Any
 
 import torch.nn as nn
 
+from monai.networks.utils import has_nvfuser_instance_norm
 from monai.utils import look_up_option, optional_import
 
-InstanceNorm3dNVFuser, has_nvfuser = optional_import("apex.normalization", name="InstanceNorm3dNVFuser")
-
 __all__ = ["LayerFactory", "Dropout", "Norm", "Act", "Conv", "Pool", "Pad", "split_args"]
 
 
 class LayerFactory:
     """
     Factory object for creating layers, this uses given factory functions to actually produce the types or constructing
     callables. These functions are referred to by name and can be added at any time.
@@ -263,20 +262,20 @@
     """
 
     if dim != 3:
         types = (nn.InstanceNorm1d, nn.InstanceNorm2d)
         warnings.warn(f"`InstanceNorm3dNVFuser` only supports 3d cases, use {types[dim - 1]} instead.")
         return types[dim - 1]
 
-    if not has_nvfuser:
+    if not has_nvfuser_instance_norm():
         warnings.warn(
             "`apex.normalization.InstanceNorm3dNVFuser` is not installed properly, use nn.InstanceNorm3d instead."
         )
         return nn.InstanceNorm3d
-    return InstanceNorm3dNVFuser
+    return optional_import("apex.normalization", name="InstanceNorm3dNVFuser")[0]
 
 
 Act.add_factory_callable("elu", lambda: nn.modules.ELU)
 Act.add_factory_callable("relu", lambda: nn.modules.ReLU)
 Act.add_factory_callable("leakyrelu", lambda: nn.modules.LeakyReLU)
 Act.add_factory_callable("prelu", lambda: nn.modules.PReLU)
 Act.add_factory_callable("relu6", lambda: nn.modules.ReLU6)
```

## monai/networks/nets/torchvision_fc.py

```diff
@@ -110,16 +110,18 @@
         fc_name: str = "fc",
         node_name: str = "",
         weights=None,
         **kwargs,
     ):
         if weights is not None:
             model = getattr(models, model_name)(weights=weights, **kwargs)
+        elif pretrained:
+            model = getattr(models, model_name)(weights="DEFAULT", **kwargs)
         else:
-            model = getattr(models, model_name)(pretrained=pretrained, **kwargs)  # 'pretrained' deprecated 0.13
+            model = getattr(models, model_name)(weights=None, **kwargs)
 
         super().__init__(
             model=model,
             num_classes=num_classes,
             dim=dim,
             in_channels=in_channels,
             use_conv=use_conv,
```

## monai/optimizers/lr_finder.py

```diff
@@ -253,15 +253,15 @@
     def range_test(
         self,
         train_loader: DataLoader,
         val_loader: DataLoader | None = None,
         image_extractor: Callable = default_image_extractor,
         label_extractor: Callable = default_label_extractor,
         start_lr: float | None = None,
-        end_lr: int = 10,
+        end_lr: float = 10.0,
         num_iter: int = 100,
         step_mode: str = "exp",
         smooth_f: float = 0.05,
         diverge_th: int = 5,
         accumulation_steps: int = 1,
         non_blocking_transfer: bool = True,
         auto_reset: bool = True,
```

## monai/transforms/__init__.py

```diff
@@ -620,14 +620,15 @@
     TransposeD,
     TransposeDict,
 )
 from .utils import (
     Fourier,
     allow_missing_keys_mode,
     attach_hook,
+    check_non_lazy_pending_ops,
     compute_divisible_spatial_size,
     convert_applied_interp_mode,
     convert_pad_mode,
     convert_to_contiguous,
     copypaste_arrays,
     create_control_grid,
     create_grid,
```

## monai/transforms/compose.py

```diff
@@ -370,15 +370,15 @@
             if not isinstance(_transform, Randomizable):
                 continue
             try:
                 _transform.randomize(data)
             except TypeError as type_error:
                 tfm_name: str = type(_transform).__name__
                 warnings.warn(
-                    f'Transform "{tfm_name}" in Compose not randomized\n{tfm_name}.{type_error}.', RuntimeWarning
+                    f"Transform '{tfm_name}' in Compose not randomized\n{tfm_name}.{type_error}.", RuntimeWarning
                 )
 
     def get_index_of_first(self, predicate):
         """
         get_index_of_first takes a ``predicate`` and returns the index of the first transform that
         satisfies the predicate (ie. makes the predicate return True). If it is unable to find
         a transform that satisfies the ``predicate``, it returns None.
@@ -466,14 +466,19 @@
     def inverse(self, data):
         invertible_transforms = [t for t in self.flatten().transforms if isinstance(t, InvertibleTransform)]
         if not invertible_transforms:
             warnings.warn("inverse has been called but no invertible transforms have been supplied")
 
         # loop backwards over transforms
         for t in reversed(invertible_transforms):
+            if isinstance(t, LazyTransform) and t.lazy_evaluation:
+                warnings.warn(
+                    f"inversing {t.__class__.__name__} lazily may not implemented"
+                    "please set `lazy_evaluation=False` before calling inverse."
+                )
             data = apply_transform(t.inverse, data, self.map_items, self.unpack_items, self.log_stats)
         return data
 
 
 class OneOf(Compose):
     """
     ``OneOf`` provides the ability to randomly choose one transform out of a
```

## monai/transforms/inverse.py

```diff
@@ -119,17 +119,18 @@
                 xform = self.pop_transform(data, check=False) if do_transform else {}
                 meta_obj = self.push_transform(data, orig_size=xform.get(TraceKeys.ORIG_SIZE), extra_info=xform)
                 return data.copy_meta_from(meta_obj)
             if do_transform:
                 xform = data.pending_operations.pop()
                 extra = xform.copy()
                 xform.update(transform_info)
-                meta_obj = self.push_transform(data, transform_info=xform, lazy_evaluation=lazy_eval, extra_info=extra)
-                return data.copy_meta_from(meta_obj)
-            return data
+            else:  # lazy, replace=True, do_transform=False
+                xform, extra = transform_info, {}
+            meta_obj = self.push_transform(data, transform_info=xform, lazy_evaluation=True, extra_info=extra)
+            return data.copy_meta_from(meta_obj)
         kwargs["lazy_evaluation"] = lazy_eval
         if "transform_info" in kwargs and isinstance(kwargs["transform_info"], dict):
             kwargs["transform_info"].update(transform_info)
         else:
             kwargs["transform_info"] = transform_info
         meta_obj = TraceableTransform.track_transform_meta(data, *args, **kwargs)
         return data.copy_meta_from(meta_obj) if isinstance(data, MetaTensor) else data
@@ -207,24 +208,34 @@
             extra_info.pop(LazyAttr.AFFINE, None)
             info[TraceKeys.EXTRA_INFO] = extra_info
 
         # push the transform info to the applied_operation or pending_operation stack
         if lazy_evaluation:
             if sp_size is None:
                 if LazyAttr.SHAPE not in info:
-                    warnings.warn("spatial size is None in push transform.")
+                    info[LazyAttr.SHAPE] = info.get(TraceKeys.ORIG_SIZE, [])
             else:
-                info[LazyAttr.SHAPE] = tuple(convert_to_numpy(sp_size, wrap_sequence=True).tolist())
+                info[LazyAttr.SHAPE] = sp_size
+            info[LazyAttr.SHAPE] = tuple(convert_to_numpy(info[LazyAttr.SHAPE], wrap_sequence=True).tolist())
             if affine is None:
                 if LazyAttr.AFFINE not in info:
-                    warnings.warn("affine is None in push transform.")
+                    info[LazyAttr.AFFINE] = MetaTensor.get_default_affine()
             else:
-                info[LazyAttr.AFFINE] = convert_to_tensor(affine, device=torch.device("cpu"))
+                info[LazyAttr.AFFINE] = affine
+            info[LazyAttr.AFFINE] = convert_to_tensor(info[LazyAttr.AFFINE], device=torch.device("cpu"))
             out_obj.push_pending_operation(info)
         else:
+            if out_obj.pending_operations:
+                transform_name = info.get(TraceKeys.CLASS_NAME, "") if isinstance(info, dict) else ""
+                warnings.warn(
+                    f"Applying transform {transform_name} to a MetaTensor with pending operations "
+                    "is not supported (as this eventually changes the ordering of applied_operations when the pending "
+                    f"operations are executed). Please clear the pending operations before transform {transform_name}."
+                    f"\nPending operations: {[x.get(TraceKeys.CLASS_NAME) for x in out_obj.pending_operations]}."
+                )
             out_obj.push_applied_operation(info)
         if isinstance(data, Mapping):
             if not isinstance(data, dict):
                 data = dict(data)
             if isinstance(data_t, MetaTensor):
                 data[key] = data_t.copy_meta_from(out_obj)
             else:
```

## monai/transforms/utils.py

```diff
@@ -71,14 +71,15 @@
 
 __all__ = [
     "allow_missing_keys_mode",
     "check_boundaries",
     "compute_divisible_spatial_size",
     "convert_applied_interp_mode",
     "copypaste_arrays",
+    "check_non_lazy_pending_ops",
     "create_control_grid",
     "create_grid",
     "create_rotate",
     "create_scale",
     "create_shear",
     "create_translate",
     "extreme_points_to_image",
@@ -290,14 +291,35 @@
     if not inplace:
         dest = np.full(resize_dims, fill_value, img.dtype)  # type: ignore
         dest[destslices] = img[srcslices]
         return dest
     return img[srcslices]
 
 
+def check_non_lazy_pending_ops(
+    input_array: NdarrayOrTensor, name: None | str = None, raise_error: bool = False
+) -> None:
+    """
+    Check whether the input array has pending operations, raise an error or warn when it has.
+
+    Args:
+        input_array: input array to be checked.
+        name: an optional name to be included in the error message.
+        raise_error: whether to raise an error, default to False, a warning message will be issued instead.
+    """
+    if isinstance(input_array, monai.data.MetaTensor) and input_array.pending_operations:
+        msg = (
+            "The input image is a MetaTensor and has pending operations,\n"
+            f"but the function {name or ''} assumes non-lazy input, result may be incorrect."
+        )
+        if raise_error:
+            raise ValueError(msg)
+        warnings.warn(msg)
+
+
 def map_binary_to_indices(
     label: NdarrayOrTensor, image: NdarrayOrTensor | None = None, image_threshold: float = 0.0
 ) -> tuple[NdarrayOrTensor, NdarrayOrTensor]:
     """
     Compute the foreground and background of input label data, return the indices after fattening.
     For example:
     ``label = np.array([[[0, 1, 1], [1, 0, 1], [1, 1, 0]]])``
@@ -306,21 +328,22 @@
     Args:
         label: use the label data to get the foreground/background information.
         image: if image is not None, use ``label = 0 & image > image_threshold``
             to define background. so the output items will not map to all the voxels in the label.
         image_threshold: if enabled `image`, use ``image > image_threshold`` to
             determine the valid image content area and select background only in this area.
     """
-
+    check_non_lazy_pending_ops(label, name="map_binary_to_indices")
     # Prepare fg/bg indices
     if label.shape[0] > 1:
         label = label[1:]  # for One-Hot format data, remove the background channel
     label_flat = ravel(any_np_pt(label, 0))  # in case label has multiple dimensions
     fg_indices = nonzero(label_flat)
     if image is not None:
+        check_non_lazy_pending_ops(image, name="map_binary_to_indices")
         img_flat = ravel(any_np_pt(image > image_threshold, 0))
         img_flat, *_ = convert_to_dst_type(img_flat, label, dtype=bool)
         bg_indices = nonzero(img_flat & ~label_flat)
     else:
         bg_indices = nonzero(~label_flat)
 
     # no need to save the indices in GPU, otherwise, still need to move to CPU at runtime when crop by indices
@@ -353,16 +376,18 @@
             region of the image (``image > image_threshold``).
         image_threshold: if enabled `image`, use ``image > image_threshold`` to
             determine the valid image content area and select class indices only in this area.
         max_samples_per_class: maximum length of indices in each class to reduce memory consumption.
             Default is None, no subsampling.
 
     """
+    check_non_lazy_pending_ops(label, name="map_classes_to_indices")
     img_flat: NdarrayOrTensor | None = None
     if image is not None:
+        check_non_lazy_pending_ops(image, name="map_classes_to_indices")
         img_flat = ravel((image > image_threshold).any(0))
 
     # assuming the first dimension is channel
     channels = len(label)
 
     num_classes_: int = channels
     if channels == 1:
@@ -406,14 +431,15 @@
         n_samples: number of patch samples
         r_state: a random state container
 
     Returns:
         a list of `n_samples` N-D integers representing the spatial sampling location of patches.
 
     """
+    check_non_lazy_pending_ops(w, name="weighted_patch_samples")
     if w is None:
         raise ValueError("w must be an ND array, got None.")
     if r_state is None:
         r_state = np.random.RandomState()
     img_size = np.asarray(w.shape, dtype=int)
     win_size = np.asarray(fall_back_tuple(spatial_size, img_size), dtype=int)
 
@@ -933,14 +959,15 @@
         select_fn: function to select expected foreground, default is to select values > 0.
         channel_indices: if defined, select foreground only on the specified channels
             of image. if None, select foreground on the whole image.
         margin: add margin value to spatial dims of the bounding box, if only 1 value provided, use it for all dims.
         allow_smaller: when computing box size with `margin`, whether allow the image size to be smaller
             than box size, default to `True`.
     """
+    check_non_lazy_pending_ops(img, name="generate_spatial_bounding_box")
     spatial_size = img.shape[1:]
     data = img[list(ensure_tuple(channel_indices))] if channel_indices is not None else img
     data = select_fn(data).any(0)
     ndim = len(data.shape)
     margin = ensure_tuple_rep(margin, ndim)
     for m in margin:
         if m < 0:
@@ -1171,14 +1198,15 @@
         The output format of the coordinates is:
 
         [1st_spatial_dim_min, 1st_spatial_dim_max, 2nd_spatial_dim_min, ..., Nth_spatial_dim_max]
 
     Raises:
         ValueError: When the input image does not have any foreground pixel.
     """
+    check_non_lazy_pending_ops(img, name="get_extreme_points")
     if rand_state is None:
         rand_state = np.random.random.__self__  # type: ignore
     indices = where(img != background)
     if np.size(indices[0]) == 0:
         raise ValueError("get_extreme_points: no foreground object in mask!")
 
     def _get_point(val, dim):
```

## monai/transforms/croppad/array.py

```diff
@@ -776,16 +776,14 @@
 
     def compute_bounding_box(self, img: torch.Tensor) -> tuple[np.ndarray, np.ndarray]:
         """
         Compute the start points and end points of bounding box to crop.
         And adjust bounding box coords to be divisible by `k`.
 
         """
-        if isinstance(img, MetaTensor) and img.pending_operations:
-            warnings.warn("foreground computation may not be accurate if the image has pending operations.")
         box_start, box_end = generate_spatial_bounding_box(
             img, self.select_fn, self.channel_indices, self.margin, self.allow_smaller
         )
         box_start_, *_ = convert_data_type(box_start, output_type=np.ndarray, dtype=np.int16, wrap_sequence=True)
         box_end_, *_ = convert_data_type(box_end, output_type=np.ndarray, dtype=np.int16, wrap_sequence=True)
         orig_spatial_size = box_end_ - box_start_
         # make the spatial size divisible by `k`
@@ -814,14 +812,26 @@
         )
         ret = self.padder.__call__(img=cropped, to_pad=pad_width, mode=mode, **pad_kwargs)
         # combine the traced cropping and padding into one transformation
         # by taking the padded info and placing it in a key inside the crop info.
         if get_track_meta() and isinstance(ret, MetaTensor):
             if not self.lazy_evaluation:
                 ret.applied_operations[-1][TraceKeys.EXTRA_INFO]["pad_info"] = ret.applied_operations.pop()
+            else:
+                pad_info = ret.pending_operations.pop()
+                crop_info = ret.pending_operations.pop()
+                extra = crop_info[TraceKeys.EXTRA_INFO]
+                extra["pad_info"] = pad_info
+                self.push_transform(
+                    ret,
+                    orig_size=crop_info.get(TraceKeys.ORIG_SIZE),
+                    sp_size=pad_info[LazyAttr.SHAPE],
+                    affine=crop_info[LazyAttr.AFFINE] @ pad_info[LazyAttr.AFFINE],
+                    extra_info=extra,
+                )
         return ret
 
     def __call__(  # type: ignore[override]
         self, img: torch.Tensor, mode: str | None = None, **pad_kwargs
     ) -> torch.Tensor:
         """
         Apply the transform to `img`, assuming `img` is channel-first and
@@ -865,16 +875,14 @@
     ):
         self.spatial_size = ensure_tuple(spatial_size)
         self.num_samples = int(num_samples)
         self.weight_map = weight_map
         self.centers: list[np.ndarray] = []
 
     def randomize(self, weight_map: NdarrayOrTensor) -> None:
-        if isinstance(weight_map, MetaTensor) and weight_map.pending_operations:
-            warnings.warn("weight map has pending operations, the sampling may not be correct.")
         self.centers = weighted_patch_samples(
             spatial_size=self.spatial_size, w=weight_map[0], n_samples=self.num_samples, r_state=self.R
         )  # using only the first channel as weight map
 
     @LazyTransform.lazy_evaluation.setter  # type: ignore
     def lazy_evaluation(self, _val: bool):
         self._lazy_evaluation = _val
@@ -1011,18 +1019,14 @@
         fg_indices: NdarrayOrTensor | None = None,
         bg_indices: NdarrayOrTensor | None = None,
         image: torch.Tensor | None = None,
     ) -> None:
         fg_indices_ = self.fg_indices if fg_indices is None else fg_indices
         bg_indices_ = self.bg_indices if bg_indices is None else bg_indices
         if fg_indices_ is None or bg_indices_ is None:
-            if isinstance(label, MetaTensor) and label.pending_operations:
-                warnings.warn("label has pending operations, the fg/bg indices may be incorrect.")
-            if isinstance(image, MetaTensor) and image.pending_operations:
-                warnings.warn("image has pending operations, the fg/bg indices may be incorrect.")
             if label is None:
                 raise ValueError("label must be provided.")
             fg_indices_, bg_indices_ = map_binary_to_indices(label, image, self.image_threshold)
         _shape = None
         if label is not None:
             _shape = label.peek_pending_shape() if isinstance(label, MetaTensor) else label.shape[1:]
         elif image is not None:
@@ -1191,18 +1195,14 @@
         self,
         label: torch.Tensor | None = None,
         indices: list[NdarrayOrTensor] | None = None,
         image: torch.Tensor | None = None,
     ) -> None:
         indices_ = self.indices if indices is None else indices
         if indices_ is None:
-            if isinstance(label, MetaTensor) and label.pending_operations:
-                warnings.warn("label has pending operations, the fg/bg indices may be incorrect.")
-            if isinstance(image, MetaTensor) and image.pending_operations:
-                warnings.warn("image has pending operations, the fg/bg indices may be incorrect.")
             if label is None:
                 raise ValueError("label must not be None.")
             indices_ = map_classes_to_indices(
                 label, self.num_classes, image, self.image_threshold, self.max_samples_per_class
             )
         _shape = None
         if label is not None:
```

## monai/transforms/lazy/utils.py

```diff
@@ -212,14 +212,15 @@
             raise ValueError(f"Resampling out_spatial_size should be positive, got {out_spatial_size}.")
         if (
             allclose(matrix_np, np.eye(len(matrix_np)), atol=atol)
             and len(in_shape) == len(out_spatial_size)
             and allclose(convert_to_numpy(in_shape, wrap_sequence=True), out_spatial_size)
         ):
             img.affine = call_kwargs["dst_affine"]
+            img = img.to(torch.float32)  # consistent with monai.transforms.spatial.functional.spatial_resample
             return img
         img = monai.transforms.crop_or_pad_nd(img, matrix_np, out_spatial_size, mode=call_kwargs["padding_mode"])
         img = img.to(torch.float32)  # consistent with monai.transforms.spatial.functional.spatial_resample
         img.affine = call_kwargs["dst_affine"]
         return img
 
     resampler = monai.transforms.SpatialResample(**init_kwargs)
```

## monai/transforms/utility/array.py

```diff
@@ -826,27 +826,32 @@
         lambd = Lambda(func=lambda x: x[:4, :, :])
         print(lambd(image).shape)
         (4, 2, 2)
 
     Args:
         func: Lambda/function to be applied.
         inv_func: Lambda/function of inverse operation, default to `lambda x: x`.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
 
     Raises:
         TypeError: When ``func`` is not an ``Optional[Callable]``.
 
     """
 
     backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
 
-    def __init__(self, func: Callable | None = None, inv_func: Callable = no_collation) -> None:
+    def __init__(
+        self, func: Callable | None = None, inv_func: Callable = no_collation, track_meta: bool = True
+    ) -> None:
         if func is not None and not callable(func):
             raise TypeError(f"func must be None or callable but is {type(func).__name__}.")
         self.func = func
         self.inv_func = inv_func
+        self.track_meta = track_meta
 
     def __call__(self, img: NdarrayOrTensor, func: Callable | None = None):
         """
         Apply `self.func` to `img`.
 
         Args:
             func: Lambda/function to be applied. Defaults to `self.func`.
@@ -856,15 +861,15 @@
 
         """
         fn = func if func is not None else self.func
         if not callable(fn):
             raise TypeError(f"func must be None or callable but is {type(fn).__name__}.")
         out = fn(img)
         # convert to MetaTensor if necessary
-        if isinstance(out, (np.ndarray, torch.Tensor)) and not isinstance(out, MetaTensor) and get_track_meta():
+        if isinstance(out, (np.ndarray, torch.Tensor)) and not isinstance(out, MetaTensor) and self.track_meta:
             out = MetaTensor(out)
         if isinstance(out, MetaTensor):
             self.push_transform(out)
         return out
 
     def inverse(self, data: torch.Tensor):
         if isinstance(data, MetaTensor):
@@ -877,29 +882,37 @@
     Randomizable version :py:class:`monai.transforms.Lambda`, the input `func` may contain random logic,
     or randomly execute the function based on `prob`.
 
     Args:
         func: Lambda/function to be applied.
         prob: probability of executing the random function, default to 1.0, with 100% probability to execute.
         inv_func: Lambda/function of inverse operation, default to `lambda x: x`.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
 
     For more details, please check :py:class:`monai.transforms.Lambda`.
     """
 
     backend = Lambda.backend
 
-    def __init__(self, func: Callable | None = None, prob: float = 1.0, inv_func: Callable = no_collation) -> None:
-        Lambda.__init__(self=self, func=func, inv_func=inv_func)
+    def __init__(
+        self,
+        func: Callable | None = None,
+        prob: float = 1.0,
+        inv_func: Callable = no_collation,
+        track_meta: bool = True,
+    ) -> None:
+        Lambda.__init__(self=self, func=func, inv_func=inv_func, track_meta=track_meta)
         RandomizableTransform.__init__(self=self, prob=prob)
 
     def __call__(self, img: NdarrayOrTensor, func: Callable | None = None):
         self.randomize(img)
         out = deepcopy(super().__call__(img, func) if self._do_transform else img)
         # convert to MetaTensor if necessary
-        if not isinstance(out, MetaTensor) and get_track_meta():
+        if not isinstance(out, MetaTensor) and self.track_meta:
             out = MetaTensor(out)
         if isinstance(out, MetaTensor):
             lambda_info = self.pop_transform(out) if self._do_transform else {}
             self.push_transform(out, extra_info=lambda_info)
         return out
 
     def inverse(self, data: torch.Tensor):
@@ -1623,21 +1636,19 @@
         if isinstance(filter, str):
             if not filter_size:
                 raise ValueError("`filter_size` must be specified when specifying filters by string.")
             if filter_size % 2 == 0:
                 raise ValueError("`filter_size` should be a single uneven integer.")
             if filter not in self.supported_filters:
                 raise NotImplementedError(f"{filter}. Supported filters are {self.supported_filters}.")
-        elif isinstance(filter, torch.Tensor) or isinstance(filter, np.ndarray):
+        elif isinstance(filter, (torch.Tensor, np.ndarray)):
             if filter.ndim not in [1, 2, 3]:
                 raise ValueError("Only 1D, 2D, and 3D filters are supported.")
             self._check_all_values_uneven(filter.shape)
-        elif isinstance(filter, (nn.Module, Transform)):
-            pass
-        else:
+        elif not isinstance(filter, (nn.Module, Transform)):
             raise TypeError(
                 f"{type(filter)} is not supported."
                 "Supported types are `class 'str'`, `class 'torch.Tensor'`, `class 'np.ndarray'`, "
                 "`class 'torch.nn.modules.module.Module'`, `class 'monai.transforms.Transform'`"
             )
 
     def _check_kwargs_are_present(self, filter, **kwargs):
```

## monai/transforms/utility/dictionary.py

```diff
@@ -1084,14 +1084,16 @@
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: :py:class:`monai.transforms.compose.MapTransform`
         func: Lambda/function to be applied. It also can be a sequence of Callable,
             each element corresponds to a key in ``keys``.
         inv_func: Lambda/function of inverse operation if want to invert transforms, default to `lambda x: x`.
             It also can be a sequence of Callable, each element corresponds to a key in ``keys``.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
         overwrite: whether to overwrite the original data in the input dictionary with lambda function output. it
             can be bool or str, when setting to str, it will create a new key for the output and keep the value of
             key intact. default to True. it also can be a sequence of bool or str, each element corresponds to a key
             in ``keys``.
         allow_missing_keys: don't raise exception if key is missing.
 
     Note: The inverse operation doesn't allow to define `extra_info` or access other information, such as the
@@ -1102,22 +1104,23 @@
     backend = Lambda.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         func: Sequence[Callable] | Callable,
         inv_func: Sequence[Callable] | Callable = no_collation,
+        track_meta: bool = True,
         overwrite: Sequence[bool] | bool | Sequence[str] | str = True,
         allow_missing_keys: bool = False,
     ) -> None:
         super().__init__(keys, allow_missing_keys)
         self.func = ensure_tuple_rep(func, len(self.keys))
         self.inv_func = ensure_tuple_rep(inv_func, len(self.keys))
         self.overwrite = ensure_tuple_rep(overwrite, len(self.keys))
-        self._lambd = Lambda()
+        self._lambd = Lambda(track_meta=track_meta)
 
     def __call__(self, data: Mapping[Hashable, torch.Tensor]) -> dict[Hashable, torch.Tensor]:
         d = dict(data)
         for key, func, overwrite in self.key_iterator(d, self.func, self.overwrite):
             ret = self._lambd(img=d[key], func=func)
             if overwrite and isinstance(overwrite, bool):
                 d[key] = ret
@@ -1142,14 +1145,16 @@
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: :py:class:`monai.transforms.compose.MapTransform`
         func: Lambda/function to be applied. It also can be a sequence of Callable,
             each element corresponds to a key in ``keys``.
         inv_func: Lambda/function of inverse operation if want to invert transforms, default to `lambda x: x`.
             It also can be a sequence of Callable, each element corresponds to a key in ``keys``.
+        track_meta:  If `False`, then standard data objects will be returned (e.g., torch.Tensor` and `np.ndarray`)
+            as opposed to MONAI's enhanced objects. By default, this is `True`.
         overwrite: whether to overwrite the original data in the input dictionary with lambda function output.
             default to True. it also can be a sequence of bool, each element corresponds to a key in ``keys``.
         prob: probability of executing the random function, default to 1.0, with 100% probability to execute.
             note that all the data specified by `keys` will share the same random probability to execute or not.
         allow_missing_keys: don't raise exception if key is missing.
 
     For more details, please check :py:class:`monai.transforms.Lambdad`.
@@ -1161,23 +1166,25 @@
     backend = Lambda.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         func: Sequence[Callable] | Callable,
         inv_func: Sequence[Callable] | Callable = no_collation,
+        track_meta: bool = True,
         overwrite: Sequence[bool] | bool = True,
         prob: float = 1.0,
         allow_missing_keys: bool = False,
     ) -> None:
         Lambdad.__init__(
             self=self,
             keys=keys,
             func=func,
             inv_func=inv_func,
+            track_meta=track_meta,
             overwrite=overwrite,
             allow_missing_keys=allow_missing_keys,
         )
         RandomizableTransform.__init__(self=self, prob=prob, do_transform=True)
 
     def __call__(self, data):
         self.randomize(data)
```

## monai/utils/__init__.py

```diff
@@ -13,14 +13,15 @@
 
 # have to explicitly bring these in here to resolve circular import issues
 from .aliases import alias, resolve_name
 from .decorators import MethodReplacer, RestartGenerator
 from .deprecate_utils import DeprecatedError, deprecated, deprecated_arg, deprecated_arg_default
 from .dist import RankFilter, evenly_divisible_all_gather, get_dist_device, string_list_all_gather
 from .enums import (
+    AlgoKeys,
     Average,
     BlendMode,
     BoxModeName,
     BundleProperty,
     BundlePropertyConfig,
     ChannelMatching,
     ColorOrder,
```

## monai/utils/aliases.py

```diff
@@ -77,15 +77,16 @@
         if obj is None:
             raise ValueError(f"Module {modname!r} does not have member {declname!r}.")
 
     # attempt to resolve a simple name
     if obj is None:
         # Get all modules having the declaration/import, need to check here that getattr returns something which doesn't
         # equate to False since in places __getattr__ returns 0 incorrectly:
-        # https://github.com/tensorflow/tensorboard/blob/a22566561d2b4fea408755a951ac9eaf3a156f8e/tensorboard/compat/tensorflow_stub/pywrap_tensorflow.py#L35  # noqa: B950
+        # https://github.com/tensorflow/tensorboard/blob/a22566561d2b4fea408755a951ac9eaf3a156f8e/
+        # tensorboard/compat/tensorflow_stub/pywrap_tensorflow.py#L35
         mods = [m for m in list(sys.modules.values()) if getattr(m, name, None)]
 
         if len(mods) > 0:  # found modules with this declaration or import
             if len(mods) > 1:  # found multiple modules, need to determine if ambiguous or just multiple imports
                 foundmods = set(filter(None, {inspect.getmodule(getattr(m, name)) for m in mods}))  # resolve imports
 
                 if len(foundmods) > 1:  # found multiple declarations with the same name
```

## monai/utils/misc.py

```diff
@@ -68,14 +68,15 @@
     "save_obj",
     "label_union",
     "path_to_uri",
     "pprint_edges",
     "check_key_duplicates",
     "CheckKeyDuplicatesYamlLoader",
     "ConvertUnits",
+    "check_kwargs_exist_in_class_init",
 ]
 
 _seed = None
 _flag_deterministic = torch.backends.cudnn.deterministic
 _flag_cudnn_benchmark = torch.backends.cudnn.benchmark
 NP_MAX = np.iinfo(np.uint32).max
 MAX_SEED = NP_MAX + 1  # 2**32, the actual seed should be in [0, MAX_SEED - 1] for uint32
@@ -796,7 +797,27 @@
             return 1.0
         input_power = self._get_unit_power(self.input_unit)
         target_power = self._get_unit_power(self.target_unit)
         self.conversion_factor = 10 ** (input_power - target_power)
 
     def __call__(self, value: int | float) -> Any:
         return float(value) * self.conversion_factor
+
+
+def check_kwargs_exist_in_class_init(cls, kwargs):
+    """
+    Check if the all keys in kwargs exist in the __init__ method of the class.
+
+    Args:
+        cls: the class to check.
+        kwargs: kwargs to examine.
+
+    Returns:
+        a boolean inidicating if all keys exist.
+        a set of extra keys that are not used in the __init__.
+    """
+    init_signature = inspect.signature(cls.__init__)
+    init_params = set(init_signature.parameters) - {"self"}  # Exclude 'self' from the parameter list
+    input_kwargs = set(kwargs)
+    extra_kwargs = input_kwargs - init_params
+
+    return extra_kwargs == set(), extra_kwargs
```

## Comparing `monai-1.2.0rc4.dist-info/LICENSE` & `monai-1.2.0rc5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai-1.2.0rc4.dist-info/METADATA` & `monai-1.2.0rc5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai
-Version: 1.2.0rc4
+Version: 1.2.0rc5
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

## Comparing `monai-1.2.0rc4.dist-info/RECORD` & `monai-1.2.0rc5.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 monai/__init__.py,sha256=N68MC4_ibRXAO-vquIMx4tT--Er8hAHlKkmIrVBLsbY,2276
-monai/_version.py,sha256=LKob9njkBRLKzrCDQ-koS9kyRykOiNZWbifkG05gSkQ,500
+monai/_version.py,sha256=YF1C3TbaZBviYayOAIDQ7H1qDqUZi8J7MKwvH52xUSw,500
 monai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 monai/_extensions/__init__.py,sha256=NEBPreRhQ8H9gVvgrLr_y52_TmqB96u_u4VQmeNT93I,642
 monai/_extensions/loader.py,sha256=7SiKw36q-nOzH8CRbBurFrz7GM40GCu7rc93Tm8XpnI,3643
 monai/_extensions/gmm/gmm.cpp,sha256=GLC_KOEFUlEB8fUs6vjeuZBxIqzuatZBDc-ZoAtQ6Xg,2931
 monai/_extensions/gmm/gmm.h,sha256=c9n8RLa4r9jTbqpY4cCHFm3ldVER_FN8pG2hQx3Lb3c,1760
 monai/_extensions/gmm/gmm_cpu.cpp,sha256=cyKn-7DjtVCPb9bnGb0bWUfagb3KUFX9rD6mI5BEXrs,1118
 monai/_extensions/gmm/gmm_cuda.cu,sha256=2CvNdiuc6JiEsdK31iiHJQytubn81fxIQim-At_-1HA,16213
 monai/_extensions/gmm/gmm_cuda_linalg.cuh,sha256=Glqg2oAcUFUXg-DVfpROkiv-DdXvvVdM1nyiFm8qlHY,3520
 monai/apps/__init__.py,sha256=VDIc3HB_uFbqKL1TS-OeRvryEMDfzm22KJRzwpkXsGo,908
-monai/apps/datasets.py,sha256=OOfRSKDAL4IEh4bsRZDQddl_d_7tbVUy7QXZsUSFWig,34560
+monai/apps/datasets.py,sha256=gA4z4WCfH4-lz66aZ3uvubopTteQjcxhg38nSOM01Sk,34568
 monai/apps/utils.py,sha256=lyUDb-HUvEb8xPAi0cwQcKEGaSrgKi8H9sikYNRyTL4,13505
-monai/apps/auto3dseg/__init__.py,sha256=nacmbm8szCtL6Jf_ZaL8JQtiBlM6B3_TiI3HHZfJLt0,952
-monai/apps/auto3dseg/__main__.py,sha256=xtGFmv2ok6wK3SDCUm3yOF8XUHwNz3nKP1Zw9fxRsv0,1349
-monai/apps/auto3dseg/auto_runner.py,sha256=HRYHlmnti6ssXLjJJeH90hjx3lhzTMNAyg6nG0l2KjA,36092
-monai/apps/auto3dseg/bundle_gen.py,sha256=VNPgHeXEJlmTXCQkGKwNtBvzJW5ZOAKfPijx4Go5PQY,23164
+monai/apps/auto3dseg/__init__.py,sha256=bnhmTnu9QWJbYDbDDrlnpWLBNa6thxPMIvgIUOTgGZ4,993
+monai/apps/auto3dseg/__main__.py,sha256=fCDhD8uhmJQKkKBxLO6hMJhEvZJRIsjTc1Ad3bYmNIY,1411
+monai/apps/auto3dseg/auto_runner.py,sha256=wua5mmnCAzGoTOF42zXj11syJvEADoMXEtXDUOQINCQ,37585
+monai/apps/auto3dseg/bundle_gen.py,sha256=qhBPV06QCbny0yd2tmowUnE0z5-AujMGWg3w7GCQJ1A,26014
 monai/apps/auto3dseg/data_analyzer.py,sha256=cVoPCOa2M2uIY8PVzCiHYgwt2ERSvpKFIDpA_UvvLH0,17319
-monai/apps/auto3dseg/ensemble_builder.py,sha256=vEHC0mcvWZeuXaIH7hFj9p22M6MWBNoxtWcZGUgSfUI,11249
+monai/apps/auto3dseg/ensemble_builder.py,sha256=WhgLtw8FfYW_-hoz5OkZz1OtYefcM0z4DZwHL-UhHzo,24328
 monai/apps/auto3dseg/hpo_gen.py,sha256=XnWjoSgkrZOS8W_AaSaXpShJjSxx5l0xaYDkJVlqewk,17523
 monai/apps/auto3dseg/transforms.py,sha256=eHueZBNFMgGa9Nz96JE7KxTH05mpMfWxaD1QHxQ-B98,3733
-monai/apps/auto3dseg/utils.py,sha256=KdU5E8jNghdONNwb2aZ7eYjA5zGkoNq_1s-drq3csm8,2765
+monai/apps/auto3dseg/utils.py,sha256=JJJQy2GDVuwasqn8dzrgJwX0ZTwk660vKW7D-cxUweo,2917
 monai/apps/deepedit/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/deepedit/interaction.py,sha256=h9zTmhHAmwndR315RknqXtLWYqyYGvdcmjP6EpRrzHg,4501
 monai/apps/deepedit/transforms.py,sha256=sgFUuMqMlxmvWmsx-lHajoUHVDMp9fLo7UiwG60IYU8,37435
 monai/apps/deepgrow/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/deepgrow/dataset.py,sha256=W0wv1QujA4sZgrAcBS64dl3OBbDBM2cF4RK0fDCQnRU,10054
 monai/apps/deepgrow/interaction.py,sha256=l-wCmetMi4g-gcgMjA68firOX4RKvFm8WgefwiUFtTs,3739
 monai/apps/deepgrow/transforms.py,sha256=C38Q5ZdR98JWFyR5lNnhIaibL9zf14c111KDLaYvwB8,42011
 monai/apps/detection/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/detection/metrics/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/detection/metrics/coco.py,sha256=1yQJjd-9M0rUmPZlAle3B7IEqVNNAn53pDkSG1GJ3U8,26617
 monai/apps/detection/metrics/matching.py,sha256=GF4wgH5Let7GwW1SGwzfzz5BRnCVEhDe7_KR7zpLr44,17161
 monai/apps/detection/networks/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/apps/detection/networks/retinanet_detector.py,sha256=CRT5q3E096S3JB5v1k7MUqYL7vNOGkda7snMhVYzkws,51663
-monai/apps/detection/networks/retinanet_network.py,sha256=WYWAOE51xBYyKSRFQRC4iLUATaj-M3U2wCJjruptQVw,17604
+monai/apps/detection/networks/retinanet_detector.py,sha256=eR0hPip-ZeXUtDv_-y-aFGhe9kHnIdAJRqS1rEojJgQ,53221
+monai/apps/detection/networks/retinanet_network.py,sha256=p7VHhgyzhC47rX3TPvyH98_m5xWPt1kPxpyT9ciGpKA,18850
 monai/apps/detection/transforms/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/detection/transforms/array.py,sha256=MeDK8I3Q3KW13chF3XVdWcYoG7ZbiesokLVBLxMPPwI,24519
-monai/apps/detection/transforms/box_ops.py,sha256=Z3GUS-XfHAAbLte8sJWQ9lODhlnMaU8DRZHyCzRP9kI,17970
+monai/apps/detection/transforms/box_ops.py,sha256=17X76HXROCdk38-1c9wEuMBm4TM0nWCZfOmkkZLxxBI,17916
 monai/apps/detection/transforms/dictionary.py,sha256=GrghYnvDUnAuE8XC9pcv6eR2vlMOZ2pB9-wqCaOz5Jo,68979
 monai/apps/detection/utils/ATSS_matcher.py,sha256=6M9UwQ2sV5xOhgZuLujunOiJ9DlDXS7OcHfJoKGXu4M,13531
 monai/apps/detection/utils/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/detection/utils/anchor_utils.py,sha256=w4SepYKRyyNn5a4irkkFmnHhUYifS-PsAaGb9xxzGlw,18681
 monai/apps/detection/utils/box_coder.py,sha256=81Qe8wf6IRb4kJgcS957yWdOpY_G8nUdyIFPXxpMQvk,11120
 monai/apps/detection/utils/box_selector.py,sha256=uXI0YrhugYR68xYshRs5JpPTT1nL3QMMS1nJ_RpddVo,9031
 monai/apps/detection/utils/detector_utils.py,sha256=pU7bOzH-ay9Lnzu1aHCrIwlaGVf5xj13E7Somx_vFnk,10306
 monai/apps/detection/utils/hard_negative_sampler.py,sha256=PywdXkFIAdudmp3W8JWM_CcLC3BKWQh5x1y0tuuokcg,13890
-monai/apps/detection/utils/predict_utils.py,sha256=3S1rd61GxBZ5Y7P2-CE6TJVaDwgqzLEREMVoJ2loWVM,5627
+monai/apps/detection/utils/predict_utils.py,sha256=6j7U-7pLtbmgE6SXKR_MVImc67-M8WtzQkT89cCVsK8,5818
 monai/apps/mmars/__init__.py,sha256=BolpgEi9jNBgrOQd3Kwp-9QQLeWQwQtlN_MJkK1eu5s,726
 monai/apps/mmars/mmars.py,sha256=AYsx5FDmJ0dT0hAkWGYhM470aPIG23PYloHihDZfOKE,13115
 monai/apps/mmars/model_desc.py,sha256=k7WSMRuyQN8xPax8aUmGKiTNZmcVatdqPYCgxDih-x4,9996
 monai/apps/nnunet/__init__.py,sha256=gyqmg1fxPf3RF6LL25gnpMTfNS14uxweuJ93e4UzjB8,745
 monai/apps/nnunet/__main__.py,sha256=h5GTEHSZliEZ38_4WOtqujPa-C3M6if-0huNHmreaNI,2975
 monai/apps/nnunet/nnunetv2_runner.py,sha256=iqKvjUHH22jq0TmkHawRvMigEKBIDIirhpT3lbYDXQY,38587
 monai/apps/nnunet/utils.py,sha256=u1jVSAJeOmpCmXczqnGuU4jnSevsawwLbuFUUKB8XrI,6791
@@ -66,15 +66,15 @@
 monai/apps/pathology/losses/__init__.py,sha256=yPGavYe8N6_bKvRN1-1awGmgnHZKpjQww3QML6UMRPQ,650
 monai/apps/pathology/losses/hovernet_loss.py,sha256=Sw9wBAilBOKB8oKaPU4yKxVOl8y4lv-XzgJ6iFN0AyU,7293
 monai/apps/pathology/metrics/__init__.py,sha256=c7xRUzhQesEWRIUFF6vM-Qs9v0Lv8QzCNNd-hJOCL-I,646
 monai/apps/pathology/metrics/lesion_froc.py,sha256=yA5bsJAAn6eIQ5Q1m0rOVAsjl9YpAXisgkJ6TxfpPhU,7225
 monai/apps/pathology/transforms/__init__.py,sha256=c3YkornqjX-fHRnwkpn_PxmnMje6pif1qxPdFNyQUWU,2243
 monai/apps/pathology/transforms/post/__init__.py,sha256=WUZbaM2bg13mpbnNhol0D0A328XgUspTWtPvli1Uqpk,1995
 monai/apps/pathology/transforms/post/array.py,sha256=_FxrRpFOnpspUdXTi5_4zHZOx9mT_4-suh96FPjEajo,37322
-monai/apps/pathology/transforms/post/dictionary.py,sha256=5qQ00PM5XJpzfJDvshi9dfGKsnxtsUO4e9FGwekv7KI,25992
+monai/apps/pathology/transforms/post/dictionary.py,sha256=ZReeFqcZRkltwhRaKsedeptprB1B89lKWFimAzkk0Vg,25928
 monai/apps/pathology/transforms/stain/__init__.py,sha256=i9HfrXiQHG5XHfqMtz2g7yBX7p1uN0xcGAPCYyXSmV8,836
 monai/apps/pathology/transforms/stain/array.py,sha256=Dr1fCmkQzc8n40XbLAHpq1EG5wkMqTjWgYN2FGJfMGk,8366
 monai/apps/pathology/transforms/stain/dictionary.py,sha256=sTF7DJVXQe1SBQrhC84Xl2kmINqoTX6Tb8YSv2VH9Vs,4761
 monai/apps/reconstruction/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/reconstruction/complex_utils.py,sha256=vIVCweWwPHL5bYK3a7aDMS64CI7L9AUh9l2gG3cisM4,8393
 monai/apps/reconstruction/fastmri_reader.py,sha256=CbAWHN9-b8TFgIpsu1UmS0zHZg3lvqIyraZFODoTMdM,3644
 monai/apps/reconstruction/mri_utils.py,sha256=WEentr9IfCdTRcRELYkIgRx2oCaIoc1JEVE1FJfQlqQ,2000
@@ -98,19 +98,19 @@
 monai/auto3dseg/operations.py,sha256=1sNDWnz5Zs2-scpb1wotxar7yGYQ-VPI-_b2KnZqW9g,5110
 monai/auto3dseg/seg_summarizer.py,sha256=39zXmyRe9aNhXS9ZliDJsUEDqzU1OPtUG5tL1peJsx0,8725
 monai/auto3dseg/utils.py,sha256=QOapCrMbguQz_t5BsU_YAY4DWwjKA38i4sc-TWgzKJA,12193
 monai/bundle/__init__.py,sha256=EFeyJGNju0ijBfKkobpdymGvbuAX_ZJWQd8sa6OWOSw,1341
 monai/bundle/__main__.py,sha256=EiWkpt3yIcT8uBKg99kQBWTYoFgSpHjR7GAvIKA9EME,926
 monai/bundle/config_item.py,sha256=sBQ_Kg93EFET_pZcdzdMatnrB2FD2bMvmg_LpupdwMA,16035
 monai/bundle/config_parser.py,sha256=tX8ZKDW43uWzCQ8EBUROu-U9wJItzF7_XzotLK-wt60,22410
-monai/bundle/properties.py,sha256=CUTh7CVwZu4D59SRf2b1p-03OD2G9VVi5JUutazmC8A,8628
+monai/bundle/properties.py,sha256=RaknletfzGrFLnwKMrrd3fFCeisRntZ7yKAN48zJ0MY,8811
 monai/bundle/reference_resolver.py,sha256=3KpSa-1n1hptY6N1C-3yt5pybTXB7QUVj8fNWWGvN2U,14353
-monai/bundle/scripts.py,sha256=K8c5RLc-QgrAZX80mk4JRL3kP13DYTCvNgl7OLIjc3M,63733
+monai/bundle/scripts.py,sha256=__72s2fWFe2Lx1H15O9_UeD0PRywr5_Gd5DJCvMWuaQ,63940
 monai/bundle/utils.py,sha256=Vou6ko4OjT1v8xOT99bZuFaAB-NPpTj-oZ4KjBJsYsY,8911
-monai/bundle/workflows.py,sha256=57BZ_GB-a3Qy7O_KtP-n-n_LS4Rku9FTi_Y2zubv7wE,16520
+monai/bundle/workflows.py,sha256=JxQKTCFAW3JgNz3NukRWpB39A7aE8aRgw9zQFGiiSGg,17082
 monai/config/__init__.py,sha256=CN28CfTdsp301gv8YXfVvkbztCfbAqrLKrJi_C8oP9s,1048
 monai/config/deviceconfig.py,sha256=TifpuOAhccn1A3UCtInAnfciyGLHSNIen5ZRmUB8eKI,9913
 monai/config/type_definitions.py,sha256=0fAuI-_uX2Ac_33bgDVXKmBSl-fJNFcsOqBqYV16fhk,3485
 monai/data/__init__.py,sha256=9FhsQ7GHbTNAX25vLY1oR63b3q7jpJpVMfLigs5h0bs,5087
 monai/data/box_utils.py,sha256=YbG6lOoYwUGmwcNmoKzq2xnNTbYA4LMkHmfsqteopCg,50102
 monai/data/csv_saver.py,sha256=fcZF4kBNQnDFwQjV9TS4zjq_zqsv_u3QldxRprMC7zI,4952
 monai/data/dataloader.py,sha256=-n_LUfm3tlSHxh1at1xOmQkMrWQaKm3KBNo4A27PECE,3835
@@ -130,44 +130,44 @@
 monai/data/samplers.py,sha256=8N72tdua63XByOrQ1SigMGimnwK9Y2KGOrsQEjIjhHI,5268
 monai/data/synthetic.py,sha256=H0MaQq2nnYxXEMlvOW1-XoWJWY_VKsgZ75tWLO1aCXg,7375
 monai/data/test_time_augmentation.py,sha256=H1yUph4SkJ-bmKRXS-SRZfNKtWkihR7o4PTUWKuHxOw,9780
 monai/data/thread_buffer.py,sha256=FtJlRwLHQzU9sf3XJk4G7b_-uKXaRQHAOMauc-zWN2Q,8840
 monai/data/torchscript_utils.py,sha256=auz2GtrklxY6PMzvd-i9Kk73uIv0qydpOtzdSfZxrhE,5500
 monai/data/utils.py,sha256=qNGP8YUAJl6N9xB8WCxPQE1JgWqQstv_qHoO35dwpX0,64795
 monai/data/video_dataset.py,sha256=5Q7bHXg32rOVQjiyLUrVuqAkpTa33uydCrZwNJw7iFM,9059
-monai/data/wsi_datasets.py,sha256=mQVqd58NmFVKxRVCHjJ0ga863H5hsgmH1j-VXkiQGeA,18631
+monai/data/wsi_datasets.py,sha256=Ga5VnOdOXU_tlhdub0ueD4VtWhkQG4IrueXX-abE3bA,18619
 monai/data/wsi_reader.py,sha256=3l_OzDM2tsCEuLbUWsHKJb3Bj9nEAwGV84hFX8QmtIY,49442
 monai/engines/__init__.py,sha256=07lWK9BRezM98bHM8Z1VBXcPs7JPnulDYtg8uXQzOio,1133
 monai/engines/evaluator.py,sha256=clfURplaABOZhhxYjYRz1ZHIQHEAGnGqljW0Ub9HbO8,24568
 monai/engines/multi_gpu_supervised_trainer.py,sha256=9UiqHpWvKxkj24-4EAzbHrRdMlSgohH-rFBus1M_Cnw,7278
 monai/engines/trainer.py,sha256=Nxt-lz0puqcWHEyVnhqR1qXwzR8PxlVSiPwH8phZAG8,21347
 monai/engines/utils.py,sha256=gmDzkD4SIL9DeFBgWdjbf2e6yTQp_e3lA9aAJRwZmDQ,11631
 monai/engines/workflow.py,sha256=EAWMehQz28o-fX8MKSVBjhI1YAM7-Gt-w1HfzcMl4gI,15250
 monai/fl/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/fl/client/__init__.py,sha256=Wnkcf-Guhi-d29eAH0p51jz1Tn9WSVM4UUGbbb9SAqQ,725
 monai/fl/client/client_algo.py,sha256=vF2OuT4I1p7Cupk5JmczY1vKsMUfC1DzVldifdzfEMY,5097
-monai/fl/client/monai_algo.py,sha256=szFeVHlYudTc-x5qxsmB2bz3ONxjSMAKfud0lQ6mXsY,32635
+monai/fl/client/monai_algo.py,sha256=3qyJDx8nKfjjYjfFbVJwGiyz8OEfkWm2jPPOf0OY-TE,33232
 monai/fl/utils/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/fl/utils/constants.py,sha256=HSFNlT-ITeydvzw1JPBgIEgXJCgjyh459WYqQHir6pU,2091
+monai/fl/utils/constants.py,sha256=B6i7O68Q-_ihQxnQ1Y-ICPC6tXRfFJH7oq1MDZPS-lE,1713
 monai/fl/utils/exchange_object.py,sha256=q41trOwBdog_g3k_Eh2EFnLufHJ1mj7nGyQ-ShuW5Mo,3527
-monai/fl/utils/filters.py,sha256=21KWHqiPx5LgPcYDqF9HBLVgAnlXuxvsOTlvvVvsusU,1628
+monai/fl/utils/filters.py,sha256=InXplYes52JJqtsNbePAPPAYS8am_uRO7UkBHyYyJCo,1633
 monai/handlers/__init__.py,sha256=PsCVxsS-cU_x9uOl_l66D5pGug94Pt4tmX6jLY0G2sU,2351
 monai/handlers/checkpoint_loader.py,sha256=CNcY_EqnlWjIPY99T_zz1Ff_yrkFIcosTUKEVs5exUY,6798
 monai/handlers/checkpoint_saver.py,sha256=NJljfsP_RbmeQvbI9g0B0hsPcV14vW37cljGRzLlXCY,16071
 monai/handlers/classification_saver.py,sha256=ujCzHyEN5lH-ZY_M5cN-J6s_JxByLkujxcTz2ZVxHow,7606
 monai/handlers/clearml_handlers.py,sha256=qs6ShyIZQY5YsDRL2QQozSlOzGqOBm6LdX1LR83QjJQ,7506
 monai/handlers/confusion_matrix.py,sha256=RK8rchjQ08BYGUTxsk8lEDClLipRc-s83OegiphHglc,3989
 monai/handlers/decollate_batch.py,sha256=96TBuau203bHRT1fuunRIxExd6vBIfVeM_1UbzcHaus,4425
 monai/handlers/earlystop_handler.py,sha256=Jv_JuvKGwvd3gfolGqTyFA91XTKEh-Pt0neZtQVIBPc,4381
 monai/handlers/garbage_collector.py,sha256=xaWAH8C2PW6BaM112dUSahbRUC1dTLixXZFJXcWvQ2Q,3338
 monai/handlers/hausdorff_distance.py,sha256=zfExI7KJSkv4i3fShDnIXrtKM957IYtDcvtzi-zlWKw,3580
 monai/handlers/ignite_metric.py,sha256=hB6sqpzd-p84J8rl1pyHYy5I7oiyTzSmhLHiKQQikm8,5578
 monai/handlers/logfile_handler.py,sha256=9iUroCpfaP_YJu5mGHJ6CW53DoiYZ7F_XjhZwXw4a84,3931
 monai/handlers/lr_schedule_handler.py,sha256=jj-ukoR3p-m0LVs-AzPqn2On8GIj70PSIPNp9t-iiQY,3575
-monai/handlers/mean_dice.py,sha256=JalWLuyZDQ-711o1vaVdFcCiKwWGdC_yAqbNiITtGOo,2832
+monai/handlers/mean_dice.py,sha256=2jF0X1dfYjyPnYsd6hJX31yQQ9Y9Y6ZQxVPnPvv8kj4,3220
 monai/handlers/mean_iou.py,sha256=rmfSOTTZ10VXf0t9m4ct7mkjlGX6KeAu25hxnwwCl_A,2831
 monai/handlers/metric_logger.py,sha256=IEXGngnGh75Mxt1w6Nd4Tau8qHQjyZFLGzoePteH1jM,5477
 monai/handlers/metrics_reloaded_handler.py,sha256=6Xqg6Uocn5dJNBW6y-zU2o6sGvbWqN5oLB5F5vledl8,6168
 monai/handlers/metrics_saver.py,sha256=GPTaIeXi0noRyW2BQYQtazFfGyezmqSBAYWeAF-C5t0,8560
 monai/handlers/mlflow_handler.py,sha256=-0Dy8mtN8y0g0ViGcmD-vdRQs6yVSvYTlx4qp6O_Oa4,16326
 monai/handlers/nvtx_handlers.py,sha256=dBITb2hboynktwZNkRrlqM7STu7n3qXrdoC1-IogWc4,6819
 monai/handlers/panoptic_quality.py,sha256=Nz2dkMeaqB3s4dFzmW-vUl_guJWj34jRPq4nUkxntpQ,3637
@@ -178,58 +178,58 @@
 monai/handlers/roc_auc.py,sha256=gKNThJLsWKaNQI3t6sWn-UrD6yfb1Rw5KWaS648dmkw,2730
 monai/handlers/smartcache_handler.py,sha256=OA6v4EC2geH419eBKSAGSb-XNxO_qSPmJ2fkh7TOv-s,3051
 monai/handlers/stats_handler.py,sha256=35tkttd-LFKfE6bO9wPVOr5oHwiP2yEWXcZSSURtN9E,14251
 monai/handlers/surface_distance.py,sha256=jfuRpuzG7Ia-Ye0Izce1n4UPBghe1xtwBPwXx3fmODw,3313
 monai/handlers/tensorboard_handlers.py,sha256=FGd3KT7AoulwWOGbiJqDAyjMpZzuIyZZoNsatRdDoNE,23325
 monai/handlers/utils.py,sha256=PumzyMPAisJ_A-4RkgkNq31YfulhuI1UcOF9-Xj2_Dw,9855
 monai/handlers/validation_handler.py,sha256=xpRB3IB7pckzgTgdzTGb_gG6tIezeIvtmhJHPNYrpvY,3269
-monai/inferers/__init__.py,sha256=B3e24tgM92C6J49FAOcawvpuyl_svG8OqfHMUjNFLl0,857
-monai/inferers/inferer.py,sha256=mdP1QnMrGRIigHi8ZDfnvmsXlIYyJt0Q8Uxi2cSJooA,27881
+monai/inferers/__init__.py,sha256=_MNRpyBTFuJQBAhWx3VAo8R3CAT7i-kcp8zp-CiXkSE,917
+monai/inferers/inferer.py,sha256=If9rhPEvNTc_vd6SlxiOMZKIAKOQo5HikwFqqIhWd2k,32038
 monai/inferers/merger.py,sha256=onJ9OiCV9YOdsljd5YFZ3Dx6nSWv_gfCf7s5TSb6tHs,6393
 monai/inferers/splitter.py,sha256=dfU1AQWVvcbqt2hvZJqk_hFh6EtFrtgBoV7aId1ns7k,9397
-monai/inferers/utils.py,sha256=O2nhe9bvN2scUmHoOX0o6yZrzEkUAtkjBJyUzhfSpCY,20036
+monai/inferers/utils.py,sha256=0wpfd6U351mNoli_M84B7eND_wHiGrYnZ-DHvrU8C14,20017
 monai/losses/__init__.py,sha256=9-QH3s0s1XACosZPhJz5LrDskiwjjcMMt9Rhr-LE4PU,1409
 monai/losses/contrastive.py,sha256=okmuiRPpwAhInBmk7wUFm0BogaxiP0EgqdV0lxIhbHY,3430
 monai/losses/deform.py,sha256=GJpIQMGFf97SMd-5PswsMFrvRokaO_NabgQn73KDfcw,4979
 monai/losses/dice.py,sha256=11wqc7MN5BfOh0STfO6YMGto9BxjmzOgnXBSPadH6Ds,46326
 monai/losses/ds_loss.py,sha256=do2z8NyW5_KUgIgiZieql_XTHd1-eK1_uVUozKQoFqs,3733
 monai/losses/focal_loss.py,sha256=GfblgQtA4qMcGhLnQdUJJrv8zQczB4GH4k6L2ZxKnRY,9490
 monai/losses/giou_loss.py,sha256=Mogq6fR0tO__Xj0Ul388QMEx03XrSS-Ue96i9ahY-uo,2795
 monai/losses/image_dissimilarity.py,sha256=RSjdWvGBY3Dk_CaKWhOxHeAq28diEoMi0-p4DAG5jZE,15492
 monai/losses/multi_scale.py,sha256=7hL4clBLa3f0tz9-74brq5XOFChrpyd_h9cHQKPnseQ,3636
 monai/losses/spatial_mask.py,sha256=UF8P6J3ZXKROhHwPoVRLEEnSYrQlJHkH6wMmwOPu3eM,2942
-monai/losses/ssim_loss.py,sha256=-uCmirU-ehwdgvly3j6JwHXesHH_YZClEgHZgwfGwac,4292
+monai/losses/ssim_loss.py,sha256=ld6SJvoGXMoP3PC4hjnQphLNIORA4JMDdjR2ARNQWJw,4825
 monai/losses/tversky.py,sha256=8idAtxrZW3SYI0vC8Hw2EDkOb4ybgCnJD3aNipWOEGc,6645
 monai/losses/unified_focal_loss.py,sha256=rCj8IpueYH_UMrOUXU0tjbXIN4Uix3bGnRZQtRvl7Sg,10224
 monai/metrics/__init__.py,sha256=NcFg8BER-LIJkfhK3sHkgorRHwST6RXQbbvOIimsYT8,1977
 monai/metrics/active_learning_metrics.py,sha256=uKID2O4mnY-9P2ZzyT4sqJd2NfgzjSpNKpAwulWCozU,8211
 monai/metrics/confusion_matrix.py,sha256=8CMnqIaNK9_cf-5Z_6E_g-blh1FnvnCmuGahJSlptgM,15101
 monai/metrics/cumulative_average.py,sha256=UINnp__332Kb4gDdIu6WAror11kQ0GxCeLydlsFx6tc,5578
 monai/metrics/f_beta_score.py,sha256=ucr0ktzfM9jZanV3aqKZnlc23tf1z5r399ZEhxgu6Pc,4026
 monai/metrics/froc.py,sha256=tGM3hIU17yNdj1YG1yW22UUpTc8nH7ZZXChvZY_T_40,6157
 monai/metrics/generalized_dice.py,sha256=0nk3-IT9s3SQshVf1QStGEmH0iBxtofzXx_bf1EWhVw,8262
 monai/metrics/hausdorff_distance.py,sha256=PDnr94AMWIBp1U0lql95BqL6wHvk3j_moqH2UTjeeBs,11470
 monai/metrics/loss_metric.py,sha256=m9jXobVHKLeDY_8yrA9m7FwfapSAb-kYIdUJOsbvBvY,4907
-monai/metrics/meandice.py,sha256=UsEJVAFbEZC7QM2j3tTleQSUTX5XWDwUPu6E0ipKZ68,10937
+monai/metrics/meandice.py,sha256=Y1xJ8Q_LrYjmJEKy5rerDHxOOK4byiotp7yBewsD3P8,12472
 monai/metrics/meaniou.py,sha256=MJd-4v-DArd_uDMWgUJhuV2CBXuU7hB2W3-IM_VxeSg,7209
 monai/metrics/metric.py,sha256=N-lnphEmh13Y2he1gnVWhwMRgMpO4r_X3uDzxiaRnmY,15140
 monai/metrics/panoptic_quality.py,sha256=2CfSB1B0mwVOfTCuRNuYAn7XI8G4NPFRPc7NTbv5JNc,13679
-monai/metrics/regression.py,sha256=mAWkqnFZGtb2pgmAXhb4T0MNrrU50Qup6UJjGF3XwjI,18235
+monai/metrics/regression.py,sha256=tBWYCWV20bETUBuS5s7QqHIqjq8mYPX1KbJQjnDT0I0,19719
 monai/metrics/rocauc.py,sha256=CJOAzDamB8TcFP1bEg-I1m5V1-Pq5RMaLFdM6MtNa_E,8038
 monai/metrics/surface_dice.py,sha256=3ged6augFI0tUieS4z0kNIWnIvil4HPlHlMybJttzhA,14415
 monai/metrics/surface_distance.py,sha256=KDbdKdQz1r8gOm0INLxAQrnaZn_71p5Tz3906rlv6k8,10186
-monai/metrics/utils.py,sha256=Vt4RxljPbrPYfpLDAAdnjtyraRLo4JgWTh0BaHKYNew,15100
+monai/metrics/utils.py,sha256=lG5150UPUUlp3ubkOonlpVCPHWfaceqEd_dNoTe2Cw4,15094
 monai/metrics/wrapper.py,sha256=eV2iUvtOViEDqt_o9rw7a3-3tL7XAoKAr1yolViDDWk,11772
 monai/networks/__init__.py,sha256=X-z-kmVt9kwoNPgfYITGycnvG_9HC3_RSRKD2YC35Ag,1020
-monai/networks/utils.py,sha256=smhCOr6f8MssKq7UkHnCt1HzIU9SQnzS0xCrzpbUv18,46286
+monai/networks/utils.py,sha256=TqAZZfRIE0CyNt1FO_PbuuKKjPa9Ye5QkATAd_ergXE,46938
 monai/networks/blocks/__init__.py,sha256=umyJFI-rDAMuseC0gD1vwCE3EowQpWjVfuCLKGFoL1g,2134
 monai/networks/blocks/acti_norm.py,sha256=bVGXbTZ_ssRvmED5R7LOQ7jj4V6WbVFl8JMO-4iZ2Dk,4275
 monai/networks/blocks/activation.py,sha256=S5k3zcP2PsHBkeIxgWgNg8ppW80tTResVP2j9ZsvTFw,5839
 monai/networks/blocks/aspp.py,sha256=GGGE7NfWj77RkaWHbcLuUP4Aff-WeiDrtgtFuSoekQk,4380
-monai/networks/blocks/backbone_fpn_utils.py,sha256=0WDppafm-y8_HeyaFLJI7Hq7wcwcs6nrptGgLbUgXOI,7490
+monai/networks/blocks/backbone_fpn_utils.py,sha256=mdXFwtnRgwuaisTlY-c7OkY1ZZBY3I82dAjpXFAZFbg,7488
 monai/networks/blocks/convolutions.py,sha256=gRmbYfy3IR4taiXuxeH5KGOFjP55FoVWfP4e1L6ai0s,11686
 monai/networks/blocks/crf.py,sha256=gHyRgBWD9DmmbCJnXwsMa6WN7N9fDLuT_SwH8MnHhXE,5009
 monai/networks/blocks/denseblock.py,sha256=5-NOgi8cKzv3M4BhtFpu0tMF7bG2aqxGOI0AiJI9sLs,4740
 monai/networks/blocks/dints_block.py,sha256=-JWz4-nnAjrOxU2oJ86-qN8Krb8FayKS8Zpbp1wLXzc,9255
 monai/networks/blocks/downsample.py,sha256=18cwYXL5H3DC5Yq12cdqTIijDJfMCE2YNHlPetFB6UY,2413
 monai/networks/blocks/dynunet_block.py,sha256=1x0yzDOG71ouHjMgVJgpB5MmOVkmh0o81WleFGI3MiI,11062
 monai/networks/blocks/encoder.py,sha256=NwH5VSQLwamJqrSbZSdQqMwZCk80CPbSpMGEE0r0Cwo,3669
@@ -239,22 +239,23 @@
 monai/networks/blocks/localnet_block.py,sha256=1tUJZh5A0Wlhy0J7kW4Sko7FVTvUjPwHJLqZNeu-O2I,11454
 monai/networks/blocks/mlp.py,sha256=udgUVvHJdyZK2DG3We4zJyNy6eB2zUJfPyI1rUMu1YI,2813
 monai/networks/blocks/patchembedding.py,sha256=gBiMZyXrmmJTR1ystbuV4fSkH-CO0R1oEGJ-jhxipxM,7987
 monai/networks/blocks/regunet_block.py,sha256=1FLIwVBtk66II6xQ7Q4LMY8DP0rMmeftN7HuaEgnf3A,8825
 monai/networks/blocks/segresnet_block.py,sha256=iwzhEJlACvmv3C9LRDkMuDs9DJtYtYAGOyDj9HhlvDg,3245
 monai/networks/blocks/selfattention.py,sha256=FUUxq5LFBHxHQz3WKK8oZK7KVPtyhL2H9PrtYLTIeuw,3099
 monai/networks/blocks/squeeze_and_excitation.py,sha256=y2kXgoSFxywu-KCGYbI_d-NCCAEbuKAIY5gSqO_T7TI,12752
+monai/networks/blocks/text_embedding.py,sha256=H1bI02_WJCn5bBuEcJAREOjm-_kOapORWb5eHmbG8uA,3811
 monai/networks/blocks/transformerblock.py,sha256=GHVjtyTjNskTRrhQzRGvI7uhvUajP_eCmQ97o3qRU3I,2322
 monai/networks/blocks/unetr_block.py,sha256=d_rqE76OFfd3QRcHuor5Zei2pOrupoleBWu3eYUup0c,9049
 monai/networks/blocks/upsample.py,sha256=If8gyKSt6oLVBabNPdPdIa-vhLPd041NdzGEE5xiC-E,13312
 monai/networks/blocks/warp.py,sha256=ATXWLFOVOx06jbCOYKvuuC1e8hXLoDhRwRVO2rYt79Q,6656
 monai/networks/layers/__init__.py,sha256=W5G4vpUDG8m3U5NTxxKhvM8NSHLDaeg1aFfnSolEu2s,1562
 monai/networks/layers/convutils.py,sha256=zwbYK4WJO1Tj2KASnOfxwYnb3p4pizXxdZRm6I1P3j4,8288
 monai/networks/layers/drop_path.py,sha256=SZtRNa1bDwk1rXWbUe70YDaw6H_NKeplm_Wk5Ye1L4Y,1802
-monai/networks/layers/factories.py,sha256=k06YAo6v9cZ5HO61HM7XxK_XedbgA8-d5IrUmWT3s5w,12620
+monai/networks/layers/factories.py,sha256=ASSVHvd1F1rV7mD2wHOUCWTaPclsEYSnhb0nenMq-Tw,12638
 monai/networks/layers/filtering.py,sha256=7ru9Yt3yOM-ko-UqzYp-2tMpb8VHt5d767F-KkzrqYY,17992
 monai/networks/layers/gmm.py,sha256=yndDwTq_q8M_jsgIKvPfAEBAfzftARFy9emrde_rOtU,3324
 monai/networks/layers/simplelayers.py,sha256=ufiioPsyzkCb7uIJCNBvba366z4ZTVK3NSZdI-QRnMA,28470
 monai/networks/layers/spatial_transforms.py,sha256=J0pMm04zvHG605OzSNbT5dtdOWiJDbOsBB_ds8n6PyA,25576
 monai/networks/layers/utils.py,sha256=_387-Au76QG5wwGs7ESg0ocGTcBzw4DJz19H7vrPKjM,4296
 monai/networks/layers/weight_init.py,sha256=ehwI5F7jm_lmDkK4qVL7ocIzCEPx5UPgLaURcsfMNwk,2253
 monai/networks/nets/__init__.py,sha256=Lj_s7D5U_IT5wA-FeTEMeWZHn85YZNL7sYLAmWpOZVE,3141
@@ -278,52 +279,52 @@
 monai/networks/nets/regressor.py,sha256=RDbBCppgOOBid-ISRNE9nDpRcKLMSdD_xFgOVKtGneU,6488
 monai/networks/nets/regunet.py,sha256=RZhLX6o0lqv3IEL2TOadTbypfpAj6yaibMzNb2gSwJQ,17189
 monai/networks/nets/resnet.py,sha256=M7MVLoeiXxN4KXUq42HBCJshYqK37U34zHcQPMHDMm0,16785
 monai/networks/nets/segresnet.py,sha256=xNkSIvdk7kAyc3eVn-U_gGj8MoGVc5nklFKc_fkgOUs,13994
 monai/networks/nets/segresnet_ds.py,sha256=RRHTxsWrxI17282KtoFSEPJeBIcQIOdHeSHQpvUGFY8,15667
 monai/networks/nets/senet.py,sha256=gulqPMYmSABbMbN39NElGzSU1TKGviJas7EPTBaZ60A,19289
 monai/networks/nets/swin_unetr.py,sha256=kV5cSRWxtjTF25mOCSenxRsI0jyvIn1CBxttUCIdWSo,42000
-monai/networks/nets/torchvision_fc.py,sha256=cPQJ8xWl3zXB6YAyCR7BIR2W737GclYw8fqVr6f8LvQ,6248
+monai/networks/nets/torchvision_fc.py,sha256=3g5PD7C1MSkQ8xndhnVd0b3aN8zfshT8uiFS0OHyQaY,6309
 monai/networks/nets/transchex.py,sha256=TpdKj3nH-PWu_2S6JYPiAcjVld7TGPVyt52rKsbm9gY,16626
 monai/networks/nets/unet.py,sha256=CvQMZcHrfQnwfkWlJNRld82rBDNSuCOArYvabMO8YIM,13722
 monai/networks/nets/unetr.py,sha256=6sWCpH8FzITiiqThDgelARZrQVs64cZERcTb690NbJs,7943
 monai/networks/nets/varautoencoder.py,sha256=I8EgeVJWGn0KspyMjAbBFRE3oD67rUqLFH3-p9cbA2c,6285
 monai/networks/nets/vit.py,sha256=PpE7SCdpqO5VhVaUNb_GrIhdUQXbJloJ_afGuPFMSic,5655
 monai/networks/nets/vitautoenc.py,sha256=AmnUQsUrm72z1cbadMYRD-V21ZuK3LxL2oKc10jP2nE,4817
 monai/networks/nets/vnet.py,sha256=6acwIN_NLyW1ANcT8C4Dr7RLCnBPJ2jxJlNbJvxHVdI,10011
 monai/optimizers/__init__.py,sha256=XUL7o9vSL7bZImpxVZqcc1c8MwUMrOZL4nJ-mjAA7yM,796
-monai/optimizers/lr_finder.py,sha256=5OKluV_a71VPNX_7BzFH7vCqcSYPXbuR3XlLwHCaASs,21948
+monai/optimizers/lr_finder.py,sha256=Qn3rxLndSdU5mvB15GMDWXHUCPDV_LggDPlgWEvX70E,21952
 monai/optimizers/lr_scheduler.py,sha256=UJYzkhqxsYkyaisnCu0ba_kcAM6IL-lLskdDtHWOBnc,3652
 monai/optimizers/novograd.py,sha256=KOl3qiwsDg06rbZ48uLZI05kHxXUtwTfHp1P9Yn8Ot0,5661
 monai/optimizers/utils.py,sha256=vDgyMemHQAwAueZlnMIu4HuNJ5BSSEw_Csru2YnudJs,4131
-monai/transforms/__init__.py,sha256=TD6NsLbPLymA6zew4P4sPrrSwBnTtKfH9kzo6Vcfh-A,15216
+monai/transforms/__init__.py,sha256=xyRnpW54Ves5pvSABM_o2iQqAOV_CBepCotJw1Oq_xs,15248
 monai/transforms/adaptors.py,sha256=IxmzJncOfEO2NPzuxP3Z41DZDqa1VLJ19Gz89ks_DyA,8946
-monai/transforms/compose.py,sha256=hDNFTg6vhnYbILozdlHjy0KNmOqUE5PJWRd_mfa_AQs,40532
-monai/transforms/inverse.py,sha256=hXuDcwbJGjoWa5VeL-4vBHN2OkZ98cEZPlNIhi3kptU,17160
+monai/transforms/compose.py,sha256=VYsWkSCfGEkguV9D0NQ3WVHhfZe-vTK-wMgy09_mmNY,40812
+monai/transforms/inverse.py,sha256=4MjvQNUW95xwVHdjRFRs3M8RpZvfLRosKBiED3MhHKs,18000
 monai/transforms/inverse_batch_transform.py,sha256=T1Kl7FQdE9omIm5SCCY9xnxGwaUxyfkgbJEtjB8LEuE,7054
 monai/transforms/nvtx.py,sha256=1EKEXZIhTUFKoIrJmd_fevwrHwo731dVFUFJQFiOk3w,3386
 monai/transforms/traits.py,sha256=HPAfD0ujRS0FYKH6bhwtKikW8Pebwrn9SoC4u7JChLg,2885
 monai/transforms/transform.py,sha256=c8B8bGgg55gpmXf3SBNUlvKyOim0s1rGTgv7RZsiZh4,18234
-monai/transforms/utils.py,sha256=NNKpgYvz7TBbUCLmH1HdXRhGvQyjYdSYuvnsHtrdzV0,71153
+monai/transforms/utils.py,sha256=zO0kp68hG91rqHtKr9aqQ8BB8L-Fx-G41q6E9ViI0P8,72516
 monai/transforms/utils_create_transform_ims.py,sha256=v-MDiukqHkmCGpcRCSZDr14taMcoOuTDeZlL67Wr48E,31081
 monai/transforms/utils_pytorch_numpy_unification.py,sha256=BItSUa0J50ihOXNxxf21C9I-GenjWgoeaKx9EZ0f7Sk,18397
 monai/transforms/croppad/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/transforms/croppad/array.py,sha256=XNgxZ-LUIId5t0rGf_ujo8stzxSfZz95fszyY3OcFk0,68728
+monai/transforms/croppad/array.py,sha256=6xGjAscfgOkqh_88XUpQRrcsLUYdnaTr9LXfMiF7SEw,68231
 monai/transforms/croppad/batch.py,sha256=0JMO2XSwS9LuM1oiogoPl9HfEBpNbcw-OyrUEXFY5rM,6194
 monai/transforms/croppad/dictionary.py,sha256=8IHu2L6rU_RBgIOq_gd4TbKjOThuuXPzkSeAx7Lu9HA,54071
 monai/transforms/croppad/functional.py,sha256=XWJx8URCgkSLBUH3InD48QFcJ_YvAhVC4QNdjrs1c2c,12673
 monai/transforms/intensity/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/intensity/array.py,sha256=GnuSE0yc-YHCNn8BRGzVrMQ50b5rn-GUXHWjFQZH_Qs,98613
 monai/transforms/intensity/dictionary.py,sha256=-W9HVPA2VQUrqplmcI43Qo8EJXgMXARgcRmlhDasM0k,76501
 monai/transforms/io/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/io/array.py,sha256=7DUqkN5P2qYrUOA2wngcltYWAGmWCN45lr3nZMvrxw4,25430
 monai/transforms/io/dictionary.py,sha256=QKQSRnmHLPLZFnmaSERTAUUI3c0J9K4RwSsWv_rts00,17821
 monai/transforms/lazy/__init__.py,sha256=SvkdIlyzIDgO8oaGIrTr1YcLTjh2mZ510ySc9tEbRpk,699
 monai/transforms/lazy/functional.py,sha256=oeHyM_HcL8EhwhCXamEWYUZUlHAXUGKjSsZl1x4URJQ,5552
-monai/transforms/lazy/utils.py,sha256=iNy9RH17_EOAd8F7G2v8oa6FP6L4Jz4aKN_LVUtiNIw,9739
+monai/transforms/lazy/utils.py,sha256=-vco90yMjoKPJb3x3j0arzenLhCvC5Igpl-aPugi_HE,9851
 monai/transforms/meta_utility/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/meta_utility/dictionary.py,sha256=YqbYeZOi4cFEmEPmrw2VIpOIwre6wxYB2UGZSrf-MoM,4896
 monai/transforms/post/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/post/array.py,sha256=Yb_qbOGoaQZFp7CpOA-4iZXvAxz3RtmDlhoPFNh3jWg,40858
 monai/transforms/post/dictionary.py,sha256=OaB9YzrJe0FztM9PETSXNNIihDiad1hnbNqnon7Mp2U,39905
 monai/transforms/signal/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/signal/array.py,sha256=gmTqVYcpsK74UaVbbIjpNFLS1emC_HrQR_AQL0H_GSE,16378
@@ -331,34 +332,34 @@
 monai/transforms/smooth_field/array.py,sha256=T_TfWUDpDi8rQMFuNI6VZNsWPPUUtXM6dkTwz0C34Ow,17833
 monai/transforms/smooth_field/dictionary.py,sha256=iU4V2VjSy2H1K03KgumMUr3cyZVWEJS0W-tgc6SZtP4,11194
 monai/transforms/spatial/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/spatial/array.py,sha256=Kb31oLKWr0Ccn2tKpirQta9_fM2EaMdfKggGkpLoPbI,168618
 monai/transforms/spatial/dictionary.py,sha256=4glbxbo4Cb0SbujSr9Fsk-OOLWR6yxiTQ_6LNcxll-s,107151
 monai/transforms/spatial/functional.py,sha256=Yr5Y93djwatUdoubmj_3I4_NnKF8QoF_X3FnYlTtCoU,31494
 monai/transforms/utility/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/transforms/utility/array.py,sha256=XOmxF_8sMcE7bavWUTjkst_zjx6af6DuUVU7jWueNKU,70325
-monai/transforms/utility/dictionary.py,sha256=MGcIVsjIj8Pm_h_H8txfLQ70IgPFGEUsdL8PYwsig5M,75816
-monai/utils/__init__.py,sha256=CHO02RotqHQrQQWeSwC9boO8PW93ZI3A36O9lkzJBtI,3366
-monai/utils/aliases.py,sha256=21E1KGE6ZMWVYbRMXWVtut2fC9qs7U6QFarxOQa4s6A,4099
+monai/transforms/utility/array.py,sha256=wu_XNG7odigV4bY4uND1tfLRRaJKRdWMH11PMA46f6M,70839
+monai/transforms/utility/dictionary.py,sha256=pxF8__rEeDIl7JHxGdr8Yn_SKE6Zd8jQM8swMi2LVPw,76330
+monai/utils/__init__.py,sha256=MUpVCcMoHgODXXUUg4kub-PL7HkUBjPIFW_O4HNUQj0,3380
+monai/utils/aliases.py,sha256=uBxkLudRfy3Rts9RZo4NDPGoq4e3Ymcaihk6lT92GFo,4096
 monai/utils/decorators.py,sha256=YRK5iEMdbc2INrWnBNDSMTaHge_0ezRf2b9yJGL-opg,3129
 monai/utils/deprecate_utils.py,sha256=gKeEV4MsI51qeQ5gci2me_C-0e-tDwa3VZzd3XPQqLk,14759
 monai/utils/dist.py,sha256=DHLwTqVqFkxP0NbOQ3kkWd-1IQuvf5_rKKABSUQ-Bs0,8526
 monai/utils/enums.py,sha256=ePkeJe5oPVsPJ5QycXyqsLed0DinlX-83bn0rJPH_Mw,16807
 monai/utils/jupyter_utils.py,sha256=F-QSbGDtHnR8FYnh6PsU2hC0nU6GOpGa4GneOeGiP9Y,15637
-monai/utils/misc.py,sha256=t6JGy38QlppWA6cuVsTdJzW1IL4-HGvuJNaNM4a9x5A,27512
+monai/utils/misc.py,sha256=ELcW01mdLYVndHAkh2VkbfEI4llWPlWlv5Kb44JPYGo,28185
 monai/utils/module.py,sha256=G_DwRNvTGxOeFmvNJIAzfDD_Ft7-4dRfkC-5ifW3kEM,23631
 monai/utils/nvtx.py,sha256=i9JBxR1uhW1ZCgLPLlTx8b907QlXkFzJyTBLMlFjhtU,6876
 monai/utils/profiling.py,sha256=HwP5q-OGebATkqPs4IMY6D7jfq2dSVf2AI6Jz_WbBkU,15936
 monai/utils/state_cacher.py,sha256=ERBE-mnnf47MwKSq-pNbfu1D2C4ZqKH-mORyLaBa3EE,5955
 monai/utils/type_conversion.py,sha256=ELgFzH78a2ovAVK4882CFJG1vE0_FLv77tB0lfjxM5w,21147
 monai/visualize/__init__.py,sha256=p7dv9-hRa9vAhlpHyk86yap9HgeDeJRO3pXmFhDx8Mc,1038
 monai/visualize/class_activation_maps.py,sha256=9BXlP-laeqz9rndM08DXZz97NzJcEsFPdC67k0B4CF8,16156
 monai/visualize/gradient_based.py,sha256=UInBLirXMr44xjxJRInlYW8onO3Zv58rDTWrZMDQzMM,6277
 monai/visualize/img2tensorboard.py,sha256=_p5olAefUs6t-y17z0TK32fKxNnUNXVkb0Op1SkfLMM,9200
 monai/visualize/occlusion_sensitivity.py,sha256=g3Au0X6LXoGKY9gPeuNWvNuFtynmPiUWgs_veCEIb_Q,18816
 monai/visualize/utils.py,sha256=xJbG68R-W17aqm0cpmMrypbZaiVfUaG9GWMFtKV7VUo,9966
 monai/visualize/visualizer.py,sha256=qckyaMZCbezYUwE20k5yc-Pb7UozVavMDbrmyQwfYHY,1377
-monai-1.2.0rc4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai-1.2.0rc4.dist-info/METADATA,sha256=fAE0BgtqM3KQTlwTmidpvplbQ6rylinwAJ9O_EalKLA,10172
-monai-1.2.0rc4.dist-info/WHEEL,sha256=4eiHlt0TVen4nP2Hk3uswqTjaQx4-AtDU2XnmdNg0Pw,112
-monai-1.2.0rc4.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai-1.2.0rc4.dist-info/RECORD,,
+monai-1.2.0rc5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai-1.2.0rc5.dist-info/METADATA,sha256=TpRsEXqK_Bhi8UepofvtzCtVX1Rm1mLTdhaQoGIkGq0,10172
+monai-1.2.0rc5.dist-info/WHEEL,sha256=akUX-06y5q3r-m-RPPS1ZNr1Qej84WXuMy5XU8CJZog,112
+monai-1.2.0rc5.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai-1.2.0rc5.dist-info/RECORD,,
```


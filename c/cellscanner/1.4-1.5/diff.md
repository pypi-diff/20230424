# Comparing `tmp/cellscanner-1.4.tar.gz` & `tmp/cellscanner-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellscanner-1.4.tar", last modified: Mon Apr 24 10:10:48 2023, max compression
+gzip compressed data, was "cellscanner-1.5.tar", last modified: Mon Apr 24 10:14:38 2023, max compression
```

## Comparing `cellscanner-1.4.tar` & `cellscanner-1.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.658844 cellscanner-1.4/
--rwxrwxrwx   0 caokangwen   (502) staff       (20)     1062 2022-07-04 05:08:38.000000 cellscanner-1.4/LICENSE
--rw-r--r--   0 caokangwen   (502) staff       (20)      144 2023-04-24 10:10:48.658918 cellscanner-1.4/PKG-INFO
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.638464 cellscanner-1.4/cellscanner.egg-info/
--rw-r--r--   0 caokangwen   (502) staff       (20)      144 2023-04-24 10:10:48.000000 cellscanner-1.4/cellscanner.egg-info/PKG-INFO
--rw-r--r--   0 caokangwen   (502) staff       (20)     3268 2023-04-24 10:10:48.000000 cellscanner-1.4/cellscanner.egg-info/SOURCES.txt
--rw-r--r--   0 caokangwen   (502) staff       (20)        1 2023-04-24 10:10:48.000000 cellscanner-1.4/cellscanner.egg-info/dependency_links.txt
--rw-r--r--   0 caokangwen   (502) staff       (20)       52 2023-04-24 10:10:48.000000 cellscanner-1.4/cellscanner.egg-info/entry_points.txt
--rw-r--r--   0 caokangwen   (502) staff       (20)        4 2023-04-24 10:10:48.000000 cellscanner-1.4/cellscanner.egg-info/top_level.txt
--rwxrwxrwx   0 caokangwen   (502) staff       (20)       79 2023-04-24 10:10:48.659238 cellscanner-1.4/setup.cfg
--rw-r--r--   0 caokangwen   (502) staff       (20)      345 2023-04-24 10:10:45.000000 cellscanner-1.4/setup.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.639335 cellscanner-1.4/src/
--rw-r--r--   0 caokangwen   (502) staff       (20)    21739 2023-04-24 10:04:02.000000 cellscanner-1.4/src/MainWindow.py
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-24 09:57:19.000000 cellscanner-1.4/src/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)       19 2023-04-24 01:33:21.000000 cellscanner-1.4/src/debug.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     9493 2023-04-23 12:19:30.000000 cellscanner-1.4/src/expplot.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.640546 cellscanner-1.4/src/labelme_local/
--rw-rw-r--   0 caokangwen   (502) staff       (20)      627 2023-04-04 04:46:26.000000 cellscanner-1.4/src/labelme_local/__init__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     6299 2023-04-04 04:47:01.000000 cellscanner-1.4/src/labelme_local/__main__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)    73709 2023-04-24 09:58:08.000000 cellscanner-1.4/src/labelme_local/app.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.641160 cellscanner-1.4/src/labelme_local/cli/
--rw-rw-r--   0 caokangwen   (502) staff       (20)      123 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/cli/__init__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     1345 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/cli/draw_json.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      636 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/cli/draw_label_png.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2388 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/cli/json_to_dataset.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2761 2023-04-04 04:46:26.000000 cellscanner-1.4/src/labelme_local/cli/on_docker.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.641291 cellscanner-1.4/src/labelme_local/config/
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2698 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/config/__init__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     6360 2023-04-04 04:46:26.000000 cellscanner-1.4/src/labelme_local/label_file.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     1836 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/logger.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     9317 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/shape.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      849 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/testing.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.641971 cellscanner-1.4/src/labelme_local/utils/
--rw-rw-r--   0 caokangwen   (502) staff       (20)      722 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/utils/__init__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      675 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/utils/_io.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2367 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/utils/image.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2525 2023-04-03 10:24:36.000000 cellscanner-1.4/src/labelme_local/utils/qt.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     3650 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/utils/shape.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.643468 cellscanner-1.4/src/labelme_local/widgets/
--rw-rw-r--   0 caokangwen   (502) staff       (20)      510 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/__init__.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     1468 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/brightness_contrast_dialog.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)    33599 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/canvas.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     1200 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/color_dialog.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      281 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/escapable_qlist_widget.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     2434 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/file_dialog_preview.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     8150 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/label_dialog.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     5792 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/label_list_widget.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      970 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/tool_bar.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)     1374 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/unique_label_qlist_widget.py
--rw-rw-r--   0 caokangwen   (502) staff       (20)      712 2022-11-20 07:09:36.000000 cellscanner-1.4/src/labelme_local/widgets/zoom_widget.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     5166 2023-04-04 04:46:26.000000 cellscanner-1.4/src/labelme_local/wind.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    17169 2023-04-24 09:58:08.000000 cellscanner-1.4/src/utils.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    53256 2023-04-24 10:10:13.000000 cellscanner-1.4/src/widgets.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.646166 cellscanner-1.4/src/yolov_res/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-02 12:22:20.000000 cellscanner-1.4/src/yolov_res/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     1491 2023-04-11 12:40:20.000000 cellscanner-1.4/src/yolov_res/debug.py
--rw-r-----   0 caokangwen   (502) staff       (20)    10193 2023-04-02 12:50:26.000000 cellscanner-1.4/src/yolov_res/detect.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    13591 2023-02-06 04:15:35.000000 cellscanner-1.4/src/yolov_res/detect_01.py
--rw-rw-rw-   0 caokangwen   (502) staff       (20)    15373 2023-04-11 12:42:59.000000 cellscanner-1.4/src/yolov_res/detect_yocls.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    16092 2023-04-02 13:04:31.000000 cellscanner-1.4/src/yolov_res/detect_yocls_01.py
--rw-r-----   0 caokangwen   (502) staff       (20)    16949 2023-03-25 05:09:18.000000 cellscanner-1.4/src/yolov_res/detect_yocls_batch.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    16998 2023-03-08 12:12:04.000000 cellscanner-1.4/src/yolov_res/detect_yocls_batch_01.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    30598 2023-04-02 13:06:48.000000 cellscanner-1.4/src/yolov_res/export.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     6608 2023-04-02 12:22:58.000000 cellscanner-1.4/src/yolov_res/hubconf.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     2690 2023-04-02 12:22:58.000000 cellscanner-1.4/src/yolov_res/make_prediction.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.646955 cellscanner-1.4/src/yolov_res/model_cls/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:15:40.000000 cellscanner-1.4/src/yolov_res/model_cls/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     3891 2023-02-06 04:16:20.000000 cellscanner-1.4/src/yolov_res/model_cls/cnm.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    12058 2023-02-06 04:15:41.000000 cellscanner-1.4/src/yolov_res/model_cls/dataset.py
--rw-r--r--   0 caokangwen   (502) staff       (20)      381 2023-02-06 04:15:40.000000 cellscanner-1.4/src/yolov_res/model_cls/plot.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     5333 2023-02-06 04:15:40.000000 cellscanner-1.4/src/yolov_res/model_cls/resnet.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     7266 2023-04-24 10:04:30.000000 cellscanner-1.4/src/yolov_res/model_cls/train.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.647786 cellscanner-1.4/src/yolov_res/models/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:58.000000 cellscanner-1.4/src/yolov_res/models/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    36107 2023-04-02 12:49:46.000000 cellscanner-1.4/src/yolov_res/models/common.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     4270 2023-04-02 13:05:22.000000 cellscanner-1.4/src/yolov_res/models/experimental.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    26076 2023-02-06 04:42:58.000000 cellscanner-1.4/src/yolov_res/models/tf.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    15752 2023-04-02 13:05:48.000000 cellscanner-1.4/src/yolov_res/models/yolo.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     4955 2023-04-04 04:46:26.000000 cellscanner-1.4/src/yolov_res/pipeline.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     6039 2023-04-04 04:46:26.000000 cellscanner-1.4/src/yolov_res/pipelinetool.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    35709 2023-04-11 12:46:43.000000 cellscanner-1.4/src/yolov_res/train.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     2464 2023-04-19 06:37:58.000000 cellscanner-1.4/src/yolov_res/train_2step.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    38597 2023-04-19 06:43:04.000000 cellscanner-1.4/src/yolov_res/train_django.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.651331 cellscanner-1.4/src/yolov_res/utils/
--rw-r--r--   0 caokangwen   (502) staff       (20)     1093 2023-02-06 04:42:42.000000 cellscanner-1.4/src/yolov_res/utils/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     3552 2023-02-06 04:42:41.000000 cellscanner-1.4/src/yolov_res/utils/activations.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    12214 2023-04-02 12:49:53.000000 cellscanner-1.4/src/yolov_res/utils/augmentations.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     7623 2023-04-02 13:06:03.000000 cellscanner-1.4/src/yolov_res/utils/autoanchor.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     2686 2023-04-11 12:47:03.000000 cellscanner-1.4/src/yolov_res/utils/autobatch.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.652223 cellscanner-1.4/src/yolov_res/utils/aws/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:55.000000 cellscanner-1.4/src/yolov_res/utils/aws/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     1238 2023-02-06 04:42:56.000000 cellscanner-1.4/src/yolov_res/utils/aws/resume.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     6473 2023-02-06 04:42:44.000000 cellscanner-1.4/src/yolov_res/utils/benchmarks.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     2473 2023-02-06 04:42:43.000000 cellscanner-1.4/src/yolov_res/utils/callbacks.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    48771 2023-04-19 06:26:24.000000 cellscanner-1.4/src/yolov_res/utils/dataloaders.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    48899 2023-04-19 06:04:14.000000 cellscanner-1.4/src/yolov_res/utils/dataloaders_list.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    45905 2023-04-02 12:50:34.000000 cellscanner-1.4/src/yolov_res/utils/datasets.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     7299 2023-04-02 13:07:01.000000 cellscanner-1.4/src/yolov_res/utils/downloads.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.653336 cellscanner-1.4/src/yolov_res/utils/flask_rest_api/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-02 12:22:20.000000 cellscanner-1.4/src/yolov_res/utils/flask_rest_api/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)      387 2023-02-06 04:42:55.000000 cellscanner-1.4/src/yolov_res/utils/flask_rest_api/example_request.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     1456 2023-02-06 04:42:55.000000 cellscanner-1.4/src/yolov_res/utils/flask_rest_api/restapi.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    42882 2023-04-19 05:25:01.000000 cellscanner-1.4/src/yolov_res/utils/general.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.653644 cellscanner-1.4/src/yolov_res/utils/loggers/
--rw-r--r--   0 caokangwen   (502) staff       (20)     8322 2023-04-11 12:54:58.000000 cellscanner-1.4/src/yolov_res/utils/loggers/__init__.py
-drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:10:48.657589 cellscanner-1.4/src/yolov_res/utils/loggers/wandb/
--rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:45.000000 cellscanner-1.4/src/yolov_res/utils/loggers/wandb/__init__.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     1059 2023-02-06 04:42:46.000000 cellscanner-1.4/src/yolov_res/utils/loggers/wandb/log_dataset.py
--rw-r--r--   0 caokangwen   (502) staff       (20)     1254 2023-02-06 04:42:45.000000 cellscanner-1.4/src/yolov_res/utils/loggers/wandb/sweep.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    28183 2023-04-11 12:55:05.000000 cellscanner-1.4/src/yolov_res/utils/loggers/wandb/wandb_utils.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    10173 2023-04-11 12:55:11.000000 cellscanner-1.4/src/yolov_res/utils/loss.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    14716 2023-02-06 04:42:43.000000 cellscanner-1.4/src/yolov_res/utils/metrics.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    21530 2023-04-02 12:50:14.000000 cellscanner-1.4/src/yolov_res/utils/plots.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    13886 2023-04-02 12:50:04.000000 cellscanner-1.4/src/yolov_res/utils/torch_utils.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    19906 2023-04-11 12:46:23.000000 cellscanner-1.4/src/yolov_res/val.py
--rw-r-----   0 caokangwen   (502) staff       (20)    20641 2023-03-25 13:03:56.000000 cellscanner-1.4/src/yolov_res/val_map.py
--rw-r--r--   0 caokangwen   (502) staff       (20)    20727 2023-03-24 04:57:57.000000 cellscanner-1.4/src/yolov_res/val_map_01.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.217772 cellscanner-1.5/
+-rwxrwxrwx   0 caokangwen   (502) staff       (20)     1062 2022-07-04 05:08:38.000000 cellscanner-1.5/LICENSE
+-rw-r--r--   0 caokangwen   (502) staff       (20)      144 2023-04-24 10:14:38.217838 cellscanner-1.5/PKG-INFO
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.206781 cellscanner-1.5/cellscanner.egg-info/
+-rw-r--r--   0 caokangwen   (502) staff       (20)      144 2023-04-24 10:14:38.000000 cellscanner-1.5/cellscanner.egg-info/PKG-INFO
+-rw-r--r--   0 caokangwen   (502) staff       (20)     3268 2023-04-24 10:14:38.000000 cellscanner-1.5/cellscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 caokangwen   (502) staff       (20)        1 2023-04-24 10:14:38.000000 cellscanner-1.5/cellscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 caokangwen   (502) staff       (20)       52 2023-04-24 10:14:38.000000 cellscanner-1.5/cellscanner.egg-info/entry_points.txt
+-rw-r--r--   0 caokangwen   (502) staff       (20)        4 2023-04-24 10:14:38.000000 cellscanner-1.5/cellscanner.egg-info/top_level.txt
+-rwxrwxrwx   0 caokangwen   (502) staff       (20)       79 2023-04-24 10:14:38.218047 cellscanner-1.5/setup.cfg
+-rw-r--r--   0 caokangwen   (502) staff       (20)      345 2023-04-24 10:14:23.000000 cellscanner-1.5/setup.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.207589 cellscanner-1.5/src/
+-rw-r--r--   0 caokangwen   (502) staff       (20)    21739 2023-04-24 10:04:02.000000 cellscanner-1.5/src/MainWindow.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-24 09:57:19.000000 cellscanner-1.5/src/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)       19 2023-04-24 01:33:21.000000 cellscanner-1.5/src/debug.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     9493 2023-04-23 12:19:30.000000 cellscanner-1.5/src/expplot.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.208617 cellscanner-1.5/src/labelme_local/
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      627 2023-04-04 04:46:26.000000 cellscanner-1.5/src/labelme_local/__init__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     6299 2023-04-04 04:47:01.000000 cellscanner-1.5/src/labelme_local/__main__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)    73709 2023-04-24 09:58:08.000000 cellscanner-1.5/src/labelme_local/app.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.209221 cellscanner-1.5/src/labelme_local/cli/
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      123 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/cli/__init__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     1345 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/cli/draw_json.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      636 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/cli/draw_label_png.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2388 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/cli/json_to_dataset.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2761 2023-04-04 04:46:26.000000 cellscanner-1.5/src/labelme_local/cli/on_docker.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.209350 cellscanner-1.5/src/labelme_local/config/
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2698 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/config/__init__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     6360 2023-04-04 04:46:26.000000 cellscanner-1.5/src/labelme_local/label_file.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     1836 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/logger.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     9317 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/shape.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      849 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/testing.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.209936 cellscanner-1.5/src/labelme_local/utils/
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      722 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/utils/__init__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      675 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/utils/_io.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2367 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/utils/image.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2525 2023-04-03 10:24:36.000000 cellscanner-1.5/src/labelme_local/utils/qt.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     3650 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/utils/shape.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.211254 cellscanner-1.5/src/labelme_local/widgets/
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      510 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/__init__.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     1468 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/brightness_contrast_dialog.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)    33599 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/canvas.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     1200 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/color_dialog.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      281 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/escapable_qlist_widget.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     2434 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/file_dialog_preview.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     8150 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/label_dialog.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     5792 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/label_list_widget.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      970 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/tool_bar.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)     1374 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/unique_label_qlist_widget.py
+-rw-rw-r--   0 caokangwen   (502) staff       (20)      712 2022-11-20 07:09:36.000000 cellscanner-1.5/src/labelme_local/widgets/zoom_widget.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     5166 2023-04-04 04:46:26.000000 cellscanner-1.5/src/labelme_local/wind.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    17127 2023-04-24 10:13:52.000000 cellscanner-1.5/src/utils.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    53256 2023-04-24 10:10:13.000000 cellscanner-1.5/src/widgets.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.213525 cellscanner-1.5/src/yolov_res/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-02 12:22:20.000000 cellscanner-1.5/src/yolov_res/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1491 2023-04-11 12:40:20.000000 cellscanner-1.5/src/yolov_res/debug.py
+-rw-r-----   0 caokangwen   (502) staff       (20)    10193 2023-04-02 12:50:26.000000 cellscanner-1.5/src/yolov_res/detect.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    13591 2023-02-06 04:15:35.000000 cellscanner-1.5/src/yolov_res/detect_01.py
+-rw-rw-rw-   0 caokangwen   (502) staff       (20)    15373 2023-04-11 12:42:59.000000 cellscanner-1.5/src/yolov_res/detect_yocls.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    16092 2023-04-02 13:04:31.000000 cellscanner-1.5/src/yolov_res/detect_yocls_01.py
+-rw-r-----   0 caokangwen   (502) staff       (20)    16949 2023-03-25 05:09:18.000000 cellscanner-1.5/src/yolov_res/detect_yocls_batch.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    16998 2023-03-08 12:12:04.000000 cellscanner-1.5/src/yolov_res/detect_yocls_batch_01.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    30598 2023-04-02 13:06:48.000000 cellscanner-1.5/src/yolov_res/export.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     6608 2023-04-02 12:22:58.000000 cellscanner-1.5/src/yolov_res/hubconf.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     2690 2023-04-02 12:22:58.000000 cellscanner-1.5/src/yolov_res/make_prediction.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.214186 cellscanner-1.5/src/yolov_res/model_cls/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:15:40.000000 cellscanner-1.5/src/yolov_res/model_cls/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     3891 2023-02-06 04:16:20.000000 cellscanner-1.5/src/yolov_res/model_cls/cnm.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    12058 2023-02-06 04:15:41.000000 cellscanner-1.5/src/yolov_res/model_cls/dataset.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)      381 2023-02-06 04:15:40.000000 cellscanner-1.5/src/yolov_res/model_cls/plot.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     5333 2023-02-06 04:15:40.000000 cellscanner-1.5/src/yolov_res/model_cls/resnet.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     7266 2023-04-24 10:04:30.000000 cellscanner-1.5/src/yolov_res/model_cls/train.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.214756 cellscanner-1.5/src/yolov_res/models/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:58.000000 cellscanner-1.5/src/yolov_res/models/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    36107 2023-04-02 12:49:46.000000 cellscanner-1.5/src/yolov_res/models/common.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     4270 2023-04-02 13:05:22.000000 cellscanner-1.5/src/yolov_res/models/experimental.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    26076 2023-02-06 04:42:58.000000 cellscanner-1.5/src/yolov_res/models/tf.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    15752 2023-04-02 13:05:48.000000 cellscanner-1.5/src/yolov_res/models/yolo.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     4955 2023-04-04 04:46:26.000000 cellscanner-1.5/src/yolov_res/pipeline.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     6039 2023-04-04 04:46:26.000000 cellscanner-1.5/src/yolov_res/pipelinetool.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    35709 2023-04-11 12:46:43.000000 cellscanner-1.5/src/yolov_res/train.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     2464 2023-04-19 06:37:58.000000 cellscanner-1.5/src/yolov_res/train_2step.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    38597 2023-04-19 06:43:04.000000 cellscanner-1.5/src/yolov_res/train_django.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.216596 cellscanner-1.5/src/yolov_res/utils/
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1093 2023-02-06 04:42:42.000000 cellscanner-1.5/src/yolov_res/utils/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     3552 2023-02-06 04:42:41.000000 cellscanner-1.5/src/yolov_res/utils/activations.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    12214 2023-04-02 12:49:53.000000 cellscanner-1.5/src/yolov_res/utils/augmentations.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     7623 2023-04-02 13:06:03.000000 cellscanner-1.5/src/yolov_res/utils/autoanchor.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     2686 2023-04-11 12:47:03.000000 cellscanner-1.5/src/yolov_res/utils/autobatch.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.216798 cellscanner-1.5/src/yolov_res/utils/aws/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:55.000000 cellscanner-1.5/src/yolov_res/utils/aws/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1238 2023-02-06 04:42:56.000000 cellscanner-1.5/src/yolov_res/utils/aws/resume.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     6473 2023-02-06 04:42:44.000000 cellscanner-1.5/src/yolov_res/utils/benchmarks.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     2473 2023-02-06 04:42:43.000000 cellscanner-1.5/src/yolov_res/utils/callbacks.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    48771 2023-04-19 06:26:24.000000 cellscanner-1.5/src/yolov_res/utils/dataloaders.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    48899 2023-04-19 06:04:14.000000 cellscanner-1.5/src/yolov_res/utils/dataloaders_list.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    45905 2023-04-02 12:50:34.000000 cellscanner-1.5/src/yolov_res/utils/datasets.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     7299 2023-04-02 13:07:01.000000 cellscanner-1.5/src/yolov_res/utils/downloads.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.217109 cellscanner-1.5/src/yolov_res/utils/flask_rest_api/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-04-02 12:22:20.000000 cellscanner-1.5/src/yolov_res/utils/flask_rest_api/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)      387 2023-02-06 04:42:55.000000 cellscanner-1.5/src/yolov_res/utils/flask_rest_api/example_request.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1456 2023-02-06 04:42:55.000000 cellscanner-1.5/src/yolov_res/utils/flask_rest_api/restapi.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    42882 2023-04-19 05:25:01.000000 cellscanner-1.5/src/yolov_res/utils/general.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.217213 cellscanner-1.5/src/yolov_res/utils/loggers/
+-rw-r--r--   0 caokangwen   (502) staff       (20)     8322 2023-04-11 12:54:58.000000 cellscanner-1.5/src/yolov_res/utils/loggers/__init__.py
+drwxr-xr-x   0 caokangwen   (502) staff       (20)        0 2023-04-24 10:14:38.217645 cellscanner-1.5/src/yolov_res/utils/loggers/wandb/
+-rw-r--r--   0 caokangwen   (502) staff       (20)        0 2023-02-06 04:42:45.000000 cellscanner-1.5/src/yolov_res/utils/loggers/wandb/__init__.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1059 2023-02-06 04:42:46.000000 cellscanner-1.5/src/yolov_res/utils/loggers/wandb/log_dataset.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)     1254 2023-02-06 04:42:45.000000 cellscanner-1.5/src/yolov_res/utils/loggers/wandb/sweep.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    28183 2023-04-11 12:55:05.000000 cellscanner-1.5/src/yolov_res/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    10173 2023-04-11 12:55:11.000000 cellscanner-1.5/src/yolov_res/utils/loss.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    14716 2023-02-06 04:42:43.000000 cellscanner-1.5/src/yolov_res/utils/metrics.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    21530 2023-04-02 12:50:14.000000 cellscanner-1.5/src/yolov_res/utils/plots.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    13886 2023-04-02 12:50:04.000000 cellscanner-1.5/src/yolov_res/utils/torch_utils.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    19906 2023-04-11 12:46:23.000000 cellscanner-1.5/src/yolov_res/val.py
+-rw-r-----   0 caokangwen   (502) staff       (20)    20641 2023-03-25 13:03:56.000000 cellscanner-1.5/src/yolov_res/val_map.py
+-rw-r--r--   0 caokangwen   (502) staff       (20)    20727 2023-03-24 04:57:57.000000 cellscanner-1.5/src/yolov_res/val_map_01.py
```

### Comparing `cellscanner-1.4/LICENSE` & `cellscanner-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/cellscanner.egg-info/SOURCES.txt` & `cellscanner-1.5/cellscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/MainWindow.py` & `cellscanner-1.5/src/MainWindow.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/expplot.py` & `cellscanner-1.5/src/expplot.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/__init__.py` & `cellscanner-1.5/src/labelme_local/__init__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/__main__.py` & `cellscanner-1.5/src/labelme_local/__main__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/app.py` & `cellscanner-1.5/src/labelme_local/app.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/cli/draw_json.py` & `cellscanner-1.5/src/labelme_local/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/cli/draw_label_png.py` & `cellscanner-1.5/src/labelme_local/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/cli/json_to_dataset.py` & `cellscanner-1.5/src/labelme_local/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/cli/on_docker.py` & `cellscanner-1.5/src/labelme_local/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/config/__init__.py` & `cellscanner-1.5/src/labelme_local/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/label_file.py` & `cellscanner-1.5/src/labelme_local/label_file.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/logger.py` & `cellscanner-1.5/src/labelme_local/logger.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/shape.py` & `cellscanner-1.5/src/labelme_local/shape.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/testing.py` & `cellscanner-1.5/src/labelme_local/testing.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/utils/__init__.py` & `cellscanner-1.5/src/labelme_local/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/utils/_io.py` & `cellscanner-1.5/src/labelme_local/utils/_io.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/utils/image.py` & `cellscanner-1.5/src/labelme_local/utils/image.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/utils/qt.py` & `cellscanner-1.5/src/labelme_local/utils/qt.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/utils/shape.py` & `cellscanner-1.5/src/labelme_local/utils/shape.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/brightness_contrast_dialog.py` & `cellscanner-1.5/src/labelme_local/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/canvas.py` & `cellscanner-1.5/src/labelme_local/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/color_dialog.py` & `cellscanner-1.5/src/labelme_local/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/file_dialog_preview.py` & `cellscanner-1.5/src/labelme_local/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/label_dialog.py` & `cellscanner-1.5/src/labelme_local/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/label_list_widget.py` & `cellscanner-1.5/src/labelme_local/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/tool_bar.py` & `cellscanner-1.5/src/labelme_local/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/unique_label_qlist_widget.py` & `cellscanner-1.5/src/labelme_local/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/widgets/zoom_widget.py` & `cellscanner-1.5/src/labelme_local/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/labelme_local/wind.py` & `cellscanner-1.5/src/labelme_local/wind.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/utils.py` & `cellscanner-1.5/src/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import os.path
 
 import numpy as np
 import cv2
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 
-from yolov_res.model_cls import train as train_res
-from yolov_res import detect, detect_yocls_01, train_2step, train_django
-from labelme_local import __main__ as labelme_main
+from src.yolov_res.model_cls import train as train_res
+from src.yolov_res import detect, detect_yocls_01, train_2step, train_django
+
 from src import expplot
 
 
 def Yores_detect(
 		source,
 		yolo_weight,
 		output_dir,
```

### Comparing `cellscanner-1.4/src/widgets.py` & `cellscanner-1.5/src/widgets.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/debug.py` & `cellscanner-1.5/src/yolov_res/debug.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect.py` & `cellscanner-1.5/src/yolov_res/detect.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect_01.py` & `cellscanner-1.5/src/yolov_res/detect_01.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect_yocls.py` & `cellscanner-1.5/src/yolov_res/detect_yocls.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect_yocls_01.py` & `cellscanner-1.5/src/yolov_res/detect_yocls_01.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect_yocls_batch.py` & `cellscanner-1.5/src/yolov_res/detect_yocls_batch.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/detect_yocls_batch_01.py` & `cellscanner-1.5/src/yolov_res/detect_yocls_batch_01.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/export.py` & `cellscanner-1.5/src/yolov_res/export.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/hubconf.py` & `cellscanner-1.5/src/yolov_res/hubconf.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/make_prediction.py` & `cellscanner-1.5/src/yolov_res/make_prediction.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/model_cls/cnm.py` & `cellscanner-1.5/src/yolov_res/model_cls/cnm.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/model_cls/dataset.py` & `cellscanner-1.5/src/yolov_res/model_cls/dataset.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/model_cls/resnet.py` & `cellscanner-1.5/src/yolov_res/model_cls/resnet.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/model_cls/train.py` & `cellscanner-1.5/src/yolov_res/model_cls/train.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/models/common.py` & `cellscanner-1.5/src/yolov_res/models/common.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/models/experimental.py` & `cellscanner-1.5/src/yolov_res/models/experimental.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/models/tf.py` & `cellscanner-1.5/src/yolov_res/models/tf.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/models/yolo.py` & `cellscanner-1.5/src/yolov_res/models/yolo.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/pipeline.py` & `cellscanner-1.5/src/yolov_res/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/pipelinetool.py` & `cellscanner-1.5/src/yolov_res/pipelinetool.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/train.py` & `cellscanner-1.5/src/yolov_res/train.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/train_2step.py` & `cellscanner-1.5/src/yolov_res/train_2step.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/train_django.py` & `cellscanner-1.5/src/yolov_res/train_django.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/__init__.py` & `cellscanner-1.5/src/yolov_res/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/activations.py` & `cellscanner-1.5/src/yolov_res/utils/activations.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/augmentations.py` & `cellscanner-1.5/src/yolov_res/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/autoanchor.py` & `cellscanner-1.5/src/yolov_res/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/autobatch.py` & `cellscanner-1.5/src/yolov_res/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/aws/resume.py` & `cellscanner-1.5/src/yolov_res/utils/aws/resume.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/benchmarks.py` & `cellscanner-1.5/src/yolov_res/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/callbacks.py` & `cellscanner-1.5/src/yolov_res/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/dataloaders.py` & `cellscanner-1.5/src/yolov_res/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/dataloaders_list.py` & `cellscanner-1.5/src/yolov_res/utils/dataloaders_list.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/datasets.py` & `cellscanner-1.5/src/yolov_res/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/downloads.py` & `cellscanner-1.5/src/yolov_res/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/flask_rest_api/restapi.py` & `cellscanner-1.5/src/yolov_res/utils/flask_rest_api/restapi.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/general.py` & `cellscanner-1.5/src/yolov_res/utils/general.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/loggers/__init__.py` & `cellscanner-1.5/src/yolov_res/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/loggers/wandb/log_dataset.py` & `cellscanner-1.5/src/yolov_res/utils/loggers/wandb/log_dataset.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/loggers/wandb/sweep.py` & `cellscanner-1.5/src/yolov_res/utils/loggers/wandb/sweep.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/loggers/wandb/wandb_utils.py` & `cellscanner-1.5/src/yolov_res/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/loss.py` & `cellscanner-1.5/src/yolov_res/utils/loss.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/metrics.py` & `cellscanner-1.5/src/yolov_res/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/plots.py` & `cellscanner-1.5/src/yolov_res/utils/plots.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/utils/torch_utils.py` & `cellscanner-1.5/src/yolov_res/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/val.py` & `cellscanner-1.5/src/yolov_res/val.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/val_map.py` & `cellscanner-1.5/src/yolov_res/val_map.py`

 * *Files identical despite different names*

### Comparing `cellscanner-1.4/src/yolov_res/val_map_01.py` & `cellscanner-1.5/src/yolov_res/val_map_01.py`

 * *Files identical despite different names*


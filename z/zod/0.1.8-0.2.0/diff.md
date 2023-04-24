# Comparing `tmp/zod-0.1.8.tar.gz` & `tmp/zod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.1.8.tar", max compression
+gzip compressed data, was "zod-0.2.0.tar", max compression
```

## Comparing `zod-0.1.8.tar` & `zod-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     1073 2023-04-13 12:11:08.669985 zod-0.1.8/LICENSE
--rw-r--r--   0        0        0     4501 2023-04-13 12:11:08.669985 zod-0.1.8/README.md
--rw-r--r--   0        0        0     1683 2023-04-13 12:11:08.669985 zod-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      982 2023-04-13 12:11:08.673985 zod-0.1.8/zod/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-13 12:11:08.673985 zod-0.1.8/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/object.py
--rw-r--r--   0        0        0     2446 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-04-13 12:11:08.673985 zod-0.1.8/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14001 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/download_zod.py
--rw-r--r--   0        0        0     6619 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1733 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-04-13 12:11:08.673985 zod-0.1.8/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2146 2023-04-13 12:11:08.673985 zod-0.1.8/zod/constants.py
--rw-r--r--   0        0        0      184 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5063 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     5516 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5562 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     3610 2023-04-13 12:11:08.673985 zod-0.1.8/zod/data_classes/sequence.py
--rw-r--r--   0        0        0       65 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-04-13 12:11:08.673985 zod-0.1.8/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/geometry.py
--rw-r--r--   0        0        0      978 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-04-13 12:11:08.677985 zod-0.1.8/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     6028 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-04-13 12:11:08.677985 zod-0.1.8/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-04-13 12:11:08.677985 zod-0.1.8/zod/zod_sequences.py
--rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 zod-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 09:13:17.585292 zod-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4501 2023-04-24 09:13:17.585292 zod-0.2.0/README.md
+-rw-r--r--   0        0        0     1683 2023-04-24 09:13:17.585292 zod-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-04-24 09:13:17.585292 zod-0.2.0/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-04-24 09:13:17.585292 zod-0.2.0/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-04-24 09:13:17.585292 zod-0.2.0/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-04-24 09:13:17.589293 zod-0.2.0/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-04-24 09:13:17.589293 zod-0.2.0/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-04-24 09:13:17.589293 zod-0.2.0/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-04-24 09:13:17.589293 zod-0.2.0/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-04-24 09:13:17.589293 zod-0.2.0/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14033 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7365 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-04-24 09:13:17.589293 zod-0.2.0/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-04-24 09:13:17.589293 zod-0.2.0/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4847 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-04-24 09:13:17.589293 zod-0.2.0/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-04-24 09:13:17.589293 zod-0.2.0/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-04-24 09:13:17.589293 zod-0.2.0/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-04-24 09:13:17.589293 zod-0.2.0/zod/utils/geometry.py
+-rw-r--r--   0        0        0      978 2023-04-24 09:13:17.589293 zod-0.2.0/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-04-24 09:13:17.589293 zod-0.2.0/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-04-24 09:13:17.589293 zod-0.2.0/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     6028 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-04-24 09:13:17.589293 zod-0.2.0/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-04-24 09:13:17.589293 zod-0.2.0/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-04-24 09:13:17.589293 zod-0.2.0/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-04-24 09:13:17.589293 zod-0.2.0/zod/zod_sequences.py
+-rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 zod-0.2.0/PKG-INFO
```

### Comparing `zod-0.1.8/LICENSE` & `zod-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/README.md` & `zod-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/pyproject.toml` & `zod-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.1.8"
+version = "0.2.0"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.1.8/zod/__init__.py` & `zod-0.2.0/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/_zod_dataset.py` & `zod-0.2.0/zod/_zod_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """ZOD Frames module."""
 import json
 import os.path as osp
 from abc import ABC, abstractmethod
 from functools import partial
 from itertools import chain
-from typing import Any, Dict, Set, Tuple, Union
+from typing import Any, Dict, Optional, Set, Tuple, Union
 
 from tqdm.contrib.concurrent import process_map
 
-from zod.constants import FULL, TRAIN, VAL, VERSIONS
+from zod.constants import FULL, TRAIN, VAL, VERSIONS, AnnotationProject, Split, Version
 from zod.data_classes.info import Information
 from zod.utils.utils import zfill_id
 
 
 def _create_frame(frame: dict, dataset_root: str) -> Information:
     info = Information.from_dict(frame)
     info.convert_paths_to_absolute(dataset_root)
     return info
 
 
 class ZodDataset(ABC):
     """Base class for all ZOD sub-datasets (frames, sequences, drives)."""
 
-    def __init__(self, dataset_root: str, version: str, mp: bool = True):
+    def __init__(self, dataset_root: str, version: Version, mp: bool = True):
         self._dataset_root = dataset_root
         self._version = version
         self._mp = mp
         assert version in VERSIONS, f"Unknown version: {version}, must be one of: {VERSIONS}"
         self._infos, self._train_ids, self._val_ids = self._load_infos()
 
     def __len__(self) -> int:
@@ -48,35 +48,48 @@
 
     @property
     @abstractmethod
     def trainval_files(self) -> Dict[str, str]:
         """Mapping of version to trainval file."""
         raise NotImplementedError
 
-    def get_split(self, split: str) -> Set[str]:
+    def get_split(self, split: Split, project: Optional[AnnotationProject] = None) -> Set[str]:
         """Get split by name (e.g. train / val)."""
         if split == TRAIN:
-            return self._train_ids
+            ids = self._train_ids
         elif split == VAL:
-            return self._val_ids
+            ids = self._val_ids
         else:
             raise ValueError(f"Unknown split: {split}, should be {TRAIN} or {VAL}")
 
+        if project is None:
+            return ids
+        else:
+            return {id_ for id_ in ids if project in self._infos[id_].annotations}
+
     def get_all_infos(self) -> Dict[str, Information]:
         """Get all infos (including blacklisted ones)."""
         return self._infos
 
     def get_all_ids(self) -> Set[str]:
         """Get all frame ids (excluding blackisted ones)."""
         return self._train_ids.union(self._val_ids)
 
     def _load_infos(self) -> Tuple[Dict[str, Information], Set[str], Set[str]]:
         """Load frames for the given version."""
-        filename = self.trainval_files[self._version]
-        with open(osp.join(self._dataset_root, filename), "r") as f:
+        trainval_path = osp.join(self._dataset_root, self.trainval_files[self._version])
+        if not osp.exists(trainval_path):
+            msg = f"Could not find trainval file: {trainval_path}."
+            if osp.exists(trainval_path.replace("-", "_")):
+                msg += (
+                    "However, found old, incompatible trainval files. Please either downgrade zod "
+                    "to < 0.2 or download new files with `zod download --no-images --no-lidar`"
+                )
+            raise FileNotFoundError(msg)
+        with open(trainval_path, "r") as f:
             all_ids = json.load(f)
 
         func = partial(_create_frame, dataset_root=self._dataset_root)
         if self._mp and self._version == FULL:
             infos = process_map(
                 func,
                 chain.from_iterable(all_ids.values()),
```

### Comparing `zod-0.1.8/zod/anno/lane.py` & `zod-0.2.0/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/anno/object.py` & `zod-0.2.0/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/anno/parser.py` & `zod-0.2.0/zod/anno/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 """Annotation parsers."""
 import json
+from dataclasses import dataclass
 from typing import Any, Dict, List
 
 from zod.anno.lane import LaneAnnotation, parse_lane_annotation
 from zod.anno.road_condition import RoadConditionAnnotation
 from zod.constants import AnnotationProject
+from zod.data_classes._serializable import JSONSerializable
 
 from .object import ObjectAnnotation
 from .tsr.traffic_sign import TrafficSignAnnotation
 
 
+@dataclass
+class AnnotationFile(JSONSerializable):
+    """Class to store information about an annotation frame."""
+
+    filepath: str
+    project: AnnotationProject
+
+    def read(self) -> Any:
+        """Read (and parse) the annotation json."""
+        return ANNOTATION_PARSERS[self.project](self.filepath)
+
+
 def _read_annotation_file(annotation_file: str) -> List[Dict[str, Any]]:
     """Read an annotation file."""
     with open(annotation_file, "r") as file:
         return json.load(file)
 
 
 def parse_object_detection_annotation(annotation_path: str) -> List[ObjectAnnotation]:
```

### Comparing `zod-0.1.8/zod/anno/tsr/class_map.py` & `zod-0.2.0/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/anno/tsr/traffic_sign.py` & `zod-0.2.0/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/cli/download_zod.py` & `zod-0.2.0/zod/cli/download_zod.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 APP_KEY = "kcvokw7c7votepo"
 REFRESH_TOKEN = "z2h_5rjphJEAAAAAAAAAAUWtQlltCYlMbZ2WqMgtymELhiSuKIksxAYeArubKnZV"
 CHUNK_SIZE = 1024 * 1024  # 1 MB
 TIMEOUT = 60 * 60  # 1 hour
 
-app = typer.Typer(help="Zenseact Open Dataset Donwloader", no_args_is_help=True)
+app = typer.Typer(help="Zenseact Open Dataset Downloader", no_args_is_help=True)
 
 
 class Version(str, Enum):
     FULL = "full"
     MINI = "mini"
 
 
@@ -293,22 +293,22 @@
     print("\nDownload settings:")
     print(download_settings)
     print("\nFilter settings:")
     if filter_settings.version == Version.MINI:
         print("    version: mini\n    (other settings are ignored for mini)")
     else:
         print(filter_settings)
-    if subset == SubDataset.FRAMES and (
-        filter_settings.num_scans_before == filter_settings.num_scans_after == 0
-    ):
-        typer.secho(
-            "Note! The current settings will only download the core lidar frames. "
-            "If you need surrounding scans, set --num-scans-before and/or --num-scans-after.",
-            fg=typer.colors.YELLOW,
-        )
+        if subset == SubDataset.FRAMES and (
+            filter_settings.num_scans_before == filter_settings.num_scans_after == 0
+        ):
+            typer.secho(
+                "Note! The current settings will only download the core lidar frames. "
+                "If you need surrounding scans, set --num-scans-before and/or --num-scans-after.",
+                fg=typer.colors.YELLOW,
+            )
     print("\n")
 
 
 REQ = "Required Arguments"
 GEN = "General Download Settings"
 FIL = "General Filter Settings"
 FRA = "Frames Filter Settings"
```

### Comparing `zod-0.1.8/zod/cli/extract_tsr_patches.py` & `zod-0.2.0/zod/cli/extract_tsr_patches.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 """
 
 import argparse
 import json
 import os
 from dataclasses import dataclass
 from itertools import repeat
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple
 
 import cv2
+import typer
 from tqdm.contrib.concurrent import process_map
 
-import zod.annotations.parser as parser
+import zod.anno.parser as parser
 import zod.constants as constants
 from zod import ZodFrames
 from zod.data_classes.frame import ZodFrame
 
 SUMMARY = """
 Finished creating dataset.
 .....................................
@@ -29,14 +31,40 @@
     by the original image size. The padding is stored in the dataset.json file.
 
 Images are saved in the following folder structure:
     <output_folder>/<traffic_sign_class>/<frame_id>_<annotation_uuid>.png
 """
 
 
+def cli_dummy(
+    dataset_root: Path = typer.Option(
+        ...,
+        exists=True,
+        dir_okay=True,
+        writable=False,
+        readable=True,
+        resolve_path=True,
+        help="Path to the root of the ZOD dataset.",
+    ),
+    output_dir: Path = typer.Option(
+        ...,
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        readable=True,
+        resolve_path=True,
+        help="Path to the output directory.",
+    ),
+    version: str = typer.Option("full", help="Version of the dataset to use. One of: full, small."),
+    path_size: Tuple[int, int] = typer.Option((64, 64), help="Path resultion."),
+):
+    typer.echo("Not Implemented Yet")
+
+
 @dataclass
 class Args:
     """Script args."""
 
     dataset_root: str
     output_folder: str
     num_workers: Optional[int]
```

### Comparing `zod-0.1.8/zod/cli/generate_coco_json.py` & `zod-0.2.0/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/cli/utils.py` & `zod-0.2.0/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/cli/visualize_lidar.py` & `zod-0.2.0/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/constants.py` & `zod-0.2.0/zod/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Relevant constants for ZOD."""
 
+import typing
 from enum import Enum
 from typing import Union
 
 # Python 3.7 compatibility
 try:
     from typing import Literal
 except ImportError:
@@ -11,32 +12,34 @@
 
 # Dataset paths
 FRAMES = "single_frames"
 SEQUENCES = "sequences"
 DRIVES = "drives"
 DB_DATE_STRING_FORMAT_W_MICROSECONDS = "%Y-%m-%dT%H:%M:%S.%f%z"
 
-# Train-val splits
-TRAIN = "train"
-VAL = "val"
-FULL = "full"
-MINI = "mini"
-VERSIONS = (FULL, MINI)
+Split = Literal["train", "val", "blacklisted"]
+SPLITS = typing.get_args(Split)
+TRAIN, VAL, BLACKLISTED = SPLITS
+
+Version = Literal["full", "mini"]
+VERSIONS = typing.get_args(Version)
+FULL, MINI = VERSIONS
+
 TRAINVAL_FILES = {
     FRAMES: {
-        FULL: f"trainval_frames_full.json",
-        MINI: f"trainval_frames_mini.json",
+        FULL: f"trainval-frames-full.json",
+        MINI: f"trainval-frames-mini.json",
     },
     SEQUENCES: {
-        FULL: f"trainval_sequences_full.json",
-        MINI: f"trainval_sequences_mini.json",
+        FULL: f"trainval-sequences-full.json",
+        MINI: f"trainval-sequences-mini.json",
     },
     DRIVES: {
-        FULL: f"trainval_drives_full.json",
-        MINI: f"trainval_drives_mini.json",
+        FULL: f"trainval-drives-full.json",
+        MINI: f"trainval-drives-mini.json",
     },
 }
 SPLIT_FILES = {
     FRAMES: {
         FULL: {
             TRAIN: "splits/frames_full_train.txt",
             VAL: "splits/frames_full_val.txt",
@@ -81,19 +84,24 @@
     TRAFFIC_SIGNS = "traffic_signs"
     EGO_ROAD = "ego_road"
     ROAD_CONDITION = "road_condition"
 
 
 ### Coordinate Frames ###
 
-EGO = "ego"
-
 
 class Camera(Enum):
     FRONT = "front"
 
 
 class Lidar(Enum):
     VELODYNE = "velodyne"
 
 
-CoordinateFrame = Union[Camera, Lidar, Literal[EGO]]
+Ego = Literal["ego"]
+EGO = typing.get_args(Ego)[0]
+CoordinateFrame = Union[Camera, Lidar, Ego]
+
+
+# ZodFrame properties
+FRAMES_IMAGE_MEAN = [0.337, 0.345, 0.367]
+FRAMES_IMAGE_STD = [0.160, 0.180, 0.214]
```

### Comparing `zod-0.1.8/zod/data_classes/box.py` & `zod-0.2.0/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/data_classes/calibration.py` & `zod-0.2.0/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/data_classes/ego_motion.py` & `zod-0.2.0/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/data_classes/frame.py` & `zod-0.2.0/zod/data_classes/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         """Get the metadata."""
         if self._metadata is None:
             self._metadata = FrameMetaData.from_json_path(self.info.metadata_path)
         return self._metadata
 
     def get_annotation(self, project: AnnotationProject) -> List[Any]:
         """Get the annotation for a given project."""
-        assert project in self.info.annotation_frames, f"Project {project} not available."
-        return self.info.get_key_annotation_frame(project).read()
+        assert project in self.info.annotations, f"Project {project} not available."
+        return self.info.annotations[project].read()
 
     def get_camera_frame(self, anonymization: Anonymization = Anonymization.BLUR) -> CameraFrame:
         """Get the camera frame."""
         return self.info.get_key_camera_frame(camera=Camera.FRONT, anonymization=anonymization)
 
     def get_image(
         self,
```

### Comparing `zod-0.1.8/zod/data_classes/geometry.py` & `zod-0.2.0/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/data_classes/info.py` & `zod-0.2.0/zod/data_classes/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os.path as osp
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import chain
-from typing import Dict, Iterator, List, Tuple
+from typing import Dict, Iterator, List, Optional, Tuple
 
+from zod.anno.parser import AnnotationFile
 from zod.constants import AnnotationProject, Anonymization, Camera, Lidar
 
 from ._serializable import JSONSerializable
-from .sensor import AnnotationFrame, CameraFrame, LidarFrame, SensorFrame
+from .sensor import CameraFrame, LidarFrame, SensorFrame
 
 
 @dataclass
 class Information(JSONSerializable):
     """Base class for frame and sequence information."""
 
     id: str
@@ -19,38 +20,45 @@
     end_time: datetime
     keyframe_time: datetime
 
     calibration_path: str
     ego_motion_path: str
     metadata_path: str
     oxts_path: str
+    vehicle_data_path: Optional[str]
 
-    annotation_frames: Dict[AnnotationProject, List[AnnotationFrame]]
+    annotations: Dict[AnnotationProject, AnnotationFile]
     camera_frames: Dict[str, List[CameraFrame]]  # key is a combination of Camera and Anonymization
     lidar_frames: Dict[Lidar, List[LidarFrame]]
 
     @property
     def all_frames(self) -> Iterator[SensorFrame]:
         """Iterate over all frames."""
         return chain(
             *self.lidar_frames.values(),
             *self.camera_frames.values(),
-            *self.annotation_frames.values(),
         )
 
     def convert_paths_to_absolute(self, root_path: str):
         self.calibration_path = osp.join(root_path, self.calibration_path)
         self.ego_motion_path = osp.join(root_path, self.ego_motion_path)
         self.metadata_path = osp.join(root_path, self.metadata_path)
         self.oxts_path = osp.join(root_path, self.oxts_path)
+        if self.vehicle_data_path is not None:
+            self.vehicle_data_path = osp.join(root_path, self.vehicle_data_path)
+        for annotation in self.annotations.values():
+            annotation.filepath = osp.join(root_path, annotation.filepath)
         for frame in self.all_frames:
             frame.filepath = osp.join(root_path, frame.filepath)
 
     def get_camera_lidar_map(
-        self, anonymization: Anonymization, camera: Camera, lidar: Lidar
+        self,
+        anonymization: Anonymization = Anonymization.BLUR,
+        camera: Camera = Camera.FRONT,
+        lidar: Lidar = Lidar.VELODYNE,
     ) -> Iterator[Tuple[CameraFrame, SensorFrame]]:
         """Iterate over all camera frames and their corresponding lidar frames.
 
         Args:
             camera: The camera to use. e.g., camera_front_blur
             lidar: The lidar to use. e.g., lidar_velodyne
         Yields:
@@ -70,25 +78,17 @@
                 self.lidar_frames[lidar],
                 key=lambda lidar_frame: abs(lidar_frame.time - camera_frame.time),
             )
             yield camera_frame, lidar_frame
 
     ### Keyframe accessors ###
 
-    def get_key_annotation_frame(self, project: AnnotationProject) -> AnnotationFrame:
-        if project not in self.annotation_frames:
-            raise ValueError(f"No annotations found for project {project.value}.")
-        if len(self.annotation_frames[project]) == 1:
-            return self.annotation_frames[project][0]
-        else:
-            return self.get_annotation_frame(self.keyframe_time, project)
-
     def get_key_camera_frame(
         self,
-        anonymization: Anonymization,
+        anonymization: Anonymization = Anonymization.BLUR,
         camera: Camera = Camera.FRONT,
     ) -> CameraFrame:
         camera_name = f"{camera.value}_{anonymization.value}"
         if len(self.camera_frames[camera_name]) == 1:
             return self.camera_frames[camera_name][0]
         else:
             return min(
@@ -97,31 +97,18 @@
             )
 
     def get_key_lidar_frame(self, lidar: Lidar = Lidar.VELODYNE) -> LidarFrame:
         return self.get_lidar_frame(self.keyframe_time, lidar)
 
     ### Timestamp accessors ###
 
-    def get_annotation_frame(
-        self,
-        time: datetime,
-        project: AnnotationProject,
-        # TODO: implement exact flag?
-    ) -> AnnotationFrame:
-        if project not in self.annotation_frames:
-            raise ValueError(f"No annotations found for project {project.value}.")
-        return min(
-            self.annotation_frames[project],
-            key=lambda annotation_frame: abs(annotation_frame.time - time),
-        )
-
     def get_camera_frame(
         self,
         time: datetime,
-        anonymization: Anonymization,
+        anonymization: Anonymization = Anonymization.BLUR,
         camera: Camera = Camera.FRONT,
     ) -> CameraFrame:
         camera_name = f"{camera.value}_{anonymization.value}"
         return min(
             self.camera_frames[camera_name],
             key=lambda camera_frame: abs(camera_frame.time - time),
         )
@@ -130,22 +117,17 @@
         return min(
             self.lidar_frames[lidar],
             key=lambda lidar_frame: abs(lidar_frame.time - time),
         )
 
     ### Full accessors ###
 
-    def get_annotation_frames(self, project: AnnotationProject) -> List[AnnotationFrame]:
-        if project not in self.annotation_frames:
-            return []
-        return self.annotation_frames[project]
-
     def get_camera_frames(
         self,
-        anonymization: Anonymization,
+        anonymization: Anonymization = Anonymization.BLUR,
         camera: Camera = Camera.FRONT,
     ) -> List[CameraFrame]:
         camera_name = f"{camera.value}_{anonymization.value}"
         return self.camera_frames[camera_name]
 
     def get_lidar_frames(self, lidar: Lidar = Lidar.VELODYNE) -> List[LidarFrame]:
         return self.lidar_frames[lidar]
```

### Comparing `zod-0.1.8/zod/data_classes/metadata.py` & `zod-0.2.0/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/data_classes/sensor.py` & `zod-0.2.0/zod/data_classes/sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,18 +151,7 @@
 
     height: int = 2168
     width: int = 3848
 
     def read(self) -> np.ndarray:
         """Read the image."""
         return np.array(Image.open(self.filepath))
-
-
-@dataclass
-class AnnotationFrame(SensorFrame):
-    """Class to store information about an annotation frame."""
-
-    project: AnnotationProject
-
-    def read(self) -> List[Any]:
-        """Read (and parse) the annotation json."""
-        return ANNOTATION_PARSERS[self.project](self.filepath)
```

### Comparing `zod-0.1.8/zod/data_classes/sequence.py` & `zod-0.2.0/zod/data_classes/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+from datetime import datetime
 from typing import Any, List, Optional
 
 from zod.constants import AnnotationProject, Lidar
 from zod.utils.compensation import motion_compensate_scanwise
 
 from .calibration import Calibration
 from .ego_motion import EgoMotion
 from .info import Information
 from .metadata import SequenceMetadata
 from .sensor import LidarData
+from .vehicle_data import VehicleData
 
 
 class ZodSequence:
     def __init__(self, info: Information):
         self.info: Information = info  # holds all the paths to the files
         self._ego_motion: EgoMotion = None  # this is the light-weight version of oxts
         self._oxts: EgoMotion = None
         self._calibration: Calibration = None
         self._metadata: SequenceMetadata = None
+        self._vehicle_data: VehicleData = None
 
     @property
     def ego_motion(self) -> EgoMotion:
         """Get the oxts file."""
         if self._ego_motion is None:
             self._ego_motion = EgoMotion.from_json_path(self.info.ego_motion_path)
         return self._ego_motion
@@ -42,26 +45,45 @@
     @property
     def metadata(self) -> SequenceMetadata:
         """Get the metadata."""
         if self._metadata is None:
             self._metadata = SequenceMetadata.from_json_path(self.info.metadata_path)
         return self._metadata
 
+    @property
+    def vehicle_data(self) -> VehicleData:
+        """Get the vehicle data."""
+        if self._vehicle_data is None:
+            assert self.info.vehicle_data_path is not None, "Vehicle data path is missing."
+            self._vehicle_data = VehicleData.from_hdf5(self.info.vehicle_data_path)
+        return self._vehicle_data
+
     def get_annotation(self, project: AnnotationProject) -> List[Any]:
         """Get the annotation for a given project."""
-        anno_frame = self.info.get_key_annotation_frame(project)
-        return anno_frame and anno_frame.read()  # read if not None
+        anno = self.info.annotations[project]
+        return anno and anno.read()  # read if not None
 
     def get_lidar(self, start: int = 0, end: int = None) -> List[LidarData]:
         """Get the point clouds."""
         return [
             lidar_frame.read()
             for lidar_frame in self.info.get_lidar_frames(Lidar.VELODYNE)[start:end]
         ]
 
+    def get_compensated_lidar(self, time: datetime) -> LidarData:
+        """Get the point cloud at a given timestamp."""
+        lid_frame = self.info.get_lidar_frame(time, Lidar.VELODYNE)
+        pcd = lid_frame.read()
+        return motion_compensate_scanwise(
+            pcd,
+            self.ego_motion,
+            self.calibration.lidars[Lidar.VELODYNE],
+            time.timestamp(),
+        )
+
     def get_aggregated_lidar(
         self, start: int = 0, end: int = None, timestamp: Optional[float] = None
     ) -> LidarData:
         """Get the aggregated point cloud."""
         lidar_scans = self.get_lidar(start, end)
         if timestamp is None:
             timestamp = lidar_scans[len(lidar_scans) // 2].core_timestamp
```

### Comparing `zod-0.1.8/zod/eval/detection/_experimental/eval.py` & `zod-0.2.0/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_experimental/matching.py` & `zod-0.2.0/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_experimental/utils.py` & `zod-0.2.0/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.0/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.0/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/utils/compensation.py` & `zod-0.2.0/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/utils/geometry.py` & `zod-0.2.0/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/utils/polygon_transformations.py` & `zod-0.2.0/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/utils/utils.py` & `zod-0.2.0/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/utils/visualization.py` & `zod-0.2.0/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/bev_utils.py` & `zod-0.2.0/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/colorlabeler.py` & `zod-0.2.0/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/lidar_bev.py` & `zod-0.2.0/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/lidar_on_image.py` & `zod-0.2.0/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/object_visualization.py` & `zod-0.2.0/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/oxts_on_image.py` & `zod-0.2.0/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/oxts_visualization.py` & `zod-0.2.0/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/visualization/polygon_utils.py` & `zod-0.2.0/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/zod_drives.py` & `zod-0.2.0/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/zod_frames.py` & `zod-0.2.0/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/zod/zod_sequences.py` & `zod-0.2.0/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.1.8/PKG-INFO` & `zod-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.1.8
+Version: 0.2.0
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


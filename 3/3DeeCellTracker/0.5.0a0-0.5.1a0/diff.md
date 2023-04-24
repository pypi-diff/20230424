# Comparing `tmp/3DeeCellTracker-0.5.0a0.tar.gz` & `tmp/3DeeCellTracker-0.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3DeeCellTracker-0.5.0a0.tar", last modified: Sun Apr 23 06:38:09 2023, max compression
+gzip compressed data, was "3DeeCellTracker-0.5.1a0.tar", last modified: Mon Apr 24 00:38:27 2023, max compression
```

## Comparing `3DeeCellTracker-0.5.0a0.tar` & `3DeeCellTracker-0.5.1a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/
--rw-rw-r--   0 wen       (1000) wen       (1000)     7899 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)      569 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/SOURCES.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/dependency_links.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)      166 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/requires.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       12 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/top_level.txt
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/CellTracker/
--rw-rw-r--   0 wen       (1000) wen       (1000)        0 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/CellTracker/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4598 2023-04-22 01:33:34.000000 3DeeCellTracker-0.5.0a0/CellTracker/analyses.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    22903 2023-04-22 08:31:03.000000 3DeeCellTracker-0.5.0a0/CellTracker/coord_image_transformer.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    11593 2023-04-22 07:34:57.000000 3DeeCellTracker-0.5.0a0/CellTracker/ffn.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     5332 2023-04-21 05:33:48.000000 3DeeCellTracker-0.5.0a0/CellTracker/preprocess.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    12898 2023-04-18 05:44:06.000000 3DeeCellTracker-0.5.0a0/CellTracker/stardist3dcustom.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    13105 2023-04-23 05:04:40.000000 3DeeCellTracker-0.5.0a0/CellTracker/stardistwrapper.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     3302 2023-04-14 05:41:05.000000 3DeeCellTracker-0.5.0a0/CellTracker/synthesize.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    23398 2023-04-21 05:29:47.000000 3DeeCellTracker-0.5.0a0/CellTracker/track.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    70284 2023-04-21 06:12:02.000000 3DeeCellTracker-0.5.0a0/CellTracker/tracker.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    20911 2023-04-22 09:18:38.000000 3DeeCellTracker-0.5.0a0/CellTracker/trackerlite.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    24761 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/CellTracker/unet3d.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     5756 2023-04-19 05:03:09.000000 3DeeCellTracker-0.5.0a0/CellTracker/watershed.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1068 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/LICENSE
--rw-rw-r--   0 wen       (1000) wen       (1000)     7899 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)     7414 2023-04-23 04:52:37.000000 3DeeCellTracker-0.5.0a0/README.md
--rw-rw-r--   0 wen       (1000) wen       (1000)      720 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/setup.cfg
--rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-04-23 06:38:07.000000 3DeeCellTracker-0.5.0a0/setup.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-24 00:38:26.997088 3DeeCellTracker-0.5.1a0/
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-24 00:38:26.997088 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/
+-rw-rw-r--   0 wen       (1000) wen       (1000)     8011 2023-04-24 00:38:26.000000 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)      569 2023-04-24 00:38:26.000000 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-04-24 00:38:26.000000 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)      166 2023-04-24 00:38:26.000000 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/requires.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       12 2023-04-24 00:38:26.000000 3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/top_level.txt
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-24 00:38:26.997088 3DeeCellTracker-0.5.1a0/CellTracker/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        0 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.1a0/CellTracker/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4598 2023-04-22 01:33:34.000000 3DeeCellTracker-0.5.1a0/CellTracker/analyses.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    23220 2023-04-23 06:41:20.000000 3DeeCellTracker-0.5.1a0/CellTracker/coord_image_transformer.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    11593 2023-04-22 07:34:57.000000 3DeeCellTracker-0.5.1a0/CellTracker/ffn.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5332 2023-04-21 05:33:48.000000 3DeeCellTracker-0.5.1a0/CellTracker/preprocess.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12898 2023-04-18 05:44:06.000000 3DeeCellTracker-0.5.1a0/CellTracker/stardist3dcustom.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13170 2023-04-23 06:41:20.000000 3DeeCellTracker-0.5.1a0/CellTracker/stardistwrapper.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3302 2023-04-14 05:41:05.000000 3DeeCellTracker-0.5.1a0/CellTracker/synthesize.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    23398 2023-04-21 05:29:47.000000 3DeeCellTracker-0.5.1a0/CellTracker/track.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    70284 2023-04-21 06:12:02.000000 3DeeCellTracker-0.5.1a0/CellTracker/tracker.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    21350 2023-04-23 06:41:20.000000 3DeeCellTracker-0.5.1a0/CellTracker/trackerlite.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    24761 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.1a0/CellTracker/unet3d.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5756 2023-04-19 05:03:09.000000 3DeeCellTracker-0.5.1a0/CellTracker/watershed.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1068 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.1a0/LICENSE
+-rw-rw-r--   0 wen       (1000) wen       (1000)     8011 2023-04-24 00:38:26.997088 3DeeCellTracker-0.5.1a0/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7526 2023-04-23 09:08:08.000000 3DeeCellTracker-0.5.1a0/README.md
+-rw-rw-r--   0 wen       (1000) wen       (1000)      720 2023-04-24 00:38:27.001088 3DeeCellTracker-0.5.1a0/setup.cfg
+-rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-04-23 06:38:07.000000 3DeeCellTracker-0.5.1a0/setup.py
```

### Comparing `3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/PKG-INFO` & `3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3DeeCellTracker
-Version: 0.5.0a0
+Version: 0.5.1a0
 Summary: A package for tracking cells in 3D time lapse images in deforming organs or moving animals
 Home-page: https://github.com/WenChentao/3DeeCellTracker
 Author: Chentao Wen
 Author-email: chintou.on@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,39 +17,39 @@
 [![PyPI](https://img.shields.io/pypi/v/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![GitHub](https://img.shields.io/github/license/WenChentao/3DeeCellTracker)](https://github.com/WenChentao/3DeeCellTracker/blob/master/LICENSE)
 [![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=ctt6o3DY2bA&list=PLGY0oNQomrHERP08iEj-MsluFW8xQJujP)
 
 **3DeeCellTracker** is a deep-learning based pipeline for tracking cells in 3D time lapse images of deforming/moving organs ([eLife, 2021](https://elifesciences.org/articles/59187)).
 
 ## Updates:
 
-**3DeeCellTracker v0.5.0-alpha will be released soon**
+**3DeeCellTracker v0.5.0-alpha has been released**
 - Allows you to use [StarDist3D](https://github.com/stardist/stardist) for segmentation
 - Reduces the requirements for fine-tuning parameters
 - Decouples the code to facilitate reuse by third-party developers.
 
 ## Installation
 
 To install 3DeeCellTracker, please follow the instructions below:
 
 ### Prerequisites
-- A computer with an NVIDIA GPU that supports CUDA.
+- A computer with an NVIDIA GPU that supports CUDA. We have tested all examples in a Nvidia Geforce GPU 3090.
 - [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://conda.io/miniconda.html) installed.
 
 ### Steps
 1. Create a new conda environment and activate it by running the following commands in your terminal:
 
    ```console
    $ conda create -n track python=3.8 pip
    $ conda activate track
    ```
    
-2. Install [TensorFlow](https://www.tensorflow.org/install).
+2. Install [TensorFlow](https://www.tensorflow.org/install). We have tested Tensorflow 2.5.0 in our computer.
 3. Install 3DeeCellTracker by running the following command in your terminal:
    ```console
-   $ pip install 3DeeCellTracker
+   $ pip install 3DeeCellTracker==0.5.0a0
    ```
    After completing the installation steps, you can start using 3DeeCellTracker for your 3D cell tracking tasks within 
    the jupyter notebooks we have provided (See below). 
    If you encounter any issues or have any questions, please refer to the project's documentation 
    or raise an issue in the GitHub repository.
 
 ## Quick Start
```

### Comparing `3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/SOURCES.txt` & `3DeeCellTracker-0.5.1a0/3DeeCellTracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/analyses.py` & `3DeeCellTracker-0.5.1a0/CellTracker/analyses.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/coord_image_transformer.py` & `3DeeCellTracker-0.5.1a0/CellTracker/coord_image_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
     @property
     def cell_num(self) -> int:
         return self._raw.shape[0]
 
 
 class CoordsToImageTransformer:
-
     auto_corrected_segmentation: ndarray
     subregions: List[Tuple[Tuple[slice, slice, slice], ndarray]]
     proofed_segmentation: ndarray
     z_slice_original_labels: slice
     coord_vol1: Coordinates
     use_8_bit: bool
 
@@ -99,19 +98,20 @@
         # Get list of paths to image slices
         slice_paths = sorted(glob(manual_vol1_path))
         if len(slice_paths) == 0:
             # Raise an error if no image slices are found in the specified directory
             raise FileNotFoundError(f"No image in {manual_vol1_path} was found")
 
         # Load the proofed segmentation and relabel it to sequential integers
-        proofed_segmentation = imread(slice_paths).transpose((1,2,0))
+        proofed_segmentation = imread(slice_paths).transpose((1, 2, 0))
         self.proofed_segmentation, _, _ = relabel_sequential(proofed_segmentation)
 
         # Print a message confirming that the proofed segmentation has been loaded and its shape
-        print(f"Loaded the proofed segmentations at vol 1 with {np.count_nonzero(np.unique(proofed_segmentation))} cells")
+        print(
+            f"Loaded the proofed segmentations at vol 1 with {np.count_nonzero(np.unique(proofed_segmentation))} cells")
 
     def interpolate(self, interpolation_factor: int, smooth_sigma: float = 2.5):
         """
         Interpolate the images along z axis and save the results in "track_results_xxx" folder
 
         Parameters
         ----------
@@ -127,14 +127,15 @@
 
         Notes
         -----
         The image is interpolated and smoothed if z_scaling > 1, or smoothed if z_scaling = 1 by a Gaussian filter.
         After interpolation/smoothing, the cell boundaries are reassigned by 2d watershed. Then the interpolated cells
         are re-segmented by 3d connectivity to separate cells incorrectly labelled as the same cell.
         """
+
         def extract_regions(segmentation: ndarray):
             self.subregions = gaussian_interpolation_3d(
                 segmentation, interpolation_factor=interpolation_factor, smooth_sigma=smooth_sigma)
 
             # Get interpolated labels image
             interpolated_labels, cell_overlaps_mask = self.move_cells(movements_nx3=None)
 
@@ -182,15 +183,16 @@
         )
         self.coord_vol1 = Coordinates(np.asarray(coord_vol1), interpolation_factor, self.voxel_size, dtype="raw")
         coords_real_path = self.results_folder / TRACK_RESULTS / COORDS_REAL
         coords_real_path.mkdir(parents=True, exist_ok=True)
         np.save(str(coords_real_path / "coords0001.npy"), np.asarray(coord_vol1))
 
     def move_cells_in_3d_image(self, movements_nx3: ndarray = None, cells_missed: Set[int] = None):
-        interpolated_labels, cell_overlaps_mask = self.move_cells(movements_nx3=movements_nx3, cells_missed=cells_missed)
+        interpolated_labels, cell_overlaps_mask = self.move_cells(movements_nx3=movements_nx3,
+                                                                  cells_missed=cells_missed)
         return recalculate_cell_boundaries(
             interpolated_labels[:, :, self.z_slice_original_labels],
             cell_overlaps_mask[:, :, self.z_slice_original_labels],
             sampling_xy=self.voxel_size[:2], print_message=False)
 
     def move_cells(self, movements_nx3: ndarray = None, cells_missed: Set[int] = None):
         """
@@ -261,22 +263,23 @@
         x_siz, y_siz, z_siz = self.proofed_segmentation.shape
         x, y, z = coordinates_real_nx3.T
 
         near_boundary = (
                 (x < boundary_xy) |
                 (y < boundary_xy) |
                 (x > (x_siz - boundary_xy) * self.voxel_size[0]) |
-                (y > (y_siz - boundary_xy) * self.voxel_size[1] ) |
+                (y > (y_siz - boundary_xy) * self.voxel_size[1]) |
                 (z < 0) |
                 (z > z_siz * self.voxel_size[2])
         )
         boundary_ids = np.where(near_boundary)[0] + 1
         return boundary_ids
 
-    def accurate_correction(self, t, grid: Tuple[int, int, int], coords: Coordinates, ensemble: bool, max_repetition: int = 20):
+    def accurate_correction(self, t, grid: Tuple[int, int, int], coords: Coordinates, ensemble: bool,
+                            max_repetition: int = 20):
         """Correct center positions of cells based on the probability map"""
         prob_map = np.load(str(self.results_folder / SEG / ("prob%04d.npy" % t)))
         prob_map = np.repeat(np.repeat(np.repeat(prob_map, grid[1], axis=0), grid[2], axis=1), grid[0], axis=2)
         if prob_map.shape != self.proofed_segmentation.shape:
             x_lim, y_lim, z_lim = self.proofed_segmentation.shape
             prob_map = prob_map[:x_lim, :y_lim, :z_lim]
 
@@ -300,34 +303,39 @@
         displacements_from_vol1 = coords - self.coord_vol1
         labels_image_interp, mask_image_interp = self.move_cells(displacements_from_vol1.interp, boundary_ids)
         labels_image = labels_image_interp[:, :, self.z_slice_original_labels]
         mask_image = mask_image_interp[:, :, self.z_slice_original_labels]
 
         # remove the overlapped regions from each label (marker for watershed)
         labels_image[mask_image > 1] = 0
-        positions_of_new_centers = ndm.center_of_mass(prob_img, labels_image, range(1, self.auto_corrected_segmentation.max() + 1))
+        positions_of_new_centers = ndm.center_of_mass(prob_img, labels_image,
+                                                      range(1, self.auto_corrected_segmentation.max() + 1))
         positions_of_new_centers = np.asarray(positions_of_new_centers)
 
         lost_cells = np.isnan(positions_of_new_centers[:, 0])
         positions_of_new_centers[lost_cells, :] = coords.raw[lost_cells, :]
 
-        corrected_coords = Coordinates(positions_of_new_centers, self.interpolation_factor, self.voxel_size, dtype="raw")
+        corrected_coords = Coordinates(positions_of_new_centers, self.interpolation_factor, self.voxel_size,
+                                       dtype="raw")
         delta_coords = corrected_coords - coords
 
         return corrected_coords, delta_coords
 
-    def save_tracking_results(self, coords: Coordinates, corrected_labels_image: ndarray, tracker, t1: int, t2: int, images_path):
+    def save_tracking_results(self, coords: Coordinates, corrected_labels_image: ndarray, tracker, t1: int, t2: int,
+                              images_path):
         np.save(str(self.results_folder / TRACK_RESULTS / COORDS_REAL / ("coords%04d.npy" % t2)), coords.real)
         save_tracked_labels(self.results_folder, corrected_labels_image, t2, self.use_8_bit)
         self.save_merged_labels(corrected_labels_image, images_path, t2)
 
-        confirmed_coord_t1 = np.load(str(self.results_folder / TRACK_RESULTS / COORDS_REAL / f"coords{str(t1).zfill(4)}.npy"))
+        confirmed_coord_t1 = np.load(
+            str(self.results_folder / TRACK_RESULTS / COORDS_REAL / f"coords{str(t1).zfill(4)}.npy"))
         segmented_pos_t2 = tracker._get_segmented_pos(t2)
         fig = plot_prgls_prediction(confirmed_coord_t1, segmented_pos_t2.real, coords.real, t1, t2)
-        fig.savefig(self.results_folder / TRACK_RESULTS / "figure" / f"matching_{str(t2).zfill(4)}.png", facecolor='white')
+        fig.savefig(self.results_folder / TRACK_RESULTS / "figure" / f"matching_{str(t2).zfill(4)}.png",
+                    facecolor='white')
         plt.close()
 
     def save_merged_labels(self, corrected_labels_image, images_path, t):
         labels_rgb = lbl_cmap.colors[corrected_labels_image.max(axis=2)]
         labels_rgb = Image.fromarray((labels_rgb * 255).astype(np.uint8))
 
         labels_rgb_xz = lbl_cmap.colors[corrected_labels_image.max(axis=0)].transpose(1, 0, 2)
@@ -343,15 +351,16 @@
 
         merged_labels = Image.blend(labels_rgb, raw_rgb, alpha=0.5)
         merged_labels_xz = Image.blend(labels_rgb_xz, raw_rgb_xz, alpha=0.5)
 
         (self.results_folder / TRACK_RESULTS / MERGED_LABELS).mkdir(parents=True, exist_ok=True)
         (self.results_folder / TRACK_RESULTS / MERGED_LABELS_XZ).mkdir(parents=True, exist_ok=True)
         merged_labels.save(str(self.results_folder / TRACK_RESULTS / MERGED_LABELS / ("merged_labels_t%04d.png" % t)))
-        merged_labels_xz.save(str(self.results_folder / TRACK_RESULTS / MERGED_LABELS_XZ / ("merged_labels_xz_t%04d.png" % t)))
+        merged_labels_xz.save(
+            str(self.results_folder / TRACK_RESULTS / MERGED_LABELS_XZ / ("merged_labels_xz_t%04d.png" % t)))
 
 
 def save_tracked_labels(results_folder: Path, labels_xyz: ndarray, t: int, use_8_bit: bool):
     tracked_labels_path = results_folder / TRACK_RESULTS / LABELS
     tracked_labels_path.mkdir(parents=True, exist_ok=True)
     dtype = np.uint8 if use_8_bit else np.uint16
     for z in range(1, labels_xyz.shape[2] + 1):
@@ -381,15 +390,16 @@
         bbox = bboxes[label - 1]
         sub_img = (label_image[bbox] == label).astype(np.float32)
         percentage = 1 - np.count_nonzero(sub_img) / sub_img.size
         img_smooth = skf.gaussian(np.repeat(sub_img, interpolation_factor, axis=2),
                                   sigma=smooth_sigma, mode='constant')
         threshold = np.percentile(img_smooth, percentage * 100)
         interpolated_bbox = (bbox[0], bbox[1],
-                             slice(bbox[2].start * interpolation_factor, bbox[2].stop * interpolation_factor, bbox[2].step))
+                             slice(bbox[2].start * interpolation_factor, bbox[2].stop * interpolation_factor,
+                                   bbox[2].step))
         subregions.append((interpolated_bbox, img_smooth > threshold))
     return subregions
 
 
 def fix_labeling_errors(segmentation: np.ndarray) -> Tuple[np.ndarray, bool]:
     """
     Relabel the separate cells that were incorrectly labeled as the same one
@@ -439,20 +449,20 @@
 
     # Plot the scatters of the ref_points and tgt_points
     ax1, ax2, fig = plot_two_pointset_scatters(dpi, fig_width_px, ref_ptrs, tgt_ptrs, t1, t2)
 
     # Plot the matching relationships between the two sets of points
     for ref_ptr, tgt_ptr in zip(ref_ptrs, predicted_ref_ptrs):
         # Get the coordinates of the matched points in the two point sets
-        pt1 = np.asarray([ref_ptr[1], -ref_ptr[ 0]])
+        pt1 = np.asarray([ref_ptr[1], -ref_ptr[0]])
         pt2 = np.asarray([tgt_ptr[1], -tgt_ptr[0]])
 
         # Draw a connection between the matched points in the two subplots using the `ConnectionPatch` class
         con = ConnectionPatch(xyA=pt2, xyB=pt1, coordsA="data", coordsB="data",
-                          axesA=ax2, axesB=ax1, color="C1")
+                              axesA=ax2, axesB=ax1, color="C1")
         ax2.add_artist(con)
 
     return fig
 
 
 def plot_two_pointset_scatters(dpi, fig_width_px, ref_ptrs, tgt_ptrs, t1: int, t2: int):
     # Calculate the figure size based on the input width and dpi
@@ -460,18 +470,18 @@
     fig_height_in = fig_width_in / 1.618  # set height to golden ratio
     # Determine whether to use a top-down or left-right layout based on the aspect ratio of the point sets
     ref_range_y, ref_range_x, _ = np.max(ref_ptrs, axis=0) - np.min(ref_ptrs, axis=0)
     tgt_range_y, tgt_range_x, _ = np.max(tgt_ptrs, axis=0) - np.min(tgt_ptrs, axis=0)
     top_down = ref_range_x + tgt_range_x >= ref_range_y + tgt_range_y
     # Create the figure and subplots
     if top_down:
-        #print("Using top-down layout")
+        # print("Using top-down layout")
         fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(fig_width_in, fig_height_in))
     else:
-        #print("Using left-right layout")
+        # print("Using left-right layout")
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(fig_width_in, fig_height_in))
     # Plot the point sets on the respective subplots
     ax1.scatter(ref_ptrs[:, 1], -ref_ptrs[:, 0], facecolors='b', edgecolors='b', label='Set 1')
     ax2.scatter(tgt_ptrs[:, 1], -tgt_ptrs[:, 0], facecolors='b', edgecolors='b', label='Set 2')
 
     unify_xy_lims(ax1, ax2)
```

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/ffn.py` & `3DeeCellTracker-0.5.1a0/CellTracker/ffn.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/preprocess.py` & `3DeeCellTracker-0.5.1a0/CellTracker/preprocess.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/stardist3dcustom.py` & `3DeeCellTracker-0.5.1a0/CellTracker/stardist3dcustom.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/stardistwrapper.py` & `3DeeCellTracker-0.5.1a0/CellTracker/stardistwrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Module Name: stardistwrapper.py
 Author: Chentao Wen
 Modification Description: This module is a wrapper of 3D StarDist modified according to 2_training.ipynb in GitHub StarDist repository
 """
 
-
 from __future__ import print_function, unicode_literals, absolute_import, division
 
 import re
 import sys
 from glob import glob
 from typing import List
 
@@ -74,28 +73,28 @@
     filenames = glob(str(images_path_search.parent / new_filename))
     assert len(filenames) > 0, f"No image files were found in {images_path_search.parent / new_filename}"
     numbers = [int(re.findall(r"t(\d+)", f)[0]) for f in filenames]
     smallest_number = min(numbers)
     largest_number = max(numbers)
 
     # Process images and predict instance coordinates
-    with tqdm(total=largest_number-smallest_number+1, desc="Segmenting images", ncols=50) as pbar:
+    with tqdm(total=largest_number - smallest_number + 1, desc="Segmenting images", ncols=50) as pbar:
         for t in range(smallest_number, largest_number + 1):
             try:
                 # Load 2D slices at time t
                 x = load_2d_slices_at_time(images_path, t=t)
             except FileNotFoundError:
                 # Handle missing image files
                 print(f"Warning: Segmentation has been stopped since images at t={t - 1} cannot be loaded!")
                 break
             (labels, details), prob_map = model.predict_instances(x)
             # Save predicted instance coordinates as numpy arrays
             coords_filepath = str(_seg_path / f"coords{str(t).zfill(4)}.npy")
             prob_filepath = str(_seg_path / f"prob{str(t).zfill(4)}.npy")
-            np.save(coords_filepath, details["points"][:, [1,2,0]])
+            np.save(coords_filepath, details["points"][:, [1, 2, 0]])
             np.save(prob_filepath, prob_map.transpose((1, 2, 0)))
             if t == smallest_number:
                 save_auto_seg_vol1(labels.transpose((1, 2, 0)), results_folder)
             pbar.update(1)
     print(f"All images from t={smallest_number} to t={largest_number} have been Segmented")
 
 
@@ -118,25 +117,25 @@
     """
     # Check if the folder exists and create it if necessary
     path = Path(folder_path)
     path.mkdir(parents=True, exist_ok=True)
 
     # Loop over the arrays and save them to the folder with numbered filenames
     for i, arr in enumerate(arrays):
-        filename = f"coords{str(i+1).zfill(4)}.npy"
+        filename = f"coords{str(i + 1).zfill(4)}.npy"
         filepath = path / filename
         np.save(filepath, arr)
 
 
 def load_training_images(path_train_images: str, path_train_labels: str, max_projection: bool):
     """Load images for training StarDist3DCustom"""
     X = sorted(glob(path_train_images))
     Y = sorted(glob(path_train_labels))
     assert len(X) > 0 and len(Y) > 0, "Error: No images found in either X or Y."
-    assert all(Path(x).name == Path(y).name for x, y in zip(X,Y)), "Error: Filenames in X and Y do not match."
+    assert all(Path(x).name == Path(y).name for x, y in zip(X, Y)), "Error: Filenames in X and Y do not match."
     X = list(map(imread, X))
     Y = list(map(imread, Y))
     n_channel = 1 if X[0].ndim == 3 else X[0].shape[-1]
     axis_norm = (0, 1, 2)  # normalize channels independently
     # axis_norm = (0,1,2,3) # normalize channels jointly
     if n_channel > 1:
         print(
@@ -196,20 +195,20 @@
     train_patch_size = np.cbrt(up_limit * a * b * c) / np.array([a, b, c])
     # 2. less than the image size
     up_limit_xyz = Y[0].shape[0], np.min(Y[0].shape[1:3]), np.min(Y[0].shape[1:3])
     scaling = np.min(np.asarray(up_limit_xyz) / train_patch_size)
     if scaling < 1:
         train_patch_size = train_patch_size * scaling
     # 3. can be divided by div_by (related to unet architecture)
-    unet_n_depth = 2 #
+    unet_n_depth = 2  #
     grid_norm = _normalize_grid(grid, 3)
-    unet_pool = 2,2,2
+    unet_pool = 2, 2, 2
     div_by = tuple(p ** unet_n_depth * g for p, g in zip(unet_pool, grid_norm))
     print(f"{div_by=}")
-    train_patch_size = [int(d*(i//d)) for i, d in zip(train_patch_size, div_by)]
+    train_patch_size = [int(d * (i // d)) for i, d in zip(train_patch_size, div_by)]
     # 4. size of x and y should be the same (since augmentation will flip x-y axes)
     train_patch_size[1] = train_patch_size[2] = min(train_patch_size[1:])
 
     conf = Config3D(
         rays=rays,
         grid=grid,
         anisotropy=anisotropy,
@@ -247,45 +246,46 @@
     for key, value in my_dict.items():
         print(f"{key}: {value}")
 
 
 def plot_img_label_center_slice(img, lbl, img_title="image (XY slice)", lbl_title="label (XY slice)", z=None):
     if z is None:
         z = img.shape[0] // 2
-    fig, (ai,al) = plt.subplots(1,2, figsize=(15,7), gridspec_kw=dict(width_ratios=(1.25,1)))
-    im = ai.imshow(img[z], cmap='gray', clim=(0,1))
+    fig, (ai, al) = plt.subplots(1, 2, figsize=(15, 7), gridspec_kw=dict(width_ratios=(1.25, 1)))
+    im = ai.imshow(img[z], cmap='gray', clim=(0, 1))
     ai.set_title(img_title)
     fig.colorbar(im, ax=ai)
     al.imshow(lbl[z], cmap=lbl_cmap)
     al.set_title(lbl_title)
     plt.tight_layout()
 
 
 def plot_img_label_max_projection(img, lbl, img_title="image (max projection/x-y)", lbl_title="label (max projection)",
                                   fig_width_px=1200, dpi=96):
     fig_width_in = fig_width_px / dpi  # convert to inches assuming 96 dpi
     fig_height_in = fig_width_in / 1.618  # set height to golden ratio
     # Create a new figure with the calculated size
-    fig, (ai,al) = plt.subplots(1,2, figsize=(fig_width_in, fig_height_in))
+    fig, (ai, al) = plt.subplots(1, 2, figsize=(fig_width_in, fig_height_in))
 
-    ai.imshow(img.max(axis=0), clim=(0,1), vmin=0, vmax=1)
+    ai.imshow(img.max(axis=0), clim=(0, 1), vmin=0, vmax=1)
     ai.set_title(img_title)
     al.imshow(lbl.max(axis=0), cmap=lbl_cmap)
     al.set_title(lbl_title)
     plt.tight_layout()
 
 
-def plot_img_label_max_projection_xz(img, lbl, img_title="image (max projection/x-z)", lbl_title="label (max projection)",
-                                  fig_width_px=1200, dpi=96, scale_z: int = 1):
+def plot_img_label_max_projection_xz(img, lbl, img_title="image (max projection/x-z)",
+                                     lbl_title="label (max projection)",
+                                     fig_width_px=1200, dpi=96, scale_z: int = 1):
     fig_width_in = fig_width_px / dpi  # convert to inches assuming 96 dpi
     fig_height_in = fig_width_in / 1.618  # set height to golden ratio
     # Create a new figure with the calculated size
-    fig, (ai,al) = plt.subplots(1,2, figsize=(fig_width_in, fig_height_in))
+    fig, (ai, al) = plt.subplots(1, 2, figsize=(fig_width_in, fig_height_in))
 
-    ai.imshow(img.max(axis=1), clim=(0,1), vmin=0, vmax=1, aspect=scale_z)
+    ai.imshow(img.max(axis=1), clim=(0, 1), vmin=0, vmax=1, aspect=scale_z)
     ai.set_title(img_title)
     al.imshow(lbl.max(axis=1), cmap=lbl_cmap, aspect=scale_z)
     al.set_title(lbl_title)
     plt.tight_layout()
 
 
 def random_fliprot(img, mask, axis=None):
@@ -319,8 +319,7 @@
     y is the corresponding ground-truth label image
     """
     # Note that we only use fliprots along axis=(1,2), i.e. the yx axis
     # as 3D microscopy acquisitions are usually not axially symmetric
     x, y = random_fliprot(x, y, axis=(1, 2))
     x = random_intensity_change(x)
     return x, y
-
```

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/synthesize.py` & `3DeeCellTracker-0.5.1a0/CellTracker/synthesize.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/track.py` & `3DeeCellTracker-0.5.1a0/CellTracker/track.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/tracker.py` & `3DeeCellTracker-0.5.1a0/CellTracker/tracker.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/trackerlite.py` & `3DeeCellTracker-0.5.1a0/CellTracker/trackerlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,58 +86,62 @@
             confirmed_coord_t1 = segmented_pos_t1
 
         # Normalize point sets
         confirmed_coords_norm_t1, (mean_t1, scale_t1) = normalize_points(confirmed_coord_t1.real, return_para=True)
         segmented_coords_norm_t2 = (segmented_pos_t2.real - mean_t1) / scale_t1
         segmented_coords_norm_t1 = (segmented_pos_t1.real - mean_t1) / scale_t1
 
-        matching_matrix = initial_matching_ffn(self.ffn_model, segmented_coords_norm_t1, segmented_coords_norm_t2, K_POINTS)
+        matching_matrix = initial_matching_ffn(self.ffn_model, segmented_coords_norm_t1, segmented_coords_norm_t2,
+                                               K_POINTS)
         normalized_prob, _ = simple_match(matching_matrix)
 
         tracked_coords_norm_t2, _ = prgls_with_two_ref(normalized_prob, segmented_coords_norm_t2,
                                                        segmented_coords_norm_t1, confirmed_coords_norm_t1,
                                                        beta=beta, lambda_=lambda_)
-        tracked_coords_t2 =  tracked_coords_norm_t2 * scale_t1 + mean_t1
+        tracked_coords_t2 = tracked_coords_norm_t2 * scale_t1 + mean_t1
         if draw_fig:
             fig = plot_prgls_prediction(confirmed_coord_t1.real, segmented_pos_t2.real, tracked_coords_t2, t1, t2)
 
         return Coordinates(tracked_coords_t2,
                            interpolation_factor=self.proofed_coords_vol1.interpolation_factor,
                            voxel_size=self.proofed_coords_vol1.voxel_size,
                            dtype="real")
 
     def predict_cell_positions_ensemble(self, skipped_volumes: List[int], t2: int, coord_t1: Coordinates,
                                         beta: float, lambda_: float, sampling_number: int = 20,
                                         adjacent: bool = False):
         coord_prgls = []
         for t1 in get_volumes_list(current_vol=t2, skip_volumes=skipped_volumes, sampling_number=sampling_number,
                                    adjacent=adjacent):
-            loaded_coord_t1 = np.load(str(self.results_dir / TRACK_RESULTS / COORDS_REAL / f"coords{str(t1).zfill(4)}.npy"))
-            loaded_coord_t1_ = Coordinates(loaded_coord_t1, coord_t1.interpolation_factor, coord_t1.voxel_size, dtype="real")
+            loaded_coord_t1 = np.load(
+                str(self.results_dir / TRACK_RESULTS / COORDS_REAL / f"coords{str(t1).zfill(4)}.npy"))
+            loaded_coord_t1_ = Coordinates(loaded_coord_t1, coord_t1.interpolation_factor, coord_t1.voxel_size,
+                                           dtype="real")
             coord_prgls.append(self.predict_cell_positions(t1=t1, t2=t2, confirmed_coord_t1=loaded_coord_t1_, beta=beta,
-                                                     lambda_=lambda_).real)
+                                                           lambda_=lambda_).real)
         return Coordinates(trim_mean(coord_prgls, 0.1, axis=0),
-                    interpolation_factor=self.proofed_coords_vol1.interpolation_factor,
-                    voxel_size=self.proofed_coords_vol1.voxel_size, dtype="real")
+                           interpolation_factor=self.proofed_coords_vol1.interpolation_factor,
+                           voxel_size=self.proofed_coords_vol1.voxel_size, dtype="real")
 
     def match_by_ffn(self, t1: int, t2: int, confirmed_coord_t1: Coordinates = None):
         assert t2 not in self.miss_frame
         segmented_pos_t1 = self._get_segmented_pos(t1)
         segmented_pos_t2 = self._get_segmented_pos(t2)
 
         if confirmed_coord_t1 is None:
             confirmed_coord_t1 = segmented_pos_t1
 
         confirmed_coords_norm_t1, (mean_t1, scale_t1) = normalize_points(confirmed_coord_t1.real, return_para=True)
         segmented_coords_norm_t2 = (segmented_pos_t2.real - mean_t1) / scale_t1
 
-        matching_matrix = initial_matching_ffn(self.ffn_model, confirmed_coords_norm_t1, segmented_coords_norm_t2, K_POINTS)
+        matching_matrix = initial_matching_ffn(self.ffn_model, confirmed_coords_norm_t1, segmented_coords_norm_t2,
+                                               K_POINTS)
         _, pairs_px2 = simple_match(matching_matrix)
         plot_initial_matching(confirmed_coord_t1.real, segmented_pos_t2.real, pairs_px2, t1, t2)
-        #plot_initial_matching(confirmed_coord_t1.real[:,[2,1,0]], segmented_pos_t2.real[:,[2,1,0]], pairs_px2)
+        # plot_initial_matching(confirmed_coord_t1.real[:,[2,1,0]], segmented_pos_t2.real[:,[2,1,0]], pairs_px2)
 
     def _get_segmented_pos(self, t: int) -> Coordinates:
         interp_factor = self.proofed_coords_vol1.interpolation_factor
         voxel_size = self.proofed_coords_vol1.voxel_size
 
         pos = Coordinates(np.load(str(self.results_dir / SEG / f"coords{str(t).zfill(4)}.npy")),
                           interpolation_factor=interp_factor, voxel_size=voxel_size, dtype="raw")
@@ -147,15 +151,15 @@
         tracked_labels_path = self.results_dir / TRACK_RESULTS / LABELS
         filenames = glob(str(tracked_labels_path / "*t*.tif"))
         assert len(filenames) > 0, f"No labels files were found in {tracked_labels_path / '*t*.tif'}"
         numbers = [int(re.findall(r"t(\d+)", f)[0]) for f in filenames]
         smallest_number = min(numbers)
         largest_number = max(numbers)
 
-        for t in range(smallest_number, largest_number+1):
+        for t in range(smallest_number, largest_number + 1):
             print(f"{t=}...", end="\r")
             try:
                 # Load 2D slices at time t
                 raw = load_2d_slices_at_time(raw_path, t=t)
             except FileNotFoundError:
                 # Handle missing image files
                 print(f"Warning: Raw images at t={t - 1} cannot be loaded! Stop calculation!")
@@ -167,34 +171,36 @@
             except FileNotFoundError:
                 # Handle missing image files
                 print(f"Warning: Label images at t={t - 1} cannot be loaded!")
                 if t == smallest_number:
                     print("Warning: stop calculation!")
                     break
                 else:
-                    print(f"Warning: skip volume {t-1}!")
+                    print(f"Warning: skip volume {t - 1}!")
                     activities[t - smallest_number, :] = np.nan
                     continue
 
             if t == smallest_number:
                 cell_num = np.max(labels_img)
                 activities = np.zeros((largest_number - smallest_number + 1, cell_num))
 
             per = (1 - discard_ratio) * 100
             for label in range(1, cell_num + 1):
                 intensity_label_i = raw[labels_img == label]
                 if intensity_label_i.size == 0:
                     activities[t - smallest_number, label - 1] = np.nan
                 else:
                     threshold = np.percentile(intensity_label_i, per)
-                    activities[t - smallest_number, label-1] = np.mean(intensity_label_i[intensity_label_i > threshold])
+                    activities[t - smallest_number, label - 1] = np.mean(
+                        intensity_label_i[intensity_label_i > threshold])
         return activities
 
 
-def plot_initial_matching(ref_ptrs: ndarray, tgt_ptrs: ndarray, pairs_px2: ndarray, t1: int, t2: int, fig_width_px=1200, dpi=96):
+def plot_initial_matching(ref_ptrs: ndarray, tgt_ptrs: ndarray, pairs_px2: ndarray, t1: int, t2: int, fig_width_px=1200,
+                          dpi=96):
     """Draws the initial matching between two sets of 3D points and their matching relationships.
 
     Args:
         ref_ptrs (ndarray): A 2D array of shape (n, 3) containing the reference points.
         tgt_ptrs (ndarray): A 2D array of shape (n, 3) containing the target points.
         pairs_px2 (ndarray): A 2D array of shape (m, 2) containing the pairs of matched points.
         fig_width_px (int): The width of the output figure in pixels. Default is 1200.
@@ -219,15 +225,15 @@
     for ref_index, tgt_index in pairs_px2:
         # Get the coordinates of the matched points in the two point sets
         pt1 = np.asarray([ref_ptrs[ref_index, 1], -ref_ptrs[ref_index, 0]])
         pt2 = np.asarray([tgt_ptrs[tgt_index, 1], -tgt_ptrs[tgt_index, 0]])
 
         # Draw a connection between the matched points in the two subplots using the `ConnectionPatch` class
         con = ConnectionPatch(xyA=pt2, xyB=pt1, coordsA="data", coordsB="data",
-                          axesA=ax2, axesB=ax1, color="C1")
+                              axesA=ax2, axesB=ax1, color="C1")
         ax2.add_artist(con)
 
 
 def simple_match(initial_match_matrix: ndarray, threshold=0.1) -> ndarray:
     """Match points from two point sets by simply choosing the pairs with the highest probability subsequently"""
     match_matrix = initial_match_matrix.copy()
     pairs_list = []
@@ -237,44 +243,45 @@
             break
         tgt_index, ref_index = np.unravel_index(match_matrix.argmax(), match_matrix.shape)
         pairs_list.append((ref_index, tgt_index))
 
         match_matrix[tgt_index, :] = 0
         match_matrix[:, ref_index] = 0
     pairs_px2 = np.array(pairs_list)
-    normalized_prob = np.full_like(match_matrix, 0.1 / (match_matrix.shape[1] -1))
+    normalized_prob = np.full_like(match_matrix, 0.1 / (match_matrix.shape[1] - 1))
     for ref, tgt in pairs_px2:
         normalized_prob[tgt, ref] = 0.9
     return normalized_prob, pairs_px2
 
 
 def prgls_quick(init_match_mxn, ptrs_tgt_mx3: ndarray, tracked_ref_nx3: ndarray,
                 beta: float, lambda_: float, max_iteration: int = MAX_ITERATION) \
         -> Tuple[ndarray, ndarray]:
     """
     Get coherent movements from the initial matching by PR-GLS algorithm
     """
 
-
     # Initiate parameters
     ratio_outliers = 0.05  # This is the gamma
     distance_weights_nxn = gaussian_kernel(tracked_ref_nx3, tracked_ref_nx3, beta ** 2)  # This is the Gram matrix
     sigma_square = dist_squares(tracked_ref_nx3, ptrs_tgt_mx3).mean() / 3  # This is the sigma^2
     predicted_coord_ref_nx3 = tracked_ref_nx3.copy()  # This is the T(X)
 
     ############################################################################
     # iteratively update predicted_ref_n1x3, ratio_outliers, sigma_square, and posterior_mxn. Plot and save results
     ############################################################################
     for iteration in range(1, max_iteration):
         # E-step: update posterior probability P_mxn
-        posterior_mxn = estimate_posterior(init_match_mxn, sigma_square, predicted_coord_ref_nx3, ptrs_tgt_mx3, ratio_outliers)
+        posterior_mxn = estimate_posterior(init_match_mxn, sigma_square, predicted_coord_ref_nx3, ptrs_tgt_mx3,
+                                           ratio_outliers)
 
         # M-step: update predicted positions of reference set
         # movements_basis_3xn is the parameter C
-        movements_basis_3xn = solve_movements_ref(sigma_square, lambda_, posterior_mxn, predicted_coord_ref_nx3, ptrs_tgt_mx3, distance_weights_nxn)
+        movements_basis_3xn = solve_movements_ref(sigma_square, lambda_, posterior_mxn, predicted_coord_ref_nx3,
+                                                  ptrs_tgt_mx3, distance_weights_nxn)
         movements_ref_nx3 = np.dot(movements_basis_3xn, distance_weights_nxn).T
         if iteration > 1:
             predicted_coord_ref_nx3 += movements_ref_nx3  # The first estimation is not reliable thus is discarded
         sum_posterior = np.sum(posterior_mxn)
         ratio_outliers = 1 - sum_posterior / ptrs_tgt_mx3.shape[0]
 
         # Sometimes this value could become minus due to the inaccurate float representation in computer.
@@ -310,19 +317,21 @@
     predicted_coord_ref_lx3 = tracked_ref_lx3.copy()
 
     ############################################################################
     # iteratively update predicted_ref_n1x3, ratio_outliers, sigma_square, and posterior_mxn. Plot and save results
     ############################################################################
     for iteration in range(1, max_iteration):
         # E-step: update posterior probability P_mxn
-        posterior_mxn = estimate_posterior(init_match_mxn, sigma_square, predicted_coord_ref_nx3, ptrs_tgt_mx3, ratio_outliers)
+        posterior_mxn = estimate_posterior(init_match_mxn, sigma_square, predicted_coord_ref_nx3, ptrs_tgt_mx3,
+                                           ratio_outliers)
 
         # M-step: update predicted positions of reference set
         # movements_basis_3xn is the parameter C
-        movements_basis_3xn = solve_movements_ref(sigma_square, lambda_, posterior_mxn, predicted_coord_ref_nx3, ptrs_tgt_mx3, distance_weights_nxn)
+        movements_basis_3xn = solve_movements_ref(sigma_square, lambda_, posterior_mxn, predicted_coord_ref_nx3,
+                                                  ptrs_tgt_mx3, distance_weights_nxn)
         movements_ref_nx3 = np.dot(movements_basis_3xn, distance_weights_nxn).T
         movements_tracked_lx3 = np.dot(movements_basis_3xn, distance_weights_nxl).T
         if iteration > 1:
             predicted_coord_ref_nx3 += movements_ref_nx3  # The first estimation is not reliable thus is discarded
             predicted_coord_ref_lx3 += movements_tracked_lx3
         sum_posterior = np.sum(posterior_mxn)
         ratio_outliers = 1 - sum_posterior / ptrs_tgt_mx3.shape[0]
@@ -356,15 +365,16 @@
     dist_square_sum_mxn = np.sum(np.square(ptrs_ref_mxnx3 - ptrs_tgt_mxnx3), axis=2)
     return np.exp(-dist_square_sum_mxn / (2 * sigma_square))
 
 
 def estimate_posterior(prior_p_mxn: ndarray, initial_sigma_square: float, predicted_ref_nx3: ndarray,
                        ptrs_tgt_mx3: ndarray, ratio_outliers: float, vol: float = 1) -> ndarray:
     p_pos_j_when_j_match_i_mxn = gaussian_kernel(predicted_ref_nx3, ptrs_tgt_mx3, initial_sigma_square)
-    p_pos_j_and_j_match_i_mxn = (1 - ratio_outliers) * prior_p_mxn * p_pos_j_when_j_match_i_mxn / (2 * np.pi * initial_sigma_square) ** 1.5
+    p_pos_j_and_j_match_i_mxn = (1 - ratio_outliers) * prior_p_mxn * p_pos_j_when_j_match_i_mxn / (
+                2 * np.pi * initial_sigma_square) ** 1.5
     posterior_sum_m = np.sum(p_pos_j_and_j_match_i_mxn, axis=1) + ratio_outliers / vol
     posterior_mxn = p_pos_j_and_j_match_i_mxn / posterior_sum_m[:, None]
     return posterior_mxn
 
 
 def softmax_normalize(similarity_matrix_mxn: ndarray) -> ndarray:
     return scipy.special.softmax(similarity_matrix_mxn, axis=1)
@@ -404,18 +414,18 @@
 def evenly_distributed_volumes(current_vol: int, sampling_number: int) -> List[int]:
     """Get evenly distributed previous volumes"""
     interval = (current_vol - 1) // sampling_number
     start = np.mod(current_vol - 1, sampling_number) + 1
     return list(range(start, current_vol - interval + 1, interval))
 
 
-def get_volumes_list(current_vol: int, skip_volumes: List[int], sampling_number: int = 20, adjacent: bool = False) -> List[int]:
+def get_volumes_list(current_vol: int, skip_volumes: List[int], sampling_number: int = 20, adjacent: bool = False) -> \
+List[int]:
     if current_vol - 1 < sampling_number:
         vols_list = list(range(1, current_vol))
     else:
         if adjacent:
             vols_list = list(range(current_vol - sampling_number, current_vol))
         else:
             vols_list = evenly_distributed_volumes(current_vol, sampling_number)
     vols_list = [vol for vol in vols_list if vol not in skip_volumes]
     return vols_list
-
```

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/unet3d.py` & `3DeeCellTracker-0.5.1a0/CellTracker/unet3d.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/CellTracker/watershed.py` & `3DeeCellTracker-0.5.1a0/CellTracker/watershed.py`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/LICENSE` & `3DeeCellTracker-0.5.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `3DeeCellTracker-0.5.0a0/PKG-INFO` & `3DeeCellTracker-0.5.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3DeeCellTracker
-Version: 0.5.0a0
+Version: 0.5.1a0
 Summary: A package for tracking cells in 3D time lapse images in deforming organs or moving animals
 Home-page: https://github.com/WenChentao/3DeeCellTracker
 Author: Chentao Wen
 Author-email: chintou.on@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,39 +17,39 @@
 [![PyPI](https://img.shields.io/pypi/v/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![GitHub](https://img.shields.io/github/license/WenChentao/3DeeCellTracker)](https://github.com/WenChentao/3DeeCellTracker/blob/master/LICENSE)
 [![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=ctt6o3DY2bA&list=PLGY0oNQomrHERP08iEj-MsluFW8xQJujP)
 
 **3DeeCellTracker** is a deep-learning based pipeline for tracking cells in 3D time lapse images of deforming/moving organs ([eLife, 2021](https://elifesciences.org/articles/59187)).
 
 ## Updates:
 
-**3DeeCellTracker v0.5.0-alpha will be released soon**
+**3DeeCellTracker v0.5.0-alpha has been released**
 - Allows you to use [StarDist3D](https://github.com/stardist/stardist) for segmentation
 - Reduces the requirements for fine-tuning parameters
 - Decouples the code to facilitate reuse by third-party developers.
 
 ## Installation
 
 To install 3DeeCellTracker, please follow the instructions below:
 
 ### Prerequisites
-- A computer with an NVIDIA GPU that supports CUDA.
+- A computer with an NVIDIA GPU that supports CUDA. We have tested all examples in a Nvidia Geforce GPU 3090.
 - [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://conda.io/miniconda.html) installed.
 
 ### Steps
 1. Create a new conda environment and activate it by running the following commands in your terminal:
 
    ```console
    $ conda create -n track python=3.8 pip
    $ conda activate track
    ```
    
-2. Install [TensorFlow](https://www.tensorflow.org/install).
+2. Install [TensorFlow](https://www.tensorflow.org/install). We have tested Tensorflow 2.5.0 in our computer.
 3. Install 3DeeCellTracker by running the following command in your terminal:
    ```console
-   $ pip install 3DeeCellTracker
+   $ pip install 3DeeCellTracker==0.5.0a0
    ```
    After completing the installation steps, you can start using 3DeeCellTracker for your 3D cell tracking tasks within 
    the jupyter notebooks we have provided (See below). 
    If you encounter any issues or have any questions, please refer to the project's documentation 
    or raise an issue in the GitHub repository.
 
 ## Quick Start
```

### Comparing `3DeeCellTracker-0.5.0a0/README.md` & `3DeeCellTracker-0.5.1a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 [![PyPI](https://img.shields.io/pypi/v/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![GitHub](https://img.shields.io/github/license/WenChentao/3DeeCellTracker)](https://github.com/WenChentao/3DeeCellTracker/blob/master/LICENSE)
 [![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=ctt6o3DY2bA&list=PLGY0oNQomrHERP08iEj-MsluFW8xQJujP)
 
 **3DeeCellTracker** is a deep-learning based pipeline for tracking cells in 3D time lapse images of deforming/moving organs ([eLife, 2021](https://elifesciences.org/articles/59187)).
 
 ## Updates:
 
-**3DeeCellTracker v0.5.0-alpha will be released soon**
+**3DeeCellTracker v0.5.0-alpha has been released**
 - Allows you to use [StarDist3D](https://github.com/stardist/stardist) for segmentation
 - Reduces the requirements for fine-tuning parameters
 - Decouples the code to facilitate reuse by third-party developers.
 
 ## Installation
 
 To install 3DeeCellTracker, please follow the instructions below:
 
 ### Prerequisites
-- A computer with an NVIDIA GPU that supports CUDA.
+- A computer with an NVIDIA GPU that supports CUDA. We have tested all examples in a Nvidia Geforce GPU 3090.
 - [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://conda.io/miniconda.html) installed.
 
 ### Steps
 1. Create a new conda environment and activate it by running the following commands in your terminal:
 
    ```console
    $ conda create -n track python=3.8 pip
    $ conda activate track
    ```
    
-2. Install [TensorFlow](https://www.tensorflow.org/install).
+2. Install [TensorFlow](https://www.tensorflow.org/install). We have tested Tensorflow 2.5.0 in our computer.
 3. Install 3DeeCellTracker by running the following command in your terminal:
    ```console
-   $ pip install 3DeeCellTracker
+   $ pip install 3DeeCellTracker==0.5.0a0
    ```
    After completing the installation steps, you can start using 3DeeCellTracker for your 3D cell tracking tasks within 
    the jupyter notebooks we have provided (See below). 
    If you encounter any issues or have any questions, please refer to the project's documentation 
    or raise an issue in the GitHub repository.
 
 ## Quick Start
```

### Comparing `3DeeCellTracker-0.5.0a0/setup.cfg` & `3DeeCellTracker-0.5.1a0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 3DeeCellTracker
-version = 0.5.0-alpha
+version = 0.5.1-alpha
 author = Chentao Wen
 author_email = chintou.on@gmail.com
 description = A package for tracking cells in 3D time lapse images in deforming organs or moving animals
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/WenChentao/3DeeCellTracker
 classifiers = 
@@ -16,17 +16,17 @@
 install_requires = 
 	numpy==1.22.3
 	scikit-learn==1.1.2
 	tifffile==2023.2.28
 	tqdm==4.64.0
 	matplotlib==3.5.1
 	scipy==1.8.0
-	pillow==9.1.0
-	scikit-image==0.15.0
+	pillow==9.3.0
+	scikit-image==0.19.3
 	stardist==0.8.3
-	notebook==6.4.10
+	notebook==6.4.12
 python_requires = >=3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


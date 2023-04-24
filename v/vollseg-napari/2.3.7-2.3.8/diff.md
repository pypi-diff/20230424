# Comparing `tmp/vollseg-napari-2.3.7.tar.gz` & `tmp/vollseg-napari-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari/dist/tmpa18sbf1x/vollseg-napari-2.3.7.tar", last modified: Mon Oct  3 17:46:26 2022, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari/dist/.tmp-5p_8sm2d/vollseg-napari-2.3.8.tar", last modified: Mon Apr 24 12:05:49 2023, max compression
```

## Comparing `vollseg-napari-2.3.7.tar` & `vollseg-napari-2.3.8.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-03 17:46:26.974800 vollseg-napari-2.3.7/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1539 2022-04-19 17:57:10.000000 vollseg-napari-2.3.7/LICENCE.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      103 2022-04-19 18:03:29.000000 vollseg-napari-2.3.7/MANIFEST.in
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    10929 2022-10-03 17:46:26.972799 vollseg-napari-2.3.7/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     9865 2022-05-16 10:29:25.000000 vollseg-napari-2.3.7/README.md
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       91 2022-04-19 18:04:08.000000 vollseg-napari-2.3.7/pyproject.toml
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       38 2022-10-03 17:46:26.975800 vollseg-napari-2.3.7/setup.cfg
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     2184 2022-09-06 23:47:51.000000 vollseg-napari-2.3.7/setup.py
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-03 17:46:26.707797 vollseg-napari-2.3.7/vollseg_napari/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-04-24 01:04:28.000000 vollseg-napari-2.3.7/vollseg_napari/__init__.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)   118812 2022-10-03 17:44:20.000000 vollseg-napari-2.3.7/vollseg_napari/_dock_widget.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      437 2022-06-20 13:27:35.000000 vollseg-napari-2.3.7/vollseg_napari/_sample_data.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    92416 2022-05-19 18:39:09.000000 vollseg-napari-2.3.7/vollseg_napari/_test_dock_widget.py
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-03 17:46:26.856800 vollseg-napari-2.3.7/vollseg_napari/_tests/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-04-19 19:15:45.000000 vollseg-napari-2.3.7/vollseg_napari/_tests/__init__.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      391 2022-04-26 21:14:59.000000 vollseg-napari-2.3.7/vollseg_napari/_tests/plugintest.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      317 2022-04-28 20:59:46.000000 vollseg-napari-2.3.7/vollseg_napari/_tests/test_open_sample_data.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    16092 2022-05-17 14:03:45.000000 vollseg-napari-2.3.7/vollseg_napari/_tests/test_open_sample_models.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      113 2022-10-03 17:44:34.000000 vollseg-napari-2.3.7/vollseg_napari/_version.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1125 2022-06-20 13:30:19.000000 vollseg-napari-2.3.7/vollseg_napari/napari.yaml
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-03 17:46:26.955798 vollseg-napari-2.3.7/vollseg_napari/resources/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-2.3.7/vollseg_napari/resources/kapoorlogo.png
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)   558497 2022-04-02 03:56:32.000000 vollseg-napari-2.3.7/vollseg_napari/resources/oneat.jpg
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)   564904 2022-04-02 03:58:52.000000 vollseg-napari-2.3.7/vollseg_napari/resources/oneat_1.jpg
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    10601 2022-05-29 15:34:47.000000 vollseg-napari-2.3.7/vollseg_napari/resources/vollseg_logo_napari.png
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-03 17:46:26.787798 vollseg-napari-2.3.7/vollseg_napari.egg-info/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    10929 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      793 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/SOURCES.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        1 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/dependency_links.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       62 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/entry_points.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      240 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/requires.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       15 2022-10-03 17:46:26.000000 vollseg-napari-2.3.7/vollseg_napari.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-24 12:05:49.427337 vollseg-napari-2.3.8/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1539 2022-04-19 17:57:10.000000 vollseg-napari-2.3.8/LICENCE.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      103 2022-04-19 18:03:29.000000 vollseg-napari-2.3.8/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10929 2023-04-24 12:05:49.423063 vollseg-napari-2.3.8/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     9865 2022-05-16 10:29:25.000000 vollseg-napari-2.3.8/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       91 2022-04-19 18:04:08.000000 vollseg-napari-2.3.8/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-04-24 12:05:49.428338 vollseg-napari-2.3.8/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2184 2022-09-06 23:47:51.000000 vollseg-napari-2.3.8/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-24 12:05:49.040253 vollseg-napari-2.3.8/vollseg_napari/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-04-24 01:04:28.000000 vollseg-napari-2.3.8/vollseg_napari/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   118567 2023-04-24 12:04:35.000000 vollseg-napari-2.3.8/vollseg_napari/_dock_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      437 2022-06-20 13:27:35.000000 vollseg-napari-2.3.8/vollseg_napari/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    92416 2022-05-19 18:39:09.000000 vollseg-napari-2.3.8/vollseg_napari/_test_dock_widget.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-24 12:05:49.347721 vollseg-napari-2.3.8/vollseg_napari/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-04-19 19:15:45.000000 vollseg-napari-2.3.8/vollseg_napari/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      391 2022-04-26 21:14:59.000000 vollseg-napari-2.3.8/vollseg_napari/_tests/plugintest.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      317 2022-04-28 20:59:46.000000 vollseg-napari-2.3.8/vollseg_napari/_tests/test_open_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16092 2022-05-17 14:03:45.000000 vollseg-napari-2.3.8/vollseg_napari/_tests/test_open_sample_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      113 2023-04-24 12:04:49.000000 vollseg-napari-2.3.8/vollseg_napari/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1125 2022-06-20 13:30:19.000000 vollseg-napari-2.3.8/vollseg_napari/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-24 12:05:49.393900 vollseg-napari-2.3.8/vollseg_napari/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-2.3.8/vollseg_napari/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-24 12:05:49.201899 vollseg-napari-2.3.8/vollseg_napari.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10929 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      672 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       62 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      240 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-04-24 12:05:48.000000 vollseg-napari-2.3.8/vollseg_napari.egg-info/top_level.txt
```

### Comparing `vollseg-napari-2.3.7/LICENCE.txt` & `vollseg-napari-2.3.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/PKG-INFO` & `vollseg-napari-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari
-Version: 2.3.7
+Version: 2.3.8
 Summary: Irregular cell shape segmentation using VollSeg
 Home-page: https://github.com/kapoorlab/vollseg-napari
 Author: Varun Kapoor
 Author-email: varun.kapoor@kapoorlabs.org
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/kapoorlab/vollseg-napari
 Project-URL: Documentation, https://github.com/kapoorlab/vollseg-napari
```

### Comparing `vollseg-napari-2.3.7/README.md` & `vollseg-napari-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/setup.py` & `vollseg-napari-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/vollseg_napari/_dock_widget.py` & `vollseg-napari-2.3.8/vollseg_napari/_dock_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,15 @@
        
         progress_bar=dict(label=' ', min=0, max=0, visible=False),
         layout='vertical',
         persist=True,
         call_button=True,
     )
     def plugin(
-        viewer: napari.Viewer,
+        viewer: Union[napari.Viewer, None],
         label_head,
         image: napari.layers.Image,
         axes,
         star_seg_model_type,
         unet_seg_model_type,
         den_model_type,
         roi_model_type,
@@ -732,34 +732,28 @@
 
             if model_star is not None:   
                 worker = _VollSeg_time(model_star, model_unet, model_roi, x_reorder, axes_reorder, model_den, scale_out, t, x)
                 worker.returned.connect(return_segment_time)
                 worker.yielded.connect(progress_thread)
                
             if model_star is None:
-                   
-                        
                     worker = _Unet_time( model_unet, model_roi, x_reorder, axes_reorder, model_den, scale_out, t, x)
                     worker.returned.connect(return_segment_unet_time)
                     worker.yielded.connect(progress_thread)
             
         else:
             
            
 
                     if model_star is not None: 
                         worker = _Segment(model_star, model_unet, model_roi, x, axes, model_den,scale_out)
                         worker.returned.connect(return_segment)
                     if model_star is None:
                         worker = _Unet(model_unet, model_roi, x, axes, model_den,scale_out)
                         worker.returned.connect(return_segment_unet)
-                        
-           
-
-
 
         # add a button to the viewew that, when clicked, stops the worker
         
         progress_bar.hide()
         plugin_stop_parameters.stop_button.native.setStyleSheet('')
             
     plugin.axes.value = ''
@@ -2163,32 +2157,32 @@
             
            yield count
            
            pre_res.append(VollSeg(
                        _x,
                        model_unet,
                        model_star,
+                       roi_model = model_roi,
                        axes=axes_reorder,
                        noise_model=noise_model,
-                       roi_model = model_roi,
                        prob_thresh=plugin_star_parameters.prob_thresh.value,
                        nms_thresh=plugin_star_parameters.nms_thresh.value,
                        min_size_mask=plugin_extra_parameters.min_size_mask.value,
                        seedpool= plugin_extra_parameters.seedpool.value,
                        min_size=plugin_extra_parameters.min_size.value,
                        max_size=plugin_extra_parameters.max_size.value,
                        n_tiles=plugin_star_parameters.n_tiles.value,
                        donormalize=plugin_star_parameters.norm_image.value,
                        lower_perc=plugin_star_parameters.perc_low.value, 
                        upper_perc=plugin_star_parameters.perc_high.value,
                        UseProbability=plugin_extra_parameters.prob_map_watershed.value,
                        ExpandLabels = plugin_extra_parameters.expand_labels.value,
                        dounet=plugin_extra_parameters.dounet.value,
                        RGB = plugin_extra_parameters.isRGB.value,
-                       iou_threshold = plugin_extra_parameters.iouthresh.value,slice_merge = plugin_extra_parameters.slicemerge.value
+                       slice_merge = plugin_extra_parameters.slicemerge.value
                    ))
                    
        pred = pre_res, scale_out, t, x
        return pred            
               
               
     @thread_worker(connect = {"returned": return_segment_unet_time } )         
@@ -2200,29 +2194,29 @@
             pre_res.append(VollSeg(_x, unet_model = model_unet, roi_model = model_roi,
                        n_tiles=plugin_star_parameters.n_tiles.value, axes = axes_reorder, noise_model = noise_model,  RGB = plugin_extra_parameters.isRGB.value,
                                 min_size_mask=plugin_extra_parameters.min_size_mask.value,
                                 ExpandLabels = plugin_extra_parameters.expand_labels.value,
                                  seedpool= plugin_extra_parameters.seedpool.value, donormalize=plugin_star_parameters.norm_image.value,
                        lower_perc=plugin_star_parameters.perc_low.value, 
                        upper_perc=plugin_star_parameters.perc_high.value,
-                       max_size=plugin_extra_parameters.max_size.value, iou_threshold = plugin_extra_parameters.iouthresh.value,slice_merge = plugin_extra_parameters.slicemerge.value))
+                       max_size=plugin_extra_parameters.max_size.value, slice_merge = plugin_extra_parameters.slicemerge.value))
         
         pred = pre_res, scale_out, t, x
         return pred           
               
     @thread_worker(connect = {"returned": return_segment_unet } )         
     def _Unet( model_unet, model_roi, x, axes, noise_model, scale_out):
     
         res = VollSeg(x, unet_model = model_unet, roi_model = model_roi, n_tiles=plugin_star_parameters.n_tiles.value, axes = axes, noise_model = noise_model, donormalize=plugin_star_parameters.norm_image.value,
                        lower_perc=plugin_star_parameters.perc_low.value, 
                        ExpandLabels = plugin_extra_parameters.expand_labels.value,
                        upper_perc=plugin_star_parameters.perc_high.value,  RGB = plugin_extra_parameters.isRGB.value,
         min_size_mask=plugin_extra_parameters.min_size_mask.value, seedpool= plugin_extra_parameters.seedpool.value,
                        max_size=plugin_extra_parameters.max_size.value,
-                     iou_threshold = plugin_extra_parameters.iouthresh.value,slice_merge = plugin_extra_parameters.slicemerge.value)
+                     slice_merge = plugin_extra_parameters.slicemerge.value)
                     
         pred = res, scale_out
         return pred           
              
     @thread_worker (connect = {"returned": return_segment } )        
     def _Segment(model_star, model_unet,  model_roi, x, axes, noise_model, scale_out):
```

### Comparing `vollseg-napari-2.3.7/vollseg_napari/_test_dock_widget.py` & `vollseg-napari-2.3.8/vollseg_napari/_test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/vollseg_napari/_tests/test_open_sample_models.py` & `vollseg-napari-2.3.8/vollseg_napari/_tests/test_open_sample_models.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/vollseg_napari/napari.yaml` & `vollseg-napari-2.3.8/vollseg_napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/vollseg_napari/resources/kapoorlogo.png` & `vollseg-napari-2.3.8/vollseg_napari/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-2.3.7/vollseg_napari.egg-info/PKG-INFO` & `vollseg-napari-2.3.8/vollseg_napari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari
-Version: 2.3.7
+Version: 2.3.8
 Summary: Irregular cell shape segmentation using VollSeg
 Home-page: https://github.com/kapoorlab/vollseg-napari
 Author: Varun Kapoor
 Author-email: varun.kapoor@kapoorlabs.org
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/kapoorlab/vollseg-napari
 Project-URL: Documentation, https://github.com/kapoorlab/vollseg-napari
```


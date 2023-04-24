# Comparing `tmp/frat_brain-1.3.6.tar.gz` & `tmp/frat_brain-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.3.6.tar", max compression
+gzip compressed data, was "frat_brain-1.3.7.tar", max compression
```

## Comparing `frat_brain-1.3.6.tar` & `frat_brain-1.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.3.6/LICENSE
--rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.3.6/README.md
--rw-r--r--   0        0        0    54049 2023-04-05 12:18:29.787029 frat_brain-1.3.6/fRAT/__main__.py
--rw-r--r--   0        0        0       22 2023-04-03 15:48:56.862090 frat_brain-1.3.6/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.3.6/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.3.6/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4291 2023-03-30 13:46:51.091125 frat_brain-1.3.6/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.3.6/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17981 2023-04-20 15:58:41.535925 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.3.6/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.3.6/fRAT/nogui.py
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.3.6/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.3.6/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.3.6/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.3.6/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.3.6/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.3.6/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22256 2023-04-20 15:50:49.215386 frat_brain-1.3.6/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.3.6/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.3.6/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.3.6/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.3.6/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.3.6/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.3.6/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.3.6/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.3.6/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.3.6/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.3.6/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.3.6/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36613 2023-04-20 15:50:28.699673 frat_brain-1.3.6/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.3.6/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.3.6/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.3.6/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.3.6/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.3.6/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.3.6/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.3.6/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-04-20 16:00:24.878174 frat_brain-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.3.6/setup.py
--rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.3.7/LICENSE
+-rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.3.7/README.md
+-rw-r--r--   0        0        0    53941 2023-04-24 16:58:06.275544 frat_brain-1.3.7/fRAT/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-24 16:55:00.522387 frat_brain-1.3.7/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.3.7/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.3.7/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4291 2023-04-24 16:58:42.676825 frat_brain-1.3.7/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.3.7/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17981 2023-04-24 16:59:58.274205 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.3.7/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.3.7/fRAT/nogui.py
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.3.7/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.3.7/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.3.7/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.3.7/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.3.7/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.3.7/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 16:45:56.879209 frat_brain-1.3.7/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.3.7/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.3.7/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.3.7/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.3.7/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.3.7/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.3.7/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.3.7/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.3.7/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.3.7/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.3.7/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.3.7/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36718 2023-04-24 17:03:51.405210 frat_brain-1.3.7/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.3.7/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.3.7/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.3.7/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.3.7/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.3.7/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.3.7/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.3.7/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-04-24 17:02:53.370793 frat_brain-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.3.7/setup.py
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.3.7/PKG-INFO
```

### Comparing `frat_brain-1.3.6/LICENSE` & `frat_brain-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/README.md` & `frat_brain-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/__main__.py` & `frat_brain-1.3.7/fRAT/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,18 +992,14 @@
         print("{roi_num}: {roi}".format(roi_num=roi_num, roi=roi))
 
     print("----------------------------\n")
 
 
 def Save_settings(page_list, file):
     with open(f'{Path(os.path.abspath(__file__)).parents[0]}/configuration_profiles/{file}', 'w') as f:
-        f.write(f"# Version Info\n")
-        f.write(f"version = '{__version__}'\n")
-        f.write("\n")
-
         for page in page_list:
             if page == 'Home':
                 continue
 
             f.write(f"# {page}\n")
 
             for key in eval(page).keys():
```

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 output_folder_name = 'DEFAULT'                                                    # Directory to save output. If set to DEFAULT, the default name for the statistical map created will be used. Recommended: DEFAULT
 
 ## High pass filtering
 temporal_filter = true                                                            # true or false. Use a high pass filter to remove low frequency drift. Recommended: true
 highpass_filter_cutoff = 0.01                                                     # Highpass filter cutoff frequency converted into sigma in seconds using the formula 1/(2*f*TR). Recommended: 0.01
 
 ## Motion correction
-remove_motion_outliers = false                                                    # true or false. Use fsl_motion_outliers to remove motion outliers(uses default fsl_motion_outliers settings). Recommended: true
-motion_correction = false                                                         # true or false. Use MCFLIRT to motion correct volumes (uses default MCFLIRT settings). Recommended: true
+remove_motion_outliers = true                                                     # true or false. Use fsl_motion_outliers to remove motion outliers(uses default fsl_motion_outliers settings). Recommended: true
+motion_correction = true                                                          # true or false. Use MCFLIRT to motion correct volumes (uses default MCFLIRT settings). Recommended: true
 
 ## Spatial smoothing
 spatial_smoothing = false                                                         # true or false. Uses SUSAN to spatial smooth. Recommended: true
 smoothing_fwhm = 8.0                                                              # fwhm of smoothing, in mm, gets converted using sqrt(8*log(2)). Recommended: 8.0
 smoothing_brightness_threshold = 2000.0                                           # Should be greater than noise level and less than contrast of edges to be preserved. Recommended: 2000.0
 
 ## Image SNR calculation
 magnitude_correction = true                                                       # true or false. Correction factor of 0.7 applied when running iSNR calculations, to correct for Rayleigh distributed noise when using magnitude vs complex images.  Reference: Constantinides, C. D., Atalar, E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude Images from NMR Phased Arrays.
 noise_volume = false                                                              # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
 noise_volume_location = 'End'                                                     # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['Beginning', 'End'].
 iSNR_std_use_only_nonzero_voxels = true                                           # true or false.
 
 ## Add Gaussian noise
-noise_multipliers = [1, 2, 5]                                                     # Provide a comma-separated list of multipliers for the standard deviation of the gaussian noise to plot e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Noise has a gaussian distribution, with a mean of 0 and a standard deviation of the noise level of each participant * multiplier.
+noise_multipliers = 1                                                             # Provide a comma-separated list of multipliers for the standard deviation of the gaussian noise to plot e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Noise has a gaussian distribution, with a mean of 0 and a standard deviation of the noise level of each participant * multiplier.
```

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,122 +1,122 @@
 # General
-run_analysis = false                                                              # true or false. Can skip this step if json files have already been created.
-run_statistics = false                                                            # true or false.
+run_analysis = true                                                               # true or false. Can skip this step if json files have already been created.
+run_statistics = true                                                             # true or false.
 run_plotting = true                                                               # true or false.
 verbose = true                                                                    # true or false.
 verbose_cmd_line_args = false                                                     # true or false.
 multicore_processing = true                                                       # true or false. Use multicore processing during analysis? Multicore processing currently works within participants not between them. Recommended: true
 max_core_usage = 'max'                                                            # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['max', 6, 5, 4, 3, 2, 1].
 brain_file_loc = ''                                                               # Either the absolute location of brain files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 report_output_folder = ''                                                         # Either the absolute location of json files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 averaging_type = 'Participant averaged'                                           # Participant averaged or Session averaged. This setting is used to determine which statistics to use for plotting, and when accessing results (for example through the interactive report).  Note: Histograms will always use the raw results. The linear mixed model from the statistics will always use session averaged data Options: ['Session averaged', 'Participant averaged'].
 parameter_file = 'paramValues.csv'                                                # Recommended: paramValues.csv Name of the file to parse for critical params. Option added to allow quick swapping between different parameter files.
 file_cleanup = 'move'                                                             # Move or delete intermediate files. Options: ['move', 'delete'].
 
 ## Installation testing
-delete_test_folder = 'Never'                                                      # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
-verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
+delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
+verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
 input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
-output_folder = 'TEST'                                                            # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
+output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
-run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
+run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
-stat_map_suffix = '_tStd.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
+stat_map_suffix = '_tSNR.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
 conf_level_number = '95%, 1.96'                                                   # Set the confidence level for confidence interval calculations. Numbers represent the confidence level and the corresponding critical z value. Recommended: 95%, 1.96. Options: ['80%, 1.28', '85%, 1.44', '90%, 1.64', '95%, 1.96', '98%, 2.33', '99%, 2.58'].
 binary_params = ['']                                                              # Add parameters here which will either be on or off.
 
 ## Outlier detection
-noise_cutoff = false                                                              # true or false. Calculate a minimum cutoff value to be included in an ROI,based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff.  Useful for statistical maps where extracranial voxels are likely to have much lower values than those inside the brain such as tSNR maps. Recommended: true.
-gaussian_outlier_detection = false                                                # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
+noise_cutoff = true                                                               # true or false. Calculate a noise cutoff based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff, Recommended: true.
+gaussian_outlier_detection = true                                                 # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
 gaussian_outlier_contamination = 0.1                                              # Percent of expected outliers in dataset Recommended: 0.1
 gaussian_outlier_location = 'below gaussian'                                      # Data to remove (if gaussian outlier detection is true). For example: if set to below gaussian, data below the gaussian will be removed. Recommended: below gaussian. Options: ['below gaussian', 'above gaussian', 'both'].
 
 # Statistics
 automatically_create_statistics_options_file = true                               # true or false. Usually statisticsOptions.csv is automatically created when creating paramValues.csv. Deselect this option if you won't be running the statistics step. The create statisticsOptions.csv button above can also be used to manually create this file.
 statistics_subfolder_name = 'stats'                                               # Directory name for statistics folder.
 print_result = true                                                               # true or false. Prints results to terminal if true in addition to saving results to file.
 minimum_voxels = 400                                                              # For bootstrapped change versus baseline, for each ROI, the average number of voxels per session for an ROI must be above this value to be included in the analysis.For running the linear mixed model, for each ROI, any sessions with a voxel count below this value will be removed. Highly recommended to set a value here, as ROIs with a small number of voxels may suggest poor fitting. Recommended value 400
 bootstrap_samples = 1000                                                          # Recommended value 1000.  Note: Bootstrapping is only used to calculate percentage change versus baseline.
 bootstrap_confidence_interval = 95                                                # Recommended value: 95  Note: Bootstrapping is only used to calculate percentage change versus baseline.
-regional_stats_rois = ['all']                                                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
-include_as_variable = ['MB', 'SENSE']                                             # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take into account when balancing data for the main effect t test data.
-brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map. 
+regional_stats_rois = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+include_as_variable = ['Multiband', 'SENSE']                                      # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take to average across when running main effect t-tests.
+brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map.
 
 ## T-tests
-run_t_tests = true                                                                # true or false. 
-IV_type = ['Between-subjects', 'Between-subjects']                                # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
+run_t_tests = true                                                                # true or false.
+IV_type = ['Within-subjects', 'Within-subjects']                                  # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
 
 ## Linear mixed models
-run_linear_mixed_models = true                                                    # true or false. 
+run_linear_mixed_models = true                                                    # true or false.
 categorical_variables = ['']                                                      # Select which variables (if any) are categorical. Used for the LMM.
 main_effects = true                                                               # true or false. Note: This option is independent from the other effect calculations.
-main_and_interaction_effects = true                                               # true or false. Note: This option is independent from the other effect calculations.
+main_and_interaction_effects = false                                              # true or false. Note: This option is independent from the other effect calculations.
 interaction_effects = false                                                       # true or false. Note: This option is independent from the other effect calculations.
 
 ## R2 vs voxel count LMM
 max_below_thresh = 0                                                              # Recommended value 0.  For a given ROI, this value sets the maximum percent of sessions that can be excluded (due to having insufficient voxel count) before the ROI is not included in r2 vs voxel count statistics. With the default value of 100(%) an ROI will not be included in this calculation if any sessions have been excluded.
 
 # Parsing
-parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables. The critical parameter settings are used to supply the names and file name abbreviations of the independent variables, therefore `fRAT` supports the use of any parameters (and any number of them). As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
+parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables.   As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: This field can also be blank.
 parameter_dict2 = ['mb', 's']                                                     # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
 make_folder_structure = false                                                     # true or false. Make folder structure when creating paramValues.csv
 parsing_folder = 'func'                                                           # Folder to find files to add to paramValues.csv. If using "Make folder structure" option, this will be the directory the files in the participant folder will be moved to.
 
 # Plotting
 
 ## General plot settings
-plot_dpi = 600                                                                    # Recommended value 600
+plot_dpi = 200                                                                    # Recommended value 600
 plot_font_size = 40                                                               # Recommended value 30
 plot_scale = 10                                                                   # Recommended value 10
-make_violin_plot = false                                                          # true or false.
+make_violin_plot = true                                                           # true or false.
 make_brain_table = true                                                           # true or false.
-make_one_region_fig = false                                                       # true or false.
-make_histogram = false                                                            # true or false.
+make_one_region_fig = true                                                        # true or false.
+make_histogram = true                                                             # true or false.
 colorblind_friendly_plot_colours = ['#ffeda0', '#feb24c', '#fc4e2a', '#bd0026']   # Hex values of colourblind friendly colour scale.
-regional_fig_rois = ['all']                                                       # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+regional_fig_rois = [18, 20]                                                      # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
 
 ## Brain table
 brain_tight_layout = false                                                        # true or false. Use a tight layout when laying out the figure. Recommended: false
 brain_fig_value_min = 0                                                           # Provides the minimum value of the colourbar when creating mean and median images. For example, set minimum to 50 to make areas with values below 50 appear black. Recommended value: 0
 brain_fig_value_max = 'None'                                                      # Provides the maximum value of the colourbar when creating mean and median images. For example, set maximum to 50 to make areas with values above 50 appear as the brighest colour on the colourbar. Recommended value: None. Note: will default to 100 for scaled maps.
 brain_x_coord = -1                                                                # Voxel location to slice the images at in the x axis. Recommended settings for both variables: 91 or 58
 brain_z_coord = 19                                                                # Voxel location to slice the images at in the z axis. Recommended settings for both variables: 91 or 58
-brain_table_col_labels = 'Multiband'                                              # Label for columns.
+brain_table_col_labels = 'MB'                                                     # Label for columns.
 brain_table_row_labels = 'SENSE'                                                  # Label for rows.
-brain_table_cols = 'Multiband'                                                    # 
-brain_table_rows = 'SENSE'                                                        # 
+brain_table_cols = 'Multiband'                                                    #
+brain_table_rows = 'SENSE'                                                        #
 
 ## Violin plot
-table_x_label = 'tSNR mean'                                                       # 
-table_y_label = 'ROI'                                                             # 
+table_x_label = 'tSNR mean'                                                       #
+table_y_label = 'ROI'                                                             #
 violin_show_data = true                                                           # true or false.
 violin_jitter = true                                                              # true or false.
 violin_colour = '#fc4e2a'                                                         # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
 boxplot_colour = '#feb24c'                                                        # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
-table_cols = 'Multiband'                                                          # 
-table_rows = 'SENSE'                                                              # 
+table_cols = 'Multiband'                                                          #
+table_rows = 'SENSE'                                                              #
 
 ## Regional bar chart
-single_roi_fig_label_x = 'Multiband factor'                                       # 
-single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         # 
-single_roi_fig_label_fill = 'SENSE factor'                                        # 
-single_roi_fig_x_axis = 'Multiband'                                               # 
-single_roi_fig_colour = 'SENSE'                                                   # 
+single_roi_fig_label_x = 'Multiband factor'                                       #
+single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         #
+single_roi_fig_label_fill = 'SENSE factor'                                        #
+single_roi_fig_x_axis = 'Multiband'                                               #
+single_roi_fig_colour = 'SENSE'                                                   #
 
 ## Regional histogram
-histogram_binwidth = 2                                                            # 
-histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          # 
-histogram_fig_label_y = 'Frequency'                                               # 
-histogram_stat_line_size = 1.5                                                    # 
+histogram_binwidth = 2                                                            #
+histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          #
+histogram_fig_label_y = 'Frequency'                                               #
+histogram_stat_line_size = 1.5                                                    #
 histogram_show_mean = true                                                        # true or false.
 histogram_show_median = true                                                      # true or false.
 histogram_show_legend = true                                                      # true or false.
-histogram_fig_x_facet = 'Multiband'                                               # 
-histogram_fig_y_facet = 'SENSE'                                                   # 
+histogram_fig_x_facet = 'Multiband'                                               #
+histogram_fig_y_facet = 'SENSE'                                                   #
 histogram_fig_colour = '#fc4e2a'                                                  # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
```

### Comparing `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,114 +9,114 @@
 brain_file_loc = ''                                                               # Either the absolute location of brain files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 report_output_folder = ''                                                         # Either the absolute location of json files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 averaging_type = 'Participant averaged'                                           # Participant averaged or Session averaged. This setting is used to determine which statistics to use for plotting, and when accessing results (for example through the interactive report).  Note: Histograms will always use the raw results. The linear mixed model from the statistics will always use session averaged data Options: ['Session averaged', 'Participant averaged'].
 parameter_file = 'paramValues.csv'                                                # Recommended: paramValues.csv Name of the file to parse for critical params. Option added to allow quick swapping between different parameter files.
 file_cleanup = 'move'                                                             # Move or delete intermediate files. Options: ['move', 'delete'].
 
 ## Installation testing
-delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
-verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
+delete_test_folder = 'If completed without error'                                 # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
+verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
 input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
-run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
+run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
 stat_map_suffix = '_tSNR.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
 conf_level_number = '95%, 1.96'                                                   # Set the confidence level for confidence interval calculations. Numbers represent the confidence level and the corresponding critical z value. Recommended: 95%, 1.96. Options: ['80%, 1.28', '85%, 1.44', '90%, 1.64', '95%, 1.96', '98%, 2.33', '99%, 2.58'].
 binary_params = ['']                                                              # Add parameters here which will either be on or off.
 
 ## Outlier detection
-noise_cutoff = true                                                               # true or false. Calculate a noise cutoff based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff, Recommended: true.
+noise_cutoff = true                                                               # true or false. Calculate a minimum cutoff value to be included in an ROI,based on voxels not assigned an ROI or that have been excluded from analysis. Voxels with values of 0 are not included when calculating the noise cutoff.  Useful for statistical maps where extracranial voxels are likely to have much lower values than those inside the brain such as tSNR maps. Recommended: true.
 gaussian_outlier_detection = true                                                 # true or false. Fit a gaussian to the data to determine outliers using Elliptic Envelope. Recommended: true.
 gaussian_outlier_contamination = 0.1                                              # Percent of expected outliers in dataset Recommended: 0.1
 gaussian_outlier_location = 'below gaussian'                                      # Data to remove (if gaussian outlier detection is true). For example: if set to below gaussian, data below the gaussian will be removed. Recommended: below gaussian. Options: ['below gaussian', 'above gaussian', 'both'].
 
 # Statistics
 automatically_create_statistics_options_file = true                               # true or false. Usually statisticsOptions.csv is automatically created when creating paramValues.csv. Deselect this option if you won't be running the statistics step. The create statisticsOptions.csv button above can also be used to manually create this file.
 statistics_subfolder_name = 'stats'                                               # Directory name for statistics folder.
 print_result = true                                                               # true or false. Prints results to terminal if true in addition to saving results to file.
 minimum_voxels = 400                                                              # For bootstrapped change versus baseline, for each ROI, the average number of voxels per session for an ROI must be above this value to be included in the analysis.For running the linear mixed model, for each ROI, any sessions with a voxel count below this value will be removed. Highly recommended to set a value here, as ROIs with a small number of voxels may suggest poor fitting. Recommended value 400
 bootstrap_samples = 1000                                                          # Recommended value 1000.  Note: Bootstrapping is only used to calculate percentage change versus baseline.
 bootstrap_confidence_interval = 95                                                # Recommended value: 95  Note: Bootstrapping is only used to calculate percentage change versus baseline.
-regional_stats_rois = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
-include_as_variable = ['Multiband', 'SENSE']                                      # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take to average across when running main effect t-tests.
-brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map.
+regional_stats_rois = ['all']                                                     # Provide a comma-separated list of regions, e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+include_as_variable = ['INCLUDE ALL VARIABLES']                                   # Select which variables to include in statistical analysis. Used to determine which variables to use as fixed effects in linear mixed models and which variables to take into account when balancing data for the main effect t test data.
+brain_map_p_thresh = 0.05                                                         # P-value threshold to use when creating brain coefficient maps. Any fixed effect that doesn't have a p-value equal to or less than this value will not be included in the coefficient map. 
 
 ## T-tests
-run_t_tests = true                                                                # true or false.
-IV_type = ['Within-subjects', 'Within-subjects']                                  # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
+run_t_tests = true                                                                # true or false. 
+IV_type = ['FILL IV TYPE AS BETWEEN-SUBJECTS']                                    # Type of variable collected. Used to choose which t-test to use for pairwise comparisons.
 
 ## Linear mixed models
-run_linear_mixed_models = true                                                    # true or false.
+run_linear_mixed_models = true                                                    # true or false. 
 categorical_variables = ['']                                                      # Select which variables (if any) are categorical. Used for the LMM.
 main_effects = true                                                               # true or false. Note: This option is independent from the other effect calculations.
-main_and_interaction_effects = false                                              # true or false. Note: This option is independent from the other effect calculations.
+main_and_interaction_effects = true                                               # true or false. Note: This option is independent from the other effect calculations.
 interaction_effects = false                                                       # true or false. Note: This option is independent from the other effect calculations.
 
 ## R2 vs voxel count LMM
 max_below_thresh = 0                                                              # Recommended value 0.  For a given ROI, this value sets the maximum percent of sessions that can be excluded (due to having insufficient voxel count) before the ROI is not included in r2 vs voxel count statistics. With the default value of 100(%) an ROI will not be included in this calculation if any sessions have been excluded.
 
 # Parsing
-parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables.   As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: This field can also be blank.
+parameter_dict1 = ['MB', 'SENSE']                                                 # Comma-separated list of independent variables. The critical parameter settings are used to supply the names and file name abbreviations of the independent variables, therefore `fRAT` supports the use of any parameters (and any number of them). As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
 parameter_dict2 = ['mb', 's']                                                     # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
-make_folder_structure = false                                                     # true or false. Make folder structure when creating paramValues.csv
+make_folder_structure = true                                                      # true or false. Make folder structure when creating paramValues.csv
 parsing_folder = 'func'                                                           # Folder to find files to add to paramValues.csv. If using "Make folder structure" option, this will be the directory the files in the participant folder will be moved to.
 
 # Plotting
 
 ## General plot settings
-plot_dpi = 200                                                                    # Recommended value 600
+plot_dpi = 600                                                                    # Recommended value 600
 plot_font_size = 40                                                               # Recommended value 30
 plot_scale = 10                                                                   # Recommended value 10
 make_violin_plot = true                                                           # true or false.
 make_brain_table = true                                                           # true or false.
 make_one_region_fig = true                                                        # true or false.
 make_histogram = true                                                             # true or false.
 colorblind_friendly_plot_colours = ['#ffeda0', '#feb24c', '#fc4e2a', '#bd0026']   # Hex values of colourblind friendly colour scale.
-regional_fig_rois = [18, 20]                                                      # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
+regional_fig_rois = ['all']                                                       # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
 
 ## Brain table
 brain_tight_layout = false                                                        # true or false. Use a tight layout when laying out the figure. Recommended: false
 brain_fig_value_min = 0                                                           # Provides the minimum value of the colourbar when creating mean and median images. For example, set minimum to 50 to make areas with values below 50 appear black. Recommended value: 0
 brain_fig_value_max = 'None'                                                      # Provides the maximum value of the colourbar when creating mean and median images. For example, set maximum to 50 to make areas with values above 50 appear as the brighest colour on the colourbar. Recommended value: None. Note: will default to 100 for scaled maps.
 brain_x_coord = -1                                                                # Voxel location to slice the images at in the x axis. Recommended settings for both variables: 91 or 58
 brain_z_coord = 19                                                                # Voxel location to slice the images at in the z axis. Recommended settings for both variables: 91 or 58
-brain_table_col_labels = 'MB'                                                     # Label for columns.
-brain_table_row_labels = 'SENSE'                                                  # Label for rows.
-brain_table_cols = 'Multiband'                                                    #
-brain_table_rows = 'SENSE'                                                        #
+brain_table_col_labels = 'CHANGE TO DESIRED LABEL'                                # Label for columns.
+brain_table_row_labels = 'CHANGE TO DESIRED LABEL'                                # Label for rows.
+brain_table_cols = 'DEFAULT'                                                      # 
+brain_table_rows = 'DEFAULT'                                                      # 
 
 ## Violin plot
-table_x_label = 'tSNR mean'                                                       #
-table_y_label = 'ROI'                                                             #
+table_x_label = 'tSNR mean'                                                       # 
+table_y_label = 'ROI'                                                             # 
 violin_show_data = true                                                           # true or false.
 violin_jitter = true                                                              # true or false.
 violin_colour = '#fc4e2a'                                                         # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
 boxplot_colour = '#feb24c'                                                        # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
-table_cols = 'Multiband'                                                          #
-table_rows = 'SENSE'                                                              #
+table_cols = 'DEFAULT'                                                            # 
+table_rows = 'DEFAULT'                                                            # 
 
 ## Regional bar chart
-single_roi_fig_label_x = 'Multiband factor'                                       #
-single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         #
-single_roi_fig_label_fill = 'SENSE factor'                                        #
-single_roi_fig_x_axis = 'Multiband'                                               #
-single_roi_fig_colour = 'SENSE'                                                   #
+single_roi_fig_label_x = 'Multiband factor'                                       # 
+single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         # 
+single_roi_fig_label_fill = 'SENSE factor'                                        # 
+single_roi_fig_x_axis = 'DEFAULT'                                                 # 
+single_roi_fig_colour = 'DEFAULT'                                                 # 
 
 ## Regional histogram
-histogram_binwidth = 2                                                            #
-histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          #
-histogram_fig_label_y = 'Frequency'                                               #
-histogram_stat_line_size = 1.5                                                    #
+histogram_binwidth = 2                                                            # 
+histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          # 
+histogram_fig_label_y = 'Frequency'                                               # 
+histogram_stat_line_size = 1.5                                                    # 
 histogram_show_mean = true                                                        # true or false.
 histogram_show_median = true                                                      # true or false.
 histogram_show_legend = true                                                      # true or false.
-histogram_fig_x_facet = 'Multiband'                                               #
-histogram_fig_y_facet = 'SENSE'                                                   #
+histogram_fig_x_facet = 'DEFAULT'                                                 # 
+histogram_fig_y_facet = 'DEFAULT'                                                 # 
 histogram_fig_colour = '#fc4e2a'                                                  # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
```

### Comparing `frat_brain-1.3.6/fRAT/images/fRAT.gif` & `frat_brain-1.3.7/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/nogui.py` & `frat_brain-1.3.7/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 15:50:28 2023 UTC, .py size: 36613 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,1391 +1,1393 @@
-00000000: 6f0d 0d0a 0000 0000 445f 4164 058f 0000  o.......D_Ad....
+00000000: 6f0d 0d0a 0000 0000 42b2 4664 2e8f 0000  o.......B.Fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 1801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c08 6d09 5a0a 0100 6400 6401 6c0b  d.l.m.Z...d.d.l.
 00000080: 5a0c 6400 6401 6c0d 5a0e 6400 6401 6c0f  Z.d.d.l.Z.d.d.l.
 00000090: 5a10 6400 6401 6c11 5a12 6400 6401 6c13  Z.d.d.l.Z.d.d.l.
 000000a0: 5a14 6400 6404 6c15 6d16 5a16 0100 6400  Z.d.d.l.m.Z...d.
 000000b0: 6405 6c17 6d18 5a19 0100 6400 6406 6c1a  d.l.m.Z...d.d.l.
-000000c0: 6d1b 5a1b 0100 6407 6408 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000d0: 0100 4700 6409 640a 8400 640a 8302 5a1e  ..G.d.d...d...Z.
-000000e0: 4700 640b 640c 8400 640c 651e 8303 5a1f  G.d.d...d.e...Z.
-000000f0: 4700 640d 640e 8400 640e 651e 8303 5a20  G.d.d...d.e...Z 
-00000100: 4700 640f 6410 8400 6410 651e 8303 5a21  G.d.d...d.e...Z!
-00000110: 4700 6411 6412 8400 6412 651e 8303 5a22  G.d.d...d.e...Z"
-00000120: 4700 6413 6414 8400 6414 651e 8303 5a23  G.d.d...d.e...Z#
-00000130: 6401 5300 2915 e900 0000 004e a901 da04  d.S.)......N....
-00000140: 676c 6f62 2901 da04 5061 7468 2901 da08  glob)...Path)...
-00000150: 706c 6f74 7469 6e67 2901 da06 7079 706c  plotting)...pypl
-00000160: 6f74 2901 da05 496d 6167 65e9 0100 0000  ot)...Image.....
-00000170: 2901 da05 5574 696c 7363 0000 0000 0000  )...Utilsc......
-00000180: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000190: 0000 7340 0000 0065 005a 0164 005a 0264  ..s@...e.Z.d.Z.d
-000001a0: 015a 0365 0464 0264 0384 0083 015a 0565  .Z.e.d.d.....Z.e
-000001b0: 0664 0464 0584 0083 015a 0765 0664 0664  .d.d.....Z.e.d.d
-000001c0: 0784 0083 015a 0865 0664 0864 0984 0083  .....Z.e.d.d....
-000001d0: 015a 0964 0153 0029 0ada 0746 6967 7572  .Z.d.S.)...Figur
-000001e0: 6573 4e63 0400 0000 0000 0000 0000 0000  esNc............
-000001f0: 0700 0000 0b00 0000 4300 0000 7344 0100  ........C...sD..
-00000200: 007c 017c 005f 0074 01a0 0274 03a0 04a1  .|.|._.t...t....
-00000210: 007c 006a 006a 05a1 025c 027d 047d 0574  .|.j.j...\.}.}.t
-00000220: 036a 06a0 0764 01a1 0173 1a74 03a0 0864  .j...d...s.t...d
-00000230: 01a1 0101 0074 016a 0964 017c 027c 0364  .....t.j.d.|.|.d
-00000240: 0264 0364 0467 0264 057c 016a 05a0 0a64  .d.d.g.d.|.j...d
-00000250: 0664 07a1 02a0 0ba1 009b 0064 089d 0367  .d.........d...g
-00000260: 0164 098d 0601 007c 006a 006a 0c72 4674  .d.....|.j.j.rFt
-00000270: 0d64 0a7c 016a 05a0 0a64 0664 07a1 02a0  .d.|.j...d.d....
-00000280: 0ba1 009b 0064 0b9d 0383 0101 007c 006a  .....d.......|.j
-00000290: 006a 0e7c 006a 006a 0f70 507c 006a 006a  .j.|.j.j.pP|.j.j
-000002a0: 1040 0072 5774 01a0 11a1 007d 066e 0264  .@.rWt.....}.n.d
-000002b0: 007d 067c 006a 006a 1272 6a7c 006a 006a  .}.|.j.j.rj|.j.j
-000002c0: 0c72 6574 0d64 0c83 0101 0074 13a0 147c  .ret.d.....t...|
-000002d0: 04a1 0101 007c 006a 006a 1572 807c 006a  .....|.j.j.r.|.j
-000002e0: 006a 0c72 7674 0d64 0d83 0101 0074 01a0  .j.rvt.d.....t..
-000002f0: 1664 0ea1 0101 0074 17a0 147c 04a1 0101  .d.....t...|....
-00000300: 007c 006a 006a 0f72 8a74 18a0 197c 047c  .|.j.j.r.t...|.|
-00000310: 06a1 0201 007c 006a 006a 1072 9474 1aa0  .....|.j.j.r.t..
-00000320: 197c 047c 06a1 0201 007c 0672 a07c 06a0  .|.|.....|.r.|..
-00000330: 1ba1 0001 007c 06a0 1ca1 0001 0064 0053  .....|.......d.S
-00000340: 0064 0053 0029 0f4e 720a 0000 005a 0a66  .d.S.).Nr....Z.f
-00000350: 6967 7572 655f 6c6f 67da 0750 6172 7369  igure_log..Parsi
-00000360: 6e67 da08 506c 6f74 7469 6e67 7a19 6461  ng..Plottingz.da
-00000370: 7461 5f75 7365 645f 666f 725f 6669 6775  ta_used_for_figu
-00000380: 7265 7320 3d20 22fa 0120 da01 5ffa 0122  res = ".. .._.."
-00000390: 2903 da0f 6e65 775f 636f 6e66 6967 5f6e  )...new_config_n
-000003a0: 616d 65da 1172 656c 6576 616e 745f 7365  ame..relevant_se
-000003b0: 6374 696f 6e73 da0f 6164 6469 7469 6f6e  ctions..addition
-000003c0: 616c 5f69 6e66 6f7a 070a 5573 696e 6720  al_infoz..Using 
-000003d0: 7a18 2064 6174 6120 746f 2063 7265 6174  z. data to creat
-000003e0: 6520 6669 6775 7265 732e 7a1c 0a2d 2d2d  e figures.z..---
-000003f0: 2042 7261 696e 2067 7269 6420 6372 6561   Brain grid crea
-00000400: 7469 6f6e 202d 2d2d 7a1d 0a2d 2d2d 2056  tion ---z..--- V
-00000410: 696f 6c69 6e20 706c 6f74 2063 7265 6174  iolin plot creat
-00000420: 696f 6e20 2d2d 2d7a 1446 6967 7572 6573  ion ---z.Figures
-00000430: 2f56 696f 6c69 6e5f 706c 6f74 7329 1dda  /Violin_plots)..
-00000440: 0663 6f6e 6669 6772 0900 0000 da15 7265  .configr......re
-00000450: 6164 5f63 6f6d 6269 6e65 645f 7265 7375  ad_combined_resu
-00000460: 6c74 73da 026f 73da 0667 6574 6377 64da  lts..os..getcwd.
-00000470: 0e61 7665 7261 6769 6e67 5f74 7970 65da  .averaging_type.
-00000480: 0470 6174 68da 0665 7869 7374 73da 086d  .path..exists..m
-00000490: 616b 6564 6972 73da 0b73 6176 655f 636f  akedirs..save_co
-000004a0: 6e66 6967 da07 7265 706c 6163 65da 056c  nfig..replace..l
-000004b0: 6f77 6572 da07 7665 7262 6f73 65da 0570  ower..verbose..p
-000004c0: 7269 6e74 da14 6d75 6c74 6963 6f72 655f  rint..multicore_
-000004d0: 7072 6f63 6573 7369 6e67 da13 6d61 6b65  processing..make
-000004e0: 5f6f 6e65 5f72 6567 696f 6e5f 6669 67da  _one_region_fig.
-000004f0: 0e6d 616b 655f 6869 7374 6f67 7261 6dda  .make_histogram.
-00000500: 1573 7461 7274 5f70 726f 6365 7373 696e  .start_processin
-00000510: 675f 706f 6f6c da10 6d61 6b65 5f62 7261  g_pool..make_bra
-00000520: 696e 5f74 6162 6c65 da09 4272 6169 6e47  in_table..BrainG
-00000530: 7269 64da 046d 616b 65da 106d 616b 655f  rid..make..make_
-00000540: 7669 6f6c 696e 5f70 6c6f 74da 1263 6865  violin_plot..che
-00000550: 636b 5f61 6e64 5f6d 616b 655f 6469 72da  ck_and_make_dir.
-00000560: 0a56 696f 6c69 6e50 6c6f 74da 0842 6172  .ViolinPlot..Bar
-00000570: 6368 6172 74da 0573 6574 7570 da09 4869  chart..setup..Hi
-00000580: 7374 6f67 7261 6dda 0563 6c6f 7365 da04  stogram..close..
-00000590: 6a6f 696e 2907 da03 636c 73da 0363 6667  join)...cls..cfg
-000005a0: da0b 636f 6e66 6967 5f70 6174 68da 0f63  ..config_path..c
-000005b0: 6f6e 6669 675f 6669 6c65 6e61 6d65 da13  onfig_filename..
-000005c0: 636f 6d62 696e 6564 5f72 6573 756c 7473  combined_results
-000005d0: 5f64 6672 0e00 0000 da04 706f 6f6c a900  _dfr......pool..
-000005e0: 7235 0000 00fa 522f 5573 6572 732f 6c70  r5....R/Users/lp
-000005f0: 7865 6831 302f 446f 6375 6d65 6e74 732f  xeh10/Documents/
-00000600: 5265 706f 7369 746f 7269 6573 2f66 4d52  Repositories/fMR
-00000610: 495f 524f 495f 616e 616c 7973 6973 5f74  I_ROI_analysis_t
-00000620: 6f6f 6c2f 6652 4154 2f75 7469 6c73 2f66  ool/fRAT/utils/f
-00000630: 6967 7572 6573 2e70 79da 0c6d 616b 655f  igures.py..make_
-00000640: 6669 6775 7265 7319 0000 0073 4600 0000  figures....sF...
-00000650: 0602 1802 0c02 0a01 0a02 0201 0201 0201  ................
-00000660: 02ff 0202 1001 08ff 06fc 0807 1e01 1802  ................
-00000670: 0a01 0402 0802 0801 0801 0a02 0802 0801  ................
-00000680: 0801 0a02 0a01 0802 0c01 0802 0c01 0402  ................
-00000690: 0801 0c01 04fe 7a14 4669 6775 7265 732e  ......z.Figures.
-000006a0: 6d61 6b65 5f66 6967 7572 6573 6303 0000  make_figuresc...
-000006b0: 0000 0000 0000 0000 0006 0000 0002 0000  ................
-000006c0: 0043 0000 0073 4a00 0000 7c01 a000 a100  .C...sJ...|.....
-000006d0: 7d03 7c03 6a01 7d04 7c02 6401 6b02 7212  }.|.j.}.|.d.k.r.
-000006e0: 7c04 6402 1900 a002 a100 7d05 6e0a 7c02  |.d.......}.n.|.
-000006f0: 6403 6b02 721c 7c04 6402 1900 a003 a100  d.k.r.|.d.......
-00000700: 7d05 6700 7c05 a201 7c00 9101 5200 7d05  }.g.|...|...R.}.
-00000710: 7c05 5300 2904 4eda 0578 6178 6973 7201  |.S.).N..xaxisr.
-00000720: 0000 00da 0579 6178 6973 2904 da04 6472  .....yaxis)...dr
-00000730: 6177 da04 6178 6573 da08 6765 745f 786c  aw..axes..get_xl
-00000740: 696d da08 6765 745f 796c 696d 2906 da07  im..get_ylim)...
-00000750: 7468 6973 726f 69da 0666 6967 7572 65da  thisroi..figure.
-00000760: 0461 7869 73da 0366 6967 723b 0000 00da  .axis..figr;....
-00000770: 036c 696d 7235 0000 0072 3500 0000 7236  .limr5...r5...r6
-00000780: 0000 00da 0f66 696e 645f 6178 6973 5f6c  .....find_axis_l
-00000790: 696d 6974 4800 0000 7310 0000 0008 0306  imitH...s.......
-000007a0: 0108 020e 0108 020c 010e 0204 027a 1746  .............z.F
-000007b0: 6967 7572 6573 2e66 696e 645f 6178 6973  igures.find_axis
-000007c0: 5f6c 696d 6974 6305 0000 0000 0000 0000  _limitc.........
-000007d0: 0000 0008 0000 000a 0000 0043 0000 0073  ...........C...s
-000007e0: e400 0000 6700 6401 a201 7d05 7c01 a000  ....g.d...}.|...
-000007f0: 6402 6403 a102 7d01 7c05 4400 5d0b 5c02  d.d...}.|.D.].\.
-00000800: 7d06 7d07 7401 a002 7c06 7c07 7c01 a103  }.}.t...|.|.|...
-00000810: 7d01 710c 7403 a004 6404 7c03 a005 a100  }.q.t...d.|.....
-00000820: 9b00 6405 7c02 9b00 6406 9d05 a101 0100  ..d.|...d.......
-00000830: 7c00 6a06 6404 7c03 a005 a100 9b00 6405  |.j.d.|.......d.
-00000840: 7c02 9b00 6406 7c01 9b00 6407 7c03 9b00  |...d.|...d.|...
-00000850: 6408 9d09 7c04 6a07 7c04 6a07 6409 1400  d...|.j.|.j.d...
-00000860: 640a 640a 640b 8d05 0100 7c00 6a06 6404  d.d.d.....|.j.d.
-00000870: 7c03 a005 a100 9b00 6405 7c02 9b00 6406  |.......d.|...d.
-00000880: 7c01 9b00 6407 7c03 9b00 640c 9d09 7c04  |...d.|...d...|.
-00000890: 6a07 7c04 6a07 6409 1400 640a 640a 640b  j.|.j.d...d.d.d.
-000008a0: 8d05 0100 7c04 6a08 7270 7409 640d 7c01  ....|.j.rpt.d.|.
-000008b0: 9b00 6407 7c03 9b00 6408 9d05 8301 0100  ..d.|...d.......
-000008c0: 6400 5300 6400 5300 290e 4e29 0329 027a  d.S.d.S.).N).).z
-000008d0: 0a5c 285b 5e28 295d 2a5c 29da 0029 027a  .\([^()]*\)..).z
-000008e0: 0c5b 5e61 2d7a 412d 5a5c 643a 5d72 0e00  .[^a-zA-Z\d:]r..
-000008f0: 0000 2902 7a05 5f7b 322c 7d72 0e00 0000  ..).z._{2,}r....
-00000900: fa01 2772 4400 0000 7a08 4669 6775 7265  ..'rD...z.Figure
-00000910: 732f 7a02 732f fa01 2f72 0e00 0000 fa04  s/z.s/../r......
-00000920: 2e70 6e67 e903 0000 0046 a904 da06 6865  .png.....F....he
-00000930: 6967 6874 da05 7769 6474 6872 1e00 0000  ight..widthr....
-00000940: 5a09 6c69 6d69 7473 697a 65fa 042e 7376  Z.limitsize...sv
-00000950: 677a 0653 6176 6564 2029 0a72 1c00 0000  gz.Saved ).r....
-00000960: da02 7265 da03 7375 6272 0900 0000 7228  ..re..subr....r(
-00000970: 0000 00da 0574 6974 6c65 da04 7361 7665  .....title..save
-00000980: da0a 706c 6f74 5f73 6361 6c65 721e 0000  ..plot_scaler...
-00000990: 0072 1f00 0000 2908 723f 0000 0072 3e00  .r....).r?...r>.
-000009a0: 0000 da06 666f 6c64 6572 5a0a 6368 6172  ....folderZ.char
-000009b0: 745f 7479 7065 7213 0000 00da 0c72 6570  t_typer......rep
-000009c0: 6c61 6365 6d65 6e74 73da 036f 6c64 da03  lacements..old..
-000009d0: 6e65 7772 3500 0000 7235 0000 0072 3600  newr5...r5...r6.
-000009e0: 0000 da0b 6669 6775 7265 5f73 6176 6558  ....figure_saveX
-000009f0: 0000 0073 2000 0000 0803 0c05 0c01 1001  ...s ...........
-00000a00: 1c02 2401 0c01 0401 06fe 2404 0c01 0401  ..$.......$.....
-00000a10: 06fe 0604 1a01 04ff 7a13 4669 6775 7265  ........z.Figure
-00000a20: 732e 6669 6775 7265 5f73 6176 6563 0400  s.figure_savec..
-00000a30: 0000 0000 0000 0000 0000 1000 0000 0900  ................
-00000a40: 0000 4300 0000 73cc 0100 0074 00a0 01a1  ..C...s....t....
-00000a50: 007d 047c 0364 016b 0272 1774 0274 0364  .}.|.d.k.r.t.t.d
-00000a60: 0067 007c 006a 04a2 0164 0291 0164 0391  .g.|.j...d...d..
-00000a70: 0183 0283 017d 056e 0c74 0274 0364 007c  .....}.n.t.t.d.|
-00000a80: 006a 057c 006a 0664 0267 0383 0283 017d  .j.|.j.d.g.....}
-00000a90: 057c 0144 005d 967d 0674 077c 0664 0483  .|.D.].}.t.|.d..
-00000aa0: 028f 107d 0774 08a0 0974 0aa0 0b7c 07a1  ...}.t...t...|..
-00000ab0: 01a1 017d 0857 0064 0004 0004 0083 0301  ...}.W.d........
-00000ac0: 006e 0831 0073 3f77 0101 0001 0001 0059  .n.1.s?w.......Y
-00000ad0: 0001 007a 097c 086a 0c64 0564 0667 0219  ...z.|.j.d.d.g..
-00000ae0: 007d 0857 006e 0904 0074 0d79 5601 0001  .}.W.n...t.yV...
-00000af0: 0001 0059 006e 0177 0067 0064 07a2 017d  ...Y.n.w.g.d...}
-00000b00: 0974 0e6a 0fa0 107c 06a1 017d 0a7c 0944  .t.j...|...}.|.D
-00000b10: 005d 097d 0b7c 0aa0 117c 0ba1 0164 0819  .].}.|...|...d..
-00000b20: 007d 0a71 637c 026a 0c7c 0264 0219 006a  .}.qc|.j.|.d...j
-00000b30: 12a0 13a1 007c 0aa0 13a1 006b 0219 007d  .....|.....k...}
-00000b40: 0c7c 0c6a 146a 12a0 13a1 007c 0c5f 147a  .|.j.j.....|._.z
-00000b50: 127c 0544 005d 0d7d 0d7c 0c7c 0da0 13a1  .|.D.].}.|.|....
-00000b60: 0019 006a 1564 0819 007c 087c 0d3c 0071  ...j.d...|.|.<.q
-00000b70: 8557 006e 1104 0074 0d79 9d01 0001 0001  .W.n...t.y......
-00000b80: 0059 006e 0904 0074 1679 a501 0001 0001  .Y.n...t.y......
-00000b90: 0059 0071 2577 007c 0364 016b 0272 b474  .Y.q%w.|.d.k.r.t
-00000ba0: 17a0 1864 097c 06a1 0264 0819 007c 0864  ...d.|...d...|.d
-00000bb0: 033c 0074 00a0 197c 047c 0867 02a1 017d  .<.t...|.|.g...}
-00000bc0: 0471 257c 046a 1564 0864 0064 0a85 0319  .q%|.j.d.d.d....
-00000bd0: 006a 1a7c 0564 0b64 0c64 0d8d 037d 0e7c  .j.|.d.d.d...}.|
-00000be0: 046a 1564 0e64 0064 0a85 0319 006a 1a7c  .j.d.d.d.....j.|
-00000bf0: 0564 0b64 0c64 0d8d 037d 0f7c 0f64 0c19  .d.d.d...}.|.d..
-00000c00: 007c 0e64 0f3c 007c 0e6a 1b64 1064 118d  .|.d.<.|.j.d.d..
-00000c10: 0101 007c 0e53 0029 124e da0a 7374 6174  ...|.S.).N..stat
-00000c20: 6973 7469 6373 da09 4669 6c65 5f6e 616d  istics..File_nam
-00000c30: 65da 0773 7562 6a65 6374 da01 72da 044d  e..subject..r..M
-00000c40: 6561 6eda 0656 6f78 656c 7329 03da 035f  ean..Voxels)..._
-00000c50: 7073 da04 5f72 6177 7a05 2e6a 736f 6e72  ps.._rawz..jsonr
-00000c60: 0100 0000 7a0a 7375 622d 5b30 2d39 5d2a  ....z.sub-[0-9]*
-00000c70: e902 0000 00da 0352 4f49 da0b 766f 7865  .......ROI..voxe
-00000c80: 6c5f 7661 6c75 6529 03da 0769 645f 7661  l_value)...id_va
-00000c90: 7273 da08 7661 725f 6e61 6d65 da0a 7661  rs..var_name..va
-00000ca0: 6c75 655f 6e61 6d65 7208 0000 005a 0c76  lue_namer....Z.v
-00000cb0: 6f78 656c 5f61 6d6f 756e 7454 2901 da07  oxel_amountT)...
-00000cc0: 696e 706c 6163 6529 1cda 0270 64da 0944  inplace)...pd..D
-00000cd0: 6174 6146 7261 6d65 da04 6c69 7374 da06  ataFrame..list..
-00000ce0: 6669 6c74 6572 da0f 7061 7261 6d65 7465  filter..paramete
-00000cf0: 725f 6469 6374 31da 1568 6973 746f 6772  r_dict1..histogr
-00000d00: 616d 5f66 6967 5f78 5f66 6163 6574 da15  am_fig_x_facet..
-00000d10: 6869 7374 6f67 7261 6d5f 6669 675f 795f  histogram_fig_y_
-00000d20: 6661 6365 74da 046f 7065 6e72 0900 0000  facet..openr....
-00000d30: da11 6469 6374 5f74 6f5f 6461 7461 6672  ..dict_to_datafr
-00000d40: 616d 65da 046a 736f 6eda 046c 6f61 64da  ame..json..load.
-00000d50: 036c 6f63 da08 4b65 7945 7272 6f72 7215  .loc..KeyErrorr.
-00000d60: 0000 0072 1800 0000 da08 6261 7365 6e61  ...r......basena
-00000d70: 6d65 da06 7273 706c 6974 da03 7374 7272  me..rsplit..strr
-00000d80: 1d00 0000 da07 636f 6c75 6d6e 73da 0469  ......columns..i
-00000d90: 6c6f 63da 0a49 6e64 6578 4572 726f 7272  loc..IndexErrorr
-00000da0: 4d00 0000 da07 6669 6e64 616c 6cda 0663  M.....findall..c
-00000db0: 6f6e 6361 74da 046d 656c 74da 0664 726f  oncat..melt..dro
-00000dc0: 706e 6129 1072 1300 0000 da05 6a73 6f6e  pna).r......json
-00000dd0: 73da 0b63 6f6d 6269 6e65 645f 6466 da09  s..combined_df..
-00000de0: 6461 7461 5f74 7970 65da 0f63 6f6d 6269  data_type..combi
-00000df0: 6e65 645f 7261 775f 6466 da0e 7369 676e  ned_raw_df..sign
-00000e00: 6966 5f63 6f6c 756d 6e73 da09 6a73 6f6e  if_columns..json
-00000e10: 5f66 696c 65da 0166 5a0c 6375 7272 656e  _file..fZ.curren
-00000e20: 745f 6a73 6f6e 5a0a 6465 6c69 6d65 7465  t_jsonZ.delimete
-00000e30: 7273 da0e 6a73 6f6e 5f66 696c 655f 6e61  rs..json_file_na
-00000e40: 6d65 5a09 6465 6c69 6d65 7465 725a 1263  meZ.delimeterZ.c
-00000e50: 6f6d 6269 6e65 645f 6466 5f73 6561 7263  ombined_df_searc
-00000e60: 68da 0663 6f6c 756d 6e5a 096d 6561 6e5f  h..columnZ.mean_
-00000e70: 6461 7461 5a0a 766f 7865 6c5f 6461 7461  dataZ.voxel_data
-00000e80: 7235 0000 0072 3500 0000 7236 0000 00da  r5...r5...r6....
-00000e90: 1a6c 6f61 645f 616e 645f 7265 7374 7275  .load_and_restru
-00000ea0: 6374 7572 655f 6a73 6f6e 7370 0000 0073  cture_jsonsp...s
-00000eb0: 4c00 0000 0802 0805 1e01 0e02 0201 08ff  L...............
-00000ec0: 0803 0c01 1201 1cff 0203 1201 0c01 0401  ................
-00000ed0: 02ff 0803 0c01 0802 1001 1c03 0e01 0202  ................
-00000ee0: 0801 1801 04ff 0c02 0401 0c01 0401 02ff  ................
-00000ef0: 0803 1401 1002 1c03 1c01 0c02 0c01 0402  ................
-00000f00: 7a22 4669 6775 7265 732e 6c6f 6164 5f61  z"Figures.load_a
-00000f10: 6e64 5f72 6573 7472 7563 7475 7265 5f6a  nd_restructure_j
-00000f20: 736f 6e73 290a da08 5f5f 6e61 6d65 5f5f  sons)...__name__
-00000f30: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000f40: 7175 616c 6e61 6d65 5f5f 7213 0000 00da  qualname__r.....
-00000f50: 0b63 6c61 7373 6d65 7468 6f64 7237 0000  .classmethodr7..
-00000f60: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
-00000f70: 4300 0000 7256 0000 0072 8600 0000 7235  C...rV...r....r5
-00000f80: 0000 0072 3500 0000 7235 0000 0072 3600  ...r5...r5...r6.
-00000f90: 0000 720a 0000 0016 0000 0073 1400 0000  ..r........s....
-00000fa0: 0800 0401 0202 0a01 022e 0a01 020f 0a01  ................
-00000fb0: 0217 0e01 720a 0000 0063 0000 0000 0000  ....r....c......
-00000fc0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000fd0: 0000 7360 0000 0065 005a 0164 005a 0265  ..s`...e.Z.d.Z.e
-00000fe0: 0364 0164 0284 0083 015a 0465 0364 0364  .d.d.....Z.e.d.d
-00000ff0: 0484 0083 015a 0565 0364 0564 0684 0083  .....Z.e.d.d....
-00001000: 015a 0665 0364 0764 0884 0083 015a 0765  .Z.e.d.d.....Z.e
-00001010: 0364 0964 0a84 0083 015a 0865 0364 0b64  .d.d.....Z.e.d.d
-00001020: 0c84 0083 015a 0965 0a64 0d64 0e84 0083  .....Z.e.d.d....
-00001030: 015a 0b64 0f53 0029 1072 2500 0000 6302  .Z.d.S.).r%...c.
-00001040: 0000 0000 0000 0000 0000 000a 0000 0008  ................
-00001050: 0000 0043 0000 0073 f600 0000 7400 a001  ...C...s....t...
-00001060: a100 9b00 6401 9d02 7d02 7402 a003 7c02  ....d...}.t...|.
-00001070: a101 0100 7402 a003 7400 a001 a100 9b00  ....t...t.......
-00001080: 6402 9d02 a101 0100 7c00 6a04 6a05 6403  d.......|.j.j.d.
-00001090: 6b02 7225 7c00 6a04 6a06 6403 1900 7d03  k.r%|.j.j.d...}.
-000010a0: 6404 7d04 6e08 7c00 6a04 6a06 6405 1900  d.}.n.|.j.j.d...
-000010b0: 7d03 6406 7d04 7c03 4400 5d49 7d05 7407  }.d.}.|.D.]I}.t.
-000010c0: 6407 7c04 9b00 6408 7c05 9b00 6409 9d05  d.|...d.|...d...
-000010d0: 8301 733d 712f 7402 a003 7400 a001 a100  ..s=q/t...t.....
-000010e0: 9b00 640a 7c05 9b00 9d03 a101 0100 640b  ..d.|.........d.
-000010f0: 7c05 9b00 640c 9d03 640b 7c05 9b00 640d  |...d...d.|...d.
-00001100: 9d03 6702 7d06 7c06 4400 5d18 7d07 7c00  ..g.}.|.D.].}.|.
-00001110: a008 7c01 7c07 7c05 7c04 a104 7d08 7c08  ..|.|.|.|...}.|.
-00001120: 4400 5d0b 7d09 7402 a009 7c09 7400 a001  D.].}.t...|.t...
-00001130: a100 7c02 a103 0100 7163 7157 7c00 6a04  ..|.....qcqW|.j.
-00001140: 6a0a 7278 740b 640e 8301 0100 712f 6400  j.rxt.d.....q/d.
-00001150: 5300 290f 4e7a 152f 4669 6775 7265 732f  S.).Nz./Figures/
-00001160: 4272 6169 6e5f 696d 6167 6573 7a14 2f46  Brain_imagesz./F
-00001170: 6967 7572 6573 2f42 7261 696e 5f67 7269  igures/Brain_gri
-00001180: 6473 7a10 5365 7373 696f 6e20 6176 6572  dsz.Session aver
-00001190: 6167 6564 5a18 5365 7373 696f 6e5f 6176  agedZ.Session_av
-000011a0: 6572 6167 6564 5f72 6573 756c 7473 7a14  eraged_resultsz.
-000011b0: 5061 7274 6963 6970 616e 7420 6176 6572  Participant aver
-000011c0: 6167 6564 5a1c 5061 7274 6963 6970 616e  agedZ.Participan
-000011d0: 745f 6176 6572 6167 6564 5f72 6573 756c  t_averaged_resul
-000011e0: 7473 fa12 4f76 6572 616c 6c2f 4e49 4654  ts..Overall/NIFT
-000011f0: 495f 524f 492f 7a02 2f2a da01 2a7a 152f  I_ROI/z./*..*z./
-00001200: 4669 6775 7265 732f 4272 6169 6e5f 6772  Figures/Brain_gr
-00001210: 6964 732f 720e 0000 00fa 072e 6e69 692e  ids/r.......nii.
-00001220: 677a 7a19 5f77 6974 6869 6e5f 726f 695f  gzz._within_roi_
-00001230: 7363 616c 6564 2e6e 6969 2e67 7ada 010a  scaled.nii.gz...
-00001240: 290c 7215 0000 0072 1600 0000 7209 0000  ).r....r....r...
-00001250: 0072 2800 0000 7213 0000 0072 1700 0000  .r(...r....r....
-00001260: da11 7374 6174 6973 7469 635f 6f70 7469  ..statistic_opti
-00001270: 6f6e 7372 0300 0000 722b 0000 00da 096d  onsr....r+.....m
-00001280: 6f76 655f 6669 6c65 721e 0000 0072 1f00  ove_filer....r..
-00001290: 0000 290a 722f 0000 0072 3300 0000 5a10  ..).r/...r3...Z.
-000012a0: 696e 6469 765f 6272 6169 6e73 5f64 6972  indiv_brains_dir
-000012b0: da10 7374 6174 6973 7469 635f 6c61 6265  ..statistic_labe
-000012c0: 6c73 da09 7375 6266 6f6c 6465 72da 0973  ls..subfolder..s
-000012d0: 7461 7469 7374 6963 5a0f 6272 6169 6e5f  tatisticZ.brain_
-000012e0: 706c 6f74 5f65 7874 73da 0e62 6173 655f  plot_exts..base_
-000012f0: 6578 7465 6e73 696f 6eda 1069 6e64 6976  extension..indiv
-00001300: 5f62 7261 696e 5f69 6d67 73da 0369 6d67  _brain_imgs..img
-00001310: 7235 0000 0072 3500 0000 7236 0000 0072  r5...r5...r6...r
-00001320: 2600 0000 a800 0000 7330 0000 000e 020a  &.......s0......
-00001330: 0114 010c 020c 0106 010c 0204 0108 0216  ................
-00001340: 0202 0118 020a 030a 0104 fe08 0610 0108  ................
-00001350: 0214 0102 ff08 0308 0102 8004 ec7a 0e42  .............z.B
-00001360: 7261 696e 4772 6964 2e6d 616b 6563 0500  rainGrid.makec..
-00001370: 0000 0000 0000 0000 0000 1100 0000 0f00  ................
-00001380: 0000 0300 0000 7390 0100 0074 006a 01a0  ......s....t.j..
-00001390: 0274 006a 01a0 0288 00a1 0164 0119 00a1  .t.j.......d....
-000013a0: 0164 0119 0064 0264 0085 0219 007d 0567  .d...d.d.....}.g
-000013b0: 007d 067c 0164 0319 00a0 03a1 007d 0787  .}.|.d.......}..
-000013c0: 0087 0166 0264 0464 0584 087c 0744 0083  ...f.d.d...|.D..
-000013d0: 017d 077c 00a0 047c 01a1 015c 047d 087d  .}.|...|...\.}.}
-000013e0: 097d 0a7d 0b7c 0b64 0676 0072 3464 077d  .}.}.|.d.v.r4d.}
-000013f0: 0c6e 047c 0b64 0814 007d 0c64 097d 0d7c  .n.|.d...}.d.}.|
-00001400: 0c7c 0d66 0274 056a 0664 0a3c 0064 0b74  .|.f.t.j.d.<.d.t
-00001410: 056a 0664 0c3c 0064 0d74 056a 0664 0e3c  .j.d.<.d.t.j.d.<
-00001420: 007c 0364 0f76 0072 5a7c 006a 076a 0804  .|.d.v.rZ|.j.j..
-00001430: 007d 0e7d 0f7c 006a 076a 097d 106e 0664  .}.}.|.j.j.}.n.d
-00001440: 0004 007d 0e7d 0f64 017d 107c 0f64 0075  ...}.}.d.}.|.d.u
-00001450: 0072 6667 007d 0f09 0088 0064 117c 039b  .rfg.}.....d.|..
-00001460: 0064 129d 036b 0372 7464 137d 0e64 017d  .d...k.rtd.}.d.}
-00001470: 106e 1088 0064 117c 039b 0064 129d 036b  .n...d.|...d...k
-00001480: 0272 847c 0e64 0075 0172 847c 0564 1437  .r.|.d.u.r.|.d.7
-00001490: 007d 057c 006a 076a 0a72 9074 0b64 157c  .}.|.j.j.r.t.d.|
-000014a0: 059b 0064 169d 0383 0101 007c 00a0 0c7c  ...d.......|...|
-000014b0: 0588 007c 097c 067c 077c 087c 037c 0e7c  ...|.|.|.|.|.|.|
-000014c0: 0f7c 107c 0b7c 0a88 01a1 0d7d 067c 0e64  .|.|.|.....}.|.d
-000014d0: 0075 0172 a809 007c 0653 0074 0d7c 0f83  .u.r...|.S.t.|..
-000014e0: 0164 1719 007d 0f7c 0f64 0119 007d 0e7c  .d...}.|.d...}.|
-000014f0: 006a 076a 0a72 c774 0b64 1874 0e7c 0f64  .j.j.r.t.d.t.|.d
-00001500: 0119 0083 019b 0064 197c 0f64 0219 009b  .......d.|.d....
-00001510: 0064 1a9d 0583 0101 0071 6729 1b4e 7201  .d.......qg).Nr.
-00001520: 0000 0072 0800 0000 7258 0000 0063 0100  ...r....rX...c..
-00001530: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00001540: 0000 1300 0000 7328 0000 0067 007c 005d  ......s(...g.|.]
-00001550: 107d 0174 0064 0088 019b 0064 017c 019b  .}.t.d.....d.|..
-00001560: 0088 009b 009d 0583 0172 027c 0191 0271  .........r.|...q
-00001570: 0253 0029 0272 8c00 0000 7246 0000 0072  .S.).r....rF...r
-00001580: 0200 0000 a902 da02 2e30 da03 6a73 6ea9  .........0..jsn.
-00001590: 0272 9500 0000 7293 0000 0072 3500 0000  .r....r....r5...
-000015a0: 7236 0000 00da 0a3c 6c69 7374 636f 6d70  r6.....<listcomp
-000015b0: 3ed3 0000 0073 0200 0000 2800 7a23 4272  >....s....(.z#Br
-000015c0: 6169 6e47 7269 642e 7365 7475 702e 3c6c  ainGrid.setup.<l
-000015d0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000015e0: 3e29 0272 0800 0000 725f 0000 00e9 2000  >).r....r_.... .
-000015f0: 0000 e910 0000 00e9 0f00 0000 7a0e 6669  ............z.fi
-00001600: 6775 7265 2e66 6967 7369 7a65 677b 14ae  gure.figsizeg{..
-00001610: 47e1 7a84 3f7a 1566 6967 7572 652e 7375  G.z.?z.figure.su
-00001620: 6270 6c6f 742e 7773 7061 6365 e79a 9999  bplot.wspace....
-00001630: 9999 99b9 3f7a 1566 6967 7572 652e 7375  ....?z.figure.su
-00001640: 6270 6c6f 742e 6873 7061 6365 2902 725b  bplot.hspace).r[
-00001650: 0000 00da 064d 6564 6961 6e54 720e 0000  .....MedianTr...
-00001660: 0072 8e00 0000 e964 0000 00da 0b5f 7361  .r.....d....._sa
-00001670: 6d65 5f73 6361 6c65 7a07 5361 7669 6e67  me_scalez.Saving
-00001680: 207a 0720 7461 626c 652e e9ff ffff ff7a   z. table......z
-00001690: 164d 6178 696d 756d 2052 4f49 2076 616c  .Maximum ROI val
-000016a0: 7565 206f 663a 207a 2120 7365 656e 2066  ue of: z! seen f
-000016b0: 6f72 2070 6172 616d 6574 6572 2063 6f6d  or parameter com
-000016c0: 6269 6e61 7469 6f6e 3a20 7a2d 2e20 4372  bination: z-. Cr
-000016d0: 6561 7469 6e67 2066 6967 7572 6573 2077  eating figures w
-000016e0: 6974 6820 7468 6973 2063 6f6c 6f75 7262  ith this colourb
-000016f0: 6172 206c 696d 6974 2e29 0f72 1500 0000  ar limit.).r....
-00001700: 7218 0000 00da 0873 706c 6974 6578 74da  r......splitext.
-00001710: 0675 6e69 7175 65da 0b74 6162 6c65 5f73  .unique..table_s
-00001720: 6574 7570 da03 706c 74da 0872 6350 6172  etup..plt..rcPar
-00001730: 616d 7372 1300 0000 da13 6272 6169 6e5f  amsr......brain_
-00001740: 6669 675f 7661 6c75 655f 6d61 78da 1362  fig_value_max..b
-00001750: 7261 696e 5f66 6967 5f76 616c 7565 5f6d  rain_fig_value_m
-00001760: 696e 721e 0000 0072 1f00 0000 da0a 6d61  inr....r......ma
-00001770: 6b65 5f74 6162 6c65 da06 736f 7274 6564  ke_table..sorted
-00001780: da05 726f 756e 6429 1172 2f00 0000 da02  ..round).r/.....
-00001790: 6466 7295 0000 0072 9400 0000 7293 0000  dfr....r....r...
-000017a0: 00da 0e62 6173 655f 6578 745f 636c 6561  ...base_ext_clea
-000017b0: 6e72 9600 0000 da0a 6a73 6f6e 5f61 7272  nr......json_arr
-000017c0: 6179 da0f 6372 6974 6963 616c 5f70 6172  ay..critical_par
-000017d0: 616d 73da 0963 656c 6c5f 6e75 6d73 da0b  ams..cell_nums..
-000017e0: 795f 6178 6973 5f73 697a 65da 0b78 5f61  y_axis_size..x_a
-000017f0: 7869 735f 7369 7a65 5a12 6272 6169 6e5f  xis_sizeZ.brain_
-00001800: 7461 626c 655f 785f 7369 7a65 5a12 6272  table_x_sizeZ.br
-00001810: 6169 6e5f 7461 626c 655f 795f 7369 7a65  ain_table_y_size
-00001820: da04 766d 6178 da0c 766d 6178 5f73 746f  ..vmax..vmax_sto
-00001830: 7261 6765 da04 766d 696e 7235 0000 0072  rage..vminr5...r
-00001840: 9b00 0000 7236 0000 0072 2b00 0000 cb00  ....r6...r+.....
-00001850: 0000 7352 0000 0024 0204 010c 0214 0312  ..sR...$........
-00001860: 0208 0206 0108 0204 020e 020a 010a 0108  ................
-00001870: 020c 010a 0108 0204 0108 0204 0102 0210  ................
-00001880: 0104 0206 0118 0108 0108 0210 010e 020c  ................
-00001890: 0104 0104 fe08 0402 0104 0c0c f808 0108  ................
-000018a0: 0202 011c 0104 ff02 e87a 0f42 7261 696e  .........z.Brain
-000018b0: 4772 6964 2e73 6574 7570 630e 0000 0000  Grid.setupc.....
-000018c0: 0000 0000 0000 0014 0000 000c 0000 0043  ...............C
-000018d0: 0000 0073 ca01 0000 7400 7c05 8301 4400  ...s....t.|...D.
-000018e0: 5da7 5c02 7d0e 7d0f 7c00 a001 7c0f 7c01  ].\.}.}.|...|.|.
-000018f0: 7c02 7c08 7c09 7c0a 7c04 7c07 7c0d a109  |.|.|.|.|.|.|...
-00001900: 5c03 7d10 7d04 7d11 7402 a003 7c10 a101  \.}.}.}.t...|...
-00001910: 7d12 7404 a005 7c0c 7c0b 7c03 7c0e 1900  }.t...|.|.|.|...
-00001920: 6401 1700 a103 0100 7404 a006 7c12 a101  d.......t...|...
-00001930: 0100 7404 a007 a100 7d13 7c13 a008 6700  ..t.....}.|...g.
-00001940: a101 0100 7c13 6a09 6a0a a00b 6700 a101  ....|.j.j...g...
-00001950: 0100 7c13 a00c 6700 a101 0100 7c13 6a09  ..|...g.....|.j.
-00001960: 6a0d a00b 6700 a101 0100 7c06 6402 1900  j...g.....|.d...
-00001970: 6403 1900 7c0e 1900 6404 6b02 727a 740e  d...|...d.k.rzt.
-00001980: 7c06 6405 1900 6406 1900 8301 6401 6b03  |.d...d.....d.k.
-00001990: 727a 7404 6a0f 7c00 6a10 6a11 6407 1700  rzt.j.|.j.j.d...
-000019a0: 7412 7c06 6405 1900 6406 1900 7c06 6405  t.|.d...d...|.d.
-000019b0: 1900 6403 1900 7c0e 1900 1900 8301 1700  ..d...|.........
-000019c0: 7c00 6a10 6a13 6408 8d02 0100 7c06 6405  |.j.j.d.....|.d.
-000019d0: 1900 6403 1900 7c0e 1900 6404 6b02 72ab  ..d...|...d.k.r.
-000019e0: 740e 7c06 6402 1900 6406 1900 8301 6401  t.|.d...d.....d.
-000019f0: 6b03 72ab 7404 6a14 7c00 6a10 6a15 6407  k.r.t.j.|.j.j.d.
-00001a00: 1700 7412 7c06 6402 1900 6406 1900 7c06  ..t.|.d...d...|.
-00001a10: 6402 1900 6403 1900 7c0e 1900 1900 8301  d...d...|.......
-00001a20: 1700 7c00 6a10 6a13 6408 8d02 0100 7104  ..|.j.j.d.....q.
-00001a30: 7c00 a016 7c06 7c03 7c0b 7c0c 7c11 a105  |...|.|.|.|.|...
-00001a40: 0100 7c00 6a10 6a17 72bd 7404 a018 a100  ..|.j.j.r.t.....
-00001a50: 0100 7404 6a19 6409 7c07 9b00 640a 7c01  ..t.j.d.|...d.|.
-00001a60: 9b00 640b 9d05 7c00 6a10 6a1a 640c 640d  ..d...|.j.j.d.d.
-00001a70: 8d03 0100 7404 6a19 6409 7c07 9b00 640a  ....t.j.d.|...d.
-00001a80: 7c01 9b00 640e 9d05 7c00 6a10 6a1a 640c  |...d...|.j.j.d.
-00001a90: 640d 8d03 0100 7404 a01b a100 0100 7c04  d.....t.......|.
-00001aa0: 5300 290f 4e72 0800 0000 da04 726f 7773  S.).Nr......rows
-00001ab0: da05 6f72 6465 7272 0100 0000 da04 636f  ..orderr......co
-00001ac0: 6c73 da06 7661 6c75 6573 720d 0000 00a9  ls..valuesr.....
-00001ad0: 01da 0866 6f6e 7473 697a 657a 1446 6967  ...fontsizez.Fig
-00001ae0: 7572 6573 2f42 7261 696e 5f67 7269 6473  ures/Brain_grids
-00001af0: 2f72 4600 0000 7247 0000 00da 0574 6967  /rF...rG.....tig
-00001b00: 6874 2902 da03 6470 695a 0b62 626f 785f  ht)...dpiZ.bbox_
-00001b10: 696e 6368 6573 724c 0000 0029 1cda 0965  inchesrL...)...e
-00001b20: 6e75 6d65 7261 7465 da0f 7361 7665 5f62  numerate..save_b
-00001b30: 7261 696e 5f69 6d67 73da 056d 7069 6d67  rain_imgs..mpimg
-00001b40: da06 696d 7265 6164 72a8 0000 00da 0773  ..imreadr......s
-00001b50: 7562 706c 6f74 da06 696d 7368 6f77 da03  ubplot..imshow..
-00001b60: 6763 615a 0a73 6574 5f79 7469 636b 7372  gcaZ.set_yticksr
-00001b70: 3b00 0000 7239 0000 005a 0e73 6574 5f74  ;...r9...Z.set_t
-00001b80: 6963 6b6c 6162 656c 73da 0a73 6574 5f78  icklabels..set_x
-00001b90: 7469 636b 7372 3800 0000 da03 6c65 6e72  ticksr8.....lenr
-00001ba0: 4f00 0000 7213 0000 00da 1662 7261 696e  O...r......brain
-00001bb0: 5f74 6162 6c65 5f63 6f6c 5f6c 6162 656c  _table_col_label
-00001bc0: 7372 7500 0000 da0e 706c 6f74 5f66 6f6e  sru.....plot_fon
-00001bd0: 745f 7369 7a65 da06 796c 6162 656c da16  t_size..ylabel..
-00001be0: 6272 6169 6e5f 7461 626c 655f 726f 775f  brain_table_row_
-00001bf0: 6c61 6265 6c73 da15 6c61 6265 6c5f 626c  labels..label_bl
-00001c00: 616e 6b5f 6365 6c6c 5f61 7865 73da 1262  ank_cell_axes..b
-00001c10: 7261 696e 5f74 6967 6874 5f6c 6179 6f75  rain_tight_layou
-00001c20: 74da 0c74 6967 6874 5f6c 6179 6f75 74da  t..tight_layout.
-00001c30: 0773 6176 6566 6967 da08 706c 6f74 5f64  .savefig..plot_d
-00001c40: 7069 722d 0000 0029 1472 2f00 0000 72b0  pir-...).r/...r.
-00001c50: 0000 0072 9500 0000 72b3 0000 0072 9600  ...r....r....r..
-00001c60: 0000 72b1 0000 0072 b200 0000 7294 0000  ..r....r....r...
-00001c70: 0072 b600 0000 72b7 0000 0072 b800 0000  .r....r....r....
-00001c80: 72b5 0000 0072 b400 0000 7293 0000 00da  r....r....r.....
-00001c90: 0866 696c 655f 6e75 6d72 6f00 0000 5a09  .file_numro...Z.
-00001ca0: 6272 6169 6e5f 696d 67da 0464 696d 7372  brain_img..dimsr
-00001cb0: 9700 0000 da02 6178 7235 0000 0072 3500  ......axr5...r5.
-00001cc0: 0000 7236 0000 0072 ac00 0000 0a01 0000  ..r6...r........
-00001cd0: 734a 0000 0010 030a 0108 0104 010a fe0a  sJ..............
-00001ce0: 0516 010a 0108 020a 010e 010a 020e 0128  ...............(
-00001cf0: 020e 011e 0102 ff06 0206 fe28 040e 011e  ...........(....
-00001d00: 0102 ff06 0206 fe02 8012 0408 0208 011a  ................
-00001d10: 0202 0106 ff1a 0202 0106 ff08 0204 027a  ...............z
-00001d20: 1442 7261 696e 4772 6964 2e6d 616b 655f  .BrainGrid.make_
-00001d30: 7461 626c 6563 0a00 0000 0000 0000 0000  tablec..........
-00001d40: 0000 1200 0000 0b00 0000 4300 0000 7326  ..........C...s&
-00001d50: 0100 007c 019b 0064 017c 029b 0064 029d  ...|...d.|...d..
-00001d60: 047d 0a7c 07a0 007c 0aa1 0101 0064 037c  .}.|...|.....d.|
-00001d70: 099b 0064 047c 019b 007c 039b 009d 057d  ...d.|...|.....}
-00001d80: 0b7c 0364 017c 089b 0064 059d 036b 0272  .|.d.|...d...k.r
-00001d90: 3e7c 02a0 0164 06a1 0164 076b 0272 3e74  >|...d...d.k.r>t
-00001da0: 02a0 037c 0ba1 017d 0c7c 0ca0 04a1 007d  ...|...}.|.....}
-00001db0: 0c74 05a0 067c 0ca1 017d 047c 05a0 0074  .t...|...}.|...t
-00001dc0: 05a0 067c 0ca1 017c 0166 02a1 0101 0074  ...|...|.f.....t
-00001dd0: 02a0 037c 0ba1 017d 0d74 02a0 0774 05a0  ...|...}.t...t..
-00001de0: 087c 0da0 04a1 00a1 017c 0d6a 097c 0d6a  .|.......|.j.|.j
-00001df0: 0aa1 037d 0d74 0b6a 0c7c 0d64 0864 0864  ...}.t.j.|.d.d.d
-00001e00: 0964 0a7c 067c 047c 006a 0d6a 0e7c 006a  .d.|.|.|.j.j.|.j
-00001e10: 0d6a 0f66 0264 0b64 0c8d 097d 0e7c 0e6a  .j.f.d.d...}.|.j
-00001e20: 107c 0a7c 006a 0d6a 1164 0d8d 0201 007c  .|.|.j.j.d.....|
-00001e30: 0ea0 12a1 0001 0074 13a0 147c 0aa1 018f  .......t...|....
-00001e40: 0d7d 0f7c 0f6a 155c 027d 107d 1157 0064  .}.|.j.\.}.}.W.d
-00001e50: 0004 0004 0083 0301 006e 0831 0073 8777  .........n.1.s.w
-00001e60: 0101 0001 0001 0059 0001 007c 0a7c 077c  .......Y...|.|.|
-00001e70: 107c 1166 0266 0353 0029 0e4e 720e 0000  .|.f.f.S.).Nr...
-00001e80: 0072 4700 0000 728c 0000 0072 4600 0000  .rG...r....rF...
-00001e90: 728e 0000 0072 a300 0000 72a4 0000 0046  r....r....r....F
-00001ea0: 54da 0278 7ada 0769 6e66 6572 6e6f 2908  T..xz..inferno).
-00001eb0: 5a0a 6472 6177 5f63 726f 7373 5a08 616e  Z.draw_crossZ.an
-00001ec0: 6e6f 7461 7465 da08 636f 6c6f 7262 6172  notate..colorbar
-00001ed0: 5a0c 6469 7370 6c61 795f 6d6f 6465 72b8  Z.display_moder.
-00001ee0: 0000 0072 b600 0000 5a0a 6375 745f 636f  ...r....Z.cut_co
-00001ef0: 6f72 6473 da04 636d 6170 2901 72c0 0000  ords..cmap).r...
-00001f00: 0029 16da 0661 7070 656e 64da 0466 696e  .)...append..fin
-00001f10: 64da 036e 6962 7270 0000 00da 0967 6574  d..nibrp.....get
-00001f20: 5f66 6461 7461 da02 6e70 da06 6e61 6e6d  _fdata..np..nanm
-00001f30: 6178 da0b 4e69 6674 6931 496d 6167 65da  ax..Nifti1Image.
-00001f40: 0a6e 616e 5f74 6f5f 6e75 6dda 0661 6666  .nan_to_num..aff
-00001f50: 696e 65da 0668 6561 6465 7272 0500 0000  ine..headerr....
-00001f60: 5a09 706c 6f74 5f61 6e61 7472 1300 0000  Z.plot_anatr....
-00001f70: da0d 6272 6169 6e5f 785f 636f 6f72 64da  ..brain_x_coord.
-00001f80: 0d62 7261 696e 5f7a 5f63 6f6f 7264 72d1  .brain_z_coordr.
-00001f90: 0000 0072 d200 0000 722d 0000 0072 0700  ...r....r-...r..
-00001fa0: 0000 726d 0000 00da 0473 697a 6529 1272  ..rm.....size).r
-00001fb0: 2f00 0000 726f 0000 0072 b000 0000 7295  /...ro...r....r.
-00001fc0: 0000 0072 b600 0000 72b7 0000 0072 b800  ...r....r....r..
-00001fd0: 0000 7296 0000 0072 9400 0000 7293 0000  ..r....r....r...
-00001fe0: 005a 0870 6e67 5f70 6174 685a 0a6e 6966  .Z.png_pathZ.nif
-00001ff0: 7469 5f70 6174 68da 0562 7261 696e 7297  ti_path..brainr.
-00002000: 0000 00da 0470 6c6f 74da 0269 6d72 4b00  .....plot..imrK.
-00002010: 0000 724a 0000 0072 3500 0000 7235 0000  ..rJ...r5...r5..
-00002020: 0072 3600 0000 72c2 0000 0035 0100 0073  .r6...r....5...s
-00002030: 2c00 0000 1004 0a01 1402 1e02 0a02 0801  ,...............
-00002040: 0a02 1404 0a03 1c01 0602 0801 0401 0e01  ................
-00002050: 0201 06fc 1205 0801 0c02 0c01 1cff 0e03  ................
-00002060: 7a19 4272 6169 6e47 7269 642e 7361 7665  z.BrainGrid.save
-00002070: 5f62 7261 696e 5f69 6d67 7363 0200 0000  _brain_imgsc....
-00002080: 0000 0000 0000 0000 1100 0000 0800 0000  ................
-00002090: 4300 0000 73be 0100 0067 007d 0267 007d  C...s....g.}.g.}
-000020a0: 037c 006a 006a 0144 005d 187d 0474 0274  .|.j.j.D.].}.t.t
-000020b0: 037c 017c 0419 00a0 04a1 0083 0183 017d  .|.|...........}
-000020c0: 0564 0164 0284 007c 0544 0083 017d 057c  .d.d...|.D...}.|
-000020d0: 02a0 057c 05a1 0101 0071 087c 027d 0674  ...|.....q.|.}.t
-000020e0: 037c 006a 006a 01a0 06a1 0083 017d 077c  .|.j.j.......}.|
-000020f0: 006a 006a 0764 0367 0167 0064 049c 037c  .j.j.d.g.g.d...|
-00002100: 006a 006a 0864 0367 0167 0064 049c 0364  .j.j.d.g.g.d...d
-00002110: 059c 027d 087c 0844 005d 1a7d 097c 087c  ...}.|.D.].}.|.|
-00002120: 0919 0064 0619 0064 076b 0272 4b71 407c  ...d...d.k.rKq@|
-00002130: 067c 07a0 097c 087c 0919 0064 0619 00a1  .|...|.|...d....
-00002140: 0119 007c 087c 0919 0064 083c 0071 4074  ...|.|...d.<.q@t
-00002150: 0a7c 0864 0919 0064 0819 0083 017d 0a74  .|.d...d.....}.t
-00002160: 0a7c 0864 0a19 0064 0819 0083 017d 0b74  .|.d...d.....}.t
-00002170: 0b7c 0164 0b19 00a0 04a1 0083 0144 005d  .|.d.........D.]
-00002180: 655c 027d 0c7d 0d67 007d 0e7c 017c 0164  e\.}.}.g.}.|.|.d
-00002190: 0b19 007c 0d6b 0219 006a 0c64 0319 007d  ...|.k...j.d...}
-000021a0: 0f7c 0844 005d 407d 097c 087c 0919 0064  .|.D.]@}.|.|...d
-000021b0: 0819 0064 0367 016b 0372 b874 0d7c 0f7c  ...d.g.k.r.t.|.|
-000021c0: 087c 0919 0064 0619 0019 0083 017d 107c  .|...d.......}.|
-000021d0: 087c 0919 0064 0c19 00a0 057c 087c 0919  .|...d.....|.|..
-000021e0: 0064 0819 00a0 097c 10a1 01a1 0101 007c  .d.....|.......|
-000021f0: 0ea0 057c 087c 0919 0064 0819 00a0 097c  ...|.|...d.....|
-00002200: 10a1 01a1 0101 0071 867c 087c 0919 0064  .......q.|.|...d
-00002210: 0c19 00a0 0564 03a1 0101 007c 0ea0 0564  .....d.....|...d
-00002220: 03a1 0101 0071 867c 03a0 0574 0ea0 0f7c  .....q.|...t...|
-00002230: 0e64 0d19 007c 0e64 0319 0066 027c 0b7c  .d...|.d...f.|.|
-00002240: 0a66 02a1 02a1 0101 0071 737c 087c 037c  .f.......qs|.|.|
-00002250: 0b7c 0a66 0453 0029 0e4e 6301 0000 0000  .|.f.S.).Nc.....
-00002260: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00002270: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-00002280: 7400 7c01 8301 9102 7102 5300 7235 0000  t.|.....q.S.r5..
-00002290: 0029 0172 7500 0000 2902 7299 0000 00da  .).ru...).r.....
-000022a0: 0570 6172 616d 7235 0000 0072 3500 0000  .paramr5...r5...
-000022b0: 7236 0000 0072 9c00 0000 6101 0000 f302  r6...r....a.....
-000022c0: 0000 0014 007a 2942 7261 696e 4772 6964  .....z)BrainGrid
-000022d0: 2e74 6162 6c65 5f73 6574 7570 2e3c 6c6f  .table_setup.<lo
-000022e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000022f0: 7201 0000 0029 0372 ea00 0000 72bc 0000  r....).r....r...
-00002300: 0072 ba00 0000 2902 72bb 0000 0072 b900  .r....).r....r..
-00002310: 0000 72ea 0000 0072 4400 0000 72bc 0000  ..r....rD...r...
-00002320: 0072 bb00 0000 72b9 0000 0072 5800 0000  .r....r....rX...
-00002330: 72ba 0000 0072 0800 0000 2910 7213 0000  r....r....).r...
-00002340: 00da 0e70 6172 616d 6574 6572 5f64 6963  ...parameter_dic
-00002350: 7472 ad00 0000 7268 0000 0072 a600 0000  tr....rh...r....
-00002360: 72da 0000 00da 046b 6579 73da 1062 7261  r......keys..bra
-00002370: 696e 5f74 6162 6c65 5f63 6f6c 73da 1062  in_table_cols..b
-00002380: 7261 696e 5f74 6162 6c65 5f72 6f77 73da  rain_table_rows.
-00002390: 0569 6e64 6578 72c9 0000 0072 c100 0000  .indexr....r....
-000023a0: 7277 0000 0072 7500 0000 72de 0000 00da  rw...ru...r.....
-000023b0: 1172 6176 656c 5f6d 756c 7469 5f69 6e64  .ravel_multi_ind
-000023c0: 6578 2911 722f 0000 0072 af00 0000 5a0d  ex).r/...r....Z.
-000023d0: 756e 6971 7565 5f70 6172 616d 7372 b300  unique_paramsr..
-000023e0: 0000 da03 6b65 79da 0670 6172 616d 735a  ....key..paramsZ
-000023f0: 0b70 6c6f 745f 7661 6c75 6573 5a0b 6178  .plot_valuesZ.ax
-00002400: 6973 5f74 6974 6c65 7372 b200 0000 7240  is_titlesr....r@
-00002410: 0000 0072 b500 0000 72b4 0000 0072 d300  ...r....r....r..
-00002420: 0000 da09 6669 6c65 5f6e 616d 655a 1074  ....file_nameZ.t
-00002430: 656d 705f 6f72 6465 725f 7374 6f72 655a  emp_order_storeZ
-00002440: 0d66 696c 655f 6e61 6d65 5f72 6f77 5a0a  .file_name_rowZ.
-00002450: 6669 6c65 5f70 6172 616d 7235 0000 0072  file_paramr5...r
-00002460: 3500 0000 7236 0000 0072 a700 0000 5a01  5...r6...r....Z.
-00002470: 0000 7342 0000 0004 0204 010c 0214 010e  ..sB............
-00002480: 010c 0104 0210 0110 0210 0106 ff08 0310  ................
-00002490: 0102 0102 0210 010e ff10 0310 0118 0204  ................
-000024a0: 0116 0108 0212 0114 0220 021a 0112 020c  ......... ......
-000024b0: 0116 0206 0108 ff0c 037a 1542 7261 696e  .........z.Brain
-000024c0: 4772 6964 2e74 6162 6c65 5f73 6574 7570  Grid.table_setup
-000024d0: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
-000024e0: 0007 0000 0043 0000 0073 4801 0000 7400  .....C...sH...t.
-000024f0: a001 6401 7c05 6402 1900 7c05 6403 1900  ..d.|.d...|.d...
-00002500: 6602 6404 a103 7d06 7402 7c01 6405 1900  f.d...}.t.|.d...
-00002510: 6406 1900 8301 4400 5d4c 5c02 7d07 7d08  d.....D.]L\.}.}.
-00002520: 7403 a004 6402 7c07 6602 7c04 7c03 6602  t...d.|.f.|.|.f.
-00002530: a102 7d09 7c09 7c02 7601 7261 7405 a006  ..}.|.|.v.rat...
-00002540: 7c04 7c03 7c09 6403 1700 a103 0100 7405  |.|.|.d.......t.
-00002550: a007 7c06 a101 0100 7c00 a008 a100 0100  ..|.....|.......
-00002560: 7405 6a09 7c00 6a0a 6a0b 6407 1700 7c08  t.j.|.j.j.d...|.
-00002570: 1700 7c00 6a0a 6a0c 6408 8d02 0100 7c09  ..|.j.j.d.....|.
-00002580: 6402 6b02 7261 7405 6a0d 7c00 6a0a 6a0e  d.k.rat.j.|.j.j.
-00002590: 6407 1700 7c01 6409 1900 6406 1900 6402  d...|.d...d...d.
-000025a0: 1900 1700 7c00 6a0a 6a0c 6408 8d02 0100  ....|.j.j.d.....
-000025b0: 7115 7402 7c01 6409 1900 6406 1900 8301  q.t.|.d...d.....
-000025c0: 4400 5d37 5c02 7d07 7d0a 7403 a004 7c07  D.]7\.}.}.t...|.
-000025d0: 6402 6602 7c04 7c03 6602 a102 7d09 7c09  d.f.|.|.f...}.|.
-000025e0: 7c02 7601 72a1 7c09 6402 6b03 72a1 7405  |.v.r.|.d.k.r.t.
-000025f0: a006 7c04 7c03 7c09 6403 1700 a103 0100  ..|.|.|.d.......
-00002600: 7405 a007 7c06 a101 0100 7c00 a008 a100  t...|.....|.....
-00002610: 0100 7405 6a0d 7c00 6a0a 6a0e 6407 1700  ..t.j.|.j.j.d...
-00002620: 7c0a 1700 7c00 6a0a 6a0c 6408 8d02 0100  |...|.j.j.d.....
-00002630: 716a 6400 5300 290a 4eda 0352 4742 7201  qjd.S.).N..RGBr.
-00002640: 0000 0072 0800 0000 2903 e9ff 0000 0072  ...r....)......r
-00002650: f600 0000 72f6 0000 0072 bb00 0000 72bc  ....r....r....r.
-00002660: 0000 0072 0d00 0000 72bd 0000 0072 b900  ...r....r....r..
-00002670: 0000 290f 7207 0000 0072 5500 0000 72c1  ..).r....rU...r.
-00002680: 0000 0072 de00 0000 72f1 0000 0072 a800  ...r....r....r..
-00002690: 0000 72c5 0000 0072 c600 0000 da13 6d61  ..r....r......ma
-000026a0: 6b65 5f63 656c 6c5f 696e 7669 7369 626c  ke_cell_invisibl
-000026b0: 6572 4f00 0000 7213 0000 0072 ca00 0000  erO...r....r....
-000026c0: 72cb 0000 0072 cc00 0000 72cd 0000 0029  r....r....r....)
-000026d0: 0b72 2f00 0000 72b2 0000 0072 b300 0000  .r/...r....r....
-000026e0: 72b5 0000 0072 b400 0000 72d4 0000 0072  r....r....r....r
-000026f0: 9700 0000 da07 636f 756e 7465 725a 0778  ......counterZ.x
-00002700: 5f74 6974 6c65 5a0b 6869 6464 656e 5f63  _titleZ.hidden_c
-00002710: 656c 6c5a 0779 5f74 6974 6c65 7235 0000  ellZ.y_titler5..
-00002720: 0072 3500 0000 7236 0000 0072 ce00 0000  .r5...r6...r....
-00002730: 8801 0000 732c 0000 001a 0318 0214 0108  ....s,..........
-00002740: 0212 010a 0108 011e 0208 021e 0106 0106  ................
-00002750: ff02 8018 0314 0110 0212 010a 0108 011e  ................
-00002760: 0202 8004 f87a 1f42 7261 696e 4772 6964  .....z.BrainGrid
-00002770: 2e6c 6162 656c 5f62 6c61 6e6b 5f63 656c  .label_blank_cel
-00002780: 6c5f 6178 6573 6300 0000 0000 0000 0000  l_axesc.........
-00002790: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000027a0: 6c00 0000 7400 a001 a100 7d00 7c00 6a02  l...t.....}.|.j.
-000027b0: a003 a100 a004 6700 a101 0100 7c00 6a02  ......g.....|.j.
-000027c0: a005 a100 a004 6700 a101 0100 7c00 6a06  ......g.....|.j.
-000027d0: 6401 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
-000027e0: 6403 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
-000027f0: 6404 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
-00002800: 6405 1900 a007 6402 a101 0100 6400 5300  d.....d.....d.S.
-00002810: 2906 4eda 046c 6566 7446 da05 7269 6768  ).N..leftF..righ
-00002820: 74da 0662 6f74 746f 6dda 0374 6f70 2908  t..bottom..top).
-00002830: 72a8 0000 0072 c700 0000 723b 0000 00da  r....r....r;....
-00002840: 0967 6574 5f78 6178 6973 5a09 7365 745f  .get_xaxisZ.set_
-00002850: 7469 636b 73da 0967 6574 5f79 6178 6973  ticks..get_yaxis
-00002860: 5a06 7370 696e 6573 da0b 7365 745f 7669  Z.spines..set_vi
-00002870: 7369 626c 6529 01da 0566 7261 6d65 7235  sible)...framer5
-00002880: 0000 0072 3500 0000 7236 0000 0072 f700  ...r5...r6...r..
-00002890: 0000 a501 0000 730e 0000 0008 0210 0110  ......s.........
-000028a0: 0110 0110 0110 0114 017a 1d42 7261 696e  .........z.Brain
-000028b0: 4772 6964 2e6d 616b 655f 6365 6c6c 5f69  Grid.make_cell_i
-000028c0: 6e76 6973 6962 6c65 4e29 0c72 8700 0000  nvisibleN).r....
-000028d0: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
-000028e0: 2600 0000 722b 0000 0072 ac00 0000 72c2  &...r+...r....r.
-000028f0: 0000 0072 a700 0000 72ce 0000 0072 8b00  ...r....r....r..
-00002900: 0000 72f7 0000 0072 3500 0000 7235 0000  ..r....r5...r5..
-00002910: 0072 3500 0000 7236 0000 0072 2500 0000  .r5...r6...r%...
-00002920: a700 0000 731e 0000 0008 0002 010a 0102  ....s...........
-00002930: 220a 0102 3e0a 0102 2a0a 0102 240a 0102  "...>...*...$...
-00002940: 2d0a 0102 1c0e 0172 2500 0000 6300 0000  -......r%...c...
-00002950: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00002960: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002970: 5a02 6503 6401 6402 8400 8301 5a04 6403  Z.e.d.d.....Z.d.
-00002980: 5300 2904 7229 0000 0063 0200 0000 0000  S.).r)...c......
-00002990: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
-000029a0: 0000 7364 0200 0074 00a0 017c 01a1 017d  ..sd...t...|...}
-000029b0: 027c 027c 0264 0119 0064 026b 037c 0264  .|.|.d...d.k.|.d
-000029c0: 0119 0064 036b 0340 0019 007d 027c 027c  ...d.k.@...}.|.|
-000029d0: 0264 0419 0064 056b 0419 007d 027c 006a  .d...d.k...}.|.j
-000029e0: 026a 0364 066b 0273 387c 006a 026a 0464  .j.d.k.s8|.j.j.d
-000029f0: 066b 0273 387c 02a0 057c 006a 026a 037c  .k.s8|...|.j.j.|
-00002a00: 006a 026a 0467 02a1 01a0 0664 0764 0884  .j.j.g.....d.d..
-00002a10: 00a1 017d 026e 257c 006a 026a 0364 066b  ...}.n%|.j.j.d.k
-00002a20: 0273 4b7c 02a0 057c 006a 026a 03a1 01a0  .sK|...|.j.j....
-00002a30: 0664 0964 0884 00a1 017d 026e 127c 006a  .d.d.....}.n.|.j
-00002a40: 026a 0464 066b 0273 5d7c 02a0 057c 006a  .j.d.k.s]|...|.j
-00002a50: 026a 04a1 01a0 0664 0a64 0884 00a1 017d  .j.....d.d.....}
-00002a60: 027c 026a 0764 0b64 0c8d 017d 0264 0d7c  .|.j.d.d...}.d.|
-00002a70: 0264 0e3c 0064 0f7d 0374 086a 0974 086a  .d.<.d.}.t.j.t.j
-00002a80: 0a64 0e64 1064 118d 0264 128d 017d 0474  .d.d.d...d...}.t
-00002a90: 086a 0974 086a 0a64 0e64 1364 118d 0264  .j.t.j.d.d.d...d
-00002aa0: 128d 017d 0574 08a0 0b7c 02a1 0174 086a  ...}.t...|...t.j
-00002ab0: 0964 0e64 0464 148d 0217 0074 086a 0c7c  .d.d.d.....t.j.|
-00002ac0: 0564 0b64 157c 006a 026a 0d64 1664 178d  .d.d.|.j.j.d.d..
-00002ad0: 0517 0074 086a 0e64 0f64 057c 006a 026a  ...t.j.d.d.|.j.j
-00002ae0: 0f64 1664 188d 0417 0074 08a0 1064 1964  .d.d.....t...d.d
-00002af0: 1aa1 0217 0074 08a0 1164 0564 00a1 0217  .....t...d.d....
-00002b00: 0074 08a0 127c 006a 026a 13a1 0117 0074  .t...|.j.j.....t
-00002b10: 08a0 1464 06a1 0117 0074 086a 157c 006a  ...d.....t.j.|.j
-00002b20: 026a 049b 0064 1b7c 006a 026a 039b 009d  .j...d.|.j.j....
-00002b30: 0364 0b64 1c64 1d8d 0317 0074 08a0 16a1  .d.d.d.....t....
-00002b40: 0017 0074 086a 1774 086a 186a 1964 0d64  ...t.j.t.j.j.d.d
-00002b50: 1e8d 0174 086a 186a 1964 0564 1e8d 0174  ...t.j.j.d.d...t
-00002b60: 086a 1a64 1f64 0f64 208d 0274 08a0 1ba1  .j.d.d.d ..t....
-00002b70: 007c 006a 026a 1c64 218d 0517 007d 067c  .|.j.j.d!....}.|
-00002b80: 006a 026a 1d90 0172 057c 006a 026a 1e72  .j.j...r.|.j.j.r
-00002b90: ff7c 0674 086a 1f64 2264 0564 238d 0237  .|.t.j.d"d.d#..7
-00002ba0: 007d 066e 067c 0674 08a0 20a1 0037 007d  .}.n.|.t.. ..7.}
-00002bb0: 067c 066a 2164 247c 006a 026a 227c 006a  .|.j!d$|.j.j"|.j
-00002bc0: 026a 2264 2514 0064 2664 2664 278d 0501  .j"d%..d&d&d'...
-00002bd0: 007c 066a 2164 287c 006a 026a 227c 006a  .|.j!d(|.j.j"|.j
-00002be0: 026a 2264 2514 0064 2664 2664 278d 0501  .j"d%..d&d&d'...
-00002bf0: 007c 006a 026a 2390 0172 3074 2464 2983  .|.j.j#..r0t$d).
-00002c00: 0101 0064 0053 0064 0053 0029 2a4e 72f0  ...d.S.d.S.)*Nr.
-00002c10: 0000 00da 074f 7665 7261 6c6c fa06 4e6f  .....Overall..No
-00002c20: 2052 4f49 725b 0000 0072 0100 0000 7244   ROIr[...r....rD
-00002c30: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002c40: 0100 0000 0300 0000 5300 0000 f30c 0000  ........S.......
-00002c50: 007c 00a0 0064 0167 01a1 0153 00a9 024e  .|...d.g...S...N
-00002c60: 725b 0000 00a9 01da 0b73 6f72 745f 7661  r[.......sort_va
-00002c70: 6c75 6573 a901 da01 7872 3500 0000 7235  lues....xr5...r5
-00002c80: 0000 0072 3600 0000 da08 3c6c 616d 6264  ...r6.....<lambd
-00002c90: 613e ba01 0000 f302 0000 000c 007a 2156  a>...........z!V
-00002ca0: 696f 6c69 6e50 6c6f 742e 6d61 6b65 2e3c  iolinPlot.make.<
-00002cb0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00002cc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002cd0: 0003 0000 0053 0000 0072 0301 0000 7204  .....S...r....r.
-00002ce0: 0100 0072 0501 0000 7207 0100 0072 3500  ...r....r....r5.
-00002cf0: 0000 7235 0000 0072 3600 0000 7209 0100  ..r5...r6...r...
-00002d00: 00bd 0100 0072 0a01 0000 6301 0000 0000  .....r....c.....
-00002d10: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-00002d20: 0000 0072 0301 0000 7204 0100 0072 0501  ...r....r....r..
-00002d30: 0000 7207 0100 0072 3500 0000 7235 0000  ..r....r5...r5..
-00002d40: 0072 3600 0000 7209 0100 00c0 0100 0072  .r6...r........r
-00002d50: 0a01 0000 54a9 01da 0464 726f 7072 0800  ....T....dropr..
-00002d60: 0000 da08 636f 6e73 7461 6e74 72a0 0000  ....constantr...
-00002d70: 007a 0778 2b73 6869 6674 2901 5a0b 6166  .z.x+shift).Z.af
-00002d80: 7465 725f 7363 616c 6572 0701 0000 7a07  ter_scaler....z.
-00002d90: 782d 7368 6966 74a9 0272 0801 0000 da01  x-shift..r......
-00002da0: 7972 f900 0000 6733 3333 3333 33e3 3f29  yr....g333333.?)
-00002db0: 04da 056e 615f 726d da05 7374 796c 65da  ...na_rm..style.
-00002dc0: 0466 696c 6c72 e600 0000 2904 724b 0000  .fillr....).rK..
-00002dd0: 005a 0d6f 7574 6c69 6572 5f61 6c70 6861  .Z.outlier_alpha
-00002de0: 7212 0100 0072 e600 0000 679a 9999 9999  r....r....g.....
-00002df0: 99d9 3f67 6666 6666 6666 f63f da01 7eda  ..?gffffff.?..~.
-00002e00: 0a6c 6162 656c 5f62 6f74 68a9 0272 0c01  .label_both..r..
-00002e10: 0000 5a08 6c61 6265 6c6c 6572 a901 da05  ..Z.labeller....
-00002e20: 616c 7068 61da 0467 7261 79a9 0272 1201  alpha..gray..r..
-00002e30: 0000 7217 0100 0029 05da 1270 616e 656c  ..r....)...panel
-00002e40: 5f67 7269 645f 6d61 6a6f 725f 79da 1270  _grid_major_y..p
-00002e50: 616e 656c 5f67 7269 645f 6d61 6a6f 725f  anel_grid_major_
-00002e60: 78da 1070 616e 656c 5f62 6163 6b67 726f  x..panel_backgro
-00002e70: 756e 64da 0b61 7869 735f 7465 7874 5f78  und..axis_text_x
-00002e80: 72c0 0000 0067 7b14 ae47 e17a a43f 2902  r....g{..G.z.?).
-00002e90: 724b 0000 0072 4a00 0000 7a23 4669 6775  rK...rJ...z#Figu
-00002ea0: 7265 732f 5669 6f6c 696e 5f70 6c6f 7473  res/Violin_plots
-00002eb0: 2f76 696f 6c69 6e70 6c6f 742e 706e 6772  /violinplot.pngr
-00002ec0: 4800 0000 4672 4900 0000 7a23 4669 6775  H...FrI...z#Figu
-00002ed0: 7265 732f 5669 6f6c 696e 5f70 6c6f 7473  res/Violin_plots
-00002ee0: 2f76 696f 6c69 6e70 6c6f 742e 7376 677a  /violinplot.svgz
-00002ef0: 1253 6176 6564 2076 696f 6c69 6e20 706c  .Saved violin pl
-00002f00: 6f74 2129 25da 0463 6f70 79da 0864 6565  ot!)%..copy..dee
-00002f10: 7063 6f70 7972 1300 0000 da0a 7461 626c  pcopyr......tabl
-00002f20: 655f 636f 6c73 da0a 7461 626c 655f 726f  e_cols..table_ro
-00002f30: 7773 da07 6772 6f75 7062 79da 0561 7070  ws..groupby..app
-00002f40: 6c79 da0b 7265 7365 745f 696e 6465 78da  ly..reset_index.
-00002f50: 0470 6c74 6eda 0361 6573 da05 7374 6167  .pltn..aes..stag
-00002f60: 65da 0667 6770 6c6f 745a 0b67 656f 6d5f  e..ggplotZ.geom_
-00002f70: 7669 6f6c 696e da0d 7669 6f6c 696e 5f63  violin..violin_c
-00002f80: 6f6c 6f75 725a 0c67 656f 6d5f 626f 7870  olourZ.geom_boxp
-00002f90: 6c6f 74da 0e62 6f78 706c 6f74 5f63 6f6c  lot..boxplot_col
-00002fa0: 6f75 72da 0478 6c69 6dda 0479 6c69 6d5a  our..xlim..ylimZ
-00002fb0: 0479 6c61 62da 0d74 6162 6c65 5f78 5f6c  .ylab..table_x_l
-00002fc0: 6162 656c 5a04 786c 6162 da0a 6661 6365  abelZ.xlab..face
-00002fd0: 745f 6772 6964 da09 7468 656d 655f 3533  t_grid..theme_53
-00002fe0: 38da 0574 6865 6d65 da06 7468 656d 6573  8..theme..themes
-00002ff0: da0c 656c 656d 656e 745f 6c69 6e65 da0c  ..element_line..
-00003000: 656c 656d 656e 745f 7265 6374 5a0d 656c  element_rectZ.el
-00003010: 656d 656e 745f 626c 616e 6b72 d200 0000  ement_blankr....
-00003020: da10 7669 6f6c 696e 5f73 686f 775f 6461  ..violin_show_da
-00003030: 7461 da0d 7669 6f6c 696e 5f6a 6974 7465  ta..violin_jitte
-00003040: 725a 0b67 656f 6d5f 6a69 7474 6572 da0a  rZ.geom_jitter..
-00003050: 6765 6f6d 5f70 6f69 6e74 7250 0000 0072  geom_pointrP...r
-00003060: 5100 0000 721e 0000 0072 1f00 0000 2907  Q...r....r....).
-00003070: 722f 0000 005a 076f 7269 675f 6466 72af  r/...Z.orig_dfr.
-00003080: 0000 00da 0573 6869 6674 da0b 7269 6768  .....shift..righ
-00003090: 745f 7368 6966 74da 0a6c 6566 745f 7368  t_shift..left_sh
-000030a0: 6966 7472 3f00 0000 7235 0000 0072 3500  iftr?...r5...r5.
-000030b0: 0000 7236 0000 0072 2600 0000 b101 0000  ..r6...r&.......
-000030c0: 7372 0000 000a 021c 0210 0118 0222 020c  sr..........."..
-000030d0: 021a 010c 0218 010c 0208 0204 0316 0216  ................
-000030e0: 0108 020c 0102 ff16 0202 fe14 0302 fd0a  ................
-000030f0: 0402 fc0a 0502 fb0c 0602 fa08 0702 f91a  ................
-00003100: 0802 0104 ff02 f806 0a02 f610 0b0c 010c  ................
-00003110: 0106 0106 0104 fc04 f50a 1108 0114 010c  ................
-00003120: 020c 020a 0104 0106 fe0c 040a 0104 0106  ................
-00003130: fe0a 040c 0104 ff7a 0f56 696f 6c69 6e50  .......z.ViolinP
-00003140: 6c6f 742e 6d61 6b65 4e29 0572 8700 0000  lot.makeN).r....
-00003150: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
-00003160: 2600 0000 7235 0000 0072 3500 0000 7235  &...r5...r5...r5
-00003170: 0000 0072 3600 0000 7229 0000 00b0 0100  ...r6...r)......
-00003180: 0073 0600 0000 0800 0201 0e01 7229 0000  .s..........r)..
-00003190: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000031a0: 0000 0300 0000 4000 0000 7324 0000 0065  ......@...s$...e
-000031b0: 005a 0164 005a 0265 0364 0164 0284 0083  .Z.d.Z.e.d.d....
-000031c0: 015a 0465 0564 0364 0484 0083 015a 0664  .Z.e.d.d.....Z.d
-000031d0: 0553 0029 0672 2a00 0000 6303 0000 0000  .S.).r*...c.....
-000031e0: 0000 0000 0000 0007 0000 000a 0000 0043  ...............C
-000031f0: 0000 0073 5001 0000 7c00 6a00 6a01 6401  ...sP...|.j.j.d.
-00003200: 6b02 720a 7402 6402 8301 8201 7403 a004  k.r.t.d.....t...
-00003210: 6403 a101 0100 7405 7c01 6404 1900 a006  d.....t.|.d.....
-00003220: a100 8301 7d03 7403 6a07 7c03 6405 7c00  ....}.t.j.|.d.|.
-00003230: 6a00 6a08 6406 8d03 7d04 7a04 7c04 0100  j.j.d...}.z.|...
-00003240: 5700 6e15 0400 7409 793a 0100 0100 0100  W.n...t.y:......
-00003250: 7c00 6a00 6a0a 7237 740b 6407 8301 0100  |.j.j.r7t.d.....
-00003260: 5900 6400 5300 5900 6400 5300 7700 7c00  Y.d.S.Y.d.S.w.|.
-00003270: 6a00 6a0a 7243 740b 6408 8301 0100 6409  j.j.rCt.d.....d.
-00003280: 7d05 0900 740c 740d a00e 7c00 6a0f a101  }...t.t...|.j...
-00003290: 7c04 740d a00e 7c01 a101 740d a00e 7c05  |.t...|...t...|.
-000032a0: a101 740d a00e 7c00 6a10 a101 740d a00e  ..t...|.j...t...
-000032b0: 7c00 6a11 a101 740d a00e 7c00 6a00 a101  |.j...t...|.j...
-000032c0: 8307 7d06 7c02 7270 7c02 a012 7403 6a13  ..}.|.rp|...t.j.
-000032d0: 7c06 a102 7d05 6e09 7405 740d a012 7403  |...}.n.t.t...t.
-000032e0: 6a13 7c06 a102 8301 7d05 7414 7c05 8301  j.|.....}.t.|...
-000032f0: 72a5 7c05 6a15 640b 640c 8400 640d 8d01  r.|.j.d.d...d...
-00003300: 0100 7c00 6a00 6a0a 729e 740b 640e 7416  ..|.j.j.r.t.d.t.
-00003310: 7c05 640f 1900 6410 1900 8301 9b00 6411  |.d...d.......d.
-00003320: 7c05 640f 1900 6412 1900 9b00 6413 9d05  |.d...d.....d...
-00003330: 8301 0100 7c05 640f 1900 6410 1900 7d05  ....|.d...d...}.
-00003340: 6e02 6400 5300 7146 2914 4e72 4400 0000  n.d.S.qF).NrD...
-00003350: 7a45 5061 7261 6d65 7465 7220 746f 2070  zEParameter to p
-00003360: 6c6f 7420 616c 6f6e 6720 7468 6520 782d  lot along the x-
-00003370: 6178 6573 206f 6620 7468 6520 6261 7263  axes of the barc
-00003380: 6861 7274 7320 6861 7320 6e6f 7420 6265  harts has not be
-00003390: 656e 2073 6574 2e7a 1146 6967 7572 6573  en set.z.Figures
-000033a0: 2f42 6172 6368 6172 7473 72f0 0000 007a  /Barchartsr....z
-000033b0: 144f 6e65 2072 6567 696f 6e20 6261 7220  .One region bar 
-000033c0: 6368 6172 74a9 02da 0966 756e 635f 6e61  chart....func_na
-000033d0: 6d65 da11 636f 6e66 6967 5f72 6567 696f  me..config_regio
-000033e0: 6e5f 7661 727a 1b53 6b69 7070 696e 6720  n_varz.Skipping 
-000033f0: 6261 7263 6861 7274 2063 7265 6174 696f  barchart creatio
-00003400: 6e2e 7a1a 0a2d 2d2d 2042 6172 6368 6172  n.z..--- Barchar
-00003410: 7420 6372 6561 7469 6f6e 202d 2d2d 7201  t creation ---r.
-00003420: 0000 0054 6301 0000 0000 0000 0000 0000  ...Tc...........
-00003430: 0001 0000 0002 0000 0053 0000 00f3 0800  .........S......
-00003440: 0000 7c00 6401 1900 5300 a902 4e72 0800  ..|.d...S...Nr..
-00003450: 0000 7235 0000 0072 0701 0000 7235 0000  ..r5...r....r5..
-00003460: 0072 3500 0000 7236 0000 0072 0901 0000  .r5...r6...r....
-00003470: 1002 0000 f302 0000 0008 007a 2042 6172  ...........z Bar
-00003480: 6368 6172 742e 7365 7475 702e 3c6c 6f63  chart.setup.<loc
-00003490: 616c 733e 2e3c 6c61 6d62 6461 3ea9 0172  als>.<lambda>..r
-000034a0: f200 0000 7a14 4d61 7869 6d75 6d20 7920  ....z.Maximum y 
-000034b0: 6c69 6d69 7420 6f66 3a20 72a4 0000 0072  limit of: r....r
-000034c0: 0800 0000 fa10 2073 6565 6e20 7769 7468  ...... seen with
-000034d0: 2052 4f49 3a20 725f 0000 007a 262e 2043   ROI: r_...z&. C
-000034e0: 7265 6174 696e 6720 6669 6775 7265 7320  reating figures 
-000034f0: 7769 7468 2074 6869 7320 7920 6c69 6d69  with this y limi
-00003500: 742e 0a29 1772 1300 0000 da15 7369 6e67  t..).r......sing
-00003510: 6c65 5f72 6f69 5f66 6967 5f78 5f61 7869  le_roi_fig_x_axi
-00003520: 73da 0945 7863 6570 7469 6f6e 7209 0000  s..Exceptionr...
-00003530: 0072 2800 0000 7268 0000 0072 a600 0000  .r(...rh...r....
-00003540: da10 6669 6e64 5f63 686f 7365 6e5f 726f  ..find_chosen_ro
-00003550: 6973 da11 7265 6769 6f6e 616c 5f66 6967  is..regional_fig
-00003560: 5f72 6f69 73da 094e 616d 6545 7272 6f72  _rois..NameError
-00003570: 721e 0000 0072 1f00 0000 da03 7a69 70da  r....r......zip.
-00003580: 0969 7465 7274 6f6f 6c73 da06 7265 7065  .itertools..repe
-00003590: 6174 7226 0000 0072 5600 0000 7243 0000  atr&...rV...rC..
-000035a0: 00da 0773 7461 726d 6170 da14 636c 6173  ...starmap..clas
-000035b0: 735f 6d65 7468 6f64 5f68 616e 646c 6572  s_method_handler
-000035c0: da03 616e 79da 0473 6f72 7472 ae00 0000  ..any..sortr....
-000035d0: 2907 722f 0000 0072 af00 0000 7234 0000  ).r/...r....r4..
-000035e0: 00da 096c 6973 745f 726f 6973 da0b 6368  ...list_rois..ch
-000035f0: 6f73 656e 5f72 6f69 7372 2c01 0000 da08  osen_roisr,.....
-00003600: 6974 6572 6162 6c65 7235 0000 0072 3500  iterabler5...r5.
-00003610: 0000 7236 0000 0072 2b00 0000 f001 0000  ..r6...r+.......
-00003620: 7340 0000 000c 0208 010a 0210 0208 0106  s@..............
-00003630: 0106 ff02 0208 010c 0108 010e 0106 ff02  ................
-00003640: ff08 0408 0104 0202 0116 0112 0114 0104  ................
-00003650: fe04 0410 0112 0308 0210 0108 022a 010e  .............*..
-00003660: 0304 0202 ec7a 0e42 6172 6368 6172 742e  .....z.Barchart.
-00003670: 7365 7475 7063 0600 0000 0000 0000 0000  setupc..........
-00003680: 0000 0b00 0000 0f00 0000 4300 0000 736c  ..........C...sl
-00003690: 0200 007c 016a 007c 0164 0119 007c 006b  ...|.j.|.d...|.k
-000036a0: 0219 007d 067c 06a0 017c 056a 0267 01a1  ...}.|...|.j.g..
-000036b0: 017d 067c 066a 0364 0264 038d 017d 0674  .}.|.j.d.d...}.t
-000036c0: 046a 057c 067c 056a 0219 007c 067c 056a  .j.|.|.j...|.|.j
-000036d0: 0219 00a0 06a1 0064 048d 027c 067c 056a  .......d...|.|.j
-000036e0: 023c 0064 0564 0684 007c 066a 0744 0083  .<.d.d...|.j.D..
-000036f0: 017c 065f 077c 056a 02a0 0864 0764 08a1  .|._.|.j...d.d..
-00003700: 027c 055f 027c 056a 09a0 0864 0764 08a1  .|._.|.j...d.d..
-00003710: 027c 055f 0974 0aa0 0b7c 06a1 0174 0aa0  .|._.t...|...t..
-00003720: 0ca1 0017 0074 0a6a 0d74 0a6a 0e64 0964  .....t.j.t.j.d.d
-00003730: 0a64 0b8d 0264 0a64 0264 0c8d 0317 0074  .d...d.d.d.....t
-00003740: 0a6a 0f64 0d74 0a6a 0e64 0964 0a64 0b8d  .j.d.t.j.d.d.d..
-00003750: 0264 0e8d 0217 0074 0a6a 1067 0064 0f8d  .d.....t.j.g.d..
-00003760: 0117 0074 0a6a 1174 0a6a 1264 1064 118d  ...t.j.t.j.d.d..
-00003770: 0174 0a6a 1364 1264 1364 148d 0274 0a6a  .t.j.d.d.d...t.j
-00003780: 1464 1564 1664 1764 188d 0374 0a6a 1464  .d.d.d.d...t.j.d
-00003790: 1564 1664 1764 188d 0374 0a6a 1464 1764  .d.d.d...t.j.d.d
-000037a0: 1664 198d 0274 0a6a 1464 1764 1564 1664  .d...t.j.d.d.d.d
-000037b0: 1a64 1769 0164 1b8d 0474 0a6a 1464 1764  .d.i.d...t.j.d.d
-000037c0: 1664 1c64 1d69 0164 1e8d 0364 1f64 2064  .d.d.i.d...d.d d
-000037d0: 2164 2269 0164 237c 056a 1564 248d 0c17  !d"i.d#|.j.d$...
-000037e0: 0074 0a6a 1674 0a6a 1764 257c 056a 0264  .t.j.t.j.d%|.j.d
-000037f0: 268d 0264 1664 1764 2764 288d 0417 0074  &..d.d.d'd(....t
-00003800: 0a6a 187c 056a 1964 298d 0117 007d 0764  .j.|.j.d)....}.d
-00003810: 2a64 0684 007c 06a0 1aa1 0044 0083 0164  *d...|.....D...d
-00003820: 1019 007d 087c 056a 0964 2b6b 0273 e77c  ...}.|.j.d+k.s.|
-00003830: 0774 0a6a 177c 056a 0264 2c64 2d7c 089b  .t.j.|.j.d,d-|..
-00003840: 009d 0264 2e7c 089b 009d 0264 2f7c 056a  ...d.|.....d/|.j
-00003850: 099b 0064 309d 0364 318d 0537 007d 076e  ...d0..d1..7.}.n
-00003860: 127c 0774 0a6a 177c 056a 0264 2c64 2d7c  .|.t.j.|.j.d,d-|
-00003870: 089b 009d 0264 2e7c 089b 009d 0264 328d  .....d.|.....d2.
-00003880: 0437 007d 077c 0774 0a6a 1b7c 056a 1c7c  .7.}.|.t.j.|.j.|
-00003890: 056a 1d7c 056a 1e64 338d 0337 007d 077c  .j.|.j.d3..7.}.|
-000038a0: 0290 0172 157c 0774 0aa0 1f64 007c 02a1  ...r.|.t...d.|..
-000038b0: 0237 007d 077c 0064 3437 007d 0064 107d  .7.}.|.d47.}.d.}
-000038c0: 097c 0264 106b 0290 0172 257c 047c 007c  .|.d.k...r%|.|.|
-000038d0: 0764 3583 037d 0964 367d 0a6e 077c 0264  .d5..}.d6}.n.|.d
-000038e0: 106b 0390 0172 2c64 377d 0a7c 037c 077c  .k...r,d7}.|.|.|
-000038f0: 007c 0a64 387c 0583 0501 007c 0953 0029  .|.d8|.....|.S.)
-00003900: 394e 72f0 0000 0054 720b 0100 0029 01da  9Nr....Tr....)..
-00003910: 0a63 6174 6567 6f72 6965 7363 0100 0000  .categoriesc....
-00003920: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00003930: 5300 0000 7318 0000 0067 007c 005d 087d  S...s....g.|.].}
-00003940: 017c 01a0 0064 0064 01a1 0291 0271 0253  .|...d.d.....q.S
-00003950: 0029 0272 0d00 0000 720e 0000 0029 0172  .).r....r....).r
-00003960: 1c00 0000 2902 7299 0000 00da 0163 7235  ....).r......cr5
-00003970: 0000 0072 3500 0000 7236 0000 0072 9c00  ...r5...r6...r..
-00003980: 0000 2402 0000 f302 0000 0018 007a 2142  ..$..........z!B
-00003990: 6172 6368 6172 742e 6d61 6b65 2e3c 6c6f  archart.make.<lo
-000039a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000039b0: 720d 0000 0072 0e00 0000 da06 7369 6e67  r....r......sing
-000039c0: 6c65 e79a 9999 9999 99e9 3f29 02da 0870  le........?)...p
-000039d0: 7265 7365 7276 6572 4b00 0000 2903 da08  reserverK...)...
-000039e0: 706f 7369 7469 6f6e 724b 0000 0072 1001  positionrK...r..
-000039f0: 0000 7208 0000 0029 0272 e600 0000 7257  ..r....).r....rW
-00003a00: 0100 0029 01da 066c 6162 656c 7372 0100  ...)...labelsr..
-00003a10: 0000 7216 0100 00da 0577 6869 7465 679a  ..r......whiteg.
-00003a20: 9999 9999 99c9 3f72 1901 0000 da04 626f  ......?r......bo
-00003a30: 6c64 da05 626c 6163 6be9 1400 0000 a903  ld..black.......
-00003a40: da06 7765 6967 6874 da05 636f 6c6f 7272  ..weight..colorr
-00003a50: e600 0000 a902 72e6 0000 0072 5f01 0000  ......r....r_...
-00003a60: da01 6229 0472 e600 0000 725e 0100 0072  ..b).r....r^...r
-00003a70: 5f01 0000 da06 6d61 7267 696e da01 6ce9  _.....margin..l.
-00003a80: 0500 0000 2903 72e6 0000 0072 5f01 0000  ....).r....r_...
-00003a90: 7262 0100 00e9 0a00 0000 e91e 0000 0072  rb.............r
-00003aa0: fa00 0000 6733 3333 3333 33eb 3f29 0267  ....g333333.?).g
-00003ab0: cdcc cccc cccc ec3f 7255 0100 0029 0c72  .......?rU...).r
-00003ac0: 1b01 0000 721c 0100 00da 0c61 7869 735f  ....r......axis_
-00003ad0: 7469 746c 655f 78da 0c61 7869 735f 7469  title_x..axis_ti
-00003ae0: 746c 655f 79da 0b61 7869 735f 7465 7874  tle_y..axis_text
-00003af0: 5f79 5a0c 6c65 6765 6e64 5f74 6974 6c65  _yZ.legend_title
-00003b00: 5a0b 6c65 6765 6e64 5f74 6578 745a 146c  Z.legend_textZ.l
-00003b10: 6567 656e 645f 656e 7472 795f 7370 6163  egend_entry_spac
-00003b20: 696e 675a 0f6c 6567 656e 645f 6b65 795f  ingZ.legend_key_
-00003b30: 7369 7a65 da0f 7375 6270 6c6f 7473 5f61  size..subplots_a
-00003b40: 646a 7573 74da 0f6c 6567 656e 645f 706f  djust..legend_po
-00003b50: 7369 7469 6f6e 72c0 0000 0067 6666 6666  sitionr....gffff
-00003b60: 6666 e6bf 2902 720f 0100 00da 056c 6162  ff..).r......lab
-00003b70: 656c 72fc 0000 0029 0372 5f01 0000 72e6  elr....).r_...r.
-00003b80: 0000 00da 0276 61a9 0172 bc00 0000 6301  .....va..r....c.
-00003b90: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00003ba0: 0000 0053 0000 0073 1800 0000 6700 7c00  ...S...s....g.|.
-00003bb0: 5d08 7d01 6400 7c01 7600 7202 7c01 9102  ].}.d.|.v.r.|...
-00003bc0: 7102 5300 2901 5a08 436f 6e66 5f49 6e74  q.S.).Z.Conf_Int
-00003bd0: 7235 0000 0029 0272 9900 0000 7208 0100  r5...).r....r...
-00003be0: 0072 3500 0000 7235 0000 0072 3600 0000  .r5...r5...r6...
-00003bf0: 729c 0000 0040 0200 0072 5301 0000 7244  r....@...rS...rD
-00003c00: 0000 0072 5b00 0000 7a05 4d65 616e 2d7a  ...r[...z.Mean-z
-00003c10: 054d 6561 6e2b 7a07 6661 6374 6f72 28fa  .Mean+z.factor(.
-00003c20: 0129 2905 7208 0100 0072 0f01 0000 da04  .)).r....r......
-00003c30: 796d 696e da04 796d 6178 7212 0100 0029  ymin..ymaxr....)
-00003c40: 0472 0801 0000 720f 0100 0072 7001 0000  .r....r....rp...
-00003c50: 7271 0100 0029 0372 0801 0000 720f 0100  rq...).r....r...
-00003c60: 0072 1201 0000 5a0a 5f73 616d 655f 796c  .r....Z._same_yl
-00003c70: 696d 7239 0000 005a 0f44 6966 6665 7265  imr9...Z.Differe
-00003c80: 6e74 5f79 6178 6973 5a0a 5361 6d65 5f79  nt_yaxisZ.Same_y
-00003c90: 6178 6973 5a08 6261 7263 6861 7274 2920  axisZ.barchart) 
-00003ca0: 7271 0000 0072 0601 0000 7242 0100 0072  rq...r....rB...r
-00003cb0: 2401 0000 7266 0000 00da 0b43 6174 6567  $...rf.....Categ
-00003cc0: 6f72 6963 616c 72a6 0000 0072 7600 0000  oricalr....rv...
-00003cd0: 721c 0000 00da 1573 696e 676c 655f 726f  r......single_ro
-00003ce0: 695f 6669 675f 636f 6c6f 7572 7225 0100  i_fig_colourr%..
-00003cf0: 0072 2801 0000 722f 0100 005a 0867 656f  .r(...r/...Z.geo
-00003d00: 6d5f 636f 6c5a 0e70 6f73 6974 696f 6e5f  m_colZ.position_
-00003d10: 646f 6467 655a 0d67 656f 6d5f 6572 726f  dodgeZ.geom_erro
-00003d20: 7262 6172 5a10 7363 616c 655f 785f 6469  rbarZ.scale_x_di
-00003d30: 7363 7265 7465 7230 0100 0072 3201 0000  screter0...r2...
-00003d40: 7233 0100 00da 0c65 6c65 6d65 6e74 5f74  r3.....element_t
-00003d50: 6578 7472 d200 0000 5a09 6765 6f6d 5f74  extr....Z.geom_t
-00003d60: 6578 7472 2601 0000 5a11 7363 616c 655f  extr&...Z.scale_
-00003d70: 6669 6c6c 5f6d 616e 7561 6cda 2063 6f6c  fill_manual. col
-00003d80: 6f72 626c 696e 645f 6672 6965 6e64 6c79  orblind_friendly
-00003d90: 5f70 6c6f 745f 636f 6c6f 7572 7372 ed00  _plot_coloursr..
-00003da0: 0000 da04 6c61 6273 da16 7369 6e67 6c65  ....labs..single
-00003db0: 5f72 6f69 5f66 6967 5f6c 6162 656c 5f78  _roi_fig_label_x
-00003dc0: da16 7369 6e67 6c65 5f72 6f69 5f66 6967  ..single_roi_fig
-00003dd0: 5f6c 6162 656c 5f79 da19 7369 6e67 6c65  _label_y..single
-00003de0: 5f72 6f69 5f66 6967 5f6c 6162 656c 5f66  _roi_fig_label_f
-00003df0: 696c 6c72 2c01 0000 290b 723e 0000 0072  illr,...).r>...r
-00003e00: af00 0000 5a06 796c 696d 6974 da0d 7361  ....Z.ylimit..sa
-00003e10: 7665 5f66 756e 6374 696f 6e5a 1266 696e  ve_functionZ.fin
-00003e20: 645f 796c 696d 5f66 756e 6374 696f 6e72  d_ylim_functionr
-00003e30: 1300 0000 da0a 6375 7272 656e 745f 6466  ......current_df
-00003e40: 723f 0000 005a 0f63 6f6e 665f 696e 745f  r?...Z.conf_int_
-00003e50: 7374 7269 6e67 5a0d 7265 7475 726e 6564  stringZ.returned
-00003e60: 5f79 6c69 6d72 5200 0000 7235 0000 0072  _ylimrR...r5...r
-00003e70: 3500 0000 7236 0000 0072 2600 0000 1a02  5...r6...r&.....
-00003e80: 0000 7382 0000 0012 020e 020c 010c 0102  ..s.............
-00003e90: 0104 0102 ff04 010c fe12 0410 0110 0108  ................
-00003ea0: 0306 0102 ff18 0202 fe16 0302 fd0a 0402  ................
-00003eb0: fc0e 050c 010e 010e 010c 0114 0112 0102  ................
-00003ec0: 0102 0106 0102 0104 0104 f502 fb12 1206  ................
-00003ed0: 0104 ff02 ee0c 1402 ec02 ff16 180a 020c  ................
-00003ee0: 0110 010c 010a fe0c 0410 0108 ff0e 0304  ................
-00003ef0: 0108 ff06 0310 0208 0104 020a 010c 0106  ................
-00003f00: 010a 0104 0110 0204 027a 0d42 6172 6368  .........z.Barch
-00003f10: 6172 742e 6d61 6b65 4e29 0772 8700 0000  art.makeN).r....
-00003f20: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
-00003f30: 2b00 0000 728b 0000 0072 2600 0000 7235  +...r....r&...r5
-00003f40: 0000 0072 3500 0000 7235 0000 0072 3600  ...r5...r5...r6.
-00003f50: 0000 722a 0000 00ef 0100 0073 0a00 0000  ..r*.......s....
-00003f60: 0800 0201 0a01 0229 0e01 722a 0000 0063  .......)..r*...c
-00003f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f80: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
-00003f90: 0164 005a 0265 0364 0164 0284 0083 015a  .d.Z.e.d.d.....Z
-00003fa0: 0465 0364 0364 0484 0083 015a 0565 0664  .e.d.d.....Z.e.d
-00003fb0: 0564 0684 0083 015a 0764 0753 0029 0872  .d.....Z.d.S.).r
-00003fc0: 2c00 0000 6303 0000 0000 0000 0000 0000  ,...c...........
-00003fd0: 000b 0000 000a 0000 0043 0000 0073 a401  .........C...s..
-00003fe0: 0000 7400 a001 6401 a101 0100 7402 7c01  ..t...d.....t.|.
-00003ff0: 6402 1900 a003 a100 8301 7d03 7400 6a04  d.........}.t.j.
-00004000: 7c03 6403 7c00 6a05 6a06 6404 8d03 7d04  |.d.|.j.j.d...}.
-00004010: 7a04 7c04 0100 5700 6e15 0400 7407 7930  z.|...W.n...t.y0
-00004020: 0100 0100 0100 7c00 6a05 6a08 722d 7409  ......|.j.j.r-t.
-00004030: 6405 8301 0100 5900 6400 5300 5900 6400  d.....Y.d.S.Y.d.
-00004040: 5300 7700 7c00 6a05 6a08 7239 7409 6406  S.w.|.j.j.r9t.d.
-00004050: 8301 0100 6407 6408 8400 7400 a00a 6409  ....d.d...t...d.
-00004060: 640a a102 4400 8301 7d05 7c00 6a0b 7c00  d...D...}.|.j.|.
-00004070: 6a05 7c05 7c01 640b 640c 8d04 7d06 6700  j.|.|.d.d...}.g.
-00004080: 7d07 7c04 4400 5d0c 7d08 7c07 a00c 7c00  }.|.D.].}.|...|.
-00004090: a00d 7c08 7c06 7c01 a103 a101 0100 7152  ..|.|.|.......qR
-000040a0: 640d 7d09 0900 740e 740f a010 7c00 6a11  d.}...t.t...|.j.
-000040b0: a101 7c04 7c07 740f a010 7c09 a101 740f  ..|.|.t...|...t.
-000040c0: a010 7c00 6a12 a101 740f a010 7c00 6a13  ..|.j...t...|.j.
-000040d0: a101 740f a010 7c00 6a05 a101 8307 7d0a  ..t...|.j.....}.
-000040e0: 7c02 7289 7c02 a014 7400 6a15 7c0a a102  |.r.|...t.j.|...
-000040f0: 7d09 6e09 7402 740f a014 7400 6a15 7c0a  }.n.t.t...t.j.|.
-00004100: a102 8301 7d09 7416 7c09 8301 72cf 7a07  ....}.t.|...r.z.
-00004110: 7c09 a017 6400 a101 0100 5700 6e09 0400  |...d.....W.n...
-00004120: 7418 79a6 0100 0100 0100 5900 6e01 7700  t.y.......Y.n.w.
-00004130: 7c09 6a19 640f 6410 8400 6411 8d01 0100  |.j.d.d...d.....
-00004140: 7c00 6a05 6a08 72c8 7409 6412 741a 7c09  |.j.j.r.t.d.t.|.
-00004150: 6413 1900 6414 1900 8301 9b00 6415 7c09  d...d.......d.|.
-00004160: 6413 1900 6416 1900 9b00 6417 9d05 8301  d...d.....d.....
-00004170: 0100 7c09 6413 1900 6414 1900 7d09 6e02  ..|.d...d...}.n.
-00004180: 6400 5300 7162 2918 4e7a 1246 6967 7572  d.S.qb).Nz.Figur
-00004190: 6573 2f48 6973 746f 6772 616d 7372 f000  es/Histogramsr..
-000041a0: 0000 722c 0000 0072 3a01 0000 7a1c 536b  ..r,...r:...z.Sk
-000041b0: 6970 7069 6e67 2068 6973 746f 6772 616d  ipping histogram
-000041c0: 2063 7265 6174 696f 6e2e 7a1b 0a2d 2d2d   creation.z..---
-000041d0: 2048 6973 746f 6772 616d 2063 7265 6174   Histogram creat
-000041e0: 696f 6e20 2d2d 2d63 0100 0000 0000 0000  ion ---c........
-000041f0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00004200: 731e 0000 0067 007c 005d 0b7d 0174 00a0  s....g.|.].}.t..
-00004210: 01a1 009b 0064 007c 019b 009d 0391 0271  .....d.|.......q
-00004220: 0253 0029 017a 152f 4f76 6572 616c 6c2f  .S.).z./Overall/
-00004230: 5261 775f 7265 7375 6c74 732f 2902 7215  Raw_results/).r.
-00004240: 0000 0072 1600 0000 7298 0000 0072 3500  ...r....r....r5.
-00004250: 0000 7235 0000 0072 3600 0000 729c 0000  ..r5...r6...r...
-00004260: 0071 0200 0073 0200 0000 1e00 7a23 4869  .q...s......z#Hi
-00004270: 7374 6f67 7261 6d2e 7365 7475 702e 3c6c  stogram.setup.<l
-00004280: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00004290: 3e7a 134f 7665 7261 6c6c 2f52 6177 5f72  >z.Overall/Raw_r
-000042a0: 6573 756c 7473 726f 0000 0072 0500 0000  esultsro...r....
-000042b0: 2901 727f 0000 0072 0100 0000 5463 0100  ).r....r....Tc..
-000042c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000042d0: 0000 5300 0000 723d 0100 0072 3e01 0000  ..S...r=...r>...
-000042e0: 7235 0000 0072 0701 0000 7235 0000 0072  r5...r....r5...r
-000042f0: 3500 0000 7236 0000 0072 0901 0000 8b02  5...r6...r......
-00004300: 0000 723f 0100 007a 2148 6973 746f 6772  ..r?...z!Histogr
-00004310: 616d 2e73 6574 7570 2e3c 6c6f 6361 6c73  am.setup.<locals
-00004320: 3e2e 3c6c 616d 6264 613e 7240 0100 007a  >.<lambda>r@...z
-00004330: 144d 6178 696d 756d 2078 206c 696d 6974  .Maximum x limit
-00004340: 206f 663a 2072 a400 0000 7208 0000 0072   of: r....r....r
-00004350: 4101 0000 725f 0000 007a 262e 2043 7265  A...r_...z&. Cre
-00004360: 6174 696e 6720 6669 6775 7265 7320 7769  ating figures wi
-00004370: 7468 2074 6869 7320 7820 6c69 6d69 742e  th this x limit.
-00004380: 0a29 1b72 0900 0000 7228 0000 0072 6800  .).r....r(...rh.
-00004390: 0000 72a6 0000 0072 4401 0000 7213 0000  ..r....rD...r...
-000043a0: 0072 4501 0000 7246 0100 0072 1e00 0000  .rE...rF...r....
-000043b0: 721f 0000 00da 0a66 696e 645f 6669 6c65  r......find_file
-000043c0: 7372 8600 0000 72da 0000 00da 2767 6574  sr....r.....'get
-000043d0: 5f6d 6561 6e5f 616e 645f 6d65 6469 616e  _mean_and_median
-000043e0: 5f66 6f72 5f65 6163 685f 6368 6f73 656e  _for_each_chosen
-000043f0: 5f72 6f69 7247 0100 0072 4801 0000 7249  _roirG...rH...rI
-00004400: 0100 0072 2600 0000 7256 0000 0072 4300  ...r&...rV...rC.
-00004410: 0000 724a 0100 0072 4b01 0000 724c 0100  ..rJ...rK...rL..
-00004420: 00da 0672 656d 6f76 65da 0a56 616c 7565  ...remove..Value
-00004430: 4572 726f 7272 4d01 0000 72ae 0000 0029  ErrorrM...r....)
-00004440: 0b72 2f00 0000 727e 0000 0072 3400 0000  .r/...r~...r4...
-00004450: 724e 0100 0072 4f01 0000 727d 0000 0072  rN...rO...r}...r
-00004460: 8000 0000 5a10 636f 6d62 696e 6564 5f72  ....Z.combined_r
-00004470: 6177 5f64 6673 da03 726f 6972 2b01 0000  aw_dfs..roir+...
-00004480: 7250 0100 0072 3500 0000 7235 0000 0072  rP...r5...r5...r
-00004490: 3600 0000 722b 0000 005f 0200 0073 5800  6...r+..._...sX.
-000044a0: 0000 0a02 1002 0801 0601 06ff 0203 0801  ................
-000044b0: 0c01 0801 0e01 06ff 02ff 0804 0801 0603  ................
-000044c0: 0a01 06ff 1402 0402 0801 0401 0c01 06ff  ................
-000044d0: 0403 0201 1001 1201 1401 04fe 0404 1001  ................
-000044e0: 1202 0802 0201 0e01 0c01 0401 02ff 1003  ................
-000044f0: 0802 2a01 0e03 0402 02e8 7a0f 4869 7374  ..*.......z.Hist
-00004500: 6f67 7261 6d2e 7365 7475 7063 0400 0000  ogram.setupc....
-00004510: 0000 0000 0000 0000 0800 0000 0700 0000  ................
-00004520: 4300 0000 732a 0100 007c 0164 016b 0272  C...s*...|.d.k.r
-00004530: 0874 00a0 01a1 0053 007c 0164 026b 0272  .t.....S.|.d.k.r
-00004540: 157c 02a0 02a1 007d 0464 027c 0464 033c  .|.....}.d.|.d.<
-00004550: 006e 0a7c 027c 0264 0319 007c 016b 0219  .n.|.|.d...|.k..
-00004560: 00a0 02a1 007d 047c 04a0 03a1 007d 047c  .....}.|.....}.|
-00004570: 036a 0464 0464 0369 0164 058d 017d 0374  .j.d.d.i.d...}.t
-00004580: 0574 0664 007c 006a 076a 087c 006a 076a  .t.d.|.j.j.|.j.j
-00004590: 0967 0283 0283 017d 057c 046a 0a7c 0364  .g.....}.|.j.|.d
-000045a0: 0367 017c 05a2 0164 0664 078d 037d 0467  .g.|...d.d...}.g
-000045b0: 007c 05a2 0164 0391 0164 0891 0164 0991  .|...d...d...d..
-000045c0: 0164 0a91 017d 067c 046a 0b44 005d 0c7d  .d...}.|.j.D.].}
-000045d0: 077c 077c 0676 0172 5e7c 046a 0c7c 0764  .|.|.v.r^|.j.|.d
-000045e0: 058d 017d 0471 5274 006a 0d7c 047c 0664  ...}.qRt.j.|.|.d
-000045f0: 0064 0b85 0219 0064 0c64 0964 0a67 0264  .d.....d.d.d.g.d
-00004600: 0d64 0e8d 057d 047c 006a 076a 0e72 827c  .d...}.|.j.j.r.|
-00004610: 006a 076a 0f73 827c 046a 107c 0464 0c19  .j.j.s.|.j.|.d..
-00004620: 0064 096b 0219 007d 047c 0453 007c 006a  .d.k...}.|.S.|.j
-00004630: 076a 0f72 937c 006a 076a 0e73 937c 046a  .j.r.|.j.j.s.|.j
-00004640: 107c 0464 0c19 0064 0a6b 0219 007d 047c  .|.d...d.k...}.|
-00004650: 0453 0029 0f4e 7202 0100 0072 0101 0000  .S.).Nr....r....
-00004660: 7260 0000 0072 f000 0000 2901 7276 0000  r`...r....).rv..
-00004670: 0072 f900 0000 2902 da02 6f6e da03 686f  .r....)...on..ho
-00004680: 7772 6100 0000 725b 0000 0072 a100 0000  wra...r[...r....
-00004690: e9fe ffff ffda 0953 7461 7469 7374 6963  .......Statistic
-000046a0: da0a 7374 6174 5f76 616c 7565 2904 7262  ..stat_value).rb
-000046b0: 0000 0072 6300 0000 da0a 7661 6c75 655f  ...rc.....value_
-000046c0: 7661 7273 7264 0000 0029 1172 6600 0000  varsrd...).rf...
-000046d0: 7267 0000 0072 1e01 0000 727c 0000 00da  rg...r....r|....
-000046e0: 0672 656e 616d 6572 6800 0000 7269 0000  .renamerh...ri..
-000046f0: 0072 1300 0000 726b 0000 0072 6c00 0000  .r....rk...rl...
-00004700: da05 6d65 7267 6572 7600 0000 720c 0100  ..mergerv...r...
-00004710: 0072 7b00 0000 da13 6869 7374 6f67 7261  .r{.....histogra
-00004720: 6d5f 7368 6f77 5f6d 6561 6eda 1568 6973  m_show_mean..his
-00004730: 746f 6772 616d 5f73 686f 775f 6d65 6469  togram_show_medi
-00004740: 616e 7271 0000 0029 0872 2f00 0000 723e  anrq...).r/...r>
-00004750: 0000 0072 8000 0000 727e 0000 0072 7b01  ...r....r~...r{.
-00004760: 0000 7281 0000 0072 ed00 0000 7285 0000  ..r....r....r...
-00004770: 0072 3500 0000 7235 0000 0072 3600 0000  .r5...r5...r6...
-00004780: 727d 0100 0095 0200 0073 3a00 0000 0804  r}.......s:.....
-00004790: 0801 0801 0801 0a01 1402 0802 0403 0601  ................
-000047a0: 06ff 1a04 0601 0801 0201 06fe 1805 0a02  ................
-000047b0: 0801 0c01 0280 1202 0801 06ff 1003 1201  ................
-000047c0: 0404 10fd 1201 0402 7a31 4869 7374 6f67  ........z1Histog
-000047d0: 7261 6d2e 6765 745f 6d65 616e 5f61 6e64  ram.get_mean_and
-000047e0: 5f6d 6564 6961 6e5f 666f 725f 6561 6368  _median_for_each
-000047f0: 5f63 686f 7365 6e5f 726f 6963 0600 0000  _chosen_roic....
-00004800: 0000 0000 0000 0000 0900 0000 1000 0000  ................
-00004810: 4300 0000 73f8 0100 007c 016a 0072 0c7c  C...s....|.j.r.|
-00004820: 056a 0172 0a74 0264 0183 0101 0064 0053  .j.r.t.d.....d.S
-00004830: 0074 03a0 047c 0174 036a 0564 0264 038d  .t...|.t.j.d.d..
-00004840: 01a1 0274 03a0 06a1 0017 0074 036a 077c  ...t.......t.j.|
-00004850: 056a 087c 056a 0964 0464 0564 068d 0417  .j.|.j.d.d.d....
-00004860: 0074 036a 0a7c 056a 0b9b 0064 077c 056a  .t.j.|.j...d.|.j
-00004870: 0c9b 009d 0364 0564 0864 098d 0317 0074  .....d.d.d.....t
-00004880: 036a 0d7c 056a 0e7c 056a 0f64 0a8d 0217  .j.|.j.|.j.d....
-00004890: 0074 036a 1074 036a 116a 1264 0464 0b8d  .t.j.t.j.j.d.d..
-000048a0: 0174 036a 116a 1264 0c64 0b8d 0174 036a  .t.j.j.d.d...t.j
-000048b0: 1264 0464 0b8d 0174 036a 1364 0d64 0e8d  .d.d...t.j.d.d..
-000048c0: 0174 036a 1364 0f64 1064 118d 0274 036a  .t.j.d.d.d...t.j
-000048d0: 1464 1264 1364 1464 158d 0374 036a 1464  .d.d.d.d...t.j.d
-000048e0: 1264 1364 1464 158d 0374 036a 1464 1264  .d.d.d...t.j.d.d
-000048f0: 1664 1364 178d 0374 036a 1464 1264 1664  .d.d...t.j.d.d.d
-00004900: 1364 178d 0374 036a 1464 1664 1364 188d  .d...t.j.d.d.d..
-00004910: 0274 036a 1464 1664 1364 188d 027c 056a  .t.j.d.d.d...|.j
-00004920: 1564 198d 0c17 007d 067c 056a 1673 8e7c  .d.....}.|.j.s.|
-00004930: 056a 1772 ad7c 0674 036a 1874 036a 0564  .j.r.|.t.j.t.j.d
-00004940: 1a64 1b64 1c8d 027c 056a 1964 1d8d 0237  .d.d...|.j.d...7
-00004950: 007d 067c 0674 036a 1a7c 056a 1b64 1e19  .}.|.t.j.|.j.d..
-00004960: 007c 056a 1b64 0c19 0067 0264 1f8d 0137  .|.j.d...g.d...7
-00004970: 007d 067c 056a 1c73 b87c 0674 036a 1064  .}.|.j.s.|.t.j.d
-00004980: 2064 218d 0137 007d 067c 0272 c77c 0674   d!..7.}.|.r.|.t
-00004990: 03a0 1d64 227c 02a1 0237 007d 067c 0064  ...d"|...7.}.|.d
-000049a0: 2337 007d 006e 087c 0674 03a0 1d64 2264  #7.}.n.|.t...d"d
-000049b0: 00a1 0237 007d 0664 047d 077c 0264 046b  ...7.}.d.}.|.d.k
-000049c0: 0272 de7c 047c 007c 0664 2483 037d 0764  .r.|.|.|.d$..}.d
-000049d0: 257d 086e 067c 0264 046b 0372 e464 267d  %}.n.|.d.k.r.d&}
-000049e0: 0874 1e6a 1f64 2774 2064 288d 0201 007c  .t.j.d't d(....|
-000049f0: 037c 067c 007c 0864 297c 0583 0501 0074  .|.|.|.d)|.....t
-00004a00: 1e6a 1f64 2a74 2064 288d 0201 007c 0753  .j.d*t d(....|.S
-00004a10: 0029 2b4e 7a38 494e 464f 3a20 4869 7374  .)+Nz8INFO: Hist
-00004a20: 6f67 7261 6d73 2063 616e 6e6f 7420 6265  ograms cannot be
-00004a30: 206d 6164 6520 666f 7220 7468 6520 4e6f   made for the No
-00004a40: 2052 4f49 2063 6174 6567 6f72 792e 7261   ROI category.ra
-00004a50: 0000 0072 0701 0000 7201 0000 0054 2904  ...r....r....T).
-00004a60: da08 6269 6e77 6964 7468 7212 0100 00da  ..binwidthr.....
-00004a70: 0862 6f75 6e64 6172 7972 1001 0000 7213  .boundaryr....r.
-00004a80: 0100 0072 1401 0000 7215 0100 0072 0e01  ...r....r....r..
-00004a90: 0000 7216 0100 0072 0800 0000 7259 0100  ..r....r....rY..
-00004aa0: 00a9 0172 1201 0000 7218 0100 0072 a000  ...r....r....r..
-00004ab0: 0000 7219 0100 0072 5a01 0000 725b 0100  ..r....rZ...r[..
-00004ac0: 0072 5c01 0000 725d 0100 0072 6501 0000  .r\...r]...re...
-00004ad0: a903 725e 0100 0072 e600 0000 725f 0100  ..r^...r....r_..
-00004ae0: 0072 6001 0000 a90c 5a12 7061 6e65 6c5f  .r`.....Z.panel_
-00004af0: 6772 6964 5f6d 696e 6f72 5f78 721b 0100  grid_minor_xr...
-00004b00: 0072 1a01 0000 5a0f 706c 6f74 5f62 6163  .r....Z.plot_bac
-00004b10: 6b67 726f 756e 6472 1c01 0000 7267 0100  kgroundr....rg..
-00004b20: 0072 6801 0000 5a0c 7374 7269 705f 7465  .rh...Z.strip_te
-00004b30: 7874 5f78 5a0c 7374 7269 705f 7465 7874  xt_xZ.strip_text
-00004b40: 5f79 721d 0100 0072 6901 0000 72c0 0000  _yr....ri...r...
-00004b50: 0072 8501 0000 7284 0100 0029 025a 0a78  .r....r....).Z.x
-00004b60: 696e 7465 7263 6570 7472 5f01 0000 2901  interceptr_...).
-00004b70: 72e6 0000 0072 4800 0000 726e 0100 00da  r....rH...rn....
-00004b80: 046e 6f6e 6529 0172 6b01 0000 72a4 0000  .none).rk...r...
-00004b90: 005a 0a5f 7361 6d65 5f78 6c69 6d72 3800  .Z._same_xlimr8.
-00004ba0: 0000 5a0f 4469 6666 6572 656e 745f 7861  ..Z.Different_xa
-00004bb0: 7869 735a 0a53 616d 655f 7861 7869 73da  xisZ.Same_xaxis.
-00004bc0: 0669 676e 6f72 6529 02da 0661 6374 696f  .ignore)...actio
-00004bd0: 6eda 0863 6174 6567 6f72 79da 0968 6973  n..category..his
-00004be0: 746f 6772 616d da07 6465 6661 756c 7429  togram..default)
-00004bf0: 21da 0565 6d70 7479 721e 0000 0072 1f00  !..emptyr....r..
-00004c00: 0000 7225 0100 0072 2801 0000 7226 0100  ..r%...r(...r&..
-00004c10: 0072 2f01 0000 5a0e 6765 6f6d 5f68 6973  .r/...Z.geom_his
-00004c20: 746f 6772 616d da12 6869 7374 6f67 7261  togram..histogra
-00004c30: 6d5f 6269 6e77 6964 7468 da14 6869 7374  m_binwidth..hist
-00004c40: 6f67 7261 6d5f 6669 675f 636f 6c6f 7572  ogram_fig_colour
-00004c50: 722e 0100 0072 6c00 0000 726b 0000 0072  r....rl...rk...r
-00004c60: 7601 0000 da15 6869 7374 6f67 7261 6d5f  v.....histogram_
-00004c70: 6669 675f 6c61 6265 6c5f 78da 1568 6973  fig_label_x..his
+000000c0: 6d1b 5a1b 0100 6400 6401 6c17 5a17 6517  m.Z...d.d.l.Z.e.
+000000d0: a01c 6407 a101 0100 6408 6409 6c1d 6d1e  ..d.....d.d.l.m.
+000000e0: 5a1e 0100 4700 640a 640b 8400 640b 8302  Z...G.d.d...d...
+000000f0: 5a1f 4700 640c 640d 8400 640d 651f 8303  Z.G.d.d...d.e...
+00000100: 5a20 4700 640e 640f 8400 640f 651f 8303  Z G.d.d...d.e...
+00000110: 5a21 4700 6410 6411 8400 6411 651f 8303  Z!G.d.d...d.e...
+00000120: 5a22 4700 6412 6413 8400 6413 651f 8303  Z"G.d.d...d.e...
+00000130: 5a23 4700 6414 6415 8400 6415 651f 8303  Z#G.d.d...d.e...
+00000140: 5a24 6401 5300 2916 e900 0000 004e a901  Z$d.S.)......N..
+00000150: da04 676c 6f62 2901 da04 5061 7468 2901  ..glob)...Path).
+00000160: da08 706c 6f74 7469 6e67 2901 da06 7079  ..plotting)...py
+00000170: 706c 6f74 2901 da05 496d 6167 65da 0361  plot)...Image..a
+00000180: 6767 e901 0000 0029 01da 0555 7469 6c73  gg.....)...Utils
+00000190: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001a0: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
+000001b0: 5a01 6400 5a02 6401 5a03 6504 6402 6403  Z.d.Z.d.Z.e.d.d.
+000001c0: 8400 8301 5a05 6506 6404 6405 8400 8301  ....Z.e.d.d.....
+000001d0: 5a07 6506 6406 6407 8400 8301 5a08 6506  Z.e.d.d.....Z.e.
+000001e0: 6408 6409 8400 8301 5a09 6401 5300 290a  d.d.....Z.d.S.).
+000001f0: da07 4669 6775 7265 734e 6304 0000 0000  ..FiguresNc.....
+00000200: 0000 0000 0000 0007 0000 000b 0000 0043  ...............C
+00000210: 0000 0073 4401 0000 7c01 7c00 5f00 7401  ...sD...|.|._.t.
+00000220: a002 7403 a004 a100 7c00 6a00 6a05 a102  ..t.....|.j.j...
+00000230: 5c02 7d04 7d05 7403 6a06 a007 6401 a101  \.}.}.t.j...d...
+00000240: 731a 7403 a008 6401 a101 0100 7401 6a09  s.t...d.....t.j.
+00000250: 6401 7c02 7c03 6402 6403 6404 6702 6405  d.|.|.d.d.d.g.d.
+00000260: 7c01 6a05 a00a 6406 6407 a102 a00b a100  |.j...d.d.......
+00000270: 9b00 6408 9d03 6701 6409 8d06 0100 7c00  ..d...g.d.....|.
+00000280: 6a00 6a0c 7246 740d 640a 7c01 6a05 a00a  j.j.rFt.d.|.j...
+00000290: 6406 6407 a102 a00b a100 9b00 640b 9d03  d.d.........d...
+000002a0: 8301 0100 7c00 6a00 6a0e 7c00 6a00 6a0f  ....|.j.j.|.j.j.
+000002b0: 7050 7c00 6a00 6a10 4000 7257 7401 a011  pP|.j.j.@.rWt...
+000002c0: a100 7d06 6e02 6400 7d06 7c00 6a00 6a12  ..}.n.d.}.|.j.j.
+000002d0: 726a 7c00 6a00 6a0c 7265 740d 640c 8301  rj|.j.j.ret.d...
+000002e0: 0100 7413 a014 7c04 a101 0100 7c00 6a00  ..t...|.....|.j.
+000002f0: 6a15 7280 7c00 6a00 6a0c 7276 740d 640d  j.r.|.j.j.rvt.d.
+00000300: 8301 0100 7401 a016 640e a101 0100 7417  ....t...d.....t.
+00000310: a014 7c04 a101 0100 7c00 6a00 6a0f 728a  ..|.....|.j.j.r.
+00000320: 7418 a019 7c04 7c06 a102 0100 7c00 6a00  t...|.|.....|.j.
+00000330: 6a10 7294 741a a019 7c04 7c06 a102 0100  j.r.t...|.|.....
+00000340: 7c06 72a0 7c06 a01b a100 0100 7c06 a01c  |.r.|.......|...
+00000350: a100 0100 6400 5300 6400 5300 290f 4e72  ....d.S.d.S.).Nr
+00000360: 0b00 0000 5a0a 6669 6775 7265 5f6c 6f67  ....Z.figure_log
+00000370: da07 5061 7273 696e 67da 0850 6c6f 7474  ..Parsing..Plott
+00000380: 696e 677a 1964 6174 615f 7573 6564 5f66  ingz.data_used_f
+00000390: 6f72 5f66 6967 7572 6573 203d 2022 fa01  or_figures = "..
+000003a0: 20da 015f fa01 2229 03da 0f6e 6577 5f63   .._..")...new_c
+000003b0: 6f6e 6669 675f 6e61 6d65 da11 7265 6c65  onfig_name..rele
+000003c0: 7661 6e74 5f73 6563 7469 6f6e 73da 0f61  vant_sections..a
+000003d0: 6464 6974 696f 6e61 6c5f 696e 666f 7a07  dditional_infoz.
+000003e0: 0a55 7369 6e67 207a 1820 6461 7461 2074  .Using z. data t
+000003f0: 6f20 6372 6561 7465 2066 6967 7572 6573  o create figures
+00000400: 2e7a 1c0a 2d2d 2d20 4272 6169 6e20 6772  .z..--- Brain gr
+00000410: 6964 2063 7265 6174 696f 6e20 2d2d 2d7a  id creation ---z
+00000420: 1d0a 2d2d 2d20 5669 6f6c 696e 2070 6c6f  ..--- Violin plo
+00000430: 7420 6372 6561 7469 6f6e 202d 2d2d 7a14  t creation ---z.
+00000440: 4669 6775 7265 732f 5669 6f6c 696e 5f70  Figures/Violin_p
+00000450: 6c6f 7473 291d da06 636f 6e66 6967 720a  lots)...configr.
+00000460: 0000 00da 1572 6561 645f 636f 6d62 696e  .....read_combin
+00000470: 6564 5f72 6573 756c 7473 da02 6f73 da06  ed_results..os..
+00000480: 6765 7463 7764 da0e 6176 6572 6167 696e  getcwd..averagin
+00000490: 675f 7479 7065 da04 7061 7468 da06 6578  g_type..path..ex
+000004a0: 6973 7473 da08 6d61 6b65 6469 7273 da0b  ists..makedirs..
+000004b0: 7361 7665 5f63 6f6e 6669 67da 0772 6570  save_config..rep
+000004c0: 6c61 6365 da05 6c6f 7765 72da 0776 6572  lace..lower..ver
+000004d0: 626f 7365 da05 7072 696e 74da 146d 756c  bose..print..mul
+000004e0: 7469 636f 7265 5f70 726f 6365 7373 696e  ticore_processin
+000004f0: 67da 136d 616b 655f 6f6e 655f 7265 6769  g..make_one_regi
+00000500: 6f6e 5f66 6967 da0e 6d61 6b65 5f68 6973  on_fig..make_his
+00000510: 746f 6772 616d da15 7374 6172 745f 7072  togram..start_pr
+00000520: 6f63 6573 7369 6e67 5f70 6f6f 6cda 106d  ocessing_pool..m
+00000530: 616b 655f 6272 6169 6e5f 7461 626c 65da  ake_brain_table.
+00000540: 0942 7261 696e 4772 6964 da04 6d61 6b65  .BrainGrid..make
+00000550: da10 6d61 6b65 5f76 696f 6c69 6e5f 706c  ..make_violin_pl
+00000560: 6f74 da12 6368 6563 6b5f 616e 645f 6d61  ot..check_and_ma
+00000570: 6b65 5f64 6972 da0a 5669 6f6c 696e 506c  ke_dir..ViolinPl
+00000580: 6f74 da08 4261 7263 6861 7274 da05 7365  ot..Barchart..se
+00000590: 7475 70da 0948 6973 746f 6772 616d da05  tup..Histogram..
+000005a0: 636c 6f73 65da 046a 6f69 6e29 07da 0363  close..join)...c
+000005b0: 6c73 da03 6366 67da 0b63 6f6e 6669 675f  ls..cfg..config_
+000005c0: 7061 7468 da0f 636f 6e66 6967 5f66 696c  path..config_fil
+000005d0: 656e 616d 65da 1363 6f6d 6269 6e65 645f  ename..combined_
+000005e0: 7265 7375 6c74 735f 6466 720f 0000 00da  results_dfr.....
+000005f0: 0470 6f6f 6ca9 0072 3600 0000 fa52 2f55  .pool..r6....R/U
+00000600: 7365 7273 2f6c 7078 6568 3130 2f44 6f63  sers/lpxeh10/Doc
+00000610: 756d 656e 7473 2f52 6570 6f73 6974 6f72  uments/Repositor
+00000620: 6965 732f 664d 5249 5f52 4f49 5f61 6e61  ies/fMRI_ROI_ana
+00000630: 6c79 7369 735f 746f 6f6c 2f66 5241 542f  lysis_tool/fRAT/
+00000640: 7574 696c 732f 6669 6775 7265 732e 7079  utils/figures.py
+00000650: da0c 6d61 6b65 5f66 6967 7572 6573 1c00  ..make_figures..
+00000660: 0000 7346 0000 0006 0218 020c 020a 010a  ..sF............
+00000670: 0202 0102 0102 0102 ff02 0210 0108 ff06  ................
+00000680: fc08 071e 0118 020a 0104 0208 0208 0108  ................
+00000690: 010a 0208 0208 0108 010a 020a 0108 020c  ................
+000006a0: 0108 020c 0104 0208 010c 0104 fe7a 1446  .............z.F
+000006b0: 6967 7572 6573 2e6d 616b 655f 6669 6775  igures.make_figu
+000006c0: 7265 7363 0300 0000 0000 0000 0000 0000  resc............
+000006d0: 0600 0000 0200 0000 4300 0000 734a 0000  ........C...sJ..
+000006e0: 007c 01a0 00a1 007d 037c 036a 017d 047c  .|.....}.|.j.}.|
+000006f0: 0264 016b 0272 127c 0464 0219 00a0 02a1  .d.k.r.|.d......
+00000700: 007d 056e 0a7c 0264 036b 0272 1c7c 0464  .}.n.|.d.k.r.|.d
+00000710: 0219 00a0 03a1 007d 0567 007c 05a2 017c  .......}.g.|...|
+00000720: 0091 0152 007d 057c 0553 0029 044e da05  ...R.}.|.S.).N..
+00000730: 7861 7869 7372 0100 0000 da05 7961 7869  xaxisr......yaxi
+00000740: 7329 04da 0464 7261 77da 0461 7865 73da  s)...draw..axes.
+00000750: 0867 6574 5f78 6c69 6dda 0867 6574 5f79  .get_xlim..get_y
+00000760: 6c69 6d29 06da 0774 6869 7372 6f69 da06  lim)...thisroi..
+00000770: 6669 6775 7265 da04 6178 6973 da03 6669  figure..axis..fi
+00000780: 6772 3c00 0000 da03 6c69 6d72 3600 0000  gr<.....limr6...
+00000790: 7236 0000 0072 3700 0000 da0f 6669 6e64  r6...r7.....find
+000007a0: 5f61 7869 735f 6c69 6d69 744b 0000 0073  _axis_limitK...s
+000007b0: 1000 0000 0803 0601 0802 0e01 0802 0c01  ................
+000007c0: 0e02 0402 7a17 4669 6775 7265 732e 6669  ....z.Figures.fi
+000007d0: 6e64 5f61 7869 735f 6c69 6d69 7463 0500  nd_axis_limitc..
+000007e0: 0000 0000 0000 0000 0000 0800 0000 0a00  ................
+000007f0: 0000 4300 0000 73e4 0000 0067 0064 01a2  ..C...s....g.d..
+00000800: 017d 057c 01a0 0064 0264 03a1 027d 017c  .}.|...d.d...}.|
+00000810: 0544 005d 0b5c 027d 067d 0774 01a0 027c  .D.].\.}.}.t...|
+00000820: 067c 077c 01a1 037d 0171 0c74 03a0 0464  .|.|...}.q.t...d
+00000830: 047c 03a0 05a1 009b 0064 057c 029b 0064  .|.......d.|...d
+00000840: 069d 05a1 0101 007c 006a 0664 047c 03a0  .......|.j.d.|..
+00000850: 05a1 009b 0064 057c 029b 0064 067c 019b  .....d.|...d.|..
+00000860: 0064 077c 039b 0064 089d 097c 046a 077c  .d.|...d...|.j.|
+00000870: 046a 0764 0914 0064 0a64 0a64 0b8d 0501  .j.d...d.d.d....
+00000880: 007c 006a 0664 047c 03a0 05a1 009b 0064  .|.j.d.|.......d
+00000890: 057c 029b 0064 067c 019b 0064 077c 039b  .|...d.|...d.|..
+000008a0: 0064 0c9d 097c 046a 077c 046a 0764 0914  .d...|.j.|.j.d..
+000008b0: 0064 0a64 0a64 0b8d 0501 007c 046a 0872  .d.d.d.....|.j.r
+000008c0: 7074 0964 0d7c 019b 0064 077c 039b 0064  pt.d.|...d.|...d
+000008d0: 089d 0583 0101 0064 0053 0064 0053 0029  .......d.S.d.S.)
+000008e0: 0e4e 2903 2902 7a0a 5c28 5b5e 2829 5d2a  .N).).z.\([^()]*
+000008f0: 5c29 da00 2902 7a0c 5b5e 612d 7a41 2d5a  \)..).z.[^a-zA-Z
+00000900: 5c64 3a5d 720f 0000 0029 027a 055f 7b32  \d:]r....).z._{2
+00000910: 2c7d 720f 0000 00fa 0127 7245 0000 007a  ,}r......'rE...z
+00000920: 0846 6967 7572 6573 2f7a 0273 2ffa 012f  .Figures/z.s/../
+00000930: 720f 0000 00fa 042e 706e 67e9 0300 0000  r.......png.....
+00000940: 46a9 04da 0668 6569 6768 74da 0577 6964  F....height..wid
+00000950: 7468 721f 0000 005a 096c 696d 6974 7369  thr....Z.limitsi
+00000960: 7a65 fa04 2e73 7667 7a06 5361 7665 6420  ze...svgz.Saved 
+00000970: 290a 721d 0000 00da 0272 65da 0373 7562  ).r......re..sub
+00000980: 720a 0000 0072 2900 0000 da05 7469 746c  r....r).....titl
+00000990: 65da 0473 6176 65da 0a70 6c6f 745f 7363  e..save..plot_sc
+000009a0: 616c 6572 1f00 0000 7220 0000 0029 0872  aler....r ...).r
+000009b0: 4000 0000 723f 0000 00da 0666 6f6c 6465  @...r?.....folde
+000009c0: 725a 0a63 6861 7274 5f74 7970 6572 1400  rZ.chart_typer..
+000009d0: 0000 da0c 7265 706c 6163 656d 656e 7473  ....replacements
+000009e0: da03 6f6c 64da 036e 6577 7236 0000 0072  ..old..newr6...r
+000009f0: 3600 0000 7237 0000 00da 0b66 6967 7572  6...r7.....figur
+00000a00: 655f 7361 7665 5b00 0000 7320 0000 0008  e_save[...s ....
+00000a10: 030c 050c 0110 011c 0224 010c 0104 0106  .........$......
+00000a20: fe24 040c 0104 0106 fe06 041a 0104 ff7a  .$.............z
+00000a30: 1346 6967 7572 6573 2e66 6967 7572 655f  .Figures.figure_
+00000a40: 7361 7665 6304 0000 0000 0000 0000 0000  savec...........
+00000a50: 0010 0000 0009 0000 0043 0000 0073 cc01  .........C...s..
+00000a60: 0000 7400 a001 a100 7d04 7c03 6401 6b02  ..t.....}.|.d.k.
+00000a70: 7217 7402 7403 6400 6700 7c00 6a04 a201  r.t.t.d.g.|.j...
+00000a80: 6402 9101 6403 9101 8302 8301 7d05 6e0c  d...d.......}.n.
+00000a90: 7402 7403 6400 7c00 6a05 7c00 6a06 6402  t.t.d.|.j.|.j.d.
+00000aa0: 6703 8302 8301 7d05 7c01 4400 5d96 7d06  g.....}.|.D.].}.
+00000ab0: 7407 7c06 6404 8302 8f10 7d07 7408 a009  t.|.d.....}.t...
+00000ac0: 740a a00b 7c07 a101 a101 7d08 5700 6400  t...|.....}.W.d.
+00000ad0: 0400 0400 8303 0100 6e08 3100 733f 7701  ........n.1.s?w.
+00000ae0: 0100 0100 0100 5900 0100 7a09 7c08 6a0c  ......Y...z.|.j.
+00000af0: 6405 6406 6702 1900 7d08 5700 6e09 0400  d.d.g...}.W.n...
+00000b00: 740d 7956 0100 0100 0100 5900 6e01 7700  t.yV......Y.n.w.
+00000b10: 6700 6407 a201 7d09 740e 6a0f a010 7c06  g.d...}.t.j...|.
+00000b20: a101 7d0a 7c09 4400 5d09 7d0b 7c0a a011  ..}.|.D.].}.|...
+00000b30: 7c0b a101 6408 1900 7d0a 7163 7c02 6a0c  |...d...}.qc|.j.
+00000b40: 7c02 6402 1900 6a12 a013 a100 7c0a a013  |.d...j.....|...
+00000b50: a100 6b02 1900 7d0c 7c0c 6a14 6a12 a013  ..k...}.|.j.j...
+00000b60: a100 7c0c 5f14 7a12 7c05 4400 5d0d 7d0d  ..|._.z.|.D.].}.
+00000b70: 7c0c 7c0d a013 a100 1900 6a15 6408 1900  |.|.......j.d...
+00000b80: 7c08 7c0d 3c00 7185 5700 6e11 0400 740d  |.|.<.q.W.n...t.
+00000b90: 799d 0100 0100 0100 5900 6e09 0400 7416  y.......Y.n...t.
+00000ba0: 79a5 0100 0100 0100 5900 7125 7700 7c03  y.......Y.q%w.|.
+00000bb0: 6401 6b02 72b4 7417 a018 6409 7c06 a102  d.k.r.t...d.|...
+00000bc0: 6408 1900 7c08 6403 3c00 7400 a019 7c04  d...|.d.<.t...|.
+00000bd0: 7c08 6702 a101 7d04 7125 7c04 6a15 6408  |.g...}.q%|.j.d.
+00000be0: 6400 640a 8503 1900 6a1a 7c05 640b 640c  d.d.....j.|.d.d.
+00000bf0: 640d 8d03 7d0e 7c04 6a15 640e 6400 640a  d...}.|.j.d.d.d.
+00000c00: 8503 1900 6a1a 7c05 640b 640c 640d 8d03  ....j.|.d.d.d...
+00000c10: 7d0f 7c0f 640c 1900 7c0e 640f 3c00 7c0e  }.|.d...|.d.<.|.
+00000c20: 6a1b 6410 6411 8d01 0100 7c0e 5300 2912  j.d.d.....|.S.).
+00000c30: 4eda 0a73 7461 7469 7374 6963 73da 0946  N..statistics..F
+00000c40: 696c 655f 6e61 6d65 da07 7375 626a 6563  ile_name..subjec
+00000c50: 74da 0172 da04 4d65 616e da06 566f 7865  t..r..Mean..Voxe
+00000c60: 6c73 2903 da03 5f70 73da 045f 7261 777a  ls)..._ps.._rawz
+00000c70: 052e 6a73 6f6e 7201 0000 007a 0a73 7562  ..jsonr....z.sub
+00000c80: 2d5b 302d 395d 2ae9 0200 0000 da03 524f  -[0-9]*.......RO
+00000c90: 49da 0b76 6f78 656c 5f76 616c 7565 2903  I..voxel_value).
+00000ca0: da07 6964 5f76 6172 73da 0876 6172 5f6e  ..id_vars..var_n
+00000cb0: 616d 65da 0a76 616c 7565 5f6e 616d 6572  ame..value_namer
+00000cc0: 0900 0000 5a0c 766f 7865 6c5f 616d 6f75  ....Z.voxel_amou
+00000cd0: 6e74 5429 01da 0769 6e70 6c61 6365 291c  ntT)...inplace).
+00000ce0: da02 7064 da09 4461 7461 4672 616d 65da  ..pd..DataFrame.
+00000cf0: 046c 6973 74da 0666 696c 7465 72da 0f70  .list..filter..p
+00000d00: 6172 616d 6574 6572 5f64 6963 7431 da15  arameter_dict1..
+00000d10: 6869 7374 6f67 7261 6d5f 6669 675f 785f  histogram_fig_x_
+00000d20: 6661 6365 74da 1568 6973 746f 6772 616d  facet..histogram
+00000d30: 5f66 6967 5f79 5f66 6163 6574 da04 6f70  _fig_y_facet..op
+00000d40: 656e 720a 0000 00da 1164 6963 745f 746f  enr......dict_to
+00000d50: 5f64 6174 6166 7261 6d65 da04 6a73 6f6e  _dataframe..json
+00000d60: da04 6c6f 6164 da03 6c6f 63da 084b 6579  ..load..loc..Key
+00000d70: 4572 726f 7272 1600 0000 7219 0000 00da  Errorr....r.....
+00000d80: 0862 6173 656e 616d 65da 0672 7370 6c69  .basename..rspli
+00000d90: 74da 0373 7472 721e 0000 00da 0763 6f6c  t..strr......col
+00000da0: 756d 6e73 da04 696c 6f63 da0a 496e 6465  umns..iloc..Inde
+00000db0: 7845 7272 6f72 724e 0000 00da 0766 696e  xErrorrN.....fin
+00000dc0: 6461 6c6c da06 636f 6e63 6174 da04 6d65  dall..concat..me
+00000dd0: 6c74 da06 6472 6f70 6e61 2910 7214 0000  lt..dropna).r...
+00000de0: 00da 056a 736f 6e73 da0b 636f 6d62 696e  ...jsons..combin
+00000df0: 6564 5f64 66da 0964 6174 615f 7479 7065  ed_df..data_type
+00000e00: da0f 636f 6d62 696e 6564 5f72 6177 5f64  ..combined_raw_d
+00000e10: 66da 0e73 6967 6e69 665f 636f 6c75 6d6e  f..signif_column
+00000e20: 73da 096a 736f 6e5f 6669 6c65 da01 665a  s..json_file..fZ
+00000e30: 0c63 7572 7265 6e74 5f6a 736f 6e5a 0a64  .current_jsonZ.d
+00000e40: 656c 696d 6574 6572 73da 0e6a 736f 6e5f  elimeters..json_
+00000e50: 6669 6c65 5f6e 616d 655a 0964 656c 696d  file_nameZ.delim
+00000e60: 6574 6572 5a12 636f 6d62 696e 6564 5f64  eterZ.combined_d
+00000e70: 665f 7365 6172 6368 da06 636f 6c75 6d6e  f_search..column
+00000e80: 5a09 6d65 616e 5f64 6174 615a 0a76 6f78  Z.mean_dataZ.vox
+00000e90: 656c 5f64 6174 6172 3600 0000 7236 0000  el_datar6...r6..
+00000ea0: 0072 3700 0000 da1a 6c6f 6164 5f61 6e64  .r7.....load_and
+00000eb0: 5f72 6573 7472 7563 7475 7265 5f6a 736f  _restructure_jso
+00000ec0: 6e73 7300 0000 734c 0000 0008 0208 051e  nss...sL........
+00000ed0: 010e 0202 0108 ff08 030c 0112 011c ff02  ................
+00000ee0: 0312 010c 0104 0102 ff08 030c 0108 0210  ................
+00000ef0: 011c 030e 0102 0208 0118 0104 ff0c 0204  ................
+00000f00: 010c 0104 0102 ff08 0314 0110 021c 031c  ................
+00000f10: 010c 020c 0104 027a 2246 6967 7572 6573  .......z"Figures
+00000f20: 2e6c 6f61 645f 616e 645f 7265 7374 7275  .load_and_restru
+00000f30: 6374 7572 655f 6a73 6f6e 7329 0ada 085f  cture_jsons)..._
+00000f40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000f50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000f60: 5f72 1400 0000 da0b 636c 6173 736d 6574  _r......classmet
+00000f70: 686f 6472 3800 0000 da0c 7374 6174 6963  hodr8.....static
+00000f80: 6d65 7468 6f64 7244 0000 0072 5700 0000  methodrD...rW...
+00000f90: 7287 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00000fa0: 3600 0000 7237 0000 0072 0b00 0000 1900  6...r7...r......
+00000fb0: 0000 7314 0000 0008 0004 0102 020a 0102  ..s.............
+00000fc0: 2e0a 0102 0f0a 0102 170e 0172 0b00 0000  ...........r....
+00000fd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000fe0: 0003 0000 0040 0000 0073 6000 0000 6500  .....@...s`...e.
+00000ff0: 5a01 6400 5a02 6503 6401 6402 8400 8301  Z.d.Z.e.d.d.....
+00001000: 5a04 6503 6403 6404 8400 8301 5a05 6503  Z.e.d.d.....Z.e.
+00001010: 6405 6406 8400 8301 5a06 6503 6407 6408  d.d.....Z.e.d.d.
+00001020: 8400 8301 5a07 6503 6409 640a 8400 8301  ....Z.e.d.d.....
+00001030: 5a08 6503 640b 640c 8400 8301 5a09 650a  Z.e.d.d.....Z.e.
+00001040: 640d 640e 8400 8301 5a0b 640f 5300 2910  d.d.....Z.d.S.).
+00001050: 7226 0000 0063 0200 0000 0000 0000 0000  r&...c..........
+00001060: 0000 0a00 0000 0800 0000 4300 0000 73f6  ..........C...s.
+00001070: 0000 0074 00a0 01a1 009b 0064 019d 027d  ...t.......d...}
+00001080: 0274 02a0 037c 02a1 0101 0074 02a0 0374  .t...|.....t...t
+00001090: 00a0 01a1 009b 0064 029d 02a1 0101 007c  .......d.......|
+000010a0: 006a 046a 0564 036b 0272 257c 006a 046a  .j.j.d.k.r%|.j.j
+000010b0: 0664 0319 007d 0364 047d 046e 087c 006a  .d...}.d.}.n.|.j
+000010c0: 046a 0664 0519 007d 0364 067d 047c 0344  .j.d...}.d.}.|.D
+000010d0: 005d 497d 0574 0764 077c 049b 0064 087c  .]I}.t.d.|...d.|
+000010e0: 059b 0064 099d 0583 0173 3d71 2f74 02a0  ...d.....s=q/t..
+000010f0: 0374 00a0 01a1 009b 0064 0a7c 059b 009d  .t.......d.|....
+00001100: 03a1 0101 0064 0b7c 059b 0064 0c9d 0364  .....d.|...d...d
+00001110: 0b7c 059b 0064 0d9d 0367 027d 067c 0644  .|...d...g.}.|.D
+00001120: 005d 187d 077c 00a0 087c 017c 077c 057c  .].}.|...|.|.|.|
+00001130: 04a1 047d 087c 0844 005d 0b7d 0974 02a0  ...}.|.D.].}.t..
+00001140: 097c 0974 00a0 01a1 007c 02a1 0301 0071  .|.t.....|.....q
+00001150: 6371 577c 006a 046a 0a72 7874 0b64 0e83  cqW|.j.j.rxt.d..
+00001160: 0101 0071 2f64 0053 0029 0f4e 7a15 2f46  ...q/d.S.).Nz./F
+00001170: 6967 7572 6573 2f42 7261 696e 5f69 6d61  igures/Brain_ima
+00001180: 6765 737a 142f 4669 6775 7265 732f 4272  gesz./Figures/Br
+00001190: 6169 6e5f 6772 6964 737a 1053 6573 7369  ain_gridsz.Sessi
+000011a0: 6f6e 2061 7665 7261 6765 645a 1853 6573  on averagedZ.Ses
+000011b0: 7369 6f6e 5f61 7665 7261 6765 645f 7265  sion_averaged_re
+000011c0: 7375 6c74 737a 1450 6172 7469 6369 7061  sultsz.Participa
+000011d0: 6e74 2061 7665 7261 6765 645a 1c50 6172  nt averagedZ.Par
+000011e0: 7469 6369 7061 6e74 5f61 7665 7261 6765  ticipant_average
+000011f0: 645f 7265 7375 6c74 73fa 124f 7665 7261  d_results..Overa
+00001200: 6c6c 2f4e 4946 5449 5f52 4f49 2f7a 022f  ll/NIFTI_ROI/z./
+00001210: 2ada 012a 7a15 2f46 6967 7572 6573 2f42  *..*z./Figures/B
+00001220: 7261 696e 5f67 7269 6473 2f72 0f00 0000  rain_grids/r....
+00001230: fa07 2e6e 6969 2e67 7a7a 195f 7769 7468  ...nii.gzz._with
+00001240: 696e 5f72 6f69 5f73 6361 6c65 642e 6e69  in_roi_scaled.ni
+00001250: 692e 677a da01 0a29 0c72 1600 0000 7217  i.gz...).r....r.
+00001260: 0000 0072 0a00 0000 7229 0000 0072 1400  ...r....r)...r..
+00001270: 0000 7218 0000 00da 1173 7461 7469 7374  ..r......statist
+00001280: 6963 5f6f 7074 696f 6e73 7203 0000 0072  ic_optionsr....r
+00001290: 2c00 0000 da09 6d6f 7665 5f66 696c 6572  ,.....move_filer
+000012a0: 1f00 0000 7220 0000 0029 0a72 3000 0000  ....r ...).r0...
+000012b0: 7234 0000 005a 1069 6e64 6976 5f62 7261  r4...Z.indiv_bra
+000012c0: 696e 735f 6469 72da 1073 7461 7469 7374  ins_dir..statist
+000012d0: 6963 5f6c 6162 656c 73da 0973 7562 666f  ic_labels..subfo
+000012e0: 6c64 6572 da09 7374 6174 6973 7469 635a  lder..statisticZ
+000012f0: 0f62 7261 696e 5f70 6c6f 745f 6578 7473  .brain_plot_exts
+00001300: da0e 6261 7365 5f65 7874 656e 7369 6f6e  ..base_extension
+00001310: da10 696e 6469 765f 6272 6169 6e5f 696d  ..indiv_brain_im
+00001320: 6773 da03 696d 6772 3600 0000 7236 0000  gs..imgr6...r6..
+00001330: 0072 3700 0000 7227 0000 00ab 0000 0073  .r7...r'.......s
+00001340: 3000 0000 0e02 0a01 1401 0c02 0c01 0601  0...............
+00001350: 0c02 0401 0802 1602 0201 1802 0a03 0a01  ................
+00001360: 04fe 0806 1001 0802 1401 02ff 0803 0801  ................
+00001370: 0280 04ec 7a0e 4272 6169 6e47 7269 642e  ....z.BrainGrid.
+00001380: 6d61 6b65 6305 0000 0000 0000 0000 0000  makec...........
+00001390: 0011 0000 000f 0000 0003 0000 0073 9001  .............s..
+000013a0: 0000 7400 6a01 a002 7400 6a01 a002 8800  ..t.j...t.j.....
+000013b0: a101 6401 1900 a101 6401 1900 6402 6400  ..d.....d...d.d.
+000013c0: 8502 1900 7d05 6700 7d06 7c01 6403 1900  ....}.g.}.|.d...
+000013d0: a003 a100 7d07 8700 8701 6602 6404 6405  ....}.....f.d.d.
+000013e0: 8408 7c07 4400 8301 7d07 7c00 a004 7c01  ..|.D...}.|...|.
+000013f0: a101 5c04 7d08 7d09 7d0a 7d0b 7c0b 6406  ..\.}.}.}.}.|.d.
+00001400: 7600 7234 6407 7d0c 6e04 7c0b 6408 1400  v.r4d.}.n.|.d...
+00001410: 7d0c 6409 7d0d 7c0c 7c0d 6602 7405 6a06  }.d.}.|.|.f.t.j.
+00001420: 640a 3c00 640b 7405 6a06 640c 3c00 640d  d.<.d.t.j.d.<.d.
+00001430: 7405 6a06 640e 3c00 7c03 640f 7600 725a  t.j.d.<.|.d.v.rZ
+00001440: 7c00 6a07 6a08 0400 7d0e 7d0f 7c00 6a07  |.j.j...}.}.|.j.
+00001450: 6a09 7d10 6e06 6400 0400 7d0e 7d0f 6401  j.}.n.d...}.}.d.
+00001460: 7d10 7c0f 6400 7500 7266 6700 7d0f 0900  }.|.d.u.rfg.}...
+00001470: 8800 6411 7c03 9b00 6412 9d03 6b03 7274  ..d.|...d...k.rt
+00001480: 6413 7d0e 6401 7d10 6e10 8800 6411 7c03  d.}.d.}.n...d.|.
+00001490: 9b00 6412 9d03 6b02 7284 7c0e 6400 7501  ..d...k.r.|.d.u.
+000014a0: 7284 7c05 6414 3700 7d05 7c00 6a07 6a0a  r.|.d.7.}.|.j.j.
+000014b0: 7290 740b 6415 7c05 9b00 6416 9d03 8301  r.t.d.|...d.....
+000014c0: 0100 7c00 a00c 7c05 8800 7c09 7c06 7c07  ..|...|...|.|.|.
+000014d0: 7c08 7c03 7c0e 7c0f 7c10 7c0b 7c0a 8801  |.|.|.|.|.|.|...
+000014e0: a10d 7d06 7c0e 6400 7501 72a8 0900 7c06  ..}.|.d.u.r...|.
+000014f0: 5300 740d 7c0f 8301 6417 1900 7d0f 7c0f  S.t.|...d...}.|.
+00001500: 6401 1900 7d0e 7c00 6a07 6a0a 72c7 740b  d...}.|.j.j.r.t.
+00001510: 6418 740e 7c0f 6401 1900 8301 9b00 6419  d.t.|.d.......d.
+00001520: 7c0f 6402 1900 9b00 641a 9d05 8301 0100  |.d.....d.......
+00001530: 7167 291b 4e72 0100 0000 7209 0000 0072  qg).Nr....r....r
+00001540: 5900 0000 6301 0000 0000 0000 0000 0000  Y...c...........
+00001550: 0002 0000 0008 0000 0013 0000 0073 2800  .............s(.
+00001560: 0000 6700 7c00 5d10 7d01 7400 6400 8801  ..g.|.].}.t.d...
+00001570: 9b00 6401 7c01 9b00 8800 9b00 9d05 8301  ..d.|...........
+00001580: 7202 7c01 9102 7102 5300 2902 728d 0000  r.|...q.S.).r...
+00001590: 0072 4700 0000 7202 0000 00a9 02da 022e  .rG...r.........
+000015a0: 30da 036a 736e a902 7296 0000 0072 9400  0..jsn..r....r..
+000015b0: 0000 7236 0000 0072 3700 0000 da0a 3c6c  ..r6...r7.....<l
+000015c0: 6973 7463 6f6d 703e d600 0000 7302 0000  istcomp>....s...
+000015d0: 0028 007a 2342 7261 696e 4772 6964 2e73  .(.z#BrainGrid.s
+000015e0: 6574 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c  etup.<locals>.<l
+000015f0: 6973 7463 6f6d 703e 2902 7209 0000 0072  istcomp>).r....r
+00001600: 6000 0000 e920 0000 00e9 1000 0000 e90f  `.... ..........
+00001610: 0000 007a 0e66 6967 7572 652e 6669 6773  ...z.figure.figs
+00001620: 697a 6567 7b14 ae47 e17a 843f 7a15 6669  izeg{..G.z.?z.fi
+00001630: 6775 7265 2e73 7562 706c 6f74 2e77 7370  gure.subplot.wsp
+00001640: 6163 65e7 9a99 9999 9999 b93f 7a15 6669  ace........?z.fi
+00001650: 6775 7265 2e73 7562 706c 6f74 2e68 7370  gure.subplot.hsp
+00001660: 6163 6529 0272 5c00 0000 da06 4d65 6469  ace).r\.....Medi
+00001670: 616e 5472 0f00 0000 728f 0000 00e9 6400  anTr....r.....d.
+00001680: 0000 da0b 5f73 616d 655f 7363 616c 657a  ...._same_scalez
+00001690: 0753 6176 696e 6720 7a07 2074 6162 6c65  .Saving z. table
+000016a0: 2ee9 ffff ffff 7a16 4d61 7869 6d75 6d20  ......z.Maximum 
+000016b0: 524f 4920 7661 6c75 6520 6f66 3a20 7a21  ROI value of: z!
+000016c0: 2073 6565 6e20 666f 7220 7061 7261 6d65   seen for parame
+000016d0: 7465 7220 636f 6d62 696e 6174 696f 6e3a  ter combination:
+000016e0: 207a 2d2e 2043 7265 6174 696e 6720 6669   z-. Creating fi
+000016f0: 6775 7265 7320 7769 7468 2074 6869 7320  gures with this 
+00001700: 636f 6c6f 7572 6261 7220 6c69 6d69 742e  colourbar limit.
+00001710: 290f 7216 0000 0072 1900 0000 da08 7370  ).r....r......sp
+00001720: 6c69 7465 7874 da06 756e 6971 7565 da0b  litext..unique..
+00001730: 7461 626c 655f 7365 7475 70da 0370 6c74  table_setup..plt
+00001740: da08 7263 5061 7261 6d73 7214 0000 00da  ..rcParamsr.....
+00001750: 1362 7261 696e 5f66 6967 5f76 616c 7565  .brain_fig_value
+00001760: 5f6d 6178 da13 6272 6169 6e5f 6669 675f  _max..brain_fig_
+00001770: 7661 6c75 655f 6d69 6e72 1f00 0000 7220  value_minr....r 
+00001780: 0000 00da 0a6d 616b 655f 7461 626c 65da  .....make_table.
+00001790: 0673 6f72 7465 64da 0572 6f75 6e64 2911  .sorted..round).
+000017a0: 7230 0000 00da 0264 6672 9600 0000 7295  r0.....dfr....r.
+000017b0: 0000 0072 9400 0000 da0e 6261 7365 5f65  ...r......base_e
+000017c0: 7874 5f63 6c65 616e 7297 0000 00da 0a6a  xt_cleanr......j
+000017d0: 736f 6e5f 6172 7261 79da 0f63 7269 7469  son_array..criti
+000017e0: 6361 6c5f 7061 7261 6d73 da09 6365 6c6c  cal_params..cell
+000017f0: 5f6e 756d 73da 0b79 5f61 7869 735f 7369  _nums..y_axis_si
+00001800: 7a65 da0b 785f 6178 6973 5f73 697a 655a  ze..x_axis_sizeZ
+00001810: 1262 7261 696e 5f74 6162 6c65 5f78 5f73  .brain_table_x_s
+00001820: 697a 655a 1262 7261 696e 5f74 6162 6c65  izeZ.brain_table
+00001830: 5f79 5f73 697a 65da 0476 6d61 78da 0c76  _y_size..vmax..v
+00001840: 6d61 785f 7374 6f72 6167 65da 0476 6d69  max_storage..vmi
+00001850: 6e72 3600 0000 729c 0000 0072 3700 0000  nr6...r....r7...
+00001860: 722c 0000 00ce 0000 0073 5200 0000 2402  r,.......sR...$.
+00001870: 0401 0c02 1403 1202 0802 0601 0802 0402  ................
+00001880: 0e02 0a01 0a01 0802 0c01 0a01 0802 0401  ................
+00001890: 0802 0401 0202 1001 0402 0601 1801 0801  ................
+000018a0: 0802 1001 0e02 0c01 0401 04fe 0804 0201  ................
+000018b0: 040c 0cf8 0801 0802 0201 1c01 04ff 02e8  ................
+000018c0: 7a0f 4272 6169 6e47 7269 642e 7365 7475  z.BrainGrid.setu
+000018d0: 7063 0e00 0000 0000 0000 0000 0000 1400  pc..............
+000018e0: 0000 0c00 0000 4300 0000 73ca 0100 0074  ......C...s....t
+000018f0: 007c 0583 0144 005d a75c 027d 0e7d 0f7c  .|...D.].\.}.}.|
+00001900: 00a0 017c 0f7c 017c 027c 087c 097c 0a7c  ...|.|.|.|.|.|.|
+00001910: 047c 077c 0da1 095c 037d 107d 047d 1174  .|.|...\.}.}.}.t
+00001920: 02a0 037c 10a1 017d 1274 04a0 057c 0c7c  ...|...}.t...|.|
+00001930: 0b7c 037c 0e19 0064 0117 00a1 0301 0074  .|.|...d.......t
+00001940: 04a0 067c 12a1 0101 0074 04a0 07a1 007d  ...|.....t.....}
+00001950: 137c 13a0 0867 00a1 0101 007c 136a 096a  .|...g.....|.j.j
+00001960: 0aa0 0b67 00a1 0101 007c 13a0 0c67 00a1  ...g.....|...g..
+00001970: 0101 007c 136a 096a 0da0 0b67 00a1 0101  ...|.j.j...g....
+00001980: 007c 0664 0219 0064 0319 007c 0e19 0064  .|.d...d...|...d
+00001990: 046b 0272 7a74 0e7c 0664 0519 0064 0619  .k.rzt.|.d...d..
+000019a0: 0083 0164 016b 0372 7a74 046a 0f7c 006a  ...d.k.rzt.j.|.j
+000019b0: 106a 1164 0717 0074 127c 0664 0519 0064  .j.d...t.|.d...d
+000019c0: 0619 007c 0664 0519 0064 0319 007c 0e19  ...|.d...d...|..
+000019d0: 0019 0083 0117 007c 006a 106a 1364 088d  .......|.j.j.d..
+000019e0: 0201 007c 0664 0519 0064 0319 007c 0e19  ...|.d...d...|..
+000019f0: 0064 046b 0272 ab74 0e7c 0664 0219 0064  .d.k.r.t.|.d...d
+00001a00: 0619 0083 0164 016b 0372 ab74 046a 147c  .....d.k.r.t.j.|
+00001a10: 006a 106a 1564 0717 0074 127c 0664 0219  .j.j.d...t.|.d..
+00001a20: 0064 0619 007c 0664 0219 0064 0319 007c  .d...|.d...d...|
+00001a30: 0e19 0019 0083 0117 007c 006a 106a 1364  .........|.j.j.d
+00001a40: 088d 0201 0071 047c 00a0 167c 067c 037c  .....q.|...|.|.|
+00001a50: 0b7c 0c7c 11a1 0501 007c 006a 106a 1772  .|.|.....|.j.j.r
+00001a60: bd74 04a0 18a1 0001 0074 046a 1964 097c  .t.......t.j.d.|
+00001a70: 079b 0064 0a7c 019b 0064 0b9d 057c 006a  ...d.|...d...|.j
+00001a80: 106a 1a64 0c64 0d8d 0301 0074 046a 1964  .j.d.d.....t.j.d
+00001a90: 097c 079b 0064 0a7c 019b 0064 0e9d 057c  .|...d.|...d...|
+00001aa0: 006a 106a 1a64 0c64 0d8d 0301 0074 04a0  .j.j.d.d.....t..
+00001ab0: 1ba1 0001 007c 0453 0029 0f4e 7209 0000  .....|.S.).Nr...
+00001ac0: 00da 0472 6f77 73da 056f 7264 6572 7201  ...rows..orderr.
+00001ad0: 0000 00da 0463 6f6c 73da 0676 616c 7565  .....cols..value
+00001ae0: 7372 0e00 0000 a901 da08 666f 6e74 7369  sr........fontsi
+00001af0: 7a65 7a14 4669 6775 7265 732f 4272 6169  zez.Figures/Brai
+00001b00: 6e5f 6772 6964 732f 7247 0000 0072 4800  n_grids/rG...rH.
+00001b10: 0000 da05 7469 6768 7429 02da 0364 7069  ....tight)...dpi
+00001b20: 5a0b 6262 6f78 5f69 6e63 6865 7372 4d00  Z.bbox_inchesrM.
+00001b30: 0000 291c da09 656e 756d 6572 6174 65da  ..)...enumerate.
+00001b40: 0f73 6176 655f 6272 6169 6e5f 696d 6773  .save_brain_imgs
+00001b50: da05 6d70 696d 67da 0669 6d72 6561 6472  ..mpimg..imreadr
+00001b60: a900 0000 da07 7375 6270 6c6f 74da 0669  ......subplot..i
+00001b70: 6d73 686f 77da 0367 6361 5a0a 7365 745f  mshow..gcaZ.set_
+00001b80: 7974 6963 6b73 723c 0000 0072 3a00 0000  yticksr<...r:...
+00001b90: 5a0e 7365 745f 7469 636b 6c61 6265 6c73  Z.set_ticklabels
+00001ba0: da0a 7365 745f 7874 6963 6b73 7239 0000  ..set_xticksr9..
+00001bb0: 00da 036c 656e 7250 0000 0072 1400 0000  ...lenrP...r....
+00001bc0: da16 6272 6169 6e5f 7461 626c 655f 636f  ..brain_table_co
+00001bd0: 6c5f 6c61 6265 6c73 7276 0000 00da 0e70  l_labelsrv.....p
+00001be0: 6c6f 745f 666f 6e74 5f73 697a 65da 0679  lot_font_size..y
+00001bf0: 6c61 6265 6cda 1662 7261 696e 5f74 6162  label..brain_tab
+00001c00: 6c65 5f72 6f77 5f6c 6162 656c 73da 156c  le_row_labels..l
+00001c10: 6162 656c 5f62 6c61 6e6b 5f63 656c 6c5f  abel_blank_cell_
+00001c20: 6178 6573 da12 6272 6169 6e5f 7469 6768  axes..brain_tigh
+00001c30: 745f 6c61 796f 7574 da0c 7469 6768 745f  t_layout..tight_
+00001c40: 6c61 796f 7574 da07 7361 7665 6669 67da  layout..savefig.
+00001c50: 0870 6c6f 745f 6470 6972 2e00 0000 2914  .plot_dpir....).
+00001c60: 7230 0000 0072 b100 0000 7296 0000 0072  r0...r....r....r
+00001c70: b400 0000 7297 0000 0072 b200 0000 72b3  ....r....r....r.
+00001c80: 0000 0072 9500 0000 72b7 0000 0072 b800  ...r....r....r..
+00001c90: 0000 72b9 0000 0072 b600 0000 72b5 0000  ..r....r....r...
+00001ca0: 0072 9400 0000 da08 6669 6c65 5f6e 756d  .r......file_num
+00001cb0: 7270 0000 005a 0962 7261 696e 5f69 6d67  rp...Z.brain_img
+00001cc0: da04 6469 6d73 7298 0000 00da 0261 7872  ..dimsr......axr
+00001cd0: 3600 0000 7236 0000 0072 3700 0000 72ad  6...r6...r7...r.
+00001ce0: 0000 000d 0100 0073 4a00 0000 1003 0a01  .......sJ.......
+00001cf0: 0801 0401 0afe 0a05 1601 0a01 0802 0a01  ................
+00001d00: 0e01 0a02 0e01 2802 0e01 1e01 02ff 0602  ......(.........
+00001d10: 06fe 2804 0e01 1e01 02ff 0602 06fe 0280  ..(.............
+00001d20: 1204 0802 0801 1a02 0201 06ff 1a02 0201  ................
+00001d30: 06ff 0802 0402 7a14 4272 6169 6e47 7269  ......z.BrainGri
+00001d40: 642e 6d61 6b65 5f74 6162 6c65 630a 0000  d.make_tablec...
+00001d50: 0000 0000 0000 0000 0012 0000 000b 0000  ................
+00001d60: 0043 0000 0073 2601 0000 7c01 9b00 6401  .C...s&...|...d.
+00001d70: 7c02 9b00 6402 9d04 7d0a 7c07 a000 7c0a  |...d...}.|...|.
+00001d80: a101 0100 6403 7c09 9b00 6404 7c01 9b00  ....d.|...d.|...
+00001d90: 7c03 9b00 9d05 7d0b 7c03 6401 7c08 9b00  |.....}.|.d.|...
+00001da0: 6405 9d03 6b02 723e 7c02 a001 6406 a101  d...k.r>|...d...
+00001db0: 6407 6b02 723e 7402 a003 7c0b a101 7d0c  d.k.r>t...|...}.
+00001dc0: 7c0c a004 a100 7d0c 7405 a006 7c0c a101  |.....}.t...|...
+00001dd0: 7d04 7c05 a000 7405 a006 7c0c a101 7c01  }.|...t...|...|.
+00001de0: 6602 a101 0100 7402 a003 7c0b a101 7d0d  f.....t...|...}.
+00001df0: 7402 a007 7405 a008 7c0d a004 a100 a101  t...t...|.......
+00001e00: 7c0d 6a09 7c0d 6a0a a103 7d0d 740b 6a0c  |.j.|.j...}.t.j.
+00001e10: 7c0d 6408 6408 6409 640a 7c06 7c04 7c00  |.d.d.d.d.|.|.|.
+00001e20: 6a0d 6a0e 7c00 6a0d 6a0f 6602 640b 640c  j.j.|.j.j.f.d.d.
+00001e30: 8d09 7d0e 7c0e 6a10 7c0a 7c00 6a0d 6a11  ..}.|.j.|.|.j.j.
+00001e40: 640d 8d02 0100 7c0e a012 a100 0100 7413  d.....|.......t.
+00001e50: a014 7c0a a101 8f0d 7d0f 7c0f 6a15 5c02  ..|.....}.|.j.\.
+00001e60: 7d10 7d11 5700 6400 0400 0400 8303 0100  }.}.W.d.........
+00001e70: 6e08 3100 7387 7701 0100 0100 0100 5900  n.1.s.w.......Y.
+00001e80: 0100 7c0a 7c07 7c10 7c11 6602 6603 5300  ..|.|.|.|.f.f.S.
+00001e90: 290e 4e72 0f00 0000 7248 0000 0072 8d00  ).Nr....rH...r..
+00001ea0: 0000 7247 0000 0072 8f00 0000 72a4 0000  ..rG...r....r...
+00001eb0: 0072 a500 0000 4654 da02 787a da07 696e  .r....FT..xz..in
+00001ec0: 6665 726e 6f29 085a 0a64 7261 775f 6372  ferno).Z.draw_cr
+00001ed0: 6f73 735a 0861 6e6e 6f74 6174 65da 0863  ossZ.annotate..c
+00001ee0: 6f6c 6f72 6261 725a 0c64 6973 706c 6179  olorbarZ.display
+00001ef0: 5f6d 6f64 6572 b900 0000 72b7 0000 005a  _moder....r....Z
+00001f00: 0a63 7574 5f63 6f6f 7264 73da 0463 6d61  .cut_coords..cma
+00001f10: 7029 0172 c100 0000 2916 da06 6170 7065  p).r....)...appe
+00001f20: 6e64 da04 6669 6e64 da03 6e69 6272 7100  nd..find..nibrq.
+00001f30: 0000 da09 6765 745f 6664 6174 61da 026e  ....get_fdata..n
+00001f40: 70da 066e 616e 6d61 78da 0b4e 6966 7469  p..nanmax..Nifti
+00001f50: 3149 6d61 6765 da0a 6e61 6e5f 746f 5f6e  1Image..nan_to_n
+00001f60: 756d da06 6166 6669 6e65 da06 6865 6164  um..affine..head
+00001f70: 6572 7205 0000 005a 0970 6c6f 745f 616e  err....Z.plot_an
+00001f80: 6174 7214 0000 00da 0d62 7261 696e 5f78  atr......brain_x
+00001f90: 5f63 6f6f 7264 da0d 6272 6169 6e5f 7a5f  _coord..brain_z_
+00001fa0: 636f 6f72 6472 d200 0000 72d3 0000 0072  coordr....r....r
+00001fb0: 2e00 0000 7207 0000 0072 6e00 0000 da04  ....r....rn.....
+00001fc0: 7369 7a65 2912 7230 0000 0072 7000 0000  size).r0...rp...
+00001fd0: 72b1 0000 0072 9600 0000 72b7 0000 0072  r....r....r....r
+00001fe0: b800 0000 72b9 0000 0072 9700 0000 7295  ....r....r....r.
+00001ff0: 0000 0072 9400 0000 5a08 706e 675f 7061  ...r....Z.png_pa
+00002000: 7468 5a0a 6e69 6674 695f 7061 7468 da05  thZ.nifti_path..
+00002010: 6272 6169 6e72 9800 0000 da04 706c 6f74  brainr......plot
+00002020: da02 696d 724c 0000 0072 4b00 0000 7236  ..imrL...rK...r6
+00002030: 0000 0072 3600 0000 7237 0000 0072 c300  ...r6...r7...r..
+00002040: 0000 3801 0000 732c 0000 0010 040a 0114  ..8...s,........
+00002050: 021e 020a 0208 010a 0214 040a 031c 0106  ................
+00002060: 0208 0104 010e 0102 0106 fc12 0508 010c  ................
+00002070: 020c 011c ff0e 037a 1942 7261 696e 4772  .......z.BrainGr
+00002080: 6964 2e73 6176 655f 6272 6169 6e5f 696d  id.save_brain_im
+00002090: 6773 6302 0000 0000 0000 0000 0000 0011  gsc.............
+000020a0: 0000 0008 0000 0043 0000 0073 be01 0000  .......C...s....
+000020b0: 6700 7d02 6700 7d03 7c00 6a00 6a01 4400  g.}.g.}.|.j.j.D.
+000020c0: 5d18 7d04 7402 7403 7c01 7c04 1900 a004  ].}.t.t.|.|.....
+000020d0: a100 8301 8301 7d05 6401 6402 8400 7c05  ......}.d.d...|.
+000020e0: 4400 8301 7d05 7c02 a005 7c05 a101 0100  D...}.|...|.....
+000020f0: 7108 7c02 7d06 7403 7c00 6a00 6a01 a006  q.|.}.t.|.j.j...
+00002100: a100 8301 7d07 7c00 6a00 6a07 6403 6701  ....}.|.j.j.d.g.
+00002110: 6700 6404 9c03 7c00 6a00 6a08 6403 6701  g.d...|.j.j.d.g.
+00002120: 6700 6404 9c03 6405 9c02 7d08 7c08 4400  g.d...d...}.|.D.
+00002130: 5d1a 7d09 7c08 7c09 1900 6406 1900 6407  ].}.|.|...d...d.
+00002140: 6b02 724b 7140 7c06 7c07 a009 7c08 7c09  k.rKq@|.|...|.|.
+00002150: 1900 6406 1900 a101 1900 7c08 7c09 1900  ..d.......|.|...
+00002160: 6408 3c00 7140 740a 7c08 6409 1900 6408  d.<.q@t.|.d...d.
+00002170: 1900 8301 7d0a 740a 7c08 640a 1900 6408  ....}.t.|.d...d.
+00002180: 1900 8301 7d0b 740b 7c01 640b 1900 a004  ....}.t.|.d.....
+00002190: a100 8301 4400 5d65 5c02 7d0c 7d0d 6700  ....D.]e\.}.}.g.
+000021a0: 7d0e 7c01 7c01 640b 1900 7c0d 6b02 1900  }.|.|.d...|.k...
+000021b0: 6a0c 6403 1900 7d0f 7c08 4400 5d40 7d09  j.d...}.|.D.]@}.
+000021c0: 7c08 7c09 1900 6408 1900 6403 6701 6b03  |.|...d...d.g.k.
+000021d0: 72b8 740d 7c0f 7c08 7c09 1900 6406 1900  r.t.|.|.|...d...
+000021e0: 1900 8301 7d10 7c08 7c09 1900 640c 1900  ....}.|.|...d...
+000021f0: a005 7c08 7c09 1900 6408 1900 a009 7c10  ..|.|...d.....|.
+00002200: a101 a101 0100 7c0e a005 7c08 7c09 1900  ......|...|.|...
+00002210: 6408 1900 a009 7c10 a101 a101 0100 7186  d.....|.......q.
+00002220: 7c08 7c09 1900 640c 1900 a005 6403 a101  |.|...d.....d...
+00002230: 0100 7c0e a005 6403 a101 0100 7186 7c03  ..|...d.....q.|.
+00002240: a005 740e a00f 7c0e 640d 1900 7c0e 6403  ..t...|.d...|.d.
+00002250: 1900 6602 7c0b 7c0a 6602 a102 a101 0100  ..f.|.|.f.......
+00002260: 7173 7c08 7c03 7c0b 7c0a 6604 5300 290e  qs|.|.|.|.f.S.).
+00002270: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00002280: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00002290: 007c 005d 067d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+000022a0: 0253 0072 3600 0000 2901 7276 0000 0029  .S.r6...).rv...)
+000022b0: 0272 9a00 0000 da05 7061 7261 6d72 3600  .r......paramr6.
+000022c0: 0000 7236 0000 0072 3700 0000 729d 0000  ..r6...r7...r...
+000022d0: 0064 0100 00f3 0200 0000 1400 7a29 4272  .d..........z)Br
+000022e0: 6169 6e47 7269 642e 7461 626c 655f 7365  ainGrid.table_se
+000022f0: 7475 702e 3c6c 6f63 616c 733e 2e3c 6c69  tup.<locals>.<li
+00002300: 7374 636f 6d70 3e72 0100 0000 2903 72eb  stcomp>r....).r.
+00002310: 0000 0072 bd00 0000 72bb 0000 0029 0272  ...r....r....).r
+00002320: bc00 0000 72ba 0000 0072 eb00 0000 7245  ....r....r....rE
+00002330: 0000 0072 bd00 0000 72bc 0000 0072 ba00  ...r....r....r..
+00002340: 0000 7259 0000 0072 bb00 0000 7209 0000  ..rY...r....r...
+00002350: 0029 1072 1400 0000 da0e 7061 7261 6d65  .).r......parame
+00002360: 7465 725f 6469 6374 72ae 0000 0072 6900  ter_dictr....ri.
+00002370: 0000 72a7 0000 0072 db00 0000 da04 6b65  ..r....r......ke
+00002380: 7973 da10 6272 6169 6e5f 7461 626c 655f  ys..brain_table_
+00002390: 636f 6c73 da10 6272 6169 6e5f 7461 626c  cols..brain_tabl
+000023a0: 655f 726f 7773 da05 696e 6465 7872 ca00  e_rows..indexr..
+000023b0: 0000 72c2 0000 0072 7800 0000 7276 0000  ..r....rx...rv..
+000023c0: 0072 df00 0000 da11 7261 7665 6c5f 6d75  .r......ravel_mu
+000023d0: 6c74 695f 696e 6465 7829 1172 3000 0000  lti_index).r0...
+000023e0: 72b0 0000 005a 0d75 6e69 7175 655f 7061  r....Z.unique_pa
+000023f0: 7261 6d73 72b4 0000 00da 036b 6579 da06  ramsr......key..
+00002400: 7061 7261 6d73 5a0b 706c 6f74 5f76 616c  paramsZ.plot_val
+00002410: 7565 735a 0b61 7869 735f 7469 746c 6573  uesZ.axis_titles
+00002420: 72b3 0000 0072 4100 0000 72b6 0000 0072  r....rA...r....r
+00002430: b500 0000 72d4 0000 00da 0966 696c 655f  ....r......file_
+00002440: 6e61 6d65 5a10 7465 6d70 5f6f 7264 6572  nameZ.temp_order
+00002450: 5f73 746f 7265 5a0d 6669 6c65 5f6e 616d  _storeZ.file_nam
+00002460: 655f 726f 775a 0a66 696c 655f 7061 7261  e_rowZ.file_para
+00002470: 6d72 3600 0000 7236 0000 0072 3700 0000  mr6...r6...r7...
+00002480: 72a8 0000 005d 0100 0073 4200 0000 0402  r....]...sB.....
+00002490: 0401 0c02 1401 0e01 0c01 0402 1001 1002  ................
+000024a0: 1001 06ff 0803 1001 0201 0202 1001 0eff  ................
+000024b0: 1003 1001 1802 0401 1601 0802 1201 1402  ................
+000024c0: 2002 1a01 1202 0c01 1602 0601 08ff 0c03   ...............
+000024d0: 7a15 4272 6169 6e47 7269 642e 7461 626c  z.BrainGrid.tabl
+000024e0: 655f 7365 7475 7063 0600 0000 0000 0000  e_setupc........
+000024f0: 0000 0000 0b00 0000 0700 0000 4300 0000  ............C...
+00002500: 7348 0100 0074 00a0 0164 017c 0564 0219  sH...t...d.|.d..
+00002510: 007c 0564 0319 0066 0264 04a1 037d 0674  .|.d...f.d...}.t
+00002520: 027c 0164 0519 0064 0619 0083 0144 005d  .|.d...d.....D.]
+00002530: 4c5c 027d 077d 0874 03a0 0464 027c 0766  L\.}.}.t...d.|.f
+00002540: 027c 047c 0366 02a1 027d 097c 097c 0276  .|.|.f...}.|.|.v
+00002550: 0172 6174 05a0 067c 047c 037c 0964 0317  .rat...|.|.|.d..
+00002560: 00a1 0301 0074 05a0 077c 06a1 0101 007c  .....t...|.....|
+00002570: 00a0 08a1 0001 0074 056a 097c 006a 0a6a  .......t.j.|.j.j
+00002580: 0b64 0717 007c 0817 007c 006a 0a6a 0c64  .d...|...|.j.j.d
+00002590: 088d 0201 007c 0964 026b 0272 6174 056a  .....|.d.k.rat.j
+000025a0: 0d7c 006a 0a6a 0e64 0717 007c 0164 0919  .|.j.j.d...|.d..
+000025b0: 0064 0619 0064 0219 0017 007c 006a 0a6a  .d...d.....|.j.j
+000025c0: 0c64 088d 0201 0071 1574 027c 0164 0919  .d.....q.t.|.d..
+000025d0: 0064 0619 0083 0144 005d 375c 027d 077d  .d.....D.]7\.}.}
+000025e0: 0a74 03a0 047c 0764 0266 027c 047c 0366  .t...|.d.f.|.|.f
+000025f0: 02a1 027d 097c 097c 0276 0172 a17c 0964  ...}.|.|.v.r.|.d
+00002600: 026b 0372 a174 05a0 067c 047c 037c 0964  .k.r.t...|.|.|.d
+00002610: 0317 00a1 0301 0074 05a0 077c 06a1 0101  .......t...|....
+00002620: 007c 00a0 08a1 0001 0074 056a 0d7c 006a  .|.......t.j.|.j
+00002630: 0a6a 0e64 0717 007c 0a17 007c 006a 0a6a  .j.d...|...|.j.j
+00002640: 0c64 088d 0201 0071 6a64 0053 0029 0a4e  .d.....qjd.S.).N
+00002650: da03 5247 4272 0100 0000 7209 0000 0029  ..RGBr....r....)
+00002660: 03e9 ff00 0000 72f7 0000 0072 f700 0000  ......r....r....
+00002670: 72bc 0000 0072 bd00 0000 720e 0000 0072  r....r....r....r
+00002680: be00 0000 72ba 0000 0029 0f72 0700 0000  ....r....).r....
+00002690: 7256 0000 0072 c200 0000 72df 0000 0072  rV...r....r....r
+000026a0: f200 0000 72a9 0000 0072 c600 0000 72c7  ....r....r....r.
+000026b0: 0000 00da 136d 616b 655f 6365 6c6c 5f69  .....make_cell_i
+000026c0: 6e76 6973 6962 6c65 7250 0000 0072 1400  nvisiblerP...r..
+000026d0: 0000 72cb 0000 0072 cc00 0000 72cd 0000  ..r....r....r...
+000026e0: 0072 ce00 0000 290b 7230 0000 0072 b300  .r....).r0...r..
+000026f0: 0000 72b4 0000 0072 b600 0000 72b5 0000  ..r....r....r...
+00002700: 0072 d500 0000 7298 0000 00da 0763 6f75  .r....r......cou
+00002710: 6e74 6572 5a07 785f 7469 746c 655a 0b68  nterZ.x_titleZ.h
+00002720: 6964 6465 6e5f 6365 6c6c 5a07 795f 7469  idden_cellZ.y_ti
+00002730: 746c 6572 3600 0000 7236 0000 0072 3700  tler6...r6...r7.
+00002740: 0000 72cf 0000 008b 0100 0073 2c00 0000  ..r........s,...
+00002750: 1a03 1802 1401 0802 1201 0a01 0801 1e02  ................
+00002760: 0802 1e01 0601 06ff 0280 1803 1401 1002  ................
+00002770: 1201 0a01 0801 1e02 0280 04f8 7a1f 4272  ............z.Br
+00002780: 6169 6e47 7269 642e 6c61 6265 6c5f 626c  ainGrid.label_bl
+00002790: 616e 6b5f 6365 6c6c 5f61 7865 7363 0000  ank_cell_axesc..
+000027a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000027b0: 0000 4300 0000 736c 0000 0074 00a0 01a1  ..C...sl...t....
+000027c0: 007d 007c 006a 02a0 03a1 00a0 0467 00a1  .}.|.j.......g..
+000027d0: 0101 007c 006a 02a0 05a1 00a0 0467 00a1  ...|.j.......g..
+000027e0: 0101 007c 006a 0664 0119 00a0 0764 02a1  ...|.j.d.....d..
+000027f0: 0101 007c 006a 0664 0319 00a0 0764 02a1  ...|.j.d.....d..
+00002800: 0101 007c 006a 0664 0419 00a0 0764 02a1  ...|.j.d.....d..
+00002810: 0101 007c 006a 0664 0519 00a0 0764 02a1  ...|.j.d.....d..
+00002820: 0101 0064 0053 0029 064e da04 6c65 6674  ...d.S.).N..left
+00002830: 46da 0572 6967 6874 da06 626f 7474 6f6d  F..right..bottom
+00002840: da03 746f 7029 0872 a900 0000 72c8 0000  ..top).r....r...
+00002850: 0072 3c00 0000 da09 6765 745f 7861 7869  .r<.....get_xaxi
+00002860: 735a 0973 6574 5f74 6963 6b73 da09 6765  sZ.set_ticks..ge
+00002870: 745f 7961 7869 735a 0673 7069 6e65 73da  t_yaxisZ.spines.
+00002880: 0b73 6574 5f76 6973 6962 6c65 2901 da05  .set_visible)...
+00002890: 6672 616d 6572 3600 0000 7236 0000 0072  framer6...r6...r
+000028a0: 3700 0000 72f8 0000 00a8 0100 0073 0e00  7...r........s..
+000028b0: 0000 0802 1001 1001 1001 1001 1001 1401  ................
+000028c0: 7a1d 4272 6169 6e47 7269 642e 6d61 6b65  z.BrainGrid.make
+000028d0: 5f63 656c 6c5f 696e 7669 7369 626c 654e  _cell_invisibleN
+000028e0: 290c 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
+000028f0: 0072 8b00 0000 7227 0000 0072 2c00 0000  .r....r'...r,...
+00002900: 72ad 0000 0072 c300 0000 72a8 0000 0072  r....r....r....r
+00002910: cf00 0000 728c 0000 0072 f800 0000 7236  ....r....r....r6
+00002920: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00002930: 0000 7226 0000 00aa 0000 0073 1e00 0000  ..r&.......s....
+00002940: 0800 0201 0a01 0222 0a01 023e 0a01 022a  ......."...>...*
+00002950: 0a01 0224 0a01 022d 0a01 021c 0e01 7226  ...$...-......r&
+00002960: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002970: 0000 0000 0300 0000 4000 0000 7318 0000  ........@...s...
+00002980: 0065 005a 0164 005a 0265 0364 0164 0284  .e.Z.d.Z.e.d.d..
+00002990: 0083 015a 0464 0353 0029 0472 2a00 0000  ...Z.d.S.).r*...
+000029a0: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
+000029b0: 0008 0000 0043 0000 0073 6402 0000 7400  .....C...sd...t.
+000029c0: a001 7c01 a101 7d02 7c02 7c02 6401 1900  ..|...}.|.|.d...
+000029d0: 6402 6b03 7c02 6401 1900 6403 6b03 4000  d.k.|.d...d.k.@.
+000029e0: 1900 7d02 7c02 7c02 6404 1900 6405 6b04  ..}.|.|.d...d.k.
+000029f0: 1900 7d02 7c00 6a02 6a03 6406 6b02 7338  ..}.|.j.j.d.k.s8
+00002a00: 7c00 6a02 6a04 6406 6b02 7338 7c02 a005  |.j.j.d.k.s8|...
+00002a10: 7c00 6a02 6a03 7c00 6a02 6a04 6702 a101  |.j.j.|.j.j.g...
+00002a20: a006 6407 6408 8400 a101 7d02 6e25 7c00  ..d.d.....}.n%|.
+00002a30: 6a02 6a03 6406 6b02 734b 7c02 a005 7c00  j.j.d.k.sK|...|.
+00002a40: 6a02 6a03 a101 a006 6409 6408 8400 a101  j.j.....d.d.....
+00002a50: 7d02 6e12 7c00 6a02 6a04 6406 6b02 735d  }.n.|.j.j.d.k.s]
+00002a60: 7c02 a005 7c00 6a02 6a04 a101 a006 640a  |...|.j.j.....d.
+00002a70: 6408 8400 a101 7d02 7c02 6a07 640b 640c  d.....}.|.j.d.d.
+00002a80: 8d01 7d02 640d 7c02 640e 3c00 640f 7d03  ..}.d.|.d.<.d.}.
+00002a90: 7408 6a09 7408 6a0a 640e 6410 6411 8d02  t.j.t.j.d.d.d...
+00002aa0: 6412 8d01 7d04 7408 6a09 7408 6a0a 640e  d...}.t.j.t.j.d.
+00002ab0: 6413 6411 8d02 6412 8d01 7d05 7408 a00b  d.d...d...}.t...
+00002ac0: 7c02 a101 7408 6a09 640e 6404 6414 8d02  |...t.j.d.d.d...
+00002ad0: 1700 7408 6a0c 7c05 640b 6415 7c00 6a02  ..t.j.|.d.d.|.j.
+00002ae0: 6a0d 6416 6417 8d05 1700 7408 6a0e 640f  j.d.d.....t.j.d.
+00002af0: 6405 7c00 6a02 6a0f 6416 6418 8d04 1700  d.|.j.j.d.d.....
+00002b00: 7408 a010 6419 641a a102 1700 7408 a011  t...d.d.....t...
+00002b10: 6405 6400 a102 1700 7408 a012 7c00 6a02  d.d.....t...|.j.
+00002b20: 6a13 a101 1700 7408 a014 6406 a101 1700  j.....t...d.....
+00002b30: 7408 6a15 7c00 6a02 6a04 9b00 641b 7c00  t.j.|.j.j...d.|.
+00002b40: 6a02 6a03 9b00 9d03 640b 641c 641d 8d03  j.j.....d.d.d...
+00002b50: 1700 7408 a016 a100 1700 7408 6a17 7408  ..t.......t.j.t.
+00002b60: 6a18 6a19 640d 641e 8d01 7408 6a18 6a19  j.j.d.d...t.j.j.
+00002b70: 6405 641e 8d01 7408 6a1a 641f 640f 6420  d.d...t.j.d.d.d 
+00002b80: 8d02 7408 a01b a100 7c00 6a02 6a1c 6421  ..t.....|.j.j.d!
+00002b90: 8d05 1700 7d06 7c00 6a02 6a1d 9001 7205  ....}.|.j.j...r.
+00002ba0: 7c00 6a02 6a1e 72ff 7c06 7408 6a1f 6422  |.j.j.r.|.t.j.d"
+00002bb0: 6405 6423 8d02 3700 7d06 6e06 7c06 7408  d.d#..7.}.n.|.t.
+00002bc0: a020 a100 3700 7d06 7c06 6a21 6424 7c00  . ..7.}.|.j!d$|.
+00002bd0: 6a02 6a22 7c00 6a02 6a22 6425 1400 6426  j.j"|.j.j"d%..d&
+00002be0: 6426 6427 8d05 0100 7c06 6a21 6428 7c00  d&d'....|.j!d(|.
+00002bf0: 6a02 6a22 7c00 6a02 6a22 6425 1400 6426  j.j"|.j.j"d%..d&
+00002c00: 6426 6427 8d05 0100 7c00 6a02 6a23 9001  d&d'....|.j.j#..
+00002c10: 7230 7424 6429 8301 0100 6400 5300 6400  r0t$d)....d.S.d.
+00002c20: 5300 292a 4e72 f100 0000 da07 4f76 6572  S.)*Nr......Over
+00002c30: 616c 6cfa 064e 6f20 524f 4972 5c00 0000  all..No ROIr\...
+00002c40: 7201 0000 0072 4500 0000 6301 0000 0000  r....rE...c.....
+00002c50: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
+00002c60: 0000 00f3 0c00 0000 7c00 a000 6401 6701  ........|...d.g.
+00002c70: a101 5300 a902 4e72 5c00 0000 a901 da0b  ..S...Nr\.......
+00002c80: 736f 7274 5f76 616c 7565 73a9 01da 0178  sort_values....x
+00002c90: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
+00002ca0: 083c 6c61 6d62 6461 3ebd 0100 00f3 0200  .<lambda>.......
+00002cb0: 0000 0c00 7a21 5669 6f6c 696e 506c 6f74  ....z!ViolinPlot
+00002cc0: 2e6d 616b 652e 3c6c 6f63 616c 733e 2e3c  .make.<locals>.<
+00002cd0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
+00002ce0: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
+00002cf0: 7204 0100 0072 0501 0000 7206 0100 0072  r....r....r....r
+00002d00: 0801 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00002d10: 0000 0072 0a01 0000 c001 0000 720b 0100  ...r........r...
+00002d20: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00002d30: 0000 0300 0000 5300 0000 7204 0100 0072  ......S...r....r
+00002d40: 0501 0000 7206 0100 0072 0801 0000 7236  ....r....r....r6
+00002d50: 0000 0072 3600 0000 7237 0000 0072 0a01  ...r6...r7...r..
+00002d60: 0000 c301 0000 720b 0100 0054 a901 da04  ......r....T....
+00002d70: 6472 6f70 7209 0000 00da 0863 6f6e 7374  dropr......const
+00002d80: 616e 7472 a100 0000 7a07 782b 7368 6966  antr....z.x+shif
+00002d90: 7429 015a 0b61 6674 6572 5f73 6361 6c65  t).Z.after_scale
+00002da0: 7208 0100 007a 0778 2d73 6869 6674 a902  r....z.x-shift..
+00002db0: 7209 0100 00da 0179 72fa 0000 0067 3333  r......yr....g33
+00002dc0: 3333 3333 e33f 2904 da05 6e61 5f72 6dda  3333.?)...na_rm.
+00002dd0: 0573 7479 6c65 da04 6669 6c6c 72e7 0000  .style..fillr...
+00002de0: 0029 0472 4c00 0000 5a0d 6f75 746c 6965  .).rL...Z.outlie
+00002df0: 725f 616c 7068 6172 1301 0000 72e7 0000  r_alphar....r...
+00002e00: 0067 9a99 9999 9999 d93f 6766 6666 6666  .g.......?gfffff
+00002e10: 66f6 3fda 017e da0a 6c61 6265 6c5f 626f  f.?..~..label_bo
+00002e20: 7468 a902 720d 0100 005a 086c 6162 656c  th..r....Z.label
+00002e30: 6c65 72a9 01da 0561 6c70 6861 da04 6772  ler....alpha..gr
+00002e40: 6179 a902 7213 0100 0072 1801 0000 2905  ay..r....r....).
+00002e50: da12 7061 6e65 6c5f 6772 6964 5f6d 616a  ..panel_grid_maj
+00002e60: 6f72 5f79 da12 7061 6e65 6c5f 6772 6964  or_y..panel_grid
+00002e70: 5f6d 616a 6f72 5f78 da10 7061 6e65 6c5f  _major_x..panel_
+00002e80: 6261 636b 6772 6f75 6e64 da0b 6178 6973  background..axis
+00002e90: 5f74 6578 745f 7872 c100 0000 677b 14ae  _text_xr....g{..
+00002ea0: 47e1 7aa4 3f29 0272 4c00 0000 724b 0000  G.z.?).rL...rK..
+00002eb0: 007a 2346 6967 7572 6573 2f56 696f 6c69  .z#Figures/Violi
+00002ec0: 6e5f 706c 6f74 732f 7669 6f6c 696e 706c  n_plots/violinpl
+00002ed0: 6f74 2e70 6e67 7249 0000 0046 724a 0000  ot.pngrI...FrJ..
+00002ee0: 007a 2346 6967 7572 6573 2f56 696f 6c69  .z#Figures/Violi
+00002ef0: 6e5f 706c 6f74 732f 7669 6f6c 696e 706c  n_plots/violinpl
+00002f00: 6f74 2e73 7667 7a12 5361 7665 6420 7669  ot.svgz.Saved vi
+00002f10: 6f6c 696e 2070 6c6f 7421 2925 da04 636f  olin plot!)%..co
+00002f20: 7079 da08 6465 6570 636f 7079 7214 0000  py..deepcopyr...
+00002f30: 00da 0a74 6162 6c65 5f63 6f6c 73da 0a74  ...table_cols..t
+00002f40: 6162 6c65 5f72 6f77 73da 0767 726f 7570  able_rows..group
+00002f50: 6279 da05 6170 706c 79da 0b72 6573 6574  by..apply..reset
+00002f60: 5f69 6e64 6578 da04 706c 746e da03 6165  _index..pltn..ae
+00002f70: 73da 0573 7461 6765 da06 6767 706c 6f74  s..stage..ggplot
+00002f80: 5a0b 6765 6f6d 5f76 696f 6c69 6eda 0d76  Z.geom_violin..v
+00002f90: 696f 6c69 6e5f 636f 6c6f 7572 5a0c 6765  iolin_colourZ.ge
+00002fa0: 6f6d 5f62 6f78 706c 6f74 da0e 626f 7870  om_boxplot..boxp
+00002fb0: 6c6f 745f 636f 6c6f 7572 da04 786c 696d  lot_colour..xlim
+00002fc0: da04 796c 696d 5a04 796c 6162 da0d 7461  ..ylimZ.ylab..ta
+00002fd0: 626c 655f 785f 6c61 6265 6c5a 0478 6c61  ble_x_labelZ.xla
+00002fe0: 62da 0a66 6163 6574 5f67 7269 64da 0974  b..facet_grid..t
+00002ff0: 6865 6d65 5f35 3338 da05 7468 656d 65da  heme_538..theme.
+00003000: 0674 6865 6d65 73da 0c65 6c65 6d65 6e74  .themes..element
+00003010: 5f6c 696e 65da 0c65 6c65 6d65 6e74 5f72  _line..element_r
+00003020: 6563 745a 0d65 6c65 6d65 6e74 5f62 6c61  ectZ.element_bla
+00003030: 6e6b 72d3 0000 00da 1076 696f 6c69 6e5f  nkr......violin_
+00003040: 7368 6f77 5f64 6174 61da 0d76 696f 6c69  show_data..violi
+00003050: 6e5f 6a69 7474 6572 5a0b 6765 6f6d 5f6a  n_jitterZ.geom_j
+00003060: 6974 7465 72da 0a67 656f 6d5f 706f 696e  itter..geom_poin
+00003070: 7472 5100 0000 7252 0000 0072 1f00 0000  trQ...rR...r....
+00003080: 7220 0000 0029 0772 3000 0000 5a07 6f72  r ...).r0...Z.or
+00003090: 6967 5f64 6672 b000 0000 da05 7368 6966  ig_dfr......shif
+000030a0: 74da 0b72 6967 6874 5f73 6869 6674 da0a  t..right_shift..
+000030b0: 6c65 6674 5f73 6869 6674 7240 0000 0072  left_shiftr@...r
+000030c0: 3600 0000 7236 0000 0072 3700 0000 7227  6...r6...r7...r'
+000030d0: 0000 00b4 0100 0073 7200 0000 0a02 1c02  .......sr.......
+000030e0: 1001 1802 2202 0c02 1a01 0c02 1801 0c02  ...."...........
+000030f0: 0802 0403 1602 1601 0802 0c01 02ff 1602  ................
+00003100: 02fe 1403 02fd 0a04 02fc 0a05 02fb 0c06  ................
+00003110: 02fa 0807 02f9 1a08 0201 04ff 02f8 060a  ................
+00003120: 02f6 100b 0c01 0c01 0601 0601 04fc 04f5  ................
+00003130: 0a11 0801 1401 0c02 0c02 0a01 0401 06fe  ................
+00003140: 0c04 0a01 0401 06fe 0a04 0c01 04ff 7a0f  ..............z.
+00003150: 5669 6f6c 696e 506c 6f74 2e6d 616b 654e  ViolinPlot.makeN
+00003160: 2905 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
+00003170: 0072 8b00 0000 7227 0000 0072 3600 0000  .r....r'...r6...
+00003180: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
+00003190: 2a00 0000 b301 0000 7306 0000 0008 0002  *.......s.......
+000031a0: 010e 0172 2a00 0000 6300 0000 0000 0000  ...r*...c.......
+000031b0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000031c0: 0073 2400 0000 6500 5a01 6400 5a02 6503  .s$...e.Z.d.Z.e.
+000031d0: 6401 6402 8400 8301 5a04 6505 6403 6404  d.d.....Z.e.d.d.
+000031e0: 8400 8301 5a06 6405 5300 2906 722b 0000  ....Z.d.S.).r+..
+000031f0: 0063 0300 0000 0000 0000 0000 0000 0700  .c..............
+00003200: 0000 0a00 0000 4300 0000 7350 0100 007c  ......C...sP...|
+00003210: 006a 006a 0164 016b 0272 0a74 0264 0283  .j.j.d.k.r.t.d..
+00003220: 0182 0174 03a0 0464 03a1 0101 0074 057c  ...t...d.....t.|
+00003230: 0164 0419 00a0 06a1 0083 017d 0374 036a  .d.........}.t.j
+00003240: 077c 0364 057c 006a 006a 0864 068d 037d  .|.d.|.j.j.d...}
+00003250: 047a 047c 0401 0057 006e 1504 0074 0979  .z.|...W.n...t.y
+00003260: 3a01 0001 0001 007c 006a 006a 0a72 3774  :......|.j.j.r7t
+00003270: 0b64 0783 0101 0059 0064 0053 0059 0064  .d.....Y.d.S.Y.d
+00003280: 0053 0077 007c 006a 006a 0a72 4374 0b64  .S.w.|.j.j.rCt.d
+00003290: 0883 0101 0064 097d 0509 0074 0c74 0da0  .....d.}...t.t..
+000032a0: 0e7c 006a 0fa1 017c 0474 0da0 0e7c 01a1  .|.j...|.t...|..
+000032b0: 0174 0da0 0e7c 05a1 0174 0da0 0e7c 006a  .t...|...t...|.j
+000032c0: 10a1 0174 0da0 0e7c 006a 11a1 0174 0da0  ...t...|.j...t..
+000032d0: 0e7c 006a 00a1 0183 077d 067c 0272 707c  .|.j.....}.|.rp|
+000032e0: 02a0 1274 036a 137c 06a1 027d 056e 0974  ...t.j.|...}.n.t
+000032f0: 0574 0da0 1274 036a 137c 06a1 0283 017d  .t...t.j.|.....}
+00003300: 0574 147c 0583 0172 a57c 056a 1564 0b64  .t.|...r.|.j.d.d
+00003310: 0c84 0064 0d8d 0101 007c 006a 006a 0a72  ...d.....|.j.j.r
+00003320: 9e74 0b64 0e74 167c 0564 0f19 0064 1019  .t.d.t.|.d...d..
+00003330: 0083 019b 0064 117c 0564 0f19 0064 1219  .....d.|.d...d..
+00003340: 009b 0064 139d 0583 0101 007c 0564 0f19  ...d.......|.d..
+00003350: 0064 1019 007d 056e 0264 0053 0071 4629  .d...}.n.d.S.qF)
+00003360: 144e 7245 0000 007a 4550 6172 616d 6574  .NrE...zEParamet
+00003370: 6572 2074 6f20 706c 6f74 2061 6c6f 6e67  er to plot along
+00003380: 2074 6865 2078 2d61 7865 7320 6f66 2074   the x-axes of t
+00003390: 6865 2062 6172 6368 6172 7473 2068 6173  he barcharts has
+000033a0: 206e 6f74 2062 6565 6e20 7365 742e 7a11   not been set.z.
+000033b0: 4669 6775 7265 732f 4261 7263 6861 7274  Figures/Barchart
+000033c0: 7372 f100 0000 7a14 4f6e 6520 7265 6769  sr....z.One regi
+000033d0: 6f6e 2062 6172 2063 6861 7274 a902 da09  on bar chart....
+000033e0: 6675 6e63 5f6e 616d 65da 1163 6f6e 6669  func_name..confi
+000033f0: 675f 7265 6769 6f6e 5f76 6172 7a1b 536b  g_region_varz.Sk
+00003400: 6970 7069 6e67 2062 6172 6368 6172 7420  ipping barchart 
+00003410: 6372 6561 7469 6f6e 2e7a 1a0a 2d2d 2d20  creation.z..--- 
+00003420: 4261 7263 6861 7274 2063 7265 6174 696f  Barchart creatio
+00003430: 6e20 2d2d 2d72 0100 0000 5463 0100 0000  n ---r....Tc....
+00003440: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00003450: 5300 0000 f308 0000 007c 0064 0119 0053  S........|.d...S
+00003460: 00a9 024e 7209 0000 0072 3600 0000 7208  ...Nr....r6...r.
+00003470: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00003480: 0000 720a 0100 0013 0200 00f3 0200 0000  ..r.............
+00003490: 0800 7a20 4261 7263 6861 7274 2e73 6574  ..z Barchart.set
+000034a0: 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  up.<locals>.<lam
+000034b0: 6264 613e a901 72f3 0000 007a 144d 6178  bda>..r....z.Max
+000034c0: 696d 756d 2079 206c 696d 6974 206f 663a  imum y limit of:
+000034d0: 2072 a500 0000 7209 0000 00fa 1020 7365   r....r...... se
+000034e0: 656e 2077 6974 6820 524f 493a 2072 6000  en with ROI: r`.
+000034f0: 0000 7a26 2e20 4372 6561 7469 6e67 2066  ..z&. Creating f
+00003500: 6967 7572 6573 2077 6974 6820 7468 6973  igures with this
+00003510: 2079 206c 696d 6974 2e0a 2917 7214 0000   y limit..).r...
+00003520: 00da 1573 696e 676c 655f 726f 695f 6669  ...single_roi_fi
+00003530: 675f 785f 6178 6973 da09 4578 6365 7074  g_x_axis..Except
+00003540: 696f 6e72 0a00 0000 7229 0000 0072 6900  ionr....r)...ri.
+00003550: 0000 72a7 0000 00da 1066 696e 645f 6368  ..r......find_ch
+00003560: 6f73 656e 5f72 6f69 73da 1172 6567 696f  osen_rois..regio
+00003570: 6e61 6c5f 6669 675f 726f 6973 da09 4e61  nal_fig_rois..Na
+00003580: 6d65 4572 726f 7272 1f00 0000 7220 0000  meErrorr....r ..
+00003590: 00da 037a 6970 da09 6974 6572 746f 6f6c  ...zip..itertool
+000035a0: 73da 0672 6570 6561 7472 2700 0000 7257  s..repeatr'...rW
+000035b0: 0000 0072 4400 0000 da07 7374 6172 6d61  ...rD.....starma
+000035c0: 70da 1463 6c61 7373 5f6d 6574 686f 645f  p..class_method_
+000035d0: 6861 6e64 6c65 72da 0361 6e79 da04 736f  handler..any..so
+000035e0: 7274 72af 0000 0029 0772 3000 0000 72b0  rtr....).r0...r.
+000035f0: 0000 0072 3500 0000 da09 6c69 7374 5f72  ...r5.....list_r
+00003600: 6f69 73da 0b63 686f 7365 6e5f 726f 6973  ois..chosen_rois
+00003610: 722d 0100 00da 0869 7465 7261 626c 6572  r-.....iterabler
+00003620: 3600 0000 7236 0000 0072 3700 0000 722c  6...r6...r7...r,
+00003630: 0000 00f3 0100 0073 4000 0000 0c02 0801  .......s@.......
+00003640: 0a02 1002 0801 0601 06ff 0202 0801 0c01  ................
+00003650: 0801 0e01 06ff 02ff 0804 0801 0402 0201  ................
+00003660: 1601 1201 1401 04fe 0404 1001 1203 0802  ................
+00003670: 1001 0802 2a01 0e03 0402 02ec 7a0e 4261  ....*.......z.Ba
+00003680: 7263 6861 7274 2e73 6574 7570 6306 0000  rchart.setupc...
+00003690: 0000 0000 0000 0000 000b 0000 000f 0000  ................
+000036a0: 0043 0000 0073 6c02 0000 7c01 6a00 7c01  .C...sl...|.j.|.
+000036b0: 6401 1900 7c00 6b02 1900 7d06 7c06 a001  d...|.k...}.|...
+000036c0: 7c05 6a02 6701 a101 7d06 7c06 6a03 6402  |.j.g...}.|.j.d.
+000036d0: 6403 8d01 7d06 7404 6a05 7c06 7c05 6a02  d...}.t.j.|.|.j.
+000036e0: 1900 7c06 7c05 6a02 1900 a006 a100 6404  ..|.|.j.......d.
+000036f0: 8d02 7c06 7c05 6a02 3c00 6405 6406 8400  ..|.|.j.<.d.d...
+00003700: 7c06 6a07 4400 8301 7c06 5f07 7c05 6a02  |.j.D...|._.|.j.
+00003710: a008 6407 6408 a102 7c05 5f02 7c05 6a09  ..d.d...|._.|.j.
+00003720: a008 6407 6408 a102 7c05 5f09 740a a00b  ..d.d...|._.t...
+00003730: 7c06 a101 740a a00c a100 1700 740a 6a0d  |...t.......t.j.
+00003740: 740a 6a0e 6409 640a 640b 8d02 640a 6402  t.j.d.d.d...d.d.
+00003750: 640c 8d03 1700 740a 6a0f 640d 740a 6a0e  d.....t.j.d.t.j.
+00003760: 6409 640a 640b 8d02 640e 8d02 1700 740a  d.d.d...d.....t.
+00003770: 6a10 6700 640f 8d01 1700 740a 6a11 740a  j.g.d.....t.j.t.
+00003780: 6a12 6410 6411 8d01 740a 6a13 6412 6413  j.d.d...t.j.d.d.
+00003790: 6414 8d02 740a 6a14 6415 6416 6417 6418  d...t.j.d.d.d.d.
+000037a0: 8d03 740a 6a14 6415 6416 6417 6418 8d03  ..t.j.d.d.d.d...
+000037b0: 740a 6a14 6417 6416 6419 8d02 740a 6a14  t.j.d.d.d...t.j.
+000037c0: 6417 6415 6416 641a 6417 6901 641b 8d04  d.d.d.d.d.i.d...
+000037d0: 740a 6a14 6417 6416 641c 641d 6901 641e  t.j.d.d.d.d.i.d.
+000037e0: 8d03 641f 6420 6421 6422 6901 6423 7c05  ..d.d d!d"i.d#|.
+000037f0: 6a15 6424 8d0c 1700 740a 6a16 740a 6a17  j.d$....t.j.t.j.
+00003800: 6425 7c05 6a02 6426 8d02 6416 6417 6427  d%|.j.d&..d.d.d'
+00003810: 6428 8d04 1700 740a 6a18 7c05 6a19 6429  d(....t.j.|.j.d)
+00003820: 8d01 1700 7d07 642a 6406 8400 7c06 a01a  ....}.d*d...|...
+00003830: a100 4400 8301 6410 1900 7d08 7c05 6a09  ..D...d...}.|.j.
+00003840: 642b 6b02 73e7 7c07 740a 6a17 7c05 6a02  d+k.s.|.t.j.|.j.
+00003850: 642c 642d 7c08 9b00 9d02 642e 7c08 9b00  d,d-|.....d.|...
+00003860: 9d02 642f 7c05 6a09 9b00 6430 9d03 6431  ..d/|.j...d0..d1
+00003870: 8d05 3700 7d07 6e12 7c07 740a 6a17 7c05  ..7.}.n.|.t.j.|.
+00003880: 6a02 642c 642d 7c08 9b00 9d02 642e 7c08  j.d,d-|.....d.|.
+00003890: 9b00 9d02 6432 8d04 3700 7d07 7c07 740a  ....d2..7.}.|.t.
+000038a0: 6a1b 7c05 6a1c 7c05 6a1d 7c05 6a1e 6433  j.|.j.|.j.|.j.d3
+000038b0: 8d03 3700 7d07 7c02 9001 7215 7c07 740a  ..7.}.|...r.|.t.
+000038c0: a01f 6400 7c02 a102 3700 7d07 7c00 6434  ..d.|...7.}.|.d4
+000038d0: 3700 7d00 6410 7d09 7c02 6410 6b02 9001  7.}.d.}.|.d.k...
+000038e0: 7225 7c04 7c00 7c07 6435 8303 7d09 6436  r%|.|.|.d5..}.d6
+000038f0: 7d0a 6e07 7c02 6410 6b03 9001 722c 6437  }.n.|.d.k...r,d7
+00003900: 7d0a 7c03 7c07 7c00 7c0a 6438 7c05 8305  }.|.|.|.|.d8|...
+00003910: 0100 7c09 5300 2939 4e72 f100 0000 5472  ..|.S.)9Nr....Tr
+00003920: 0c01 0000 2901 da0a 6361 7465 676f 7269  ....)...categori
+00003930: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
+00003940: 0000 0006 0000 0053 0000 0073 1800 0000  .......S...s....
+00003950: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
+00003960: a102 9102 7102 5300 2902 720e 0000 0072  ....q.S.).r....r
+00003970: 0f00 0000 2901 721d 0000 0029 0272 9a00  ....).r....).r..
+00003980: 0000 da01 6372 3600 0000 7236 0000 0072  ....cr6...r6...r
+00003990: 3700 0000 729d 0000 0027 0200 00f3 0200  7...r....'......
+000039a0: 0000 1800 7a21 4261 7263 6861 7274 2e6d  ....z!Barchart.m
+000039b0: 616b 652e 3c6c 6f63 616c 733e 2e3c 6c69  ake.<locals>.<li
+000039c0: 7374 636f 6d70 3e72 0e00 0000 720f 0000  stcomp>r....r...
+000039d0: 00da 0673 696e 676c 65e7 9a99 9999 9999  ...single.......
+000039e0: e93f 2902 da08 7072 6573 6572 7665 724c  .?)...preserverL
+000039f0: 0000 0029 03da 0870 6f73 6974 696f 6e72  ...)...positionr
+00003a00: 4c00 0000 7211 0100 0072 0900 0000 2902  L...r....r....).
+00003a10: 72e7 0000 0072 5801 0000 2901 da06 6c61  r....rX...)...la
+00003a20: 6265 6c73 7201 0000 0072 1701 0000 da05  belsr....r......
+00003a30: 7768 6974 6567 9a99 9999 9999 c93f 721a  whiteg.......?r.
+00003a40: 0100 00da 0462 6f6c 64da 0562 6c61 636b  .....bold..black
+00003a50: e914 0000 00a9 03da 0677 6569 6768 74da  .........weight.
+00003a60: 0563 6f6c 6f72 72e7 0000 00a9 0272 e700  .colorr......r..
+00003a70: 0000 7260 0100 00da 0162 2904 72e7 0000  ..r`.....b).r...
+00003a80: 0072 5f01 0000 7260 0100 00da 066d 6172  .r_...r`.....mar
+00003a90: 6769 6eda 016c e905 0000 0029 0372 e700  gin..l.....).r..
+00003aa0: 0000 7260 0100 0072 6301 0000 e90a 0000  ..r`...rc.......
+00003ab0: 00e9 1e00 0000 72fb 0000 0067 3333 3333  ......r....g3333
+00003ac0: 3333 eb3f 2902 67cd cccc cccc ccec 3f72  33.?).g.......?r
+00003ad0: 5601 0000 290c 721c 0100 0072 1d01 0000  V...).r....r....
+00003ae0: da0c 6178 6973 5f74 6974 6c65 5f78 da0c  ..axis_title_x..
+00003af0: 6178 6973 5f74 6974 6c65 5f79 da0b 6178  axis_title_y..ax
+00003b00: 6973 5f74 6578 745f 795a 0c6c 6567 656e  is_text_yZ.legen
+00003b10: 645f 7469 746c 655a 0b6c 6567 656e 645f  d_titleZ.legend_
+00003b20: 7465 7874 5a14 6c65 6765 6e64 5f65 6e74  textZ.legend_ent
+00003b30: 7279 5f73 7061 6369 6e67 5a0f 6c65 6765  ry_spacingZ.lege
+00003b40: 6e64 5f6b 6579 5f73 697a 65da 0f73 7562  nd_key_size..sub
+00003b50: 706c 6f74 735f 6164 6a75 7374 da0f 6c65  plots_adjust..le
+00003b60: 6765 6e64 5f70 6f73 6974 696f 6e72 c100  gend_positionr..
+00003b70: 0000 6766 6666 6666 66e6 bf29 0272 1001  ..gffffff..).r..
+00003b80: 0000 da05 6c61 6265 6c72 fd00 0000 2903  ....labelr....).
+00003b90: 7260 0100 0072 e700 0000 da02 7661 a901  r`...r......va..
+00003ba0: 72bd 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00003bb0: 0000 0200 0000 0400 0000 5300 0000 7318  ..........S...s.
+00003bc0: 0000 0067 007c 005d 087d 0164 007c 0176  ...g.|.].}.d.|.v
+00003bd0: 0072 027c 0191 0271 0253 0029 015a 0843  .r.|...q.S.).Z.C
+00003be0: 6f6e 665f 496e 7472 3600 0000 2902 729a  onf_Intr6...).r.
+00003bf0: 0000 0072 0901 0000 7236 0000 0072 3600  ...r....r6...r6.
+00003c00: 0000 7237 0000 0072 9d00 0000 4302 0000  ..r7...r....C...
+00003c10: 7254 0100 0072 4500 0000 725c 0000 007a  rT...rE...r\...z
+00003c20: 054d 6561 6e2d 7a05 4d65 616e 2b7a 0766  .Mean-z.Mean+z.f
+00003c30: 6163 746f 7228 fa01 2929 0572 0901 0000  actor(..)).r....
+00003c40: 7210 0100 00da 0479 6d69 6eda 0479 6d61  r......ymin..yma
+00003c50: 7872 1301 0000 2904 7209 0100 0072 1001  xr....).r....r..
+00003c60: 0000 7271 0100 0072 7201 0000 2903 7209  ..rq...rr...).r.
+00003c70: 0100 0072 1001 0000 7213 0100 005a 0a5f  ...r....r....Z._
+00003c80: 7361 6d65 5f79 6c69 6d72 3a00 0000 5a0f  same_ylimr:...Z.
+00003c90: 4469 6666 6572 656e 745f 7961 7869 735a  Different_yaxisZ
+00003ca0: 0a53 616d 655f 7961 7869 735a 0862 6172  .Same_yaxisZ.bar
+00003cb0: 6368 6172 7429 2072 7200 0000 7207 0100  chart) rr...r...
+00003cc0: 0072 4301 0000 7225 0100 0072 6700 0000  .rC...r%...rg...
+00003cd0: da0b 4361 7465 676f 7269 6361 6c72 a700  ..Categoricalr..
+00003ce0: 0000 7277 0000 0072 1d00 0000 da15 7369  ..rw...r......si
+00003cf0: 6e67 6c65 5f72 6f69 5f66 6967 5f63 6f6c  ngle_roi_fig_col
+00003d00: 6f75 7272 2601 0000 7229 0100 0072 3001  ourr&...r)...r0.
+00003d10: 0000 5a08 6765 6f6d 5f63 6f6c 5a0e 706f  ..Z.geom_colZ.po
+00003d20: 7369 7469 6f6e 5f64 6f64 6765 5a0d 6765  sition_dodgeZ.ge
+00003d30: 6f6d 5f65 7272 6f72 6261 725a 1073 6361  om_errorbarZ.sca
+00003d40: 6c65 5f78 5f64 6973 6372 6574 6572 3101  le_x_discreter1.
+00003d50: 0000 7233 0100 0072 3401 0000 da0c 656c  ..r3...r4.....el
+00003d60: 656d 656e 745f 7465 7874 72d3 0000 005a  ement_textr....Z
+00003d70: 0967 656f 6d5f 7465 7874 7227 0100 005a  .geom_textr'...Z
+00003d80: 1173 6361 6c65 5f66 696c 6c5f 6d61 6e75  .scale_fill_manu
+00003d90: 616c da20 636f 6c6f 7262 6c69 6e64 5f66  al. colorblind_f
+00003da0: 7269 656e 646c 795f 706c 6f74 5f63 6f6c  riendly_plot_col
+00003db0: 6f75 7273 72ee 0000 00da 046c 6162 73da  oursr......labs.
+00003dc0: 1673 696e 676c 655f 726f 695f 6669 675f  .single_roi_fig_
+00003dd0: 6c61 6265 6c5f 78da 1673 696e 676c 655f  label_x..single_
+00003de0: 726f 695f 6669 675f 6c61 6265 6c5f 79da  roi_fig_label_y.
+00003df0: 1973 696e 676c 655f 726f 695f 6669 675f  .single_roi_fig_
+00003e00: 6c61 6265 6c5f 6669 6c6c 722d 0100 0029  label_fillr-...)
+00003e10: 0b72 3f00 0000 72b0 0000 005a 0679 6c69  .r?...r....Z.yli
+00003e20: 6d69 74da 0d73 6176 655f 6675 6e63 7469  mit..save_functi
+00003e30: 6f6e 5a12 6669 6e64 5f79 6c69 6d5f 6675  onZ.find_ylim_fu
+00003e40: 6e63 7469 6f6e 7214 0000 00da 0a63 7572  nctionr......cur
+00003e50: 7265 6e74 5f64 6672 4000 0000 5a0f 636f  rent_dfr@...Z.co
+00003e60: 6e66 5f69 6e74 5f73 7472 696e 675a 0d72  nf_int_stringZ.r
+00003e70: 6574 7572 6e65 645f 796c 696d 7253 0000  eturned_ylimrS..
+00003e80: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00003e90: 7227 0000 001d 0200 0073 8200 0000 1202  r'.......s......
+00003ea0: 0e02 0c01 0c01 0201 0401 02ff 0401 0cfe  ................
+00003eb0: 1204 1001 1001 0803 0601 02ff 1802 02fe  ................
+00003ec0: 1603 02fd 0a04 02fc 0e05 0c01 0e01 0e01  ................
+00003ed0: 0c01 1401 1201 0201 0201 0601 0201 0401  ................
+00003ee0: 04f5 02fb 1212 0601 04ff 02ee 0c14 02ec  ................
+00003ef0: 02ff 1618 0a02 0c01 1001 0c01 0afe 0c04  ................
+00003f00: 1001 08ff 0e03 0401 08ff 0603 1002 0801  ................
+00003f10: 0402 0a01 0c01 0601 0a01 0401 1002 0402  ................
+00003f20: 7a0d 4261 7263 6861 7274 2e6d 616b 654e  z.Barchart.makeN
+00003f30: 2907 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
+00003f40: 0072 8b00 0000 722c 0000 0072 8c00 0000  .r....r,...r....
+00003f50: 7227 0000 0072 3600 0000 7236 0000 0072  r'...r6...r6...r
+00003f60: 3600 0000 7237 0000 0072 2b00 0000 f201  6...r7...r+.....
+00003f70: 0000 730a 0000 0008 0002 010a 0102 290e  ..s...........).
+00003f80: 0172 2b00 0000 6300 0000 0000 0000 0000  .r+...c.........
+00003f90: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00003fa0: 3000 0000 6500 5a01 6400 5a02 6503 6401  0...e.Z.d.Z.e.d.
+00003fb0: 6402 8400 8301 5a04 6503 6403 6404 8400  d.....Z.e.d.d...
+00003fc0: 8301 5a05 6506 6405 6406 8400 8301 5a07  ..Z.e.d.d.....Z.
+00003fd0: 6407 5300 2908 722d 0000 0063 0300 0000  d.S.).r-...c....
+00003fe0: 0000 0000 0000 0000 0b00 0000 0a00 0000  ................
+00003ff0: 4300 0000 73a4 0100 0074 00a0 0164 01a1  C...s....t...d..
+00004000: 0101 0074 027c 0164 0219 00a0 03a1 0083  ...t.|.d........
+00004010: 017d 0374 006a 047c 0364 037c 006a 056a  .}.t.j.|.d.|.j.j
+00004020: 0664 048d 037d 047a 047c 0401 0057 006e  .d...}.z.|...W.n
+00004030: 1504 0074 0779 3001 0001 0001 007c 006a  ...t.y0......|.j
+00004040: 056a 0872 2d74 0964 0583 0101 0059 0064  .j.r-t.d.....Y.d
+00004050: 0053 0059 0064 0053 0077 007c 006a 056a  .S.Y.d.S.w.|.j.j
+00004060: 0872 3974 0964 0683 0101 0064 0764 0884  .r9t.d.....d.d..
+00004070: 0074 00a0 0a64 0964 0aa1 0244 0083 017d  .t...d.d...D...}
+00004080: 057c 006a 0b7c 006a 057c 057c 0164 0b64  .|.j.|.j.|.|.d.d
+00004090: 0c8d 047d 0667 007d 077c 0444 005d 0c7d  ...}.g.}.|.D.].}
+000040a0: 087c 07a0 0c7c 00a0 0d7c 087c 067c 01a1  .|...|...|.|.|..
+000040b0: 03a1 0101 0071 5264 0d7d 0909 0074 0e74  .....qRd.}...t.t
+000040c0: 0fa0 107c 006a 11a1 017c 047c 0774 0fa0  ...|.j...|.|.t..
+000040d0: 107c 09a1 0174 0fa0 107c 006a 12a1 0174  .|...t...|.j...t
+000040e0: 0fa0 107c 006a 13a1 0174 0fa0 107c 006a  ...|.j...t...|.j
+000040f0: 05a1 0183 077d 0a7c 0272 897c 02a0 1474  .....}.|.r.|...t
+00004100: 006a 157c 0aa1 027d 096e 0974 0274 0fa0  .j.|...}.n.t.t..
+00004110: 1474 006a 157c 0aa1 0283 017d 0974 167c  .t.j.|.....}.t.|
+00004120: 0983 0172 cf7a 077c 09a0 1764 00a1 0101  ...r.z.|...d....
+00004130: 0057 006e 0904 0074 1879 a601 0001 0001  .W.n...t.y......
+00004140: 0059 006e 0177 007c 096a 1964 0f64 1084  .Y.n.w.|.j.d.d..
+00004150: 0064 118d 0101 007c 006a 056a 0872 c874  .d.....|.j.j.r.t
+00004160: 0964 1274 1a7c 0964 1319 0064 1419 0083  .d.t.|.d...d....
+00004170: 019b 0064 157c 0964 1319 0064 1619 009b  ...d.|.d...d....
+00004180: 0064 179d 0583 0101 007c 0964 1319 0064  .d.......|.d...d
+00004190: 1419 007d 096e 0264 0053 0071 6229 184e  ...}.n.d.S.qb).N
+000041a0: 7a12 4669 6775 7265 732f 4869 7374 6f67  z.Figures/Histog
+000041b0: 7261 6d73 72f1 0000 0072 2d00 0000 723b  ramsr....r-...r;
+000041c0: 0100 007a 1c53 6b69 7070 696e 6720 6869  ...z.Skipping hi
+000041d0: 7374 6f67 7261 6d20 6372 6561 7469 6f6e  stogram creation
+000041e0: 2e7a 1b0a 2d2d 2d20 4869 7374 6f67 7261  .z..--- Histogra
+000041f0: 6d20 6372 6561 7469 6f6e 202d 2d2d 6301  m creation ---c.
+00004200: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00004210: 0000 0053 0000 0073 1e00 0000 6700 7c00  ...S...s....g.|.
+00004220: 5d0b 7d01 7400 a001 a100 9b00 6400 7c01  ].}.t.......d.|.
+00004230: 9b00 9d03 9102 7102 5300 2901 7a15 2f4f  ......q.S.).z./O
+00004240: 7665 7261 6c6c 2f52 6177 5f72 6573 756c  verall/Raw_resul
+00004250: 7473 2f29 0272 1600 0000 7217 0000 0072  ts/).r....r....r
+00004260: 9900 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00004270: 0000 0072 9d00 0000 7402 0000 7302 0000  ...r....t...s...
+00004280: 001e 007a 2348 6973 746f 6772 616d 2e73  ...z#Histogram.s
+00004290: 6574 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c  etup.<locals>.<l
+000042a0: 6973 7463 6f6d 703e 7a13 4f76 6572 616c  istcomp>z.Overal
+000042b0: 6c2f 5261 775f 7265 7375 6c74 7372 7000  l/Raw_resultsrp.
+000042c0: 0000 7205 0000 0029 0172 8000 0000 7201  ..r....).r....r.
+000042d0: 0000 0054 6301 0000 0000 0000 0000 0000  ...Tc...........
+000042e0: 0001 0000 0002 0000 0053 0000 0072 3e01  .........S...r>.
+000042f0: 0000 723f 0100 0072 3600 0000 7208 0100  ..r?...r6...r...
+00004300: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00004310: 720a 0100 008e 0200 0072 4001 0000 7a21  r........r@...z!
+00004320: 4869 7374 6f67 7261 6d2e 7365 7475 702e  Histogram.setup.
+00004330: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00004340: 3e72 4101 0000 7a14 4d61 7869 6d75 6d20  >rA...z.Maximum 
+00004350: 7820 6c69 6d69 7420 6f66 3a20 72a5 0000  x limit of: r...
+00004360: 0072 0900 0000 7242 0100 0072 6000 0000  .r....rB...r`...
+00004370: 7a26 2e20 4372 6561 7469 6e67 2066 6967  z&. Creating fig
+00004380: 7572 6573 2077 6974 6820 7468 6973 2078  ures with this x
+00004390: 206c 696d 6974 2e0a 291b 720a 0000 0072   limit..).r....r
+000043a0: 2900 0000 7269 0000 0072 a700 0000 7245  )...ri...r....rE
+000043b0: 0100 0072 1400 0000 7246 0100 0072 4701  ...r....rF...rG.
+000043c0: 0000 721f 0000 0072 2000 0000 da0a 6669  ..r....r .....fi
+000043d0: 6e64 5f66 696c 6573 7287 0000 0072 db00  nd_filesr....r..
+000043e0: 0000 da27 6765 745f 6d65 616e 5f61 6e64  ...'get_mean_and
+000043f0: 5f6d 6564 6961 6e5f 666f 725f 6561 6368  _median_for_each
+00004400: 5f63 686f 7365 6e5f 726f 6972 4801 0000  _chosen_roirH...
+00004410: 7249 0100 0072 4a01 0000 7227 0000 0072  rI...rJ...r'...r
+00004420: 5700 0000 7244 0000 0072 4b01 0000 724c  W...rD...rK...rL
+00004430: 0100 0072 4d01 0000 da06 7265 6d6f 7665  ...rM.....remove
+00004440: da0a 5661 6c75 6545 7272 6f72 724e 0100  ..ValueErrorrN..
+00004450: 0072 af00 0000 290b 7230 0000 0072 7f00  .r....).r0...r..
+00004460: 0000 7235 0000 0072 4f01 0000 7250 0100  ..r5...rO...rP..
+00004470: 0072 7e00 0000 7281 0000 005a 1063 6f6d  .r~...r....Z.com
+00004480: 6269 6e65 645f 7261 775f 6466 73da 0372  bined_raw_dfs..r
+00004490: 6f69 722c 0100 0072 5101 0000 7236 0000  oir,...rQ...r6..
+000044a0: 0072 3600 0000 7237 0000 0072 2c00 0000  .r6...r7...r,...
+000044b0: 6202 0000 7358 0000 000a 0210 0208 0106  b...sX..........
+000044c0: 0106 ff02 0308 010c 0108 010e 0106 ff02  ................
+000044d0: ff08 0408 0106 030a 0106 ff14 0204 0208  ................
+000044e0: 0104 010c 0106 ff04 0302 0110 0112 0114  ................
+000044f0: 0104 fe04 0410 0112 0208 0202 010e 010c  ................
+00004500: 0104 0102 ff10 0308 022a 010e 0304 0202  .........*......
+00004510: e87a 0f48 6973 746f 6772 616d 2e73 6574  .z.Histogram.set
+00004520: 7570 6304 0000 0000 0000 0000 0000 0008  upc.............
+00004530: 0000 0007 0000 0043 0000 0073 2a01 0000  .......C...s*...
+00004540: 7c01 6401 6b02 7208 7400 a001 a100 5300  |.d.k.r.t.....S.
+00004550: 7c01 6402 6b02 7215 7c02 a002 a100 7d04  |.d.k.r.|.....}.
+00004560: 6402 7c04 6403 3c00 6e0a 7c02 7c02 6403  d.|.d.<.n.|.|.d.
+00004570: 1900 7c01 6b02 1900 a002 a100 7d04 7c04  ..|.k.......}.|.
+00004580: a003 a100 7d04 7c03 6a04 6404 6403 6901  ....}.|.j.d.d.i.
+00004590: 6405 8d01 7d03 7405 7406 6400 7c00 6a07  d...}.t.t.d.|.j.
+000045a0: 6a08 7c00 6a07 6a09 6702 8302 8301 7d05  j.|.j.j.g.....}.
+000045b0: 7c04 6a0a 7c03 6403 6701 7c05 a201 6406  |.j.|.d.g.|...d.
+000045c0: 6407 8d03 7d04 6700 7c05 a201 6403 9101  d...}.g.|...d...
+000045d0: 6408 9101 6409 9101 640a 9101 7d06 7c04  d...d...d...}.|.
+000045e0: 6a0b 4400 5d0c 7d07 7c07 7c06 7601 725e  j.D.].}.|.|.v.r^
+000045f0: 7c04 6a0c 7c07 6405 8d01 7d04 7152 7400  |.j.|.d...}.qRt.
+00004600: 6a0d 7c04 7c06 6400 640b 8502 1900 640c  j.|.|.d.d.....d.
+00004610: 6409 640a 6702 640d 640e 8d05 7d04 7c00  d.d.g.d.d...}.|.
+00004620: 6a07 6a0e 7282 7c00 6a07 6a0f 7382 7c04  j.j.r.|.j.j.s.|.
+00004630: 6a10 7c04 640c 1900 6409 6b02 1900 7d04  j.|.d...d.k...}.
+00004640: 7c04 5300 7c00 6a07 6a0f 7293 7c00 6a07  |.S.|.j.j.r.|.j.
+00004650: 6a0e 7393 7c04 6a10 7c04 640c 1900 640a  j.s.|.j.|.d...d.
+00004660: 6b02 1900 7d04 7c04 5300 290f 4e72 0301  k...}.|.S.).Nr..
+00004670: 0000 7202 0100 0072 6100 0000 72f1 0000  ..r....ra...r...
+00004680: 0029 0172 7700 0000 72fa 0000 0029 02da  .).rw...r....)..
+00004690: 026f 6eda 0368 6f77 7262 0000 0072 5c00  .on..howrb...r\.
+000046a0: 0000 72a2 0000 00e9 feff ffff da09 5374  ..r...........St
+000046b0: 6174 6973 7469 63da 0a73 7461 745f 7661  atistic..stat_va
+000046c0: 6c75 6529 0472 6300 0000 7264 0000 00da  lue).rc...rd....
+000046d0: 0a76 616c 7565 5f76 6172 7372 6500 0000  .value_varsre...
+000046e0: 2911 7267 0000 0072 6800 0000 721f 0100  ).rg...rh...r...
+000046f0: 0072 7d00 0000 da06 7265 6e61 6d65 7269  .r}.....renameri
+00004700: 0000 0072 6a00 0000 7214 0000 0072 6c00  ...rj...r....rl.
+00004710: 0000 726d 0000 00da 056d 6572 6765 7277  ..rm.....mergerw
+00004720: 0000 0072 0d01 0000 727c 0000 00da 1368  ...r....r|.....h
+00004730: 6973 746f 6772 616d 5f73 686f 775f 6d65  istogram_show_me
+00004740: 616e da15 6869 7374 6f67 7261 6d5f 7368  an..histogram_sh
+00004750: 6f77 5f6d 6564 6961 6e72 7200 0000 2908  ow_medianrr...).
+00004760: 7230 0000 0072 3f00 0000 7281 0000 0072  r0...r?...r....r
+00004770: 7f00 0000 727c 0100 0072 8200 0000 72ee  ....r|...r....r.
+00004780: 0000 0072 8600 0000 7236 0000 0072 3600  ...r....r6...r6.
+00004790: 0000 7237 0000 0072 7e01 0000 9802 0000  ..r7...r~.......
+000047a0: 733a 0000 0008 0408 0108 0108 010a 0114  s:..............
+000047b0: 0208 0204 0306 0106 ff1a 0406 0108 0102  ................
+000047c0: 0106 fe18 050a 0208 010c 0102 8012 0208  ................
+000047d0: 0106 ff10 0312 0104 0410 fd12 0104 027a  ...............z
+000047e0: 3148 6973 746f 6772 616d 2e67 6574 5f6d  1Histogram.get_m
+000047f0: 6561 6e5f 616e 645f 6d65 6469 616e 5f66  ean_and_median_f
+00004800: 6f72 5f65 6163 685f 6368 6f73 656e 5f72  or_each_chosen_r
+00004810: 6f69 6306 0000 0000 0000 0000 0000 0009  oic.............
+00004820: 0000 0010 0000 0043 0000 0073 f801 0000  .......C...s....
+00004830: 7c01 6a00 720c 7c05 6a01 720a 7402 6401  |.j.r.|.j.r.t.d.
+00004840: 8301 0100 6400 5300 7403 a004 7c01 7403  ....d.S.t...|.t.
+00004850: 6a05 6402 6403 8d01 a102 7403 a006 a100  j.d.d.....t.....
+00004860: 1700 7403 6a07 7c05 6a08 7c05 6a09 6404  ..t.j.|.j.|.j.d.
+00004870: 6405 6406 8d04 1700 7403 6a0a 7c05 6a0b  d.d.....t.j.|.j.
+00004880: 9b00 6407 7c05 6a0c 9b00 9d03 6405 6408  ..d.|.j.....d.d.
+00004890: 6409 8d03 1700 7403 6a0d 7c05 6a0e 7c05  d.....t.j.|.j.|.
+000048a0: 6a0f 640a 8d02 1700 7403 6a10 7403 6a11  j.d.....t.j.t.j.
+000048b0: 6a12 6404 640b 8d01 7403 6a11 6a12 640c  j.d.d...t.j.j.d.
+000048c0: 640b 8d01 7403 6a12 6404 640b 8d01 7403  d...t.j.d.d...t.
+000048d0: 6a13 640d 640e 8d01 7403 6a13 640f 6410  j.d.d...t.j.d.d.
+000048e0: 6411 8d02 7403 6a14 6412 6413 6414 6415  d...t.j.d.d.d.d.
+000048f0: 8d03 7403 6a14 6412 6413 6414 6415 8d03  ..t.j.d.d.d.d...
+00004900: 7403 6a14 6412 6416 6413 6417 8d03 7403  t.j.d.d.d.d...t.
+00004910: 6a14 6412 6416 6413 6417 8d03 7403 6a14  j.d.d.d.d...t.j.
+00004920: 6416 6413 6418 8d02 7403 6a14 6416 6413  d.d.d...t.j.d.d.
+00004930: 6418 8d02 7c05 6a15 6419 8d0c 1700 7d06  d...|.j.d.....}.
+00004940: 7c05 6a16 738e 7c05 6a17 72ad 7c06 7403  |.j.s.|.j.r.|.t.
+00004950: 6a18 7403 6a05 641a 641b 641c 8d02 7c05  j.t.j.d.d.d...|.
+00004960: 6a19 641d 8d02 3700 7d06 7c06 7403 6a1a  j.d...7.}.|.t.j.
+00004970: 7c05 6a1b 641e 1900 7c05 6a1b 640c 1900  |.j.d...|.j.d...
+00004980: 6702 641f 8d01 3700 7d06 7c05 6a1c 73b8  g.d...7.}.|.j.s.
+00004990: 7c06 7403 6a10 6420 6421 8d01 3700 7d06  |.t.j.d d!..7.}.
+000049a0: 7c02 72c7 7c06 7403 a01d 6422 7c02 a102  |.r.|.t...d"|...
+000049b0: 3700 7d06 7c00 6423 3700 7d00 6e08 7c06  7.}.|.d#7.}.n.|.
+000049c0: 7403 a01d 6422 6400 a102 3700 7d06 6404  t...d"d...7.}.d.
+000049d0: 7d07 7c02 6404 6b02 72de 7c04 7c00 7c06  }.|.d.k.r.|.|.|.
+000049e0: 6424 8303 7d07 6425 7d08 6e06 7c02 6404  d$..}.d%}.n.|.d.
+000049f0: 6b03 72e4 6426 7d08 741e 6a1f 6427 7420  k.r.d&}.t.j.d't 
+00004a00: 6428 8d02 0100 7c03 7c06 7c00 7c08 6429  d(....|.|.|.|.d)
+00004a10: 7c05 8305 0100 741e 6a1f 642a 7420 6428  |.....t.j.d*t d(
+00004a20: 8d02 0100 7c07 5300 292b 4e7a 3849 4e46  ....|.S.)+Nz8INF
+00004a30: 4f3a 2048 6973 746f 6772 616d 7320 6361  O: Histograms ca
+00004a40: 6e6e 6f74 2062 6520 6d61 6465 2066 6f72  nnot be made for
+00004a50: 2074 6865 204e 6f20 524f 4920 6361 7465   the No ROI cate
+00004a60: 676f 7279 2e72 6200 0000 7208 0100 0072  gory.rb...r....r
+00004a70: 0100 0000 5429 04da 0862 696e 7769 6474  ....T)...binwidt
+00004a80: 6872 1301 0000 da08 626f 756e 6461 7279  hr......boundary
+00004a90: 7211 0100 0072 1401 0000 7215 0100 0072  r....r....r....r
+00004aa0: 1601 0000 720f 0100 0072 1701 0000 7209  ....r....r....r.
+00004ab0: 0000 0072 5a01 0000 a901 7213 0100 0072  ...rZ.....r....r
+00004ac0: 1901 0000 72a1 0000 0072 1a01 0000 725b  ....r....r....r[
+00004ad0: 0100 0072 5c01 0000 725d 0100 0072 5e01  ...r\...r]...r^.
+00004ae0: 0000 7266 0100 00a9 0372 5f01 0000 72e7  ..rf.....r_...r.
+00004af0: 0000 0072 6001 0000 7261 0100 00a9 0c5a  ...r`...ra.....Z
+00004b00: 1270 616e 656c 5f67 7269 645f 6d69 6e6f  .panel_grid_mino
+00004b10: 725f 7872 1c01 0000 721b 0100 005a 0f70  r_xr....r....Z.p
+00004b20: 6c6f 745f 6261 636b 6772 6f75 6e64 721d  lot_backgroundr.
+00004b30: 0100 0072 6801 0000 7269 0100 005a 0c73  ...rh...ri...Z.s
+00004b40: 7472 6970 5f74 6578 745f 785a 0c73 7472  trip_text_xZ.str
+00004b50: 6970 5f74 6578 745f 7972 1e01 0000 726a  ip_text_yr....rj
+00004b60: 0100 0072 c100 0000 7286 0100 0072 8501  ...r....r....r..
+00004b70: 0000 2902 5a0a 7869 6e74 6572 6365 7074  ..).Z.xintercept
+00004b80: 7260 0100 0029 0172 e700 0000 7249 0000  r`...).r....rI..
+00004b90: 0072 6f01 0000 da04 6e6f 6e65 2901 726c  .ro.....none).rl
+00004ba0: 0100 0072 a500 0000 5a0a 5f73 616d 655f  ...r....Z._same_
+00004bb0: 786c 696d 7239 0000 005a 0f44 6966 6665  xlimr9...Z.Diffe
+00004bc0: 7265 6e74 5f78 6178 6973 5a0a 5361 6d65  rent_xaxisZ.Same
+00004bd0: 5f78 6178 6973 da06 6967 6e6f 7265 2902  _xaxis..ignore).
+00004be0: da06 6163 7469 6f6e da08 6361 7465 676f  ..action..catego
+00004bf0: 7279 da09 6869 7374 6f67 7261 6dda 0764  ry..histogram..d
+00004c00: 6566 6175 6c74 2921 da05 656d 7074 7972  efault)!..emptyr
+00004c10: 1f00 0000 7220 0000 0072 2601 0000 7229  ....r ...r&...r)
+00004c20: 0100 0072 2701 0000 7230 0100 005a 0e67  ...r'...r0...Z.g
+00004c30: 656f 6d5f 6869 7374 6f67 7261 6dda 1268  eom_histogram..h
+00004c40: 6973 746f 6772 616d 5f62 696e 7769 6474  istogram_binwidt
+00004c50: 68da 1468 6973 746f 6772 616d 5f66 6967  h..histogram_fig
+00004c60: 5f63 6f6c 6f75 7272 2f01 0000 726d 0000  _colourr/...rm..
+00004c70: 0072 6c00 0000 7277 0100 00da 1568 6973  .rl...rw.....his
 00004c80: 746f 6772 616d 5f66 6967 5f6c 6162 656c  togram_fig_label
-00004c90: 5f79 7230 0100 0072 3101 0000 7232 0100  _yr0...r1...r2..
-00004ca0: 0072 3301 0000 7274 0100 0072 d200 0000  .r3...rt...r....
-00004cb0: 7289 0100 0072 8a01 0000 5a0a 6765 6f6d  r....r....Z.geom
-00004cc0: 5f76 6c69 6e65 da18 6869 7374 6f67 7261  _vline..histogra
-00004cd0: 6d5f 7374 6174 5f6c 696e 655f 7369 7a65  m_stat_line_size
-00004ce0: 5a12 7363 616c 655f 636f 6c6f 725f 6d61  Z.scale_color_ma
-00004cf0: 6e75 616c 7275 0100 00da 1568 6973 746f  nualru.....histo
-00004d00: 6772 616d 5f73 686f 775f 6c65 6765 6e64  gram_show_legend
-00004d10: 722b 0100 00da 0877 6172 6e69 6e67 73da  r+.....warnings.
-00004d20: 0c73 696d 706c 6566 696c 7465 72da 0d46  .simplefilter..F
-00004d30: 7574 7572 6557 6172 6e69 6e67 2909 723e  utureWarning).r>
-00004d40: 0000 0072 8000 0000 5a06 786c 696d 6974  ...r....Z.xlimit
-00004d50: 727a 0100 005a 1266 696e 645f 786c 696d  rz...Z.find_xlim
-00004d60: 5f66 756e 6374 696f 6e72 1300 0000 723f  _functionr....r?
-00004d70: 0000 005a 0d72 6574 7572 6e65 645f 786c  ...Z.returned_xl
-00004d80: 696d 7252 0000 0072 3500 0000 7235 0000  imrR...r5...r5..
-00004d90: 0072 3600 0000 7226 0000 00be 0200 0073  .r6...r&.......s
-00004da0: 7200 0000 0602 0601 0801 0401 1203 0601  r...............
-00004db0: 02ff 0c02 0201 0201 04fe 02fe 1405 0401  ................
-00004dc0: 04ff 02fb 1007 02f9 0408 0c01 0c01 0a01  ................
-00004dd0: 0a01 0c01 0e01 0e01 0e01 0e01 0c01 0c01  ................
-00004de0: 0401 04f4 02f8 02ff 0c1a 1201 0401 08ff  ................
-00004df0: 0e02 0801 0aff 0604 1001 0402 1002 0a01  ................
-00004e00: 1002 0402 0801 0c01 0601 0801 0401 0e03  ................
-00004e10: 1002 0e02 0402 7a0e 4869 7374 6f67 7261  ......z.Histogra
-00004e20: 6d2e 6d61 6b65 4e29 0872 8700 0000 7288  m.makeN).r....r.
-00004e30: 0000 0072 8900 0000 728a 0000 0072 2b00  ...r....r....r+.
-00004e40: 0000 727d 0100 0072 8b00 0000 7226 0000  ..r}...r....r&..
-00004e50: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
-00004e60: 7236 0000 0072 2c00 0000 5e02 0000 730e  r6...r,...^...s.
-00004e70: 0000 0008 0002 010a 0102 350a 0102 280e  ..........5...(.
-00004e80: 0172 2c00 0000 6300 0000 0000 0000 0000  .r,...c.........
-00004e90: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00004ea0: 3400 0000 6500 5a01 6400 5a02 6401 5a03  4...e.Z.d.Z.d.Z.
-00004eb0: 6504 6402 6403 8400 8301 5a05 6504 6404  e.d.d.....Z.e.d.
-00004ec0: 6405 8400 8301 5a06 6504 6406 6407 8400  d.....Z.e.d.d...
-00004ed0: 8301 5a07 6401 5300 2908 da0e 436f 6d70  ..Z.d.S.)...Comp
-00004ee0: 6172 654f 7574 7075 7473 4e63 0200 0000  areOutputsNc....
-00004ef0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00004f00: 4300 0000 7320 0000 007c 00a0 007c 01a1  C...s ...|...|..
-00004f10: 015c 027d 027d 037c 00a0 017c 027c 037c  .\.}.}.|...|.|.|
-00004f20: 01a1 0301 0064 0053 0029 014e 2902 da08  .....d.S.).N)...
-00004f30: 7365 7475 705f 6466 da0c 4d61 6b65 5f73  setup_df..Make_s
-00004f40: 6361 7474 6572 2904 722f 0000 0072 1300  catter).r/...r..
-00004f50: 0000 72af 0000 0072 5801 0000 7235 0000  ..r....rX...r5..
-00004f60: 0072 3500 0000 7236 0000 00da 0372 756e  .r5...r6.....run
-00004f70: 0403 0000 7304 0000 000e 0212 017a 1243  ....s........z.C
-00004f80: 6f6d 7061 7265 4f75 7470 7574 732e 7275  ompareOutputs.ru
-00004f90: 6e63 0200 0000 0000 0000 0000 0000 0a00  nc..............
-00004fa0: 0000 0900 0000 4300 0000 73b8 0000 0069  ......C...s....i
-00004fb0: 007d 0267 007d 0374 0064 0183 0144 005d  .}.g.}.t.d...D.]
-00004fc0: 3e7d 0474 016a 0264 0264 038d 017d 0574  >}.t.j.d.d...}.t
-00004fd0: 037c 059b 0064 049d 0264 0583 028f 267d  .|...d...d....&}
-00004fe0: 0674 04a0 057c 06a1 017d 0774 06a0 077c  .t...|...}.t...|
-00004ff0: 07a1 017c 027c 043c 007c 03a0 0874 096a  ...|.|.<.|...t.j
-00005000: 0aa0 0b7c 05a1 01a1 0101 0074 0c64 0664  ...|.......t.d.d
-00005010: 0784 007c 0744 0083 0183 017d 0857 0064  ...|.D.....}.W.d
-00005020: 0004 0004 0083 0301 0071 0831 0073 4177  .........q.1.sAw
-00005030: 0101 0001 0001 0059 0001 0071 087c 0264  .......Y...q.|.d
-00005040: 0819 006a 0d7c 0264 0919 0064 0a64 0b7c  ...j.|.d...d.d.|
-00005050: 016a 0e7c 016a 0f67 0364 0c8d 037d 097c  .j.|.j.g.d...}.|
-00005060: 097c 0366 0253 0029 0d4e 725f 0000 007a  .|.f.S.).Nr_...z
-00005070: 2753 656c 6563 7420 7468 6520 6469 7265  'Select the dire
-00005080: 6374 6f72 7920 6f75 7470 7574 2062 7920  ctory output by 
-00005090: 7468 6520 6652 4154 2901 724f 0000 007a  the fRAT).rO...z
-000050a0: 292f 5375 6d6d 6172 6973 6564 5f72 6573  )/Summarised_res
-000050b0: 756c 7473 2f63 6f6d 6269 6e65 645f 7265  ults/combined_re
-000050c0: 7375 6c74 732e 6a73 6f6e 725a 0000 0063  sults.jsonrZ...c
-000050d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000050e0: 0400 0000 5300 0000 7314 0000 0068 007c  ....S...s....h.|
-000050f0: 005d 067d 017c 0164 0019 0092 0271 0253  .].}.|.d.....q.S
-00005100: 0029 0172 f000 0000 7235 0000 0029 0272  .).r....r5...).r
-00005110: 9900 0000 da01 6472 3500 0000 7235 0000  ......dr5...r5..
-00005120: 0072 3600 0000 da09 3c73 6574 636f 6d70  .r6.....<setcomp
-00005130: 3e15 0300 0072 eb00 0000 7a2a 436f 6d70  >....r....z*Comp
-00005140: 6172 654f 7574 7075 7473 2e73 6574 7570  areOutputs.setup
-00005150: 5f64 662e 3c6c 6f63 616c 733e 2e3c 7365  _df.<locals>.<se
-00005160: 7463 6f6d 703e 7201 0000 0072 0800 0000  tcomp>r....r....
-00005170: da05 6f75 7465 7272 f000 0000 2902 7282  ..outerr....).r.
-00005180: 0100 0072 8101 0000 2910 da05 7261 6e67  ...r....)...rang
-00005190: 6572 0900 0000 da0c 6669 6c65 5f62 726f  er......file_bro
-000051a0: 7773 6572 726d 0000 0072 6f00 0000 7270  wserrm...ro...rp
-000051b0: 0000 0072 6600 0000 7267 0000 0072 da00  ...rf...rg...r..
-000051c0: 0000 7215 0000 0072 1800 0000 7273 0000  ..r....r....rs..
-000051d0: 0072 ad00 0000 7288 0100 0072 6c00 0000  .r....r....rl...
-000051e0: 726b 0000 0029 0a72 2f00 0000 7213 0000  rk...).r/...r...
-000051f0: 00da 0364 6673 7258 0100 0072 0801 0000  ...dfsrX...r....
-00005200: da09 6469 7265 6374 6f72 79da 0772 6573  ..directory..res
-00005210: 756c 7473 da04 6461 7461 5a04 726f 6973  ults..dataZ.rois
-00005220: 5a03 6466 6d72 3500 0000 7235 0000 0072  Z.dfmr5...r5...r
-00005230: 3600 0000 72a1 0100 0009 0300 0073 1c00  6...r........s..
-00005240: 0000 0402 0401 0c01 0c01 1202 0a01 0e01  ................
-00005250: 1201 1402 1efb 1007 0c01 06ff 0803 7a17  ..............z.
-00005260: 436f 6d70 6172 654f 7574 7075 7473 2e73  CompareOutputs.s
-00005270: 6574 7570 5f64 6663 0400 0000 0000 0000  etup_dfc........
-00005280: 0000 0000 0500 0000 1000 0000 4300 0000  ............C...
-00005290: 731c 0100 0074 00a0 017c 0174 006a 0264  s....t...|.t.j.d
-000052a0: 0164 0264 038d 02a1 0274 00a0 03a1 0017  .d.d.....t......
-000052b0: 0074 00a0 04a1 0017 0074 006a 057c 036a  .t.......t.j.|.j
-000052c0: 069b 0064 047c 036a 079b 009d 0364 0564  ...d.|.j.....d.d
-000052d0: 0664 078d 0317 0074 006a 0864 0864 098d  .d.....t.j.d.d..
-000052e0: 0117 0074 006a 097c 0264 0a19 007c 0264  ...t.j.|.d...|.d
-000052f0: 0b19 0064 038d 0217 0074 006a 0a74 006a  ...d.....t.j.t.j
-00005300: 0b6a 0c64 0b64 0c8d 0174 006a 0b6a 0c64  .j.d.d...t.j.j.d
-00005310: 0a64 0c8d 0174 006a 0c64 0b64 0c8d 0174  .d...t.j.d.d...t
-00005320: 006a 0d64 0d64 0e8d 0174 006a 0d64 0f64  .j.d.d...t.j.d.d
-00005330: 1064 118d 0274 006a 0e64 1264 1364 1464  .d...t.j.d.d.d.d
-00005340: 158d 0374 006a 0e64 1264 1364 1464 158d  ...t.j.d.d.d.d..
-00005350: 0374 006a 0e64 1264 1664 1364 178d 0374  .t.j.d.d.d.d...t
-00005360: 006a 0e64 1264 1664 1364 178d 0374 006a  .j.d.d.d.d...t.j
-00005370: 0e64 1664 1364 188d 0274 006a 0e64 1664  .d.d.d...t.j.d.d
-00005380: 1364 188d 027c 036a 0f64 198d 0c17 007d  .d...|.j.d.....}
-00005390: 047c 046a 1064 1a7c 036a 117c 036a 1164  .|.j.d.|.j.|.j.d
-000053a0: 1b14 0064 1c64 1c64 1d8d 0501 0064 0053  ...d.d.d.....d.S
-000053b0: 0029 1e4e 5a06 4d65 616e 5f78 5a06 4d65  .).NZ.Mean_xZ.Me
-000053c0: 616e 5f79 720e 0100 0072 1301 0000 5472  an_yr....r....Tr
-000053d0: 1401 0000 7215 0100 00da 026c 6d29 01da  ....r......lm)..
-000053e0: 066d 6574 686f 6472 0800 0000 7201 0000  .methodr....r...
-000053f0: 0072 1601 0000 7259 0100 0072 8d01 0000  .r....rY...r....
-00005400: 7218 0100 0072 a000 0000 7219 0100 0072  r....r....r....r
-00005410: 5a01 0000 725b 0100 0072 5c01 0000 725d  Z...r[...r\...r]
-00005420: 0100 0072 6501 0000 728e 0100 0072 6001  ...re...r....r`.
-00005430: 0000 728f 0100 007a 0854 4553 542e 706e  ..r....z.TEST.pn
-00005440: 6772 4800 0000 4672 4900 0000 2912 7225  grH...FrI...).r%
-00005450: 0100 0072 2801 0000 7226 0100 0072 2f01  ...r(...r&...r/.
-00005460: 0000 7236 0100 0072 2e01 0000 726c 0000  ..r6...r....rl..
-00005470: 0072 6b00 0000 5a0b 6765 6f6d 5f73 6d6f  .rk...Z.geom_smo
-00005480: 6f74 6872 7601 0000 7230 0100 0072 3101  othrv...r0...r1.
-00005490: 0000 7232 0100 0072 3301 0000 7274 0100  ..r2...r3...rt..
-000054a0: 0072 d200 0000 7250 0000 0072 5100 0000  .r....rP...rQ...
-000054b0: 2905 722f 0000 0072 af00 0000 7258 0100  ).r/...r....rX..
-000054c0: 0072 1300 0000 723f 0000 0072 3500 0000  .r....r?...r5...
-000054d0: 7235 0000 0072 3600 0000 72a2 0100 001c  r5...r6...r.....
-000054e0: 0300 0073 4200 0000 1403 0601 02ff 0602  ...sB...........
-000054f0: 02fe 1403 0401 04ff 02fd 0a05 02fb 1406  ................
-00005500: 02fa 0407 0c01 0c01 0a01 0a01 0c01 0e01  ................
-00005510: 0e01 0e01 0e01 0c01 0c01 0401 04f4 02f9  ................
-00005520: 02ff 0a18 0801 0401 0afe 7a1b 436f 6d70  ..........z.Comp
-00005530: 6172 654f 7574 7075 7473 2e4d 616b 655f  areOutputs.Make_
-00005540: 7363 6174 7465 7229 0872 8700 0000 7288  scatter).r....r.
-00005550: 0000 0072 8900 0000 727b 0100 0072 8a00  ...r....r{...r..
-00005560: 0000 72a3 0100 0072 a101 0000 72a2 0100  ..r....r....r...
-00005570: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
-00005580: 7236 0000 0072 a001 0000 0103 0000 7310  r6...r........s.
-00005590: 0000 0008 0004 0102 020a 0102 040a 0102  ................
-000055a0: 120e 0172 a001 0000 2924 721e 0100 0072  ...r....)$r....r
-000055b0: 4801 0000 7215 0000 0072 4d00 0000 729d  H...r....rM...r.
-000055c0: 0100 0072 0300 0000 da07 7061 7468 6c69  ...r......pathli
-000055d0: 6272 0400 0000 da10 6d61 7470 6c6f 746c  br......matplotl
-000055e0: 6962 2e69 6d61 6765 da05 696d 6167 6572  ib.image..imager
-000055f0: c300 0000 da05 6e75 6d70 7972 de00 0000  ......numpyr....
-00005600: da07 6e69 6261 6265 6c72 dc00 0000 da06  ..nibabelr......
-00005610: 7061 6e64 6173 7266 0000 005a 0870 6c6f  pandasrf...Z.plo
-00005620: 746e 696e 6572 2501 0000 da0a 7369 6d70  tniner%.....simp
-00005630: 6c65 6a73 6f6e 726f 0000 00da 076e 696c  lejsonro.....nil
-00005640: 6561 726e 7205 0000 00da 0a6d 6174 706c  earnr......matpl
-00005650: 6f74 6c69 6272 0600 0000 72a8 0000 00da  otlibr....r.....
-00005660: 0350 494c 7207 0000 00da 0575 7469 6c73  .PILr......utils
-00005670: 7209 0000 0072 0a00 0000 7225 0000 0072  r....r....r%...r
-00005680: 2900 0000 722a 0000 0072 2c00 0000 72a0  )...r*...r,...r.
-00005690: 0100 0072 3500 0000 7235 0000 0072 3500  ...r5...r5...r5.
-000056a0: 0000 7236 0000 00da 083c 6d6f 6475 6c65  ..r6.....<module
-000056b0: 3e01 0000 0073 3600 0000 0800 0801 0801  >....s6.........
-000056c0: 0801 0801 0c01 0c01 0c02 0801 0801 0801  ................
-000056d0: 0801 0801 0c01 0c01 0c01 0c02 0e03 007f  ................
-000056e0: 1012 007f 007f 100b 103f 106f 007f 1424  .........?.o...$
+00004c90: 5f78 da15 6869 7374 6f67 7261 6d5f 6669  _x..histogram_fi
+00004ca0: 675f 6c61 6265 6c5f 7972 3101 0000 7232  g_label_yr1...r2
+00004cb0: 0100 0072 3301 0000 7234 0100 0072 7501  ...r3...r4...ru.
+00004cc0: 0000 72d3 0000 0072 8a01 0000 728b 0100  ..r....r....r...
+00004cd0: 005a 0a67 656f 6d5f 766c 696e 65da 1868  .Z.geom_vline..h
+00004ce0: 6973 746f 6772 616d 5f73 7461 745f 6c69  istogram_stat_li
+00004cf0: 6e65 5f73 697a 655a 1273 6361 6c65 5f63  ne_sizeZ.scale_c
+00004d00: 6f6c 6f72 5f6d 616e 7561 6c72 7601 0000  olor_manualrv...
+00004d10: da15 6869 7374 6f67 7261 6d5f 7368 6f77  ..histogram_show
+00004d20: 5f6c 6567 656e 6472 2c01 0000 da08 7761  _legendr,.....wa
+00004d30: 726e 696e 6773 da0c 7369 6d70 6c65 6669  rnings..simplefi
+00004d40: 6c74 6572 da0d 4675 7475 7265 5761 726e  lter..FutureWarn
+00004d50: 696e 6729 0972 3f00 0000 7281 0000 005a  ing).r?...r....Z
+00004d60: 0678 6c69 6d69 7472 7b01 0000 5a12 6669  .xlimitr{...Z.fi
+00004d70: 6e64 5f78 6c69 6d5f 6675 6e63 7469 6f6e  nd_xlim_function
+00004d80: 7214 0000 0072 4000 0000 5a0d 7265 7475  r....r@...Z.retu
+00004d90: 726e 6564 5f78 6c69 6d72 5300 0000 7236  rned_xlimrS...r6
+00004da0: 0000 0072 3600 0000 7237 0000 0072 2700  ...r6...r7...r'.
+00004db0: 0000 c102 0000 7372 0000 0006 0206 0108  ......sr........
+00004dc0: 0104 0112 0306 0102 ff0c 0202 0102 0104  ................
+00004dd0: fe02 fe14 0504 0104 ff02 fb10 0702 f904  ................
+00004de0: 080c 010c 010a 010a 010c 010e 010e 010e  ................
+00004df0: 010e 010c 010c 0104 0104 f402 f802 ff0c  ................
+00004e00: 1a12 0104 0108 ff0e 0208 010a ff06 0410  ................
+00004e10: 0104 0210 020a 0110 0204 0208 010c 0106  ................
+00004e20: 0108 0104 010e 0310 020e 0204 027a 0e48  .............z.H
+00004e30: 6973 746f 6772 616d 2e6d 616b 654e 2908  istogram.makeN).
+00004e40: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
+00004e50: 8b00 0000 722c 0000 0072 7e01 0000 728c  ....r,...r~...r.
+00004e60: 0000 0072 2700 0000 7236 0000 0072 3600  ...r'...r6...r6.
+00004e70: 0000 7236 0000 0072 3700 0000 722d 0000  ..r6...r7...r-..
+00004e80: 0061 0200 0073 0e00 0000 0800 0201 0a01  .a...s..........
+00004e90: 0235 0a01 0228 0e01 722d 0000 0063 0000  .5...(..r-...c..
+00004ea0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00004eb0: 0000 4000 0000 7334 0000 0065 005a 0164  ..@...s4...e.Z.d
+00004ec0: 005a 0264 015a 0365 0464 0264 0384 0083  .Z.d.Z.e.d.d....
+00004ed0: 015a 0565 0464 0464 0584 0083 015a 0665  .Z.e.d.d.....Z.e
+00004ee0: 0464 0664 0784 0083 015a 0764 0153 0029  .d.d.....Z.d.S.)
+00004ef0: 08da 0e43 6f6d 7061 7265 4f75 7470 7574  ...CompareOutput
+00004f00: 734e 6302 0000 0000 0000 0000 0000 0004  sNc.............
+00004f10: 0000 0005 0000 0043 0000 0073 2000 0000  .......C...s ...
+00004f20: 7c00 a000 7c01 a101 5c02 7d02 7d03 7c00  |...|...\.}.}.|.
+00004f30: a001 7c02 7c03 7c01 a103 0100 6400 5300  ..|.|.|.....d.S.
+00004f40: 2901 4e29 02da 0873 6574 7570 5f64 66da  ).N)...setup_df.
+00004f50: 0c4d 616b 655f 7363 6174 7465 7229 0472  .Make_scatter).r
+00004f60: 3000 0000 7214 0000 0072 b000 0000 7259  0...r....r....rY
+00004f70: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00004f80: 0000 da03 7275 6e07 0300 0073 0400 0000  ....run....s....
+00004f90: 0e02 1201 7a12 436f 6d70 6172 654f 7574  ....z.CompareOut
+00004fa0: 7075 7473 2e72 756e 6302 0000 0000 0000  puts.runc.......
+00004fb0: 0000 0000 000a 0000 0009 0000 0043 0000  .............C..
+00004fc0: 0073 b800 0000 6900 7d02 6700 7d03 7400  .s....i.}.g.}.t.
+00004fd0: 6401 8301 4400 5d3e 7d04 7401 6a02 6402  d...D.]>}.t.j.d.
+00004fe0: 6403 8d01 7d05 7403 7c05 9b00 6404 9d02  d...}.t.|...d...
+00004ff0: 6405 8302 8f26 7d06 7404 a005 7c06 a101  d....&}.t...|...
+00005000: 7d07 7406 a007 7c07 a101 7c02 7c04 3c00  }.t...|...|.|.<.
+00005010: 7c03 a008 7409 6a0a a00b 7c05 a101 a101  |...t.j...|.....
+00005020: 0100 740c 6406 6407 8400 7c07 4400 8301  ..t.d.d...|.D...
+00005030: 8301 7d08 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+00005040: 7108 3100 7341 7701 0100 0100 0100 5900  q.1.sAw.......Y.
+00005050: 0100 7108 7c02 6408 1900 6a0d 7c02 6409  ..q.|.d...j.|.d.
+00005060: 1900 640a 640b 7c01 6a0e 7c01 6a0f 6703  ..d.d.|.j.|.j.g.
+00005070: 640c 8d03 7d09 7c09 7c03 6602 5300 290d  d...}.|.|.f.S.).
+00005080: 4e72 6000 0000 7a27 5365 6c65 6374 2074  Nr`...z'Select t
+00005090: 6865 2064 6972 6563 746f 7279 206f 7574  he directory out
+000050a0: 7075 7420 6279 2074 6865 2066 5241 5429  put by the fRAT)
+000050b0: 0172 5000 0000 7a29 2f53 756d 6d61 7269  .rP...z)/Summari
+000050c0: 7365 645f 7265 7375 6c74 732f 636f 6d62  sed_results/comb
+000050d0: 696e 6564 5f72 6573 756c 7473 2e6a 736f  ined_results.jso
+000050e0: 6e72 5b00 0000 6301 0000 0000 0000 0000  nr[...c.........
+000050f0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00005100: 1400 0000 6800 7c00 5d06 7d01 7c01 6400  ....h.|.].}.|.d.
+00005110: 1900 9202 7102 5300 2901 72f1 0000 0072  ....q.S.).r....r
+00005120: 3600 0000 2902 729a 0000 00da 0164 7236  6...).r......dr6
+00005130: 0000 0072 3600 0000 7237 0000 00da 093c  ...r6...r7.....<
+00005140: 7365 7463 6f6d 703e 1803 0000 72ec 0000  setcomp>....r...
+00005150: 007a 2a43 6f6d 7061 7265 4f75 7470 7574  .z*CompareOutput
+00005160: 732e 7365 7475 705f 6466 2e3c 6c6f 6361  s.setup_df.<loca
+00005170: 6c73 3e2e 3c73 6574 636f 6d70 3e72 0100  ls>.<setcomp>r..
+00005180: 0000 7209 0000 00da 056f 7574 6572 72f1  ..r......outerr.
+00005190: 0000 0029 0272 8301 0000 7282 0100 0029  ...).r....r....)
+000051a0: 10da 0572 616e 6765 720a 0000 00da 0c66  ...ranger......f
+000051b0: 696c 655f 6272 6f77 7365 7272 6e00 0000  ile_browserrn...
+000051c0: 7270 0000 0072 7100 0000 7267 0000 0072  rp...rq...rg...r
+000051d0: 6800 0000 72db 0000 0072 1600 0000 7219  h...r....r....r.
+000051e0: 0000 0072 7400 0000 72ae 0000 0072 8901  ...rt...r....r..
+000051f0: 0000 726d 0000 0072 6c00 0000 290a 7230  ..rm...rl...).r0
+00005200: 0000 0072 1400 0000 da03 6466 7372 5901  ...r......dfsrY.
+00005210: 0000 7209 0100 00da 0964 6972 6563 746f  ..r......directo
+00005220: 7279 da07 7265 7375 6c74 73da 0464 6174  ry..results..dat
+00005230: 615a 0472 6f69 735a 0364 666d 7236 0000  aZ.roisZ.dfmr6..
+00005240: 0072 3600 0000 7237 0000 0072 a201 0000  .r6...r7...r....
+00005250: 0c03 0000 731c 0000 0004 0204 010c 010c  ....s...........
+00005260: 0112 020a 010e 0112 0114 021e fb10 070c  ................
+00005270: 0106 ff08 037a 1743 6f6d 7061 7265 4f75  .....z.CompareOu
+00005280: 7470 7574 732e 7365 7475 705f 6466 6304  tputs.setup_dfc.
+00005290: 0000 0000 0000 0000 0000 0005 0000 0010  ................
+000052a0: 0000 0043 0000 0073 1c01 0000 7400 a001  ...C...s....t...
+000052b0: 7c01 7400 6a02 6401 6402 6403 8d02 a102  |.t.j.d.d.d.....
+000052c0: 7400 a003 a100 1700 7400 a004 a100 1700  t.......t.......
+000052d0: 7400 6a05 7c03 6a06 9b00 6404 7c03 6a07  t.j.|.j...d.|.j.
+000052e0: 9b00 9d03 6405 6406 6407 8d03 1700 7400  ....d.d.d.....t.
+000052f0: 6a08 6408 6409 8d01 1700 7400 6a09 7c02  j.d.d.....t.j.|.
+00005300: 640a 1900 7c02 640b 1900 6403 8d02 1700  d...|.d...d.....
+00005310: 7400 6a0a 7400 6a0b 6a0c 640b 640c 8d01  t.j.t.j.j.d.d...
+00005320: 7400 6a0b 6a0c 640a 640c 8d01 7400 6a0c  t.j.j.d.d...t.j.
+00005330: 640b 640c 8d01 7400 6a0d 640d 640e 8d01  d.d...t.j.d.d...
+00005340: 7400 6a0d 640f 6410 6411 8d02 7400 6a0e  t.j.d.d.d...t.j.
+00005350: 6412 6413 6414 6415 8d03 7400 6a0e 6412  d.d.d.d...t.j.d.
+00005360: 6413 6414 6415 8d03 7400 6a0e 6412 6416  d.d.d...t.j.d.d.
+00005370: 6413 6417 8d03 7400 6a0e 6412 6416 6413  d.d...t.j.d.d.d.
+00005380: 6417 8d03 7400 6a0e 6416 6413 6418 8d02  d...t.j.d.d.d...
+00005390: 7400 6a0e 6416 6413 6418 8d02 7c03 6a0f  t.j.d.d.d...|.j.
+000053a0: 6419 8d0c 1700 7d04 7c04 6a10 641a 7c03  d.....}.|.j.d.|.
+000053b0: 6a11 7c03 6a11 641b 1400 641c 641c 641d  j.|.j.d...d.d.d.
+000053c0: 8d05 0100 6400 5300 291e 4e5a 064d 6561  ....d.S.).NZ.Mea
+000053d0: 6e5f 785a 064d 6561 6e5f 7972 0f01 0000  n_xZ.Mean_yr....
+000053e0: 7214 0100 0054 7215 0100 0072 1601 0000  r....Tr....r....
+000053f0: da02 6c6d 2901 da06 6d65 7468 6f64 7209  ..lm)...methodr.
+00005400: 0000 0072 0100 0000 7217 0100 0072 5a01  ...r....r....rZ.
+00005410: 0000 728e 0100 0072 1901 0000 72a1 0000  ..r....r....r...
+00005420: 0072 1a01 0000 725b 0100 0072 5c01 0000  .r....r[...r\...
+00005430: 725d 0100 0072 5e01 0000 7266 0100 0072  r]...r^...rf...r
+00005440: 8f01 0000 7261 0100 0072 9001 0000 7a08  ....ra...r....z.
+00005450: 5445 5354 2e70 6e67 7249 0000 0046 724a  TEST.pngrI...FrJ
+00005460: 0000 0029 1272 2601 0000 7229 0100 0072  ...).r&...r)...r
+00005470: 2701 0000 7230 0100 0072 3701 0000 722f  '...r0...r7...r/
+00005480: 0100 0072 6d00 0000 726c 0000 005a 0b67  ...rm...rl...Z.g
+00005490: 656f 6d5f 736d 6f6f 7468 7277 0100 0072  eom_smoothrw...r
+000054a0: 3101 0000 7232 0100 0072 3301 0000 7234  1...r2...r3...r4
+000054b0: 0100 0072 7501 0000 72d3 0000 0072 5100  ...ru...r....rQ.
+000054c0: 0000 7252 0000 0029 0572 3000 0000 72b0  ..rR...).r0...r.
+000054d0: 0000 0072 5901 0000 7214 0000 0072 4000  ...rY...r....r@.
+000054e0: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+000054f0: 0072 a301 0000 1f03 0000 7342 0000 0014  .r........sB....
+00005500: 0306 0102 ff06 0202 fe14 0304 0104 ff02  ................
+00005510: fd0a 0502 fb14 0602 fa04 070c 010c 010a  ................
+00005520: 010a 010c 010e 010e 010e 010e 010c 010c  ................
+00005530: 0104 0104 f402 f902 ff0a 1808 0104 010a  ................
+00005540: fe7a 1b43 6f6d 7061 7265 4f75 7470 7574  .z.CompareOutput
+00005550: 732e 4d61 6b65 5f73 6361 7474 6572 2908  s.Make_scatter).
+00005560: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
+00005570: 7c01 0000 728b 0000 0072 a401 0000 72a2  |...r....r....r.
+00005580: 0100 0072 a301 0000 7236 0000 0072 3600  ...r....r6...r6.
+00005590: 0000 7236 0000 0072 3700 0000 72a1 0100  ..r6...r7...r...
+000055a0: 0004 0300 0073 1000 0000 0800 0401 0202  .....s..........
+000055b0: 0a01 0204 0a01 0212 0e01 72a1 0100 0029  ..........r....)
+000055c0: 2572 1f01 0000 7249 0100 0072 1600 0000  %r....rI...r....
+000055d0: 724e 0000 0072 9e01 0000 7203 0000 00da  rN...r....r.....
+000055e0: 0770 6174 686c 6962 7204 0000 00da 106d  .pathlibr......m
+000055f0: 6174 706c 6f74 6c69 622e 696d 6167 65da  atplotlib.image.
+00005600: 0569 6d61 6765 72c4 0000 00da 056e 756d  .imager......num
+00005610: 7079 72df 0000 00da 076e 6962 6162 656c  pyr......nibabel
+00005620: 72dd 0000 00da 0670 616e 6461 7372 6700  r......pandasrg.
+00005630: 0000 5a08 706c 6f74 6e69 6e65 7226 0100  ..Z.plotniner&..
+00005640: 00da 0a73 696d 706c 656a 736f 6e72 7000  ...simplejsonrp.
+00005650: 0000 da07 6e69 6c65 6172 6e72 0500 0000  ....nilearnr....
+00005660: da0a 6d61 7470 6c6f 746c 6962 7206 0000  ..matplotlibr...
+00005670: 0072 a900 0000 da03 5049 4c72 0700 0000  .r......PILr....
+00005680: da03 7573 65da 0575 7469 6c73 720a 0000  ..use..utilsr...
+00005690: 0072 0b00 0000 7226 0000 0072 2a00 0000  .r....r&...r*...
+000056a0: 722b 0000 0072 2d00 0000 72a1 0100 0072  r+...r-...r....r
+000056b0: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
+000056c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000056d0: 0073 3a00 0000 0800 0801 0801 0801 0801  .s:.............
+000056e0: 0c01 0c01 0c02 0801 0801 0801 0801 0801  ................
+000056f0: 0c01 0c01 0c01 0802 0a01 0c02 0e03 007f  ................
+00005700: 1012 007f 007f 100b 103f 106f 007f 1424  .........?.o...$
```

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.3.7/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/analysis.py` & `frat_brain-1.3.7/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/bootstrap.css` & `frat_brain-1.3.7/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/dash_report.py` & `frat_brain-1.3.7/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/directory_comparison.py` & `frat_brain-1.3.7/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.3.7/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/figures.py` & `frat_brain-1.3.7/fRAT/utils/figures.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 import simplejson as json
 from nilearn import plotting
 from matplotlib import pyplot as plt
 from PIL import Image
 
 from .utils import Utils
 
+import matplotlib
+matplotlib.use('agg') # Use non-GUI backend to prevent memory leak caused by creating subplots in a loop
+
 
 class Figures:
     config = None
 
     @classmethod
     def make_figures(cls, cfg, config_path, config_filename):
         cls.config = cfg
@@ -185,15 +188,15 @@
 
             Utils.check_and_make_dir(f"{os.getcwd()}/Figures/Brain_grids/{statistic}")
 
             brain_plot_exts = [
                 f"_{statistic}.nii.gz",
                 f"_{statistic}_within_roi_scaled.nii.gz",
                 # f"_{statistic}_mixed_roi_scaled.nii.gz"
-                               ]
+            ]
 
             for base_extension in brain_plot_exts:
                 indiv_brain_imgs = cls.setup(combined_results_df, base_extension, statistic, subfolder)
 
                 for img in indiv_brain_imgs:
                     Utils.move_file(img, os.getcwd(), indiv_brains_dir)
```

### Comparing `frat_brain-1.3.6/fRAT/utils/html_report.py` & `frat_brain-1.3.7/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/printResults.py` & `frat_brain-1.3.7/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/statistics.py` & `frat_brain-1.3.7/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/statmap.py` & `frat_brain-1.3.7/fRAT/utils/statmap.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.3.7/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/fRAT/utils/utils.py` & `frat_brain-1.3.7/fRAT/utils/utils.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.6/pyproject.toml` & `frat_brain-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.3.6"
+version = "1.3.7"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.3.6/setup.py` & `frat_brain-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.3.6',
+    'version': '1.3.7',
     'description': 'Application for ROI fMRI data analysis.',
     'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
```

### Comparing `frat_brain-1.3.6/PKG-INFO` & `frat_brain-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.3.6
+Version: 1.3.7
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


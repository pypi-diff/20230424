# Comparing `tmp/steam_sdk-2023.4.2.tar.gz` & `tmp/steam-sdk-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam_sdk-2023.4.2.tar", last modified: Thu Apr 20 16:50:27 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.4.3.tar", last modified: Mon Apr 24 13:26:58 2023, max compression
```

## Comparing `steam_sdk-2023.4.2.tar` & `steam-sdk-2023.4.3.tar`

### file list

```diff
@@ -1,206 +1,207 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.412520 steam_sdk-2023.4.2/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.2/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-04-20 16:50:27.412520 steam_sdk-2023.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.2/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/mkdocs.yaml
--rw-rw-rw-   0        0        0     1685 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 16:50:27.413519 steam_sdk-2023.4.2/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-20 15:51:06.000000 steam_sdk-2023.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.157204 steam_sdk-2023.4.2/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.169171 steam_sdk-2023.4.2/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   103197 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.174159 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.178148 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.188122 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.190116 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.195102 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.197097 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.203081 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.205075 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.245966 steam_sdk-2023.4.2/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    38418 2023-04-13 17:10:32.000000 steam_sdk-2023.4.2/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.2/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.247960 steam_sdk-2023.4.2/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.255939 steam_sdk-2023.4.2/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.262921 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.265913 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.266910 steam_sdk-2023.4.2/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.268905 steam_sdk-2023.4.2/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.297828 steam_sdk-2023.4.2/steam_sdk/data/
--rw-rw-rw-   0        0        0    10087 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.2/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.2/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.2/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     3076 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.2/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.2/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.313786 steam_sdk-2023.4.2/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.320766 steam_sdk-2023.4.2/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.348691 steam_sdk-2023.4.2/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.349689 steam_sdk-2023.4.2/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.2/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.361657 steam_sdk-2023.4.2/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    44535 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    59090 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.2/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.362654 steam_sdk-2023.4.2/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     1735 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.370632 steam_sdk-2023.4.2/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/plotters/PlotterSIGMA.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.372627 steam_sdk-2023.4.2/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.395566 steam_sdk-2023.4.2/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.2/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.2/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     6908 2023-04-20 15:50:04.000000 steam_sdk-2023.4.2/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.401550 steam_sdk-2023.4.2/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.2/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.405540 steam_sdk-2023.4.2/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.406537 steam_sdk-2023.4.2/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.407534 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.410526 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.2/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:50:27.163187 steam_sdk-2023.4.2/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7273 2023-04-20 16:50:25.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1596 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 16:50:00.000000 steam_sdk-2023.4.2/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.552091 steam-sdk-2023.4.3/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.4.3/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-04-24 13:26:58.551093 steam-sdk-2023.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.4.3/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1686 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:26:58.552091 steam-sdk-2023.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-24 13:24:31.000000 steam-sdk-2023.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.368581 steam-sdk-2023.4.3/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.378588 steam-sdk-2023.4.3/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   103257 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.378588 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.380554 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.387530 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.389526 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.393514 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.395509 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.399498 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.401494 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.418448 steam-sdk-2023.4.3/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    33654 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.4.3/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.419445 steam-sdk-2023.4.3/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.421440 steam-sdk-2023.4.3/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.424432 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.427424 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.429418 steam-sdk-2023.4.3/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.432413 steam-sdk-2023.4.3/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.460336 steam-sdk-2023.4.3/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10087 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.4.3/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35441 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2620 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.4.3/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.472317 steam-sdk-2023.4.3/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     7741 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.474298 steam-sdk-2023.4.3/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.503222 steam-sdk-2023.4.3/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.504219 steam-sdk-2023.4.3/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.511200 steam-sdk-2023.4.3/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    54678 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    59090 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.512197 steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2204 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.517184 steam-sdk-2023.4.3/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0    17127 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterSIGMA.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.519178 steam-sdk-2023.4.3/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.540123 steam-sdk-2023.4.3/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0    11647 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/utils/builder_SIGMA_helpers.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     6908 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.544112 steam-sdk-2023.4.3/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.4.3/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.546107 steam-sdk-2023.4.3/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.547103 steam-sdk-2023.4.3/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.549099 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.550096 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.374566 steam-sdk-2023.4.3/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7314 2023-04-24 13:26:57.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1597 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam_sdk-2023.4.2/.gitignore` & `steam-sdk-2023.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/.gitlab-ci.yml` & `steam-sdk-2023.4.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/PKG-INFO` & `steam-sdk-2023.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: steam_sdk
-Version: 2023.4.2
+Name: steam-sdk
+Version: 2023.4.3
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,API,STEAM,SDK
+Keywords: STEAM,CERN,API,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.2/Readme.md` & `steam-sdk-2023.4.3/Readme.md`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/mkdocs.yaml` & `steam-sdk-2023.4.3/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/requirements.txt` & `steam-sdk-2023.4.3/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.4.8
+steam-pysigma==2023.4.15
```

### Comparing `steam_sdk-2023.4.2/setup.py` & `steam-sdk-2023.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 with open("Readme.md", "r") as fh:
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
-    name='steam_sdk',
-    version="2023.4.2",
+    name='steam-sdk',
+    version="2023.4.3",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1389,28 +1389,28 @@
                 current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
                 magnets_list = self.__get_magnets_list(number_of_magnets)
                 t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 magnet_types = self.__get_magnet_types_list(number_of_magnets)
                 if circuit_family_name == "RQ":
                     circuit_name_1 = circuit_name.replace(".", "D_")
                     circuit_name_2 = circuit_name.replace(".", "F_")
-                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
                 else:
-                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
                 if circuit_family_name == "IPD":
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f'{event_number + 1}', 'coil_resistances.stl')
                 else:
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f'{event_number + 1}', 'coil_resistances.stl')
                 if circuit_family_name == "RQ":
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "RQX":
                     current_level = [current_level[0]+current_level[1], current_level[0]+current_level[2], current_level[0]+current_level[2], current_level[0]]
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 else:
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 # start parsim sweep step with newly created event file
                 parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
                                                     model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                 self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
                 self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
                 self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.4.3/steam_sdk/builders/BuilderSIGMA.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
 import time
 from pathlib import Path
 import numpy as np
+import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.lines as lines
+import subprocess
 from steam_sdk.plotters import PlotterSIGMA as p
 from steam_sdk.data import DataRoxieParser as dR
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserRoxie import arcCenter
+from steam_sdk.utils.builder_SIGMA_helpers import *
 from steam_pysigma import pysigma as ps
+import logging
 
 class BuilderSIGMA:
     """
         Class to generate SIGMA models
     """
 
     def __init__(self, input_model_data: DataModelMagnet = None,
@@ -71,29 +75,32 @@
                 raise Exception("Not supporting any other versions than 6.0 and 5.3a")
             self.model_java_file_path = f"{os.path.join(self.output_path, self.model_name)}.java"
             self.compile_batch_file_path = f"{os.path.join(self.output_path, self.model_name)}_Compile_and_Open.bat"
             self.model_class_file_path = f"{os.path.join(self.output_path, self.model_name)}.class"
             self.split_java_file_path = []
             self.study_type = self.model_data.Options_SIGMA.simulation.study_type
             self.num_qh = self.model_data.Quench_Protection.Quench_Heaters.N_strips
-            self.make_batch_mode_executable = False if self.model_data.Options_SIGMA.simulation.make_batch_mode_executable is None else self.model_data.Options_SIGMA.simulation.make_batch_mode_executable
+            self.make_batch_mode_executable = self.model_data.Options_SIGMA.simulation.make_batch_mode_executable
             self.generate_study = self.model_data.Options_SIGMA.simulation.generate_study
             self.input_coordinates_path = self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source
             self.cfg = self.g.ConfigSigma()
             self.cfg.setComsolVersion(self.COMSOL_version)  # for sigma_60
             self.cfg.setOutputModelPath(self.model_java_file_path)
             self.cfg.setComsolBatchPath(self.COMSOL_batch_path)
             self.cfg.setComsolCompilePath(self.COMSOL_compile_path)
             self.cfg.setExternalCFunLibPath(self.settings_dict["CFunLibPath"])
             self.cfg.setRunStudy(self.make_batch_mode_executable)
             self.cfg.setNumOfQHs(self.num_qh)
             self.cfg.setStudyType(self.study_type)
             self.cfg.setSymFactor(1)
-            self.cfg.setQuenchInitHT(str(self.model_data.Options_SIGMA.quench_initialization.quench_init_HT[0]))
-            self.cfg.setQuenchInitHeat(float(self.model_data.Options_SIGMA.quench_initialization.quench_init_heat[0]))
+            if self.model_data.Options_SIGMA.quench_initialization.quench_init_HT is not None:
+                array = self.a.convert_list_to_string_array(self.g.gateway, self.model_data.Options_SIGMA.quench_initialization.quench_init_HT)
+                self.cfg.setQuenchInitHT(array)
+            if self.model_data.Options_SIGMA.quench_initialization.quench_init_heat is not None:
+                self.cfg.setQuenchInitHeat(float(self.model_data.Options_SIGMA.quench_initialization.quench_init_heat))
             QHPositions = self.g.gateway.jvm.java.util.ArrayList()
             if self.model_data.Options_SIGMA.quench_heaters.quench_heater_positions is not None:
                 for qh in self.model_data.Options_SIGMA.quench_heaters.quench_heater_positions:
                     temp = self.g.gateway.jvm.java.util.ArrayList()
                     for pos in qh:
                         temp.add(pos)
                     QHPositions.add(temp)
@@ -107,16 +114,17 @@
             self.variables2DConverted = self.postprocessing_data.out_2D_at_points.variables # List of all exported variables
             self.time2DConverted = self.postprocessing_data.out_2D_at_points.time  # List of all exported time
             self.variables1DvsTime = self.postprocessing_data.out_1D_vs_times.variables
             self.time1DConverted = self.postprocessing_data.out_1D_vs_times.time
             self.variables1DvsTimeVector = self.postprocessing_data.out_1D_vs_times.variables
             self.timeRange = ", ".join(["range(" + ", ".join(map(str, lst)) + ")" for lst in
                                         self.model_data.Options_SIGMA.time_vector_solution.time_step])
-            #if verbose: print(f"Comsol compile path {self.COMSOL_compile_path}")
-            #if verbose: print(f"Comsol version {self.COMSOL_version}")
+            print(f"Comsol compile path {self.COMSOL_compile_path}")
+            print(f"Comsol version {self.COMSOL_version}")
+            validate_sigma_model_data(self.model_data, self.g.MPHC)
             self.build_magnet()
             self.save_model_java()
             self.save_compile_and_open_bat()
             #self.plot_magnet()
 
     def build_magnet(self):
         """
@@ -379,22 +387,20 @@
         :param domains: a tuple of domains to be included in the MPH model.
         :return: None
         """
 
         self.srv.connect(self.cfg.getComsolBatchPath())
         self.model = self.g.MagnetMPHBuilder(self.cfg, self.srv)
         # Create map with I0.
-        map = self.g.gateway.jvm.java.util.HashMap()
-        map.put("I_0", f"{self.model_data.Options_LEDET.field_map_files.Iref}[A]")
-        globalMap = self.build_global_variables()
+        globalMap = build_global_variables(self.g, self.model_data)
+        globalMap.put(self.g.MPHC.LABEL_CLIQ_CURRENT_EXT_INITIAL, f"{self.model_data.Options_LEDET.field_map_files.Iref}")
         #magnet = self.g.Magnet_T0_QH()
         #domains = magnet.getDomains()
         self.model = self.g.MagnetMPHBuilder(self.cfg, self.srv)
-        self.model.buildMPH(self.a.create_domain_array(self.g.gateway, tuple(domains)), map, 4, 1,
-                            globalMap)
+        self.model.buildMPH(self.a.create_domain_array(self.g.gateway, tuple(domains)), globalMap, 4, 1)
         if self.study_type=="Transient" and self.cfg.getNumOfQHs() > 0:
             builderQH = self.g.QuenchHeaterMPHBuilder(self.cfg, self.srv)
             self.model.connectToServer()
             builderQH.buildQuenchHeaterMPH()
 
     def create_results(self, input_coordinates_path, path_to_results):
         """
@@ -402,23 +408,25 @@
         :param input_coordinates_path: path to coordinate file to evaluate 2D variables in.
         :param path_to_results: path to result folder
         :return:
         """
         if self.make_batch_mode_executable:
             for i in range(len(self.variables2DConverted)):
                 time_vector_2D = ', '.join(str(x) for x in self.time2DConverted[i])
-                time_vector_1D = ', '.join(str(x) for x in self.time1DConverted[i])
 
                 self.g.ResultsAPI.create2DResultNode(self.srv, self.cfg, self.variables2DConverted[i], time_vector_2D, f"data {i}",
                                               input_coordinates_path, str(path_to_results))
             if self.study_type == "Transient":
                 for j in range(len(self.variables1DvsTime)):
                     self.g.ResultsAPI.create1DResultNodeAllTimes(self.srv, self.cfg, self.variables1DvsTime[j], f"1DExport_{j}", path_to_results)
 
                 for k in range(len(self.variables1DvsTimeVector)):
+                    print(self.variables1DvsTimeVector[k], self.time1DConverted[k])
+
+                    time_vector_1D = ', '.join(str(x) for x in self.time1DConverted[k])
                     self.g.ResultsAPI.create1DResultNodeTimeVector(self.srv, self.cfg, self.variables1DvsTimeVector[k], time_vector_1D,
                                                             f"data {i + 1 + k}", path_to_results)
         else:
             pass
             #print("No study run, no results to be exported.")
 
     def save_model_java(self):
@@ -554,14 +562,15 @@
         plt.show()
 
     def save_compile_and_open_bat(self):
         """
         Function writes a .bat file which has to be run to create a COMSOL model.
         :return: None
         """
+        print("Excecuting bat file")
         script_lines = []
         class_paths = ''
         for file in self.split_java_file_path:
             script_lines += [f'"{self.COMSOL_compile_path}" -jdkroot "{self.java_jdk_path}" "{file}.java"',
                              f'"{self.java_jdk_path}\\bin\\jar.exe" cf "{file}.jar" "{file}.class"']
             class_paths += f'-classpathadd "{file}.jar" '
 
@@ -577,100 +586,16 @@
 
     def build_study(self):
         """
         If valid study time defined function creates a COMSOL study
         :return: None
         """
         if self.study_type is not None:
-            if self.study_type == "Stationary":
+            if self.study_type == self.g.MPHC.LABEL_STATIONARY:
                 # Add code to create and run study
                 self.g.StudyAPI.setNewBasicStationaryStudy(self.srv, self.cfg, "sol1")
-            elif (self.study_type == "Transient"):
+            elif (self.study_type == self.g.MPHC.LABEL_TRANSIENT):
                 self.g.StudyAPI.setNewMonolithicStudy(self.srv, self.cfg, "Default_study", self.timeRange)
             else:
-                print("Invaid study_type input")
+                ValueError("Invaid study_type input")
 
-    def build_global_variables(self):
-        """
-        Function builds all global variables nessesary for QH simulations.
-        :return: map with global variables
-        """
-        map = self.g.gateway.jvm.java.util.HashMap()
-        constants = self.g.constants
-
-        FLAG_M_pers = self.model_data.Options_SIGMA.physics.FLAG_M_pers
-        FLAG_M_pers = "0" if FLAG_M_pers is None else FLAG_M_pers
-
-        FLAG_ifcc = self.model_data.Options_SIGMA.physics.FLAG_ifcc
-        FLAG_ifcc = "0" if FLAG_ifcc is None else FLAG_ifcc
-
-        FLAG_iscc_crossover = self.model_data.Options_SIGMA.physics.FLAG_iscc_crossover
-        FLAG_iscc_crossover = "0" if FLAG_iscc_crossover is None else FLAG_iscc_crossover
-
-        FLAG_iscc_adjw = self.model_data.Options_SIGMA.physics.FLAG_iscc_adjw
-        FLAG_iscc_adjw = "0" if FLAG_iscc_adjw is None else FLAG_iscc_adjw
-
-        FLAG_iscc_adjn =  self.model_data.Options_SIGMA.physics.FLAG_iscc_adjn
-        FLAG_iscc_adjn = "0" if FLAG_iscc_adjn is None else FLAG_iscc_adjn
-
-        FLAG_quench_all =  self.model_data.Options_SIGMA.quench_initialization.FLAG_quench_all
-        FLAG_quench_all = "0" if FLAG_quench_all is None else FLAG_quench_all
-
-        FLAG_quench_off = self.model_data.Options_SIGMA.quench_initialization.FLAG_quench_off
-        FLAG_quench_off = "0" if FLAG_quench_off is None else FLAG_quench_off
-
-
-        PARAM_time_quench = self.model_data.Options_SIGMA.quench_initialization.PARAM_time_quench
-        PARAM_time_quench = "0" if PARAM_time_quench is None else PARAM_time_quench
-
-        magnetic_length = self.model_data.GeneralParameters.magnetic_length
-        T_initial = self.model_data.GeneralParameters.T_initial
-
-        quench_heat = self.model_data.Options_SIGMA.quench_initialization.quench_init_heat
-        quench_temp =  self.model_data.Options_SIGMA.quench_initialization.quench_stop_temp
-
-        map.put(constants.LABEL_FLAG_IFCC, FLAG_ifcc)
-        map.put(constants.LABEL_FLAG_ISCC_CROSSOVER, FLAG_iscc_crossover)
-        map.put(constants.LABEL_FLAG_ISCC_ADJW, FLAG_iscc_adjw)
-        map.put(constants.LABEL_FLAG_ISCC_ADJN, FLAG_iscc_adjn)
-        map.put(constants.LABEL_FLAG_MPERS, FLAG_M_pers)
-        map.put(constants.LABEL_FLAG_QUENCH_ALL, FLAG_quench_all)
-        map.put(constants.LABEL_FLAG_QUENCH_OFF, FLAG_quench_off)
-        map.put(constants.LABEL_PARAM_QUENCH_TIME, PARAM_time_quench)
-        map.put(constants.LABEL_MAGNETIC_LENGTH, magnetic_length)
-        map.put(constants.LABEL_OPERATIONAL_TEMPERATUR, str(T_initial))
-        map.put(constants.LABEL_INIT_QUENCH_HEAT, str(quench_heat[0]))
-        map.put(constants.LABEL_QUENCH_TEMP, str(quench_temp))
-
-
-
-
-        ins_list = self.model_data.Quench_Protection.Quench_Heaters.s_ins
-        w_list = self.model_data.Quench_Protection.Quench_Heaters.w
-        qh_to_bath_list = self.model_data.Quench_Protection.Quench_Heaters.s_ins_He
-        qh_steel_strip = self.model_data.Quench_Protection.Quench_Heaters.h
-        tau = [round(a*b, 4) for a,b in zip(self.model_data.Quench_Protection.Quench_Heaters.R_warm,self.model_data.Quench_Protection.Quench_Heaters.C)]
-        num_qh_div = self.model_data.Options_SIGMA.quench_initialization.num_qh_div
-        u_init = self.model_data.Quench_Protection.Quench_Heaters.U0
-        i_init = [round(a/b, 3) for a,b in zip(self.model_data.Quench_Protection.Quench_Heaters.U0,self.model_data.Quench_Protection.Quench_Heaters.R_warm)]
-        frac_heater = self.model_data.Quench_Protection.Quench_Heaters.f_cover
-        trigger_time = self.model_data.Quench_Protection.Quench_Heaters.t_trigger
-        ins_thick_to_coil = self.model_data.Options_SIGMA.quench_heaters.th_coils
-        lengths_qh = self.model_data.Quench_Protection.Quench_Heaters.l
-
-        for i in range(self.num_qh):
-            if self.model_data.Options_SIGMA.time_vector_solution.time_step[-1][-1] < trigger_time[i]:
-                trigger_time[i] = self.model_data.Options_SIGMA.time_vector_solution.time_step[-1][-1]
-            map.put(constants.LABEL_INSULATION_THICKNESS_QH_TO_COIL+str(i+1), str(ins_list[i]))
-            map.put(constants.LABEL_WIDTH_QH+str(i+1), str(w_list[i]))
-            map.put(constants.LABEL_INSULATION_THICKNESS_QH_TO_BATH+str(i+1), str(qh_to_bath_list[i]))
-            map.put(constants.LABEL_INSULATION_THICKNESS_QH_STRIP + str(i + 1), str(qh_steel_strip[i]))
-            map.put(constants.LABEL_EXPONENTIAL_TIME_CONSTANT_DECAY + str(i + 1), str(tau[i]))
-            map.put(constants.LABEL_QH + constants.LABEL_L + str(i + 1), str(lengths_qh[i]))
-            map.put(constants.LABEL_NUMBER_OF_QH_SUBDIVISIONS + str(i + 1), str(num_qh_div[i]))
-            map.put(constants.LABEL_INITIAL_QH_CURRENT + str(i + 1), str(i_init[i]))
-            map.put(constants.LABEL_INITIAL_QH_VOLTAGE + str(i + 1), str(u_init[i]))
-            map.put(constants.LABEL_QH  + str(i + 1) + constants.LABEL_FRACTION_OF_QH_STATION, str(frac_heater[i]))
-            map.put(constants.LABEL_TRIGGER_TIME_QH + str(i + 1), str(trigger_time[i]))
-            map.put(constants.LABEL_INSULATION_THICKNESS_TO_COIL + str(i + 1), str(ins_thick_to_coil[i]))
 
-        return map
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.4.3/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.4.3/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.4.3/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml` & `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataModelMagnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,22 +920,20 @@
         Level 2: Class for simulation parameters in SIGMA
     """
     generate_study: bool = None
     study_type: str = None
     make_batch_mode_executable: bool = None
     nbr_elements_mesh_width: int = None
     nbr_elements_mesh_height: int = None
-    max_mesh_size: float = None
-
 
 class PhysicsSIGMA(BaseModel):
     """
         Level 2: Class for physics parameters in SIGMA
     """
-    FLAG_M_pers: float = None
+    FLAG_M_pers: float = None # change to int
     FLAG_ifcc: int = None
     FLAG_iscc_crossover: int = None
     FLAG_iscc_adjw: int = None
     FLAG_iscc_adjn: int = None
     tauCC_PE: float = None
 
 
@@ -943,22 +941,21 @@
     """
         Level 2: Class for quench initialization parameters in SIGMA
     """
     PARAM_time_quench: float = None
     FLAG_quench_all: int = None
     FLAG_quench_off: int = None
     num_qh_div: List[int] = None
-    quench_init_heat: List[float] = None
+    quench_init_heat: float = None
     quench_init_HT: List[str] = None
     quench_stop_temp: float = None
 
 class Out2DAtPointsSIGMA(BaseModel):
-    coordinate_source: List[str] = None
+    coordinate_source: str = None
     variables: List[str] = None
-    time_transient: List[List[float]] = None
     time: List[List[float]] = None
 
 
 class Out1DVsTimeSIGMA(BaseModel):
     variables: List[str] = None
     time: List[List[float]] = None
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataParsimConductor.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,16 @@
 
 ############################
 # Magnet
 class Magnet(BaseModel):
     coils: List[str] = []
     measured_inductance_versus_current: List[List[float]] = []   # TODO why is this needed?
 
-# ############################
-# # Coils
-# class Coil(BaseModel):
-#     ID: str = None
-#     cable_ID: str = None
-#     coil_length: float = None
-#     coil_RRR: float = None
-#     T_ref_RRR_low: float = None
-#     T_ref_RRR_high: float = None
-#     coil_resistance_room_T: float = None
-#     T_ref_coil_resistance: float = None
-#     conductors: List[str] = []
-#     weight_conductors: List[float] = []
-
 ############################
-# Conductors
+# Coils
 class IcMeasurement(BaseModel):
     """
         Level 1: Class for parameters of a critical current measurement to adjust Jc fit parameters
     """
     Ic: float = None
     T_ref_Ic: float = None
     B_ref_Ic: float = None
@@ -49,49 +35,53 @@
     bare_height: float = None
 
 
 class ConductorSample(BaseModel):
     # ID: str = None
     # Ra: float = None
     # Rc: float = None
-    index_of_conductor_in_modelData: int = None
-    group_indices_in_modelData: List[int] = []  # TODO new
     number_of_strands: int = None
     width: float = None
     height: float = None
     strand_twist_pitch: float = None
     filament_twist_pitch: float = None
-    # Resistance measurement attributes
-    coil_resistance_room_T: float = None  # TODO new
-    Cu_noCu_resistance_meas: float = None   # TODO new
-    total_conductor_length: float = None  # TODO new
+    RRR: float = None
+    Cu_noCu: float = None
     # critical current measurement attributes
     Tc0: float = None
     Bc20: float = None
-    f_rho_eff: float = None
+    f_rho_eff: float = None  # TODO unused
     Ic_measurements: List[IcMeasurement] = []
     strand_geometry: StrandGeometry = StrandGeometry()
-    # weighted entries with weight factors
+
+
+
+class Coil(BaseModel):
+    ID: str = None  # TODO unused
+    cable_ID: str = None  # TODO unused
+    coil_length: float = None  # TODO unused
+    # Resistance measurement attributes
+    coil_resistance_room_T: float = None
+    Cu_noCu_resistance_meas: float = None
+    total_conductor_length: float = None
+    T_ref_coil_resistance: float = None
+    T_ref_RRR_low: float = None
+    T_ref_RRR_high: float = None
+    # list of conductor samples and weight factor
+    conductorSamples: List[ConductorSample] = []
     weight_factors: List[float] = []
-    RRR: List[float] = []
-    Cu_noCu: List[float] = []
-    # names of entries that can be weighted as a read-only attribute
-    _names_of_attributes_to_weight: List[str] = ['RRR', 'Cu_noCu']
-    @property
-    def names_of_attributes_to_weight(self) -> List[str]:
-        return self._names_of_attributes_to_weight
 
 
 
 class DataParsimConductor(BaseModel):
     '''
         **Class for the STEAM conductor**
 
         This class contains the data structure of a Conductor parsim  analyzed with STEAM_SDK.
 
         :return: DataParsimConductor object
     '''
 
     GeneralParameters: GeneralParameters = GeneralParameters()
     Magnet: Magnet = Magnet()
-    # Coils: Dict[str, Coil] = {}
-    ConductorSamples: Dict[str, ConductorSample] = {}
+    Coils: Dict[str, Coil] = {}  # Datastructure representing one row in the csv file
+    # ConductorSamples: Dict[str, ConductorSample] = {}
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.4.3/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.4.3/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/temp/postLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/temp/postLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/temp/runLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/temp/runLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/drivers/temp/simLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/drivers/temp/simLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.4.3/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsers/templates/template_Dakota.in` & `steam-sdk-2023.4.3/steam_sdk/parsers/templates/template_Dakota.in`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimConductor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import csv
 import warnings
 import math
-
 from scipy.optimize import fsolve
 import numpy as np
 import pandas as pd
 import steammaterials
 from steammaterials.STEAM_materials import STEAM_materials
 import os
 import yaml
 from typing import List, Dict
 
-from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement
+from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement, Coil
 from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
 from steam_sdk.utils.get_attribute_type import get_attribute_type
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
+from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.utils.sgetattr import rsetattr, rgetattr
 from steam_sdk.data.DataParsimConductor import ConductorSample
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 
 
 class ParsimConductor:
     """
@@ -31,63 +31,73 @@
         """
         # Unpack arguments
         self.verbose: bool = verbose
         self.model_data = model_data
         self.dict_coilName_to_conductorIndex = dict_coilName_to_conductorIndex
         self.groups_to_coils = groups_to_coils
 
-        # groups_to_coil_length is either None (coil_length will be optimized) or dict
+        # groups_to_coil_length is either None (coil_length will be optimized) or dict (fCu will be optimized)
         self.number_of_groups = max([max(values) for values in self.groups_to_coils.values()])
         if groups_to_coil_length and type(groups_to_coil_length) == float:
             expected_group_numbers = list(range(1, self.number_of_groups + 1))
             self.groups_to_coil_length = {groups_to_coil_length: expected_group_numbers}
         else:
             self.groups_to_coil_length = groups_to_coil_length
 
+        # check input: coil names in groups_to_coils and dict_coilName_to_conductorIndex have to be the same
+        if not set(groups_to_coils.keys()) == set(dict_coilName_to_conductorIndex.keys()):
+            raise Exception(f'Coils of input dictionaries dont have the same names.')
+
         # DataParsimConductor object that will hold all the information from the input csv file
         self.data_parsim_conductor = DataParsimConductor()
 
     def read_from_input(self, path_input_file: str, magnet_name: str, strand_critical_current_measurements: Dict[str, Dict]):
         '''
         Read a .csv file and assign its content to a instance of DataParsimConductor().
 
         Parameters:
             path_input_file: Path to the .csv file to read
             magnet_name: name of the magnet that should be changed
-            strand_critical_current_measurements: dict of all the critical current measurements specified by the user
+            strand_critical_current_measurements: dict of all the critical current measurements details specified by the user
         '''
 
         # read table into pandas dataframe
         if path_input_file.endswith('.csv'):
-            df_conductors = pd.read_csv(path_input_file)
+            df_coils = pd.read_csv(path_input_file)
         elif path_input_file.endswith('.xlsx'):
-            df_conductors = pd.read_excel(path_input_file)
+            df_coils = pd.read_excel(path_input_file)
         else:
             raise Exception(f'The extension of the file {path_input_file} is not supported. Use either csv or xlsx.')
-        df_conductors = df_conductors.dropna(axis=1, how='all')
+        df_coils = df_coils.dropna(axis=1, how='all')
+
+        # read dict for reading columns into local dataclass
+        yaml_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "translation_dicts", "conductor_column_names.yaml")
+        with open(yaml_path, 'r') as file:
+            dict_attribute_to_column = yaml.safe_load(file) # TODO discuss with mariusz and implement also in ParsimEventMagnet
 
         # set magnet name to local model
         rsetattr(self.data_parsim_conductor, 'GeneralParameters.magnet_name', magnet_name)
 
         # get column name of coil and magnet
         parsed_columns = []  # list containing the column names that were parsed
-        column_name_magnets, column_name_coils = self.__get_and_check_main_column_names(df_conductors, parsed_columns)
+        column_name_magnets, column_name_coils = self.__get_and_check_main_column_names(df_coils, parsed_columns, dict_attribute_to_column['MainColumnNames'])
 
         # delete all rows of dataframe that don't belong to the magnet
-        mask = df_conductors[column_name_magnets] != magnet_name  # create a boolean mask for the rows that do not have the value in the column
-        df_conductors = df_conductors.drop(df_conductors[mask].index)  # drop the rows that do not have the value in the column
+        mask = df_coils[column_name_magnets] != magnet_name  # create a boolean mask for the rows that do not have the value in the column
+        df_coils = df_coils.drop(df_coils[mask].index)  # drop the rows that do not have the value in the column
 
         # Assign the content to a dataclass structure - loop over all the coils of the magnet in the database
-        for _, row in df_conductors.iterrows():
+        for _, row in df_coils.iterrows():
             self.__read_magnet(row, column_name_coils, parsed_columns)
-            # self.__read_coils(row, column_name_coils, parsed_columns)
-            self.read_conductors(row, column_name_coils, parsed_columns, strand_critical_current_measurements)
+            self.__read_coils(row, column_name_coils, parsed_columns, dict_attribute_to_column['Coil'])
+            self.__read_conductors(row, column_name_coils, parsed_columns, strand_critical_current_measurements,
+                                   dict_attribute_to_column['ConductorSample'])
 
         # show the user all the columns that where ignored by the code
-        ignored_column_names = list(set(df_conductors.columns) - set(parsed_columns))
+        ignored_column_names = list(set(df_coils.columns) - set(parsed_columns))
         if self.verbose: print(f'Names of ignored columns: {ignored_column_names}')
 
     def write_conductor_parameter_file(self, path_output_file: str, simulation_name: str, simulation_number: int):
         """
         Write the Parsim Conductor information to a CSV file, that can be used to run a ParsimSweep Step.
 
         Parameters:
@@ -98,218 +108,274 @@
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_output_file))
 
         # save all conductor parameters in a dict
         dict_sweeper = dict()
         dict_sweeper['simulation_name'] = simulation_name
         dict_sweeper['simulation_number'] = int(simulation_number)
-        self.__write_parsweep_conductors(dict_sweeper)
-        if not self.groups_to_coil_length: self.__write_parsweep_half_turn_length(dict_sweeper)
+
+        # write all the ConductorSample data to
+        if self.groups_to_coil_length:
+            # if groups_to_coil_length is specified, optimize the fraction of superconductor
+            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=True)
+        else:
+            # if no groups_to_coil_length is specified, optimize the length of the magnet
+            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=False)
+            # self.__write_parsweep_optimized_ht_length(dict_sweeper)
 
         # open file in writing mode and write the dict of the parameters as a row in the sweeper csv file
         with open(path_output_file, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=dict_sweeper.keys())
             writer.writeheader()
             writer.writerow(dict_sweeper)
 
     ################ HELPERS
 
-    def __get_and_check_main_column_names(self, df_conductors, parsed_columns):
+    def __get_and_check_main_column_names(self, df_coils, parsed_columns, dict_attr_to_colname):
         '''
             TODO refactoring and docstrings
         '''
         # allowed names for the magnet
-        csv_column_names_for_magnet_name = ['Magnet', 'Magnet Name', 'magnet', 'magnet name']
-        csv_column_names_for_coil_name = ['Coil', 'Coil Name', 'coil', 'coil name']
+        csv_column_names_for_magnet_name = dict_attr_to_colname['magnet_name']
+        csv_column_names_for_coil_name = dict_attr_to_colname['coil_name']
 
         # find out what name is being used for the magnet and coil column
         column_name_magnets, column_name_coils = None, None
         for col_name_magnet in csv_column_names_for_magnet_name:
-            if col_name_magnet in df_conductors.keys():
+            if col_name_magnet in df_coils.keys():
                 column_name_magnets = col_name_magnet
         for col_name_coil in csv_column_names_for_coil_name:
-            if col_name_coil in df_conductors.keys():
+            if col_name_coil in df_coils.keys():
                 column_name_coils = col_name_coil
         # TODO do i check later if coilnames are valid?
 
         # check if there is a column for magnet and coil
         if not column_name_magnets:
             raise Exception(f'No column for the magnet name could be found in the input table. Make sure this column is present.\nAllowed values :{csv_column_names_for_magnet_name}')
         if not column_name_coils:
             raise Exception(f'No column for the coil names could be found in the input table. Make sure this columns are present.\nAllowed values:{csv_column_names_for_coil_name}')
 
         # check if magnet name is present in the xlsx file
-        if not any(df_conductors[column_name_magnets] == self.data_parsim_conductor.GeneralParameters.magnet_name):
+        if not any(df_coils[column_name_magnets] == self.data_parsim_conductor.GeneralParameters.magnet_name):
             raise Exception(f'The magnet "{self.data_parsim_conductor.GeneralParameters.magnet_name}" is not present in the conductor database. ')
 
-        # and mark columns as parsed
+        # mark columns as parsed
         parsed_columns.append(column_name_magnets)
         parsed_columns.append(column_name_coils)
 
         return column_name_magnets, column_name_coils
 
-
-    def __read_general_parameters(self, magnet_name):
-        rsetattr(self.data_parsim_conductor, 'GeneralParameters.magnet_name', magnet_name)
-
-
     def __read_magnet(self, row, column_name_coils, parsed_columns):
         # add coil name to Coils list
         self.data_parsim_conductor.Magnet.coils.append(row[column_name_coils])
+        
+    def __read_coils(self, row, column_name_coils, parsed_columns, dict_attr_to_colname):
+        # create new coil instance
+        coil_name = row[column_name_coils]
+        new_Coil = Coil()
+
+        # change parameters of coil instance according to yaml translation file
+        for attribute_name, column_names in dict_attr_to_colname.items():
+            # check if only one column for the attribute can be found
+            used_column_names = [entry for entry in column_names if entry in row]
+            if len(used_column_names) == 1:
+                used_column_name = used_column_names[0]
+            elif len(used_column_names) == 0:
+                warnings.warn(f'No column for Coil attribute "{attribute_name}" found.')
+                continue
+            else: raise ValueError(f"More then one column for the ConductorSample attribute '{attribute_name}' found.")
 
-    def read_conductors(self, row, column_name_coils, parsed_columns, strand_critical_current_measurements):
+            # check dimension of input column to convert number into SI unit
+            dim = used_column_name[used_column_name.find('[') + 1:used_column_name.find(']')] if '[' in used_column_name else ''
+            # check if value is set in csv file
+            if not pd.isna(row[used_column_name]):
+                # if input is a float list in string format, parse it into a float list
+                if get_attribute_type(new_Coil, attribute_name)[0] == List[float]:
+                    if isinstance(row[used_column_name], str):
+                        float_list = parse_str_to_list(row[used_column_name], only_float_list=True)
+                    else:
+                        float_list = [row[used_column_name]]
+                    rsetattr(new_Coil, attribute_name, [make_value_SI(val, dim) for val in float_list])
+                else:
+                    # change parameter and convert number into SI unit
+                    rsetattr(new_Coil, attribute_name, make_value_SI(row[used_column_name], dim))
+                # mark column as parsed
+                if used_column_name not in parsed_columns: parsed_columns.append(used_column_name)
+
+        self.data_parsim_conductor.Coils[coil_name] = new_Coil
+
+    def __read_conductors(self, row, column_name_coils, parsed_columns, strand_critical_current_measurements, dict_attr_to_colname):
         '''
-        Function to read Conductors of ParsimConductors
+        Function to read ConductorSamples of ParsimConductors
 
         :param row: Series of parameters (read from csv file)
         :param parsed_columns: list of parsed table columns names
         '''
+        coil_name = row[column_name_coils]
 
-        # create ConductorSample instance
-        cond_name = row[column_name_coils]
-        new_Conductor = ConductorSample()
-        new_Conductor.index_of_conductor_in_modelData = self.dict_coilName_to_conductorIndex[cond_name]
-        new_Conductor.group_indices_in_modelData = self.groups_to_coils[cond_name]
+        # read how many conductor samples there are in the database for this coil
+        n_conductor_samples_found = []
+        all_col_names = [string for string_list in dict_attr_to_colname.values() for string in string_list]
+        # add column names for Ic measurements
+        for meas in strand_critical_current_measurements:
+            if coil_name in meas.coil_names:
+                all_col_names.append(meas.column_name_I_critical)
+                all_col_names.append(meas.column_name_CuNoCu_short_sample)
+        for col_name in all_col_names:
+            if col_name in row and not pd.isna(row[col_name]) and isinstance(row[col_name], str):
+                float_list = parse_str_to_list(row[col_name], only_float_list=True)
+                n_conductor_samples_found.append(len(float_list))
+        if all(element == n_conductor_samples_found[0] for element in n_conductor_samples_found):
+            n_conductor_samples = n_conductor_samples_found[0]
+        else:
+            raise Exception(f'Different number of Conductor Samples found for Coil "{coil_name}".')
 
-        # read dict for reading columns into local dataclass
-        yaml_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "translation_dicts", "conductor_column_names.yaml")
-        with open(yaml_path, 'r') as file:
-            dict_attribute_to_column = yaml.safe_load(file) # TODO i think this is the better way...we should also use that for ParsimEventMagnet
+        # check length of weight factors
+        if self.data_parsim_conductor.Coils[coil_name].weight_factors:
+            if len(self.data_parsim_conductor.Coils[coil_name].weight_factors) != n_conductor_samples:
+                raise Exception(f'Length of weight factor for coil {coil_name} is not similar to number of Conductor samples. Please correct the length to {n_conductor_samples} or delete entry (the average of the values will then be calculated)')
 
-        # read the critical current measurements into the local conductor dataclass
+        # create ConductorSample instances for every conductor sample
+        new_Conductors = [ConductorSample() for _ in range(n_conductor_samples)]
+
+        # read the critical current measurements into instances of the local conductor sample dataclasses
         for meas in strand_critical_current_measurements:
-            # raise error when col name of IcMeasurement is in translation dictionary
-            for attr_name, col_names in dict_attribute_to_column.items():
+            # raise error when col name of IcMeasurement is in translation dictionary (meaning it is already used)
+            for attr_name, col_names in dict_attr_to_colname.items():
                 if meas.column_name_I_critical in col_names:
                     raise Exception(f'Invalid column name for I_critical. "{meas.column_name_I_critical}" already used for the attribute "{attr_name}". Please change.')
                 if meas.column_name_CuNoCu_short_sample in col_names:
                     raise Exception(f'Invalid column name for I_critical. "{meas.column_name_CuNoCu_short_sample}" already used for the attribute "{attr_name}". Please change.')
 
-            if cond_name in meas.coil_names:
-                # create new IcMeasurement instance, add all values and append it to the measurement list of the conductor
-                new_Ic_meas = IcMeasurement()
+            if coil_name in meas.coil_names:
+                # create new IcMeasurement instances, add all values and append it to the measurement list of the conductor
+                new_Ic_measurements = [IcMeasurement() for _ in range(n_conductor_samples)]
+                  # TODO falsch - ConductorSample braucht list of IcMeasurement
                 # add temperature and magnetic flux of the measurements (directly given in step definition)
-                rsetattr(new_Ic_meas, 'B_ref_Ic', meas.reference_mag_field)
-                rsetattr(new_Ic_meas, 'T_ref_Ic', meas.reference_temperature)
+                for Ic_meas in new_Ic_measurements:
+                    rsetattr(Ic_meas, 'B_ref_Ic', meas.reference_mag_field)
+                    rsetattr(Ic_meas, 'T_ref_Ic', meas.reference_temperature)
                 # read critical current form csv file
                 if meas.column_name_I_critical in row and not pd.isna(row[meas.column_name_I_critical]):
-                    dim = meas.column_name_I_critical[meas.column_name_I_critical.find('[') + 1:meas.column_name_I_critical.find(']')] if '[' in meas.column_name_I_critical else ''
-                    rsetattr(new_Ic_meas, 'Ic', make_value_SI(row[meas.column_name_I_critical], dim))
+                    setattr_to_list(new_Ic_measurements, row, meas.column_name_I_critical, 'Ic')
                 else:
-                    raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty for coil {cond_name}.')
+                    raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty for coil {coil_name}.')
                 # read CuNoCu ratio of the short sample measurement
                 if meas.column_name_CuNoCu_short_sample in row and not pd.isna(row[meas.column_name_CuNoCu_short_sample]):
-                    dim = meas.column_name_CuNoCu_short_sample[meas.column_name_CuNoCu_short_sample.find('[') + 1:meas.column_name_CuNoCu_short_sample.find(']')] if '[' in meas.column_name_CuNoCu_short_sample else ''
-                    rsetattr(new_Ic_meas, 'Cu_noCu_sample', make_value_SI(row[meas.column_name_CuNoCu_short_sample], dim))
+                    setattr_to_list(new_Ic_measurements, row, meas.column_name_CuNoCu_short_sample, 'Cu_noCu_sample')
                 else:
                     raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_CuNoCu_short_sample}" was not found in the conductor database or is empty.')
-                new_Conductor.Ic_measurements.append(new_Ic_meas)
+                # append the new Ic measurements to a conductor sample
+                for cond, Ic_meas in zip(new_Conductors, new_Ic_measurements):
+                    cond.Ic_measurements.append(Ic_meas)
 
         # change parameters of conductors instance according to yaml translation file
-        for attribute_name, column_names in dict_attribute_to_column.items():
+        for attribute_name, column_names in dict_attr_to_colname.items():
             # check if only one column for the attribute can be found
             used_column_names = [entry for entry in column_names if entry in row]
             if len(used_column_names) == 1:
                 used_column_name = used_column_names[0]
             elif len(used_column_names) == 0:
                 warnings.warn(f'No column for ConductorSample attribute "{attribute_name}" found.')
                 continue
-            else:
-                raise ValueError(f"More then one column for the ConductorSample attribute '{attribute_name}' found.")
+            else: raise ValueError(f"More then one column for the ConductorSample attribute '{attribute_name}' found.")
 
-            # check dimension of input column to convert number into SI unit - if
-            dim = used_column_name[used_column_name.find('[') + 1:used_column_name.find(']')] if '[' in used_column_name else ''
-            # check if value is set in csv file
+            # check if value is set in csv file and set it to all the conductor instances
             if not pd.isna(row[used_column_name]):
-                # if input is a float list in string format, parse it into a string
-                if get_attribute_type(new_Conductor, attribute_name)[0] == List[float]:
-                    if isinstance(row[used_column_name], str):
-                        float_list = parse_str_to_list(row[used_column_name], only_float_list=True)
-                    else: float_list = [row[used_column_name]]
-                    rsetattr(new_Conductor, attribute_name, [make_value_SI(val, dim) for val in float_list])
-                else:
-                    # change parameter and convert number into SI unit
-                    rsetattr(new_Conductor, attribute_name, make_value_SI(row[used_column_name], dim))
+                setattr_to_list(new_Conductors, row, used_column_name, attribute_name)
             # mark column as parsed
             if used_column_name not in parsed_columns: parsed_columns.append(used_column_name)
 
         # check if only either diameter or bare w/h is set and check if original conductor type is the right one
-        original_conductor_type = self.model_data.Conductors[new_Conductor.index_of_conductor_in_modelData].strand.type
-        if original_conductor_type == 'Round':
-            if new_Conductor.strand_geometry.bare_width or new_Conductor.strand_geometry.bare_height:
-                raise Exception(f'Tried to change bare with/height of Round conductor named {cond_name}')
-        elif original_conductor_type == 'Rectangular':
-            if new_Conductor.strand_geometry.diameter:
-                raise Exception(f'Tried to change diameter of Rectangular conductor named {cond_name}')
-        else:
-            raise Exception(f'Unknown conductor type {original_conductor_type} for for conductor {cond_name}.')
+        original_conductor_type = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]].strand.type
+        if not original_conductor_type: raise Exception(f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
+        for cond in new_Conductors:
+            if original_conductor_type == 'Round':
+                if cond.strand_geometry.bare_width or cond.strand_geometry.bare_height:
+                    raise Exception(f'Tried to change bare with/height of Round coil named {coil_name}')
+            elif original_conductor_type == 'Rectangular':
+                if cond.strand_geometry.diameter:
+                    raise Exception(f'Tried to change diameter of Rectangular coil named {coil_name}')
+            else:
+                raise Exception(f'Unknown conductor type {original_conductor_type} for for coil {coil_name}.')
 
         # append new conductor instance to Conductors dictionary of ParsimConductor
-        self.data_parsim_conductor.ConductorSamples.update({cond_name: new_Conductor})
+        self.data_parsim_conductor.Coils[coil_name].conductorSamples = new_Conductors
 
-    def __write_parsweep_half_turn_length(self, dict_sweeper):
+
+    def __write_parsweep_optimized_ht_length(self, dict_sweeper):
         # create empty list to later fill with optimized values
         half_turn_length = [None for _ in range(self.number_of_groups)]
 
-        # looping through the conductor sample list
-        for name, conductor_sample in self.data_parsim_conductor.ConductorSamples.items():
-            original_conductor = self.model_data.Conductors[conductor_sample.index_of_conductor_in_modelData]
-            for index in conductor_sample.group_indices_in_modelData:
-                half_turn_length[index-1] = self.optimize_coil_length_with_resistance_meas(conductor_sample, original_conductor, dict_sweeper)
+        # looping through the coil list
+        for coil_name, coil in self.data_parsim_conductor.Coils.items():
+            original_conductor = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]]
+            for index in self.groups_to_coils[coil_name]:
+                for sample in coil.conductorSamples:
+                    half_turn_length[index-1] = self.optimize_coil_length_with_resistance_meas(sample, original_conductor, dict_sweeper)
 
         # raise Exception if there is still a None value in half_turn_length
         if not all(item is not None for item in half_turn_length):
-            raise Exception('Something went wrong when calculating the half_turn_length. Not every listentry could be calculated.')
+            raise Exception('Something went wrong when calculating the half_turn_length. Not every list entry could be calculated.')
 
         # add the list to the sweeper dict as a string
-        dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in half_turn_length) + ']'
+        dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in half_turn_length) + ']'  # TODO test if this works with ParsimSweeper in AnalysisSTEAM
 
     # TODO correction factor strand twist-pitch: f_twist_pitch = sqrt(wBare^2+(Lp_s/2)^2)/(Lp_s/2) , where w=wBare cable width, Lp_s=strand twist-pitch; if set to 2, take into account the increases of electrical resistance, ohmic loss per unit length, inter-filament and inter-strand coupling loss per unit length, and fractions of superconductor and stabilizer in the cable bare cross-section due to strand twist-pitch (default=0)
     # R = C_rho_Cu_NIST_fit with the coil_resistance_room_T, T_ref_coil_resistance and RRR (between 273 and 4) - most people take between RT and 4K
 
 
-    def optimize_coil_length_with_resistance_meas(self, conductor_sample, original_conductor, dict_sweeper):
-        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-        f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
-
-        # get number of half turns from map2d file if present
-        if self.model_data.Sources.magnetic_field_fromROXIE:
-            path_map2d = self.model_data.Sources.magnetic_field_fromROXIE
-            number_of_ht, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d) # TODO test this in AnalysisSTEAM
-        else:
-            number_of_ht = self.model_data.CoilWindings.n_half_turn_in_group
-
-        # define function to solve
-        def resistance_as_function_of_L(L, *args):
-            fCu, A_cond, temperature, mag_field, RRR, Tup_RRR  = args  # unpack arguments
-            numpy2d = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
-            matpath = os.path.dirname(steammaterials.__file__)
-            CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
-            rho = CFUN_rhoCuNIST.evaluate(numpy2d)[0]
-            return rho * L / (fCu * A_cond) * f_twist_pitch
-
-        # define parameters needed for function
-        fCu = conductor_sample.Cu_noCu_resistance_meas / (1 + conductor_sample.Cu_noCu_resistance_meas)  # TODO is this formula correct?
-        key_RRR = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].strand.RRR'
-        if key_RRR in dict_sweeper: RRR = dict_sweeper[key_RRR]  # use RRR from database - if not existing use modelData
-        else: RRR = original_conductor.strand.RRR
-        A_cond = calc_strand_area(strand_geometry=conductor_sample.strand_geometry, original_conductor=original_conductor) # TODO is this right?
-        temperature = 273  # TODO hardcoded RT?
-        mag_field = 0  # TODO hardcoded?
-        Tup_RRR  = 273  # TODO i need to know what the function exactely needs
-
-        # solve equation for magnetic length
-        args = (fCu, A_cond, temperature, mag_field, RRR, Tup_RRR )
-        if self.model_data.GeneralParameters.magnetic_length:
-            initial_guess = [self.model_data.GeneralParameters.magnetic_length]
-        else: initial_guess = [10]
-        L = fsolve(func=resistance_as_function_of_L, x0=initial_guess, args=args)
-        L_ht = L[0] / number_of_ht
-        return L_ht
-    
+    # def optimize_coil_length_with_resistance_meas(self, conductor_sample, conductor_samples, weight_factors, original_conductor):
+    #     # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+    #     bare_cable_width = getattr_from_list(conductor_samples, 'bare_cable_width', weight_factors=weight_factors)
+    #     if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
+    #
+    #     f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, conductor_samples, original_conductor)
+    #
+    #     # get number of half turns from map2d file if present
+    #     if self.model_data.Sources.magnetic_field_fromROXIE:
+    #         path_map2d = self.model_data.Sources.magnetic_field_fromROXIE
+    #         number_of_ht, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d) # TODO test this in AnalysisSTEAM
+    #     else:
+    #         number_of_ht = self.model_data.CoilWindings.n_half_turn_in_group
+    #
+    #     # define function to solve
+    #     def resistance_as_function_of_L(L, *args):
+    #         fCu, A_cond, temperature, mag_field, RRR, Tup_RRR  = args  # unpack arguments
+    #         rho_parameters = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+    #         matpath = os.path.dirname(steammaterials.__file__)
+    #         CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', rho_parameters.shape[0], rho_parameters.shape[1], matpath)
+    #         rho = CFUN_rhoCuNIST.evaluate(rho_parameters)[0]
+    #         return rho * L / (fCu * A_cond) * f_twist_pitch  # TODO solve it analytically
+    #
+    #     # define parameters needed for function
+    #     fCu = conductor_sample.Cu_noCu_resistance_meas / (1 + conductor_sample.Cu_noCu_resistance_meas)  # TODO if not present modeldata
+    #     key_RRR = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].strand.RRR'
+    #     if key_RRR in dict_sweeper:
+    #         RRR = dict_sweeper[key_RRR]  # use RRR from database - if not existing use modelData
+    #         Tup_RRR  = ...#TODO Cond.T_ref_RRR_high if not use 293.0
+    #     else:
+    #         if not original_conductor.strand.RRR: raise Exception('TODO')
+    #         if not original_conductor.strand.T_ref_RRR_high: raise Exception('TODO')
+    #         RRR = original_conductor.strand.RRR
+    #         Tup_RRR = original_conductor.strand.T_ref_RRR_high
+    #     A_cond = calc_strand_area(strand_geometry=conductor_sample.strand_geometry, original_conductor=original_conductor) # TODO is this right? * n_strands
+    #     temperature = ...#TODO Cond.coil_resistance_room_T if not 293.0  # TODO
+    #     mag_field = 0
+    #       # TODO if measured find in column
+    #
+    #     # solve equation for magnetic length
+    #     args = (fCu, A_cond, temperature, mag_field, RRR, Tup_RRR)
+    #     if self.model_data.GeneralParameters.magnetic_length:
+    #         initial_guess = [self.model_data.GeneralParameters.magnetic_length]
+    #     else: initial_guess = [10]
+    #     L = fsolve(func=resistance_as_function_of_L, x0=initial_guess, args=args)
+    #     L_ht = L[0] / number_of_ht
+    #     return L_ht
+    #
     def calculate_f_twist_pitch(self, conductor_sample, dict_sweeper, original_conductor):
         # get the bare_cable_width from the database if it has been changed, if not: use the default one from model_data
         key_bare_cable_width = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].cable.bare_cable_width'
         if key_bare_cable_width in dict_sweeper:
             bare_cable_width = dict_sweeper[key_bare_cable_width]
         else:
             bare_cable_width = original_conductor.cable.bare_cable_width
@@ -322,178 +388,198 @@
             strand_twist_pitch = original_conductor.cable.strand_twist_pitch
             
         # calculate correction factor strand twist-pitch
         f_twist_pitch = np.sqrt(bare_cable_width ** 2 + (strand_twist_pitch / 2) ** 2) / (strand_twist_pitch / 2)  # TODO should be around 1.03-1.05
         return f_twist_pitch
 
 
-    def __write_parsweep_conductors(self, dict_sweeper):
+    def __write_parsweep_conductors(self, dict_sweeper, flag_optimize_fCu: bool):
         """
         Writes the Conductor parameter for a sweeper csv file to a dict.
 
         Parameters:
         - dict_sweeper (dict): input dict where the sweeper entries will be stored  int the format {columnName: value}
-        - dict_coilName_to_conductorIndex (dict): input dict that specifies what column corresponds to what conductor index in the model {coilName: conductorIndex}
+        - flag_optimize_fCu (bool): TODO
 
         """
         # parameter dict for creating the column names of sweeper csv file
         dict_param = {
-            # format {parameter_name_of_conductor_object: parameter_name_of_DataModelMagnet_object}
+            # format {attribute_name_of_ConductorSample_object: attribute_name_of_Conductor_from_DataModelMagnet_object}
             'strand_geometry.diameter': 'strand.diameter',
             'strand_geometry.bare_width': 'strand.bare_width',
             'strand_geometry.bare_height': 'strand.bare_height',
             'RRR': 'strand.RRR',
             'Cu_noCu': 'strand.Cu_noCu_in_strand',
-            'width': 'cable.bare_cable_width',  # TODO is this correct?
+            'width': 'cable.bare_cable_width',
             'filament_twist_pitch': 'strand.fil_twist_pitch',
             'strand_twist_pitch': 'cable.strand_twist_pitch',
+# TODO name the attribute_name_of_ConductorSample_object identical to attribute_name_of_Conductor_from_DataModelMagnet_object to not need this dict?
         }
 
-        # looping through the conductor list
-        for name, conductor_sample in self.data_parsim_conductor.ConductorSamples.items():
-            idx = conductor_sample.index_of_conductor_in_modelData
+        # looping through the coil list
+        for coil_name, coil in self.data_parsim_conductor.Coils.items():
+            idx = self.dict_coilName_to_conductorIndex[coil_name]
             sweeper_cond_name = f'Conductors[{idx}].'
 
             # parse data from DataParsimConductor to strings for sweeper csv and store them in dict_sweeper
             for sample_attribute_name, conductor_attribute_name in dict_param.items():
-                if rgetattr(conductor_sample, sample_attribute_name):
-                    # check if conductor is rutherford before changing strand twist pitch
-                    if sample_attribute_name == 'strand_twist_pitch' and self.model_data.Conductors[idx].cable.type != 'Rutherford':
-                        raise Exception(f'Tried to change strand twist pitch property of a non Rutherford cable.')
-                    # add value to the sweeper dict
-                    val = rgetattr(conductor_sample, sample_attribute_name)
-                    if sample_attribute_name in conductor_sample.names_of_attributes_to_weight:
-                        dict_sweeper[sweeper_cond_name + conductor_attribute_name] = weight_list(val, conductor_sample.weight_factors)
-                    else:
-                        dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
+                val = getattr_from_list(coil.conductorSamples, sample_attribute_name, coil.weight_factors)
+                if val:
+                    # check if the original conductor has the attribute that will be changed to avoid errors when running parsim sweeper
+                    if not rhasattr(self.model_data.Conductors[idx], conductor_attribute_name):
+                        raise Exception(f'Tried to change conductor attribute "{conductor_attribute_name}" that is not specified for the conductor of coil {coil_name}.')
+                    # append value to sweeper dict
+                    dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
 
             # insert Jc fit value(s) depending on their fitting function (usual Bottura, CUDI1, CUDI3 for NbTi and Summers, Bordini for Nb3Sn)
-            Jc_dict = get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], strand_geometry=conductor_sample.strand_geometry,
-                                        Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0, Bc20=conductor_sample.Bc20,
-                                        sample_name=name, mag_name=self.data_parsim_conductor.GeneralParameters.magnet_name)
-            for name, val in Jc_dict.items():
+            Jc_dict_list = []
+            for conductor_sample in coil.conductorSamples:
+                # calculate the parameters for Jc fit for every conductor sample of this coil
+                Jc_dict = get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], coil_name=coil_name,
+                                  strand_geometry=conductor_sample.strand_geometry, Bc20=conductor_sample.Bc20,
+                                  Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0)
+                Jc_dict_list.append(Jc_dict)
+            # Calculate the average of values for each key across all dictionaries in the list
+            Jc_avg_dict = {key: sum(d[key] for d in Jc_dict_list) / len(Jc_dict_list) for key in Jc_dict_list[0]}
+            for name, val in Jc_avg_dict.items():
                 if val: dict_sweeper[sweeper_cond_name + 'Jc_fit.' + name] = val
 
-            # TODO
-            if self.groups_to_coil_length:
-                val = self.optimize_fCu_with_resistance_meas(conductor_sample, self.model_data.Conductors[idx], dict_sweeper)
-                dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = val
-
-    def optimize_fCu_with_resistance_meas(self, conductor_sample, original_conductor, dict_sweeper):
-        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-        f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
-
-        # define function to solve
-        def resistance_as_function_of_fCu(fCu, *args):
-            L, A_cond, temperature, mag_field, RRR, RRR_ref = args  # unpack arguments
-            numpy2d = np.vstack((temperature, mag_field, RRR, RRR_ref))  # create parameter v stack for c function
-            matpath = os.path.dirname(steammaterials.__file__)
-            CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
-            rho = CFUN_rhoCuNIST.evaluate(numpy2d)  # TODO check dimension (1x1 array)
-            return rho * L / (fCu * A_cond) * f_twist_pitch
-
-        # solve equation for fraction of Copper
-        args = (1, 0.2, 273, 0, 100, 1)  # TODO: copy from optimize_L_with_resistance_meas if working
-        if original_conductor.strand.Cu_noCu_in_strand:
-            initial_guess = [original_conductor.strand.Cu_noCu_in_strand]
-        else: initial_guess = [0.1]
-        fCu = fsolve(func=resistance_as_function_of_fCu, x0=initial_guess, args=args)
-        Cu_noCu = fCu[0] / (1 - fCu[0])
-        if Cu_noCu < 0.01:
-            Cu_noCu = 0.01  # TODO delete this and find cause of problem
-        return Cu_noCu
+            # optimize the fraction of copper with the resistance measurement at room temperature
+            # if flag_optimize_fCu:
+                # list_optimized_Cu_noCu = []
+                # for conductor_sample in coil.conductorSamples:
+                #     list_optimized_Cu_noCu.append(self.optimize_fCu_with_resistance_meas(coil.conductorSamples, self.model_data.Conductors[idx], dict_sweeper))
+                # dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = val
+
+    def optimize_fCu_with_resistance_meas(self, conductor_samples, original_conductor, dict_sweeper):
+        # # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+        # f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
+        #
+        # # define function to solve
+        # def resistance_as_function_of_fCu(fCu, *args):
+        #     L, A_cond, temperature, mag_field, RRR, RRR_ref = args  # unpack arguments
+        #     numpy2d = np.vstack((temperature, mag_field, RRR, RRR_ref))  # create parameter v stack for c function
+        #     matpath = os.path.dirname(steammaterials.__file__)
+        #     CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
+        #     rho = CFUN_rhoCuNIST.evaluate(numpy2d)  # TODO check dimension (1x1 array)
+        #     return rho * L / (fCu * A_cond) * f_twist_pitch
+        #
+        # # solve equation for fraction of Copper
+        # args = (1, 0.2, 273, 0, 100, 1)  # TODO: copy from optimize_L_with_resistance_meas if working
+        # if original_conductor.strand.Cu_noCu_in_strand:
+        #     initial_guess = [original_conductor.strand.Cu_noCu_in_strand]
+        # else: initial_guess = [0.1]
+        # fCu = fsolve(func=resistance_as_function_of_fCu, x0=initial_guess, args=args)
+        # Cu_noCu = fCu[0] / (1 - fCu[0])
+        # if Cu_noCu < 0.01:
+        #     Cu_noCu = 0.01  # TODO delete this and find cause of problem
+        # return Cu_noCu
+        pass
 
 
-
-def get_Jc_fit_params(original_conductor, strand_geometry, Tc0, Bc20, Ic_measurements, sample_name, mag_name):
+def get_Jc_fit_params(original_conductor, strand_geometry, Tc0, Bc20, Ic_measurements, coil_name):
     # TODO: use C-python-wrapper functions(see steam-materials-library) - ask Mariusz how to set it up (when it is implemented)
     if original_conductor.Jc_fit.type == 'Summers':
         # check inputs
-        if not original_conductor.strand.type: raise Exception(f'Strand type of conductor in coil {sample_name} is not specified in modelData.')
+        if not original_conductor.strand.type: raise Exception(
+            f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
         if len(Ic_measurements) > 1:
             # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
-            raise Exception(f'More then one Measurement for Summers fit provided for coil {sample_name}. Please only provide 1 or 0.')
+            raise Exception(
+                f'More then one Measurement for Summers fit provided for coil {coil_name}. Please only provide 1 or 0.')
         elif len(Ic_measurements) < 1:
-            warnings.warn(f'No Measurement for Summers fit provided for coil {sample_name}. Calculation of new Summers parameters will be skipped.')
+            warnings.warn(
+                f'No Measurement for Summers fit provided for coil {coil_name}. Calculation of new Summers parameters will be skipped.')
             return {}
         else:
             Ic_measurement = Ic_measurements[0]
-            if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-            if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {sample_name}.')
-            if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {sample_name}.')
-            if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-        
+            if not Ic_measurement.Ic: raise Exception(
+                f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not Ic_measurement.B_ref_Ic: raise Exception(
+                f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
+            if not Ic_measurement.T_ref_Ic: raise Exception(
+                f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
+            if not Ic_measurement.Cu_noCu_sample: raise Exception(
+                f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+
         # use parameters of modelData if they are not changed with the conductor database
         if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_Summers
         if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_Summers
 
         # calculate critical current density from critical current by using the area of
-        fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample+1)
+        fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample + 1)
         A = calc_strand_area(strand_geometry, original_conductor)
-        A_noCu = A * (1-fCu)
-        Jc_Tref_Bref = Ic_measurement.Ic/A_noCu
+        A_noCu = A * (1 - fCu)
+        Jc_Tref_Bref = Ic_measurement.Ic / A_noCu
 
         # search for the best C0  # TODO use np.linalg.solve?
         tol = 1e-6  # hardcoded
         if original_conductor.Jc_fit.Jc0_Summers:
             val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
             print(val_range)
-        else: val_range = [1e6, 1e14]
-        n_iterations = math.ceil(np.log((val_range[1]-val_range[0])/tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
+        else:
+            val_range = [1e6, 1e14]
+        n_iterations = math.ceil(
+            np.log((val_range[1] - val_range[0]) / tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
         for _ in range(n_iterations):
             try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
             tryJc_Summers = np.zeros(len(try_CO_Summers))
             # calculate Jc for every selected C0 value
             for j in range(len(try_CO_Summers)):
-                tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic, try_CO_Summers[j], Tc0, Bc20)
+                tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic,
+                                                       try_CO_Summers[j], Tc0, Bc20)
             # find indices of the list values that are higher than Jc_Tref_Bref
             tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
             if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
             # set new value range for net iteration
-            val_range = [try_CO_Summers[tempIdx[0]-1], try_CO_Summers[tempIdx[0]]]
-            C0 = try_CO_Summers[tempIdx[0]-1]
+            val_range = [try_CO_Summers[tempIdx[0] - 1], try_CO_Summers[tempIdx[0]]]
+            C0 = try_CO_Summers[tempIdx[0] - 1]
 
         return {
-                'Jc0_Summers': C0,
-                'Tc0_Summers': Tc0,
-                'Bc20_Summers': Bc20,
-                }
+            'Jc0_Summers': C0,
+            'Tc0_Summers': Tc0,
+            'Bc20_Summers': Bc20,
+        }
     elif original_conductor.Jc_fit.type == 'Bordini':
         # TODO use C-function when wrapper is available
         return {
-                'C0_Bordini': todo(),
-                'alpha_Bordini': todo(),
-                'Tc0_Bordini': todo(),
-                'Bc20_Bordini': todo(),
-                }
+            'C0_Bordini': todo(),
+            'alpha_Bordini': todo(),
+            'Tc0_Bordini': todo(),
+            'Bc20_Bordini': todo(),
+        }
     elif original_conductor.Jc_fit.type == 'CUDI1':
         # general equation for CUDI1: Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59)
 
         # depending on the number of critical current measurements, use different ways to calculate C1 and C2 parameter
         if len(Ic_measurements) not in [0, 1, 2]:
             # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
-            raise Exception(f'More then two measurements for CUDI1 fit provided in coil {sample_name}. Please only provide 2, 1 or 0 measurements.')
+            raise Exception(
+                f'More then two measurements for CUDI1 fit provided in coil {coil_name}. Please only provide 2, 1 or 0 measurements.')
         elif len(Ic_measurements) == 2:
             # if two measurements are specified, we have 2 equations and 2 unknowns -> system can be solved
 
             # check inputs and use parameters of modelData if they are not changed with the conductor database
             for Ic_measurement in Ic_measurements:
-                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
-                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
-                # if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-            if not original_conductor.cable.n_strands: raise Exception('No number of strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception('No Tc0 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception('No Bc02 specified in modelData of the conductor that should be changed.')
+                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                # if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not original_conductor.cable.n_strands: raise Exception(
+                'No number of strands specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception(
+                'No Tc0 specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception(
+                'No Bc02 specified in modelData of the conductor that should be changed.')
             if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
             if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
 
             # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable1 = Ic_measurements[0].Ic # TODO * original_conductor.cable.n_strands
-            Ic_cable2 = Ic_measurements[1].Ic # TODO * original_conductor.cable.n_strands
+            Ic_cable1 = Ic_measurements[0].Ic  # TODO * original_conductor.cable.n_strands
+            Ic_cable2 = Ic_measurements[1].Ic  # TODO * original_conductor.cable.n_strands
 
             # # # solve system of linear equations: A*x = b - redundant way
             # A = np.array([[1, Ic_measurements[0].B_ref_Ic], [1, Ic_measurements[1].B_ref_Ic]])
             # b_1 = Ic_cable1 / (1 - Ic_measurements[0].T_ref_Ic / Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** -0.59)
             # b_2 = Ic_cable2 / (1 - Ic_measurements[1].T_ref_Ic / Tc0 * (1 - Ic_measurements[1].B_ref_Ic / Bc20) ** -0.59)
             # b = np.array([b_1, b_2])
             # x = np.linalg.solve(A, b,)
@@ -503,49 +589,63 @@
                 Ic1, Ic2, T1, T2, Tc0, B1, B2, Bc20 = args
 
                 eq1 = Ic1 - (C1 + C2 * B1) * (1 - T1 / (Tc0 * (1 - B1 / Bc20) ** 0.59))
                 eq2 = Ic2 - (C1 + C2 * B2) * (1 - T2 / (Tc0 * (1 - B2 / Bc20) ** 0.59))
 
                 return [eq1, eq2]
 
-            initial_values = [787.327, -63.073]  # values come from magnet "MQML" in csv file "Strand and cable characteristics"
+            initial_values = [787.327,
+                              -63.073]  # values come from magnet "MQML" in csv file "Strand and cable characteristics"
             args = (Ic_cable1, Ic_cable2, Ic_measurements[0].T_ref_Ic, Ic_measurements[1].T_ref_Ic, Tc0,
                     Ic_measurements[0].B_ref_Ic, Ic_measurements[1].B_ref_Ic, Bc20)
             x = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_values, args=args)
 
             if len(x) == 2:
                 C1, C2 = x
             else:
-                raise Exception(f'No valid solution for CUDI1 fitting parameters C1 and C2 could be found for coil {sample_name}.')
+                raise Exception(
+                    f'No valid solution for CUDI1 fitting parameters C1 and C2 could be found for coil {coil_name}.')
         elif len(Ic_measurements) == 1:
             # if only one measurement is provided use one equation and the ratio of C1 and C2 according to modelData and warn the user
-            warnings.warn(f'Only one Measurement for CUDI1 fit provided for coil {sample_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
+            warnings.warn(
+                f'Only one Measurement for CUDI1 fit provided for coil {coil_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
 
             # check inputs and use parameters of modelData if they are not changed with the conductor database
-            if not Ic_measurements[0].Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-            if not Ic_measurements[0].B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
-            if not Ic_measurements[0].T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {sample_name}.')
-            # if not Ic_measurements[0].Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {sample_name}. Please check column name in step definition.')
-            if not original_conductor.cable.n_strands: raise Exception('No number of strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception('No Tc0 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception('No Bc02 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.C1_CUDI1: raise Exception('No C1_CUDI1 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.C2_CUDI1: raise Exception('No C2_CUDI1 specified in modelData of the conductor that should be changed.')
+            if not Ic_measurements[0].Ic: raise Exception(
+                f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not Ic_measurements[0].B_ref_Ic: raise Exception(
+                f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+            if not Ic_measurements[0].T_ref_Ic: raise Exception(
+                f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+            # if not Ic_measurements[0].Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+            if not original_conductor.cable.n_strands: raise Exception(
+                'No number of strands specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception(
+                'No Tc0 specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception(
+                'No Bc02 specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.C1_CUDI1: raise Exception(
+                'No C1_CUDI1 specified in modelData of the conductor that should be changed.')
+            if not original_conductor.Jc_fit.C2_CUDI1: raise Exception(
+                'No C2_CUDI1 specified in modelData of the conductor that should be changed.')
             if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
             if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
 
             # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable = Ic_measurements[0].Ic  # TODO why delete this "* original_conductor.cable.n_strands" - in csv we only use n_strands=1
+            Ic_cable = Ic_measurements[
+                0].Ic  # TODO why delete this "* original_conductor.cable.n_strands" - in csv we only use n_strands=1
 
             # try to read C1 over C2 ratio from modelData - if not existing use usual ratio for NbTi superconductors
             if not original_conductor.Jc_fit.C1_CUDI1 or not original_conductor.Jc_fit.C2_CUDI1:
-                warnings.warn(f'No C1 or C2 parameter defined in modelData for coil {sample_name}. Using usual ratio for NbTi superconductors.')
+                warnings.warn(
+                    f'No C1 or C2 parameter defined in modelData for coil {coil_name}. Using usual ratio for NbTi superconductors.')
                 # 787.327 and -63.073 are hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
                 # saving signed angle instead of ratio to keep track of signs - tan(angle_C1_C2) = C1/C2
-                angle_C1_C2 = math.atan2(787.327, -63.073)  # atan2 is a tangens calcualtion that also saves the sign of the angle depending on the quadrant
+                angle_C1_C2 = math.atan2(787.327,
+                                         -63.073)  # atan2 is a tangens calcualtion that also saves the sign of the angle depending on the quadrant
                 initial_guess = [787.327, -63.073]
             else:
                 angle_C1_C2 = math.atan2(original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1)
                 initial_guess = [original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1]
 
             def CUDI1_equation_fixed_ratio(C, *args):
                 C1, C2 = C
@@ -563,48 +663,102 @@
 
             # old approach with analytical solution
             # # Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59) where only C1 and C2 are unknown - second equation: tan(angle_C1_C2) = C1/C2
             # C2 = Ic_cable / (1 - Ic_measurements[0].T_ref_Ic / (Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** 0.59)) / (Ic_measurements[0].B_ref_Ic + math.tan(angle_C1_C2))
             # C1 = C2 * math.tan(angle_C1_C2)
         elif len(Ic_measurements) == 0:
             # if no measurement is provided use the usual ratio for NbTi superconductors and scale that value by cross section of superconductor and warn the user
-            warnings.warn(f'No Measurement for CUDI1 fit provided for coil {sample_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
+            warnings.warn(
+                f'No Measurement for CUDI1 fit provided for coil {coil_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
 
             # check inputs
-            if not original_conductor.cable.n_strands: raise Exception('No n_strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.strand.Cu_noCu_in_strand: raise Exception('No n_strands specified in modelData of the conductor that should be changed.')
+            if not original_conductor.cable.n_strands: raise Exception(
+                'No n_strands specified in modelData of the conductor that should be changed.')
+            if not original_conductor.strand.Cu_noCu_in_strand: raise Exception(
+                'No n_strands specified in modelData of the conductor that should be changed.')
 
             # hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
             # NOTE: cab...cable, str...strand, C1_cab = C1_str * nStrands  and  C1_str = C1_str_MB / A_MB * A_thisMagnet
             C1_per_square_meter_of_NbTi = 787.327 / 6.580e-08  # C1_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
             C2_per_square_meter_of_NbTi = -63.073 / 6.580e-08  # C2_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
 
             # scale it with the cross-section of superconductor
             strand_cross_section = calc_strand_area(strand_geometry, original_conductor)
-            fraction_of_superconductor = 1 / (original_conductor.strand.Cu_noCu_in_strand+1)
-            total_NbTi_area =  fraction_of_superconductor * strand_cross_section  # TODO why do i have to delete this? "* original_conductor.cable.n_strands" (AH97)
+            fraction_of_superconductor = 1 / (original_conductor.strand.Cu_noCu_in_strand + 1)
+            total_NbTi_area = fraction_of_superconductor * strand_cross_section  # TODO why do i have to delete this? "* original_conductor.cable.n_strands" (AH97)
             C1 = C1_per_square_meter_of_NbTi * total_NbTi_area
             C2 = C2_per_square_meter_of_NbTi * total_NbTi_area
 
         # check if values are real and not imaginary (e.g. when Bc20 is bigger than B_ref_Ic)
         if np.iscomplex(complex(C1)) or np.iscomplex(complex(C2)):
-            raise Exception(f'When calculating CUDI1 parameters (C1, C2) the values turned out to have an imaginary part. Please check the inputs.')
+            raise Exception(
+                f'When calculating CUDI1 parameters (C1, C2) the values turned out to have an imaginary part. Please check the inputs.')
 
         return {
             # TODO: shall we add a plausibility check - e.g. if the value will be changed by many orders of magnitude
             'Tc0_CUDI1': Tc0,
             'Bc20_CUDI1': Bc20,
             'C1_CUDI1': C1,
             'C2_CUDI1': C2,
-                }
+        }
+    else:
+        raise Exception(
+            f'No implementation for fit type "{original_conductor.Jc_fit.type}" defined in ParsimConductor.')
+
+
+def calc_C0_summers(new_conductor, original_conductor, coil_name):
+    # check inputs
+    Ic_measurement = new_conductor.Ic_measurements[0]
+    if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+    if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
+    if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
+    if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+
+    # use parameters of modelData if they are not changed with the conductor database
+    Tc0 = new_conductor.Tc0  # TODO should this be done like this with Tc0, or shall i take the avg before the calculation?
+    Bc20 = new_conductor.Bc20
+    if not Tc0:
+        Tc0 = original_conductor.Jc_fit.Tc0_Summers
+    if not Bc20:
+        Bc20 = original_conductor.Jc_fit.Bc20_Summers
+
+    # calculate critical current density from critical current
+    fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample + 1)
+    A = calc_strand_area(new_conductor.strand_geometry, original_conductor)
+    A_noCu = A * (1 - fCu)
+    Jc_Tref_Bref = Ic_measurement.Ic / A_noCu
+
+    # search for the best C0  # TODO use np.linalg.solve or method to use Jc c-func more easily
+    tol = 1e-6  # hardcoded
+    if original_conductor.Jc_fit.Jc0_Summers:
+        val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
+        print(val_range)
     else:
-        raise Exception(f'No implementation for fit type "{original_conductor.Jc_fit.type}" defined in ParsimConductor.')
+        val_range = [1e6, 1e14]
+    n_iterations = math.ceil(
+        np.log((val_range[1] - val_range[0]) / tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
+    for _ in range(n_iterations):
+        try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
+        tryJc_Summers = np.zeros(len(try_CO_Summers))
+        # calculate Jc for every selected C0 value
+        for j in range(len(try_CO_Summers)):
+            tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic, try_CO_Summers[j], Tc0, Bc20)
+        # find indices of the list values that are higher than Jc_Tref_Bref
+        tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
+        if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
+        # set new value range for net iteration
+        val_range = [try_CO_Summers[tempIdx[0] - 1], try_CO_Summers[tempIdx[0]]]
+        C0 = try_CO_Summers[tempIdx[0] - 1]
+    return C0
 
 
 def calc_strand_area(strand_geometry, original_conductor):
+    # check inputs
+    if not original_conductor.strand.type: raise Exception(f'Strand type is not specified in modelData.')
+    
     if original_conductor.strand.type == 'Round':
 
         # if diameter is not changed in conductor database, use the one form modeldata
         if not strand_geometry.diameter: diameter = original_conductor.strand.diameter
         else: diameter = strand_geometry.diameter
 
         # calculate area of circle
@@ -670,32 +824,68 @@
     return Jc_T_B
 
 
 def todo():
     #TODO make functions whereever this function is used
     return None
 
-def weight_list(val, weight_factors):
-    # if there is only one entry, dont calculate
-    if len(val) == 1:
-        return val[0]
-
-    # if no weight factor specified or if weight factor length is different, take the average
-    if not weight_factors or len(val) != len(weight_factors):
-        # TODO should an exception be raised when length is different?
-        weight_factors = [1.0 for _ in val]
-
-    # Normalize the weight_factors
-    weight_sum = sum(weight_factors)
-    normalized_weights = [w / weight_sum for w in weight_factors]
-
-    return sum([v * w for v, w in zip(val, normalized_weights)])
-
 def make_value_SI(val: float, dim: str):
     if dim in ['mm', 'mOhm', 'mV']:
         return val / 1000
     elif dim in ['m', 'T', 'K', 'Ohm', 'V', '', ' ', '-']:
         return val
     elif dim in ['kA', 'kV', 'km']:
         return val * 1000
+    elif dim in ['degC']:
+        return val + 273.15
     else:
         raise Exception(f'unknown physical unit "{dim}".')
+
+def setattr_to_list(list_instances, row, col_name, attr_name):
+    # get dimension from csv column name
+    dim = col_name[col_name.find('[') + 1:col_name.find(']')] if '[' in col_name else ''
+
+    # parse str into list or make single float to
+    if isinstance(row[col_name], str):
+        val_list = parse_str_to_list(row[col_name], only_float_list=True)
+    elif type(row[col_name]) in [float, int]:
+        val_list = [row[col_name] for _ in range(len(list_instances))]
+    else:
+        raise Exception(f'Unknown datatype in column "{col_name}".')
+
+    for val, instance in zip(val_list, list_instances):
+        rsetattr(instance, attr_name, make_value_SI(val, dim))
+
+def getattr_from_list(conductor_samples, sample_attribute_name, weight_factors):
+    # check if attribute is either set in all of the conductor_samples (return weighted values) or in none (return None)
+    attr_present = []
+    for con in conductor_samples:
+        if rgetattr(con, sample_attribute_name): attr_present.append(True)
+        else: attr_present.append(False)
+    if True in attr_present and False in attr_present:
+        raise Exception(f'The attribute "{sample_attribute_name}" is only set in a few instances of the ConductorSample list.')
+    if not all(attr_present):
+        return None
+
+    # read the values for the specific attribute for all the ConductorSample instances and store them in a list
+    val_list = []
+    for con in conductor_samples:
+        val_list.append(rgetattr(con, sample_attribute_name))
+
+    # if there is no weight_factors specified, weight them equally (average)
+    if not weight_factors:
+        weight_factors = [1.0 for _ in range(len(conductor_samples))]
+
+    # check if length is the same
+    if len(weight_factors) != len(val_list):
+        raise Exception(f'The length of the weight factors {len(weight_factors)} is not the same as the number of conductor samples {len(val_list)}.')
+
+    # Normalize the weight_factors
+    weight_sum = sum(weight_factors)
+    normalized_weights = [w / weight_sum for w in weight_factors]
+
+    # calculate weighting
+    return sum([v * w for v, w in zip(val_list, normalized_weights)])
+
+
+
+
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,101 @@
-strand_geometry.diameter:
-  - Ds
-  - Ds [m]
-  - Ds [mm]
-  - strand_diameter
-  - Strand diameter [m]
-  - Strand diameter [mm]
-Tc0:
-  - Tc0
-  - Tc0 [K]
-Bc20:
-  - Bc20
-  - Bc20 [T]
-strand_geometry.bare_width:
-  - bare strand width
-  - bare strand width [m]
-  - bare strand width [mm]
-  - strand width
-  - Bare strand width [m]
-  - Strand width [mm]
-strand_geometry.bare_height:
-  - bare strand height
-  - bare strand height [m]
-  - bare strand height [mm]
-  - strand height
-  - strand height [m]
-  - strand height [mm]
-  - Bare strand height [m]
-  - Strand height [mm]
-width:
-  - width [m]
-  - width [mm]
-  - width
-  - Width
-  - Width [m]
-  - Width [mm]
-strand_twist_pitch:
-  - Strand twist pitch
-  - strand_twist_pitch
-  - Strand twist-pitch [m]
-  - Strand twist-pitch [mm]
-  - Strand twist pitch [m]
-  - Strand twist pitch [mm]
-filament_twist_pitch:
-  - Filament twist pitch
-  - filament_twist_pitch
-  - Fil twist-pitch [mm]
-  - Fil twist-pitch [m]
-  - Filament twist pitch [m]
-  - Filament twist pitch [mm]
-RRR:
-  - coil RRR
-  - RRR
-  - Estimated coil RRR
-weight_factors:
-  - weight factor
-  - Weight factor
-Cu_noCu:
-  - Ave Cu/noCu
-  - Copper to non-Copper ratio
-  - Cu/noCu
-  - Cu_noCu
-coil_resistance_room_T:
-  - RT coil resistance [Ohm]
-Cu_noCu_resistance_meas:
-  - Cu/nocu from RT meas
-total_conductor_length:
-  - tot coil length [m]
+MainColumnNames:
+  magnet_name:
+    - Magnet
+    - Magnet Name
+    - magnet
+    - magnet name
+  coil_name:
+    - Coil
+    - Coil Name
+    - coil
+    - coil name
+ConductorSample:
+  strand_geometry.diameter:
+    - Ds
+    - Ds [m]
+    - Ds [mm]
+    - strand_diameter
+    - Strand diameter [m]
+    - Strand diameter [mm]
+  number_of_strands:
+    - Ns
+    - Ns [-]
+  Tc0:
+    - Tc0
+    - Tc0 [K]
+  Bc20:
+    - Bc20
+    - Bc20 [T]
+  strand_geometry.bare_width:
+    - bare strand width
+    - bare strand width [m]
+    - bare strand width [mm]
+    - strand width
+    - Bare strand width [m]
+    - Strand width [mm]
+  strand_geometry.bare_height:
+    - bare strand height
+    - bare strand height [m]
+    - bare strand height [mm]
+    - strand height
+    - strand height [m]
+    - strand height [mm]
+    - Bare strand height [m]
+    - Strand height [mm]
+  width:
+    - width [m]
+    - width [mm]
+    - width
+    - Width
+    - Width [m]
+    - Width [mm]
+  strand_twist_pitch:
+    - Strand twist pitch
+    - strand_twist_pitch
+    - Strand twist-pitch [m]
+    - Strand twist-pitch [mm]
+    - Strand twist pitch [m]
+    - Strand twist pitch [mm]
+  filament_twist_pitch:
+    - Filament twist pitch
+    - filament_twist_pitch
+    - Fil twist-pitch [mm]
+    - Fil twist-pitch [m]
+    - Filament twist pitch [m]
+    - Filament twist pitch [mm]
+  RRR:
+    - coil RRR
+    - RRR
+    - Estimated coil RRR
+  Cu_noCu:
+    - Ave Cu/noCu
+    - Copper to non-Copper ratio
+    - Cu/noCu
+    - Cu_noCu
+Coil:
+  coil_resistance_room_T:
+    - RT coil resistance [Ohm]
+  Cu_noCu_resistance_meas:
+    - Cu/nocu from RT meas
+  total_conductor_length:
+    - tot coil length [m]
+  T_ref_coil_resistance:
+    - RT coil resistance temperature [degC]
+  weight_factors:
+    - weight factor
+    - Weight factor
+  T_ref_RRR_low:
+    - T ref RRR low
+  T_ref_RRR_high:
+    - T ref RRR high
+
+
+
+
 
 # 'Number of strands': 'number_of_strands', 'number_of_strands': 'number_of_strands',
 # 'Height [m]': 'height', 'Height [mm]': 'height', 'height': 'height',
-# 'Cu noCu': 'Cu_noCu', 'Cu_noCu': 'Cu_noCu', 'Ave Cu/noCu': 'Cu_noCu',
 # 'F rho eff': 'f_rho_eff', 'f_rho_eff': 'f_rho_eff',
 # 'Ra [Ohm]': 'Ra',
-# 'Rc [Ohm]': 'Rc'
+# 'Rc [Ohm]': 'Rc'
+
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/plotters/PlotterSIGMA.py` & `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterSIGMA.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import matplotlib.patches as patches
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib.colors import LogNorm
 import matplotlib.cm as cm
 #from steam_sdk.plotters.PlotterRoxie import plotEdges
+from steam_sdk.utils.misc import displayWaitAndClose
+
 
 def plot_multiple_areas(ax, areas, color=None):
     """
     Functions takes in a list of area objects and plot them on axis ax.
     :param ax: Axis to create plots.
     :param areas: list of SIGMA area objects.
     :param color: Color of the object
@@ -65,15 +67,15 @@
         min_Bmod_error = abs(df["Bmod_error"]).min() * 1000
         myfile.write(f"{n1*n2} {mean_Bmod_error} {std_Bmod_error} {abs_mean_Bmod_error} {max_Bmod_error} {min_Bmod_error}\n")
         max_index = abs(df["Bmod_error"]).idxmax()
         print(f"Absolute Bmod error mean: {abs_mean_Bmod_error}")
 
         print(f"Absolute Bmod error mean max index : {max_index}")
 
-def plot_Bmod(df, map2d_name1, map2d_name2, fig, ax, type, xPos, yPos, xBarePos, yBarePos, iPos, cmap='plasma', plot_coil=False):
+def plot_Bmod(df, map2d_name1, map2d_name2, fig, ax, type, cmap='plasma'):
     fig.suptitle(f"Bmod: {map2d_name1} and {map2d_name2} (mT)")
     ax[0, 0].set_title(f"Bmod: {map2d_name1} (mT)")
     ax[0, 0].set_xlabel('x-coordinate/mm')
     ax[0, 0].set_ylabel('y-coordinate/mm')
     ax[0, 1].set_title(f"Bmod: {map2d_name2} (mT)")
     ax[0, 1].set_xlabel('x-coordinate/mm')
     ax[0, 1].set_ylabel('y-coordinate/mm')
@@ -101,20 +103,17 @@
 
         tpc1 = ax[0, 0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
         tpc2 = ax[0, 1].tripcolor(x, y, z2, shading='gouraud', cmap=cmap)
 
         fig.colorbar(tpc1)
         fig.colorbar(tpc2)
 
-    if plot_coil:
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0, 0])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0,1])
 
 
-def plot_B_mod_error(df, map2d_name1, map2d_name2, fig, ax, type, xPos, yPos, xBarePos, yBarePos, iPos, cmap='winter', plot_coil=False):
+def plot_B_mod_error(df, map2d_name1, map2d_name2, fig, ax, type, cmap='winter'):
     fig.suptitle(f"Bmod error: {map2d_name1} - {map2d_name2} (mT)")
     ax[0].set_title(f"Bmod error (mT)")
     ax[0].set_xlabel('x-coordinate/mm', fontsize=9)
     ax[0].set_ylabel('y-coordinate/mm', fontsize=9)
     ax[0].set_aspect("equal")
     ax[1].set_title(f"Bmod error scatter (mT)")
 
@@ -129,18 +128,17 @@
         y = np.array(df['y'].tolist())
         z1 = np.array(df['Bmod_error'].tolist())*1000
 
         np.random.seed(1234)  # fix seed for reproducibility
 
         tpc = ax[0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
         fig.colorbar(tpc)
-    if plot_coil:
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0])
 
-def plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig, ax, type, xPos, yPos, xBarePos, yBarePos, iPos, cmap='CMRmap', plot_coil=False):
+
+def plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig, ax, type, cmap='CMRmap'):
     fig.suptitle(f"Relative error: {map2d_name1} and {map2d_name2} (T)")
     ax[0, 0].set_aspect("equal")
     ax[0, 1].set_aspect("equal")
 
     ax[0, 0].set_title(f"Relative error Bx %")
     ax[0, 0].set_xlabel('x-coordinate/mm')
     ax[0, 0].set_ylabel('y-coordinate/mm')
@@ -169,19 +167,17 @@
         np.random.seed(1234)  # fix seed for reproducibility
 
         tpc1 = ax[0, 0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
         tpc2 = ax[0, 1].tripcolor(x, y, z2, shading='gouraud', cmap=cmap)
 
         fig.colorbar(tpc1)
         fig.colorbar(tpc2)
-    if plot_coil:
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0,0])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0,1])
 
-def plot_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, xPos, yPos, xBarePos, yBarePos, iPos, cmap='seismic', plot_coil=False):
+
+def plot_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
     fig.suptitle(f"Bx and By field: {map2d_name1} and {map2d_name2} (mT)", fontsize=12)
 
     ax[0, 0].set_title(f"Bx {map2d_name1} (mT)", fontsize=10)
     ax[0, 0].set_ylabel('y-coordinate/mm', fontsize=9)
     ax[0, 0].set_aspect("equal")
     ax[0, 1].set_aspect("equal")
     ax[1, 0].set_aspect("equal")
@@ -230,21 +226,17 @@
         tpc3 = ax[1, 0].tripcolor(x, y, Bx2, shading='gouraud', cmap=cmap)
         tpc4 = ax[1, 1].tripcolor(x, y, By2, shading='gouraud', cmap=cmap)
 
         fig.colorbar(tpc1, ax=ax[0, 0])
         fig.colorbar(tpc2, ax=ax[0, 1])
         fig.colorbar(tpc3, ax=ax[1, 0])
         fig.colorbar(tpc4, ax=ax[1, 1])
-    if plot_coil:
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0,0])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0,1])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[1,0])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[1,1])
 
-def plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, xPos, yPos, xBarePos, yBarePos, iPos, cmap='seismic', plot_coil=False):
+
+def plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
     fig.suptitle(f"Difference: {map2d_name1} - {map2d_name2} (mT)")
     ax[0, 0].set_title(f"Difference Bx (mT)")
     ax[0, 0].set_xlabel('x-coordinate/mm')
     ax[0, 0].set_ylabel('y-coordinate/mm')
     ax[0, 1].set_title(f"Difference By (mT)")
     ax[0, 1].set_xlabel('x-coordinate/mm')
     ax[0, 1].set_ylabel('y-coordinate/mm')
@@ -273,17 +265,14 @@
         np.random.seed(1234)  # fix seed for reproducibility
         tpc1 = ax[0, 0].tripcolor(x, y, diff_x, shading='gouraud', cmap=cmap)
         tpc2 = ax[0, 1].tripcolor(x, y, diff_y, shading='gouraud', cmap=cmap)
 
         fig.colorbar(tpc1, ax=ax[0, 0])
         fig.colorbar(tpc2, ax=ax[0, 1])
 
-    if plot_coil:
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0, 0])
-        plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax[0, 1])
 
 
 def get_df_map2d(map2d_file_path1, map2d_file_path2):
 
     df1 = pd.read_csv(map2d_file_path1, delim_whitespace=True)
     df2 = pd.read_csv(map2d_file_path2, delim_whitespace=True)
     df = pd.DataFrame()
@@ -302,53 +291,51 @@
     df["abs_err_x"] = abs(df["Bx1"] - df["Bx2"])
     df["abs_err_y"] = abs(df["By1"] - df["By2"])
     df["Bmod1"] = np.sqrt(df["Bx1"] ** 2 + df["By1"] ** 2)
     df["Bmod2"] = np.sqrt(df["Bx2"] ** 2 + df["By2"] ** 2)
     df["Bmod_error"] = df["Bmod1"] - df["Bmod2"]
     return df
 
-def generate_report_from_map2d(plot, map2d_file_path1, map2d_name1, map2d_file_path2, map2d_name2, type, roxie_data, n1, n2):
+def generate_report_from_map2d(plot, map2d_file_path1, map2d_name1, map2d_file_path2, map2d_name2, type):
     """
     Generate plots for comparing two map2d files. Method generates the following plots:
     Bmod fields, Bmod error, relative error Bx/By, Bx/By field, Bx/By error, absolut difference Bx/By
     :param map2d_file_path1: Path to map2d file nr 1
     :param map2d_name1: String name of map2d nr 1 (e.g SIGMA/ROXIE)
     :param map2d_file_path2: Path to map2d file nr 2
     :param map2d_name2: String name of map2d nr 1 (e.g SIGMA/ROXIE)
     :return: 
     """
     df=get_df_map2d(map2d_file_path1, map2d_file_path2)
     if plot:
-        xPos, yPos, xBarePos, yBarePos, iPos=plot_roxie_coil(roxie_data)
         fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
         fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
         fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
         fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
         fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
-        plot_Bmod(df, map2d_name1, map2d_name2, fig1, ax1, type, xPos, yPos, xBarePos, yBarePos, iPos)
-        plot_B_mod_error(df,map2d_name1, map2d_name2, fig2, ax2, type, xPos, yPos, xBarePos, yBarePos, iPos)
-        plot_Bx_By(df, map2d_name1, map2d_name2, fig3, ax3, type, xPos, yPos, xBarePos, yBarePos,iPos)
+        plot_Bmod(df, map2d_name1, map2d_name2, fig1, ax1, type)
+        plot_B_mod_error(df,map2d_name1, map2d_name2, fig2, ax2, type)
+        plot_Bx_By(df, map2d_name1, map2d_name2, fig3, ax3, type)
         try:
-            plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig4, ax4, type, xPos, yPos, xBarePos, yBarePos, iPos)
+            plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig4, ax4, type)
         except:
             print("Couldn't generate relative error plots.")
-        plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig5, ax5, type, xPos, yPos, xBarePos, yBarePos, iPos)
+        plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig5, ax5, type)
         print("----Bmod error description----- ")
         print(df["Bmod_error"].describe())
         print(df["Bmod_error"].nlargest(10))
 
         print("----Rel error x description----- ")
         print(df["rel_err_x"].describe())
         print(df["rel_err_x"].nlargest(10))
         print("----Rel error y description----- ")
         print(df["rel_err_y"].describe())
         print(df["rel_err_y"].nlargest(10))
-        #try_plot(df, map2d_name1, map2d_name2, fig6, fig6)
-    write_result_summary(df, n1, n2)
-    plt.show()
+        displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=10)
+        plt.close('all')
 
 def plot_roxie_coil(roxie_data):
     xPos = []
     yPos = []
     xBarePos = []
     yBarePos = []
     iPos = []
@@ -362,15 +349,14 @@
                             bare = halfTurn.corners.bare
                             xPos.append([insu.iH.x, insu.oH.x, insu.oLA.x, insu.iLA.x])
                             yPos.append([insu.iH.y, insu.oH.y, insu.oLA.y, insu.iLA.y])
                             xBarePos.append([bare.iH.x, bare.oH.x, bare.oLA.x, bare.iLA.x])
                             yBarePos.append([bare.iH.y, bare.oH.y, bare.oLA.y, bare.iLA.y])
                             iPos.append(block.current_sign)
     return (xPos, yPos, xBarePos, yBarePos, iPos)
-    #plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax)
 
 def plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax):
     # Plot edges
     for c, (cXPos, cYPos) in enumerate(zip(xPos, yPos)):
         pt1, pt2, pt3, pt4 = [cXPos[0]*1000, cYPos[0]*1000], [cXPos[1]*1000, cYPos[1]*1000], [cXPos[2]*1000, cYPos[2]*1000], [cXPos[3]*1000, cYPos[3]*1000]
         points = [pt1, pt2, pt3, pt4]*1000
         if iPos[c] > 0:
```

### Comparing `steam_sdk-2023.4.2/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.4.3/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.4.3/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.4.3/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.4.3/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.4.3/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/misc.py` & `steam-sdk-2023.4.3/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.4.3/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.4.3/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.4.3/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.4.3/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.4.3/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.4.3/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar` & `steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/steam-sing.jar`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.4.3/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.2/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.4.3/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,API,STEAM,SDK
+Keywords: STEAM,CERN,API,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.2/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.4.3/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 steam_sdk/postprocs/__init__.py
 steam_sdk/utils/MTF_reading_functions.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
 steam_sdk/utils/__init__.py
+steam_sdk/utils/builder_SIGMA_helpers.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_two_parameters.py
 steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
 steam_sdk/utils/misc.py
 steam_sdk/utils/parse_str_to_list.py
```

### Comparing `steam_sdk-2023.4.2/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.4.3/steam_sdk.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.4.8
+steam-pysigma==2023.4.15
```


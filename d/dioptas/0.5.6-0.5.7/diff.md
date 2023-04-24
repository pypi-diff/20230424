# Comparing `tmp/dioptas-0.5.6.tar.gz` & `tmp/dioptas-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Clemens\Documents\Programming\Python\Dioptas\dist\.tmp-n2j48r7e\dioptas-0.5.6.tar", last modified: Wed Nov 23 16:33:41 2022, max compression
+gzip compressed data, was "dioptas-0.5.7.tar", last modified: Mon Apr 24 14:21:08 2023, max compression
```

## Comparing `dioptas-0.5.6.tar` & `dioptas-0.5.7.tar`

### file list

```diff
@@ -1,339 +1,419 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/
--rw-rw-rw-   0        0        0     2615 2022-11-23 13:02:41.000000 dioptas-0.5.6/.gitattributes
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/.github/
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/.github/workflows/
--rw-rw-rw-   0        0        0     1735 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/CI_backend.yml
--rw-rw-rw-   0        0        0     1999 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/CI_batch.yml
--rw-rw-rw-   0        0        0     3336 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/CI_frontend.yml
--rw-rw-rw-   0        0        0     2093 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/CI_functional.yml
--rw-rw-rw-   0        0        0     2729 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/build_linux.yml
--rw-rw-rw-   0        0        0     2460 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/build_mac.yml
--rw-rw-rw-   0        0        0     2330 2022-11-23 13:02:41.000000 dioptas-0.5.6/.github/workflows/build_windows.yml
--rw-rw-rw-   0        0        0     2648 2022-11-23 13:02:41.000000 dioptas-0.5.6/.gitignore
--rw-rw-rw-   0        0        0     1033 2022-11-23 13:02:41.000000 dioptas-0.5.6/.travis.yml
--rw-rw-rw-   0        0        0       36 2022-11-23 13:02:41.000000 dioptas-0.5.6/Dioptas.py
--rw-rw-rw-   0        0        0     6456 2022-11-23 13:02:41.000000 dioptas-0.5.6/Dioptas.spec
--rw-rw-rw-   0        0        0      154 2022-11-23 16:05:02.000000 dioptas-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1395 2022-11-23 16:33:41.000000 dioptas-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2022-11-23 13:02:41.000000 dioptas-0.5.6/README.md
--rw-rw-rw-   0        0        0    22033 2022-11-23 16:19:43.000000 dioptas-0.5.6/changelog.rst
--rw-rw-rw-   0        0        0     1371 2022-11-23 13:02:41.000000 dioptas-0.5.6/circle.yml
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/conda_scripts/
--rw-rw-rw-   0        0        0      983 2022-11-23 13:02:41.000000 dioptas-0.5.6/conda_scripts/construct.yaml
--rw-rw-rw-   0        0        0       48 2022-11-23 13:02:41.000000 dioptas-0.5.6/conda_scripts/post_install_unix.sh
--rwxrwxrwx   0        0        0       67 2022-11-23 13:02:41.000000 dioptas-0.5.6/conda_scripts/post_install_windows.bat
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/conda_scripts/recipe/
--rw-rw-rw-   0        0        0     1127 2022-11-23 13:02:41.000000 dioptas-0.5.6/conda_scripts/recipe/meta.yaml
--rwxrwxrwx   0        0        0     1300 2022-11-23 13:02:41.000000 dioptas-0.5.6/create_executable.bat
--rw-rw-rw-   0        0        0       69 2022-11-23 13:02:41.000000 dioptas-0.5.6/create_executable.sh
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/
--rw-rw-rw-   0        0        0     2604 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/__init__.py
--rw-rw-rw-   0        0        0     7850 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/_desktop_shortcuts.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/controller/
--rw-rw-rw-   0        0        0    36139 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/CalibrationController.py
--rw-rw-rw-   0        0        0     4745 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/ConfigurationController.py
--rw-rw-rw-   0        0        0    14690 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/MainController.py
--rw-rw-rw-   0        0        0    20438 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/MaskController.py
--rw-rw-rw-   0        0        0     1172 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/controller/integration/
--rw-rw-rw-   0        0        0    16627 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/BackgroundController.py
--rw-rw-rw-   0        0        0    56792 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/BatchController.py
--rw-rw-rw-   0        0        0    15957 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/CorrectionController.py
--rw-rw-rw-   0        0        0     9155 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/EpicsController.py
--rw-rw-rw-   0        0        0    48531 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/ImageController.py
--rw-rw-rw-   0        0        0     3129 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/IntegrationController.py
--rw-rw-rw-   0        0        0     6592 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/OptionsController.py
--rw-rw-rw-   0        0        0    15772 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/OverlayController.py
--rw-rw-rw-   0        0        0    18707 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/PatternController.py
--rw-rw-rw-   0        0        0     1577 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/__init__.py
--rw-rw-rw-   0        0        0     1260 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/econfig.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/controller/integration/phase/
--rw-rw-rw-   0        0        0    18648 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/JcpdsEditorController.py
--rw-rw-rw-   0        0        0    13863 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/PhaseController.py
--rw-rw-rw-   0        0        0     5645 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInBatchController.py
--rw-rw-rw-   0        0        0     5734 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInCakeController.py
--rw-rw-rw-   0        0        0     6541 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInPatternController.py
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/controller/integration/phase/__init__.py
--rw-rw-rw-   0        0        0     2882 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/excepthook.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/model/
--rw-rw-rw-   0        0        0    14909 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/BatchModel.py
--rw-rw-rw-   0        0        0    40631 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/CalibrationModel.py
--rw-rw-rw-   0        0        0    34923 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/Configuration.py
--rw-rw-rw-   0        0        0    23592 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/DioptasModel.py
--rw-rw-rw-   0        0        0    34785 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/ImgModel.py
--rw-rw-rw-   0        0        0    11976 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/MaskModel.py
--rw-rw-rw-   0        0        0     4867 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/OverlayModel.py
--rw-rw-rw-   0        0        0     6225 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/PatternModel.py
--rw-rw-rw-   0        0        0    13966 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/PhaseModel.py
--rw-rw-rw-   0        0        0     1292 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/model/loader/
--rw-rw-rw-   0        0        0     1429 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/FabioLoader.py
--rw-rw-rw-   0        0        0     1941 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/KaraboLoader.py
--rw-rw-rw-   0        0        0     4852 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/LambdaLoader.py
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/__init__.py
--rw-rw-rw-   0        0        0     2096 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/hdf5Loader.py
--rw-rw-rw-   0        0        0    17952 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/loader/spe.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/model/util/
--rw-rw-rw-   0        0        0     2944 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/BackgroundExtraction.py
--rw-rw-rw-   0        0        0    14793 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/HelperModule.py
--rw-rw-rw-   0        0        0    14920 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/ImgCorrection.py
--rw-rw-rw-   0        0        0     4602 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/NewFileWatcher.py
--rw-rw-rw-   0        0        0    13833 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/Pattern.py
--rw-rw-rw-   0        0        0     1312 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/PeakShapes.py
--rw-rw-rw-   0        0        0     1164 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/__init__.py
--rw-rw-rw-   0        0        0     3027 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/calc.py
--rw-rw-rw-   0        0        0    23862 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/cif.py
--rw-rw-rw-   0        0        0    29427 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/cosmics.py
--rw-rw-rw-   0        0        0    37847 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/jcpds.py
--rw-rw-rw-   0        0        0     2776 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/signal.py
--rw-rw-rw-   0        0        0     2112 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/smooth_bruckner.f95
--rw-rw-rw-   0        0        0   794948 2022-11-23 13:05:43.000000 dioptas-0.5.6/dioptas/model/util/smooth_bruckner_cython.c
--rw-rw-rw-   0        0        0     2542 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/smooth_bruckner_cython.pyx
--rw-rw-rw-   0        0        0     2119 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/model/util/smooth_bruckner_python.py
--rw-rw-rw-   0        0        0     1324 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/paths.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/resources/
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/resources/calibrants/
--rw-rw-rw-   0        0        0     1427 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/AgBh.D
--rw-rw-rw-   0        0        0      747 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Al.D
--rw-rw-rw-   0        0        0      601 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Au.D
--rw-rw-rw-   0        0        0      711 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/C14H30O.D
--rw-rw-rw-   0        0        0     1255 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/CeO2.D
--rw-rw-rw-   0        0        0      749 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Cr2O3.D
--rw-rw-rw-   0        0        0      276 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/CrOx.D
--rw-rw-rw-   0        0        0      317 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/CuO.D
--rw-rw-rw-   0        0        0    41796 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/LaB6.D
--rw-rw-rw-   0        0        0     2623 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660a.D
--rw-rw-rw-   0        0        0     2623 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660b.D
--rw-rw-rw-   0        0        0     2639 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660c.D
--rw-rw-rw-   0        0        0      720 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/NaCl.D
--rw-rw-rw-   0        0        0      302 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Ni.D
--rw-rw-rw-   0        0        0     3492 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/PBBA.D
--rw-rw-rw-   0        0        0    20758 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si.D
--rw-rw-rw-   0        0        0      585 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640.D
--rw-rw-rw-   0        0        0      587 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640a.D
--rw-rw-rw-   0        0        0      581 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640b.D
--rw-rw-rw-   0        0        0      580 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640c.D
--rw-rw-rw-   0        0        0      587 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640d.D
--rw-rw-rw-   0        0        0      588 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640e.D
--rw-rw-rw-   0        0        0      852 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/TiO2.D
--rw-rw-rw-   0        0        0      644 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/ZnO.D
--rw-rw-rw-   0        0        0     1112 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/alpha_Al2O3.D
--rw-rw-rw-   0        0        0      960 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/cristobaltite.D
--rw-rw-rw-   0        0        0      743 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/calibrants/quartz.D
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/resources/data/
--rw-rw-rw-   0        0        0     6760 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/data/atomic_scattering_params.json
--rw-rw-rw-   0        0        0   120293 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/data/periodic_table.json
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/resources/icons/
--rw-rw-rw-   0        0        0      199 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/CreateICNS.src
--rw-rw-rw-   0        0        0   101959 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/arrow_down.ico
--rw-rw-rw-   0        0        0   101925 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/arrow_up.ico
--rw-rw-rw-   0        0        0     1741 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/delete.png
--rw-rw-rw-   0        0        0     3190 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/delete.svg
--rw-rw-rw-   0        0        0     4908 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/edit.png
--rw-rw-rw-   0        0        0     3434 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/edit.svg
--rw-rw-rw-   0        0        0   361999 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/icon.icns
--rw-rw-rw-   0        0        0    25821 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/icon.ico
--rw-rw-rw-   0        0        0    58861 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/icon.png
--rw-rw-rw-   0        0        0    97956 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/icon.svg
--rw-rw-rw-   0        0        0   168996 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/open.ico
--rw-rw-rw-   0        0        0   404086 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/reset.ico
--rw-rw-rw-   0        0        0   203590 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/reset_dark.ico
--rw-rw-rw-   0        0        0   191481 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/icons/save.ico
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/resources/style/
--rw-rw-rw-   0        0        0    11001 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/resources/style/stylesheet.qss
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/
--rw-rw-rw-   0        0        0       39 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/.coveragerc
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/Profiling/
--rw-rw-rw-   0        0        0     1026 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/Profiling/__init__.py
--rw-rw-rw-   0        0        0     2534 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/Profiling/profiling_cbn_correction.py
--rw-rw-rw-   0        0        0     1024 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/controller_tests/
--rw-rw-rw-   0        0        0     1022 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/__init__.py
--rw-rw-rw-   0        0        0     5166 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_BackgroundController.py
--rw-rw-rw-   0        0        0     8777 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part1.py
--rw-rw-rw-   0        0        0     9139 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part2.py
--rw-rw-rw-   0        0        0    10727 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part3.py
--rw-rw-rw-   0        0        0    14569 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_CalibrationController.py
--rw-rw-rw-   0        0        0     9930 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_ConfigurationController.py
--rw-rw-rw-   0        0        0     9044 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_CorrectionController.py
--rw-rw-rw-   0        0        0     4131 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_EpicsController.py
--rw-rw-rw-   0        0        0    14367 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_ImageController.py
--rw-rw-rw-   0        0        0     5237 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_IntegrationBackgroundController.py
--rw-rw-rw-   0        0        0    10464 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_IntegrationController.py
--rw-rw-rw-   0        0        0    13670 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_JcpdsEditorController.py
--rw-rw-rw-   0        0        0     6221 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_MaskController.py
--rw-rw-rw-   0        0        0     2656 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_OptionsController.py
--rw-rw-rw-   0        0        0    16500 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_OverlayController.py
--rw-rw-rw-   0        0        0     6357 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_PatternController.py
--rw-rw-rw-   0        0        0    13023 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseController.py
--rw-rw-rw-   0        0        0     5426 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseInCakeController.py
--rw-rw-rw-   0        0        0     7717 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseInPatternController.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/CbnCorrectionOptimization/
--rw-rw-rw-   0        0        0      336 2022-11-23 13:02:41.000000 dioptas-0.5.6/dioptas/tests/data/CbnCorrectionOptimization/LaB6_40keV side.poni
--rw-rw-rw-   0        0        0      340 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/CeO2_Pilatus1M.poni
--rw-rw-rw-   0        0        0    52093 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/CeO2_Pilatus1M.xy
--rw-rw-rw-   0        0        0      340 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/CeO2_Pilatus1M_2.poni
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/dummy1_1.txt
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/dummy1_2.txt
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/dummy2_1.txt
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run1/
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run1/dummy_1.txt
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run1/run_1_evt_2.0.txt
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run2/
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run2/dummy_1.txt
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/FileIterator/run2/run_2_evt_2.0.txt
--rw-rw-rw-   0        0        0      672 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/LaB6_40keV_MarCCD.poni
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/TransferCorrection/
--rw-rw-rw-   0        0        0      419 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/TransferCorrection/transfer.poni
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/cif/
--rw-rw-rw-   0        0        0    18720 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/Fe2O3_shelx.cif
--rw-rw-rw-   0        0        0     3421 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/ICSD_triclinic.cif
--rw-rw-rw-   0        0        0     4263 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/amcsd.cif
--rw-rw-rw-   0        0        0     4491 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/apatite.cif
--rw-rw-rw-   0        0        0     5657 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/fcc.cif
--rw-rw-rw-   0        0        0     1856 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/hcp.cif
--rw-rw-rw-   0        0        0     7033 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/cif/magnesiowustite.cif
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas/tests/data/distortion/
--rw-rw-rw-   0        0        0     7764 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/distortion/f4mnew.spline
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/
--rw-rw-rw-   0        0        0      941 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/FeGeO3_cpx.jcpds
--rw-rw-rw-   0        0        0      586 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/ag.jcpds
--rw-rw-rw-   0        0        0      426 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/ar.jcpds
--rw-rw-rw-   0        0        0      812 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/au_Anderson.jcpds
--rw-rw-rw-   0        0        0      325 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/au_mal_anders.jcpds
--rw-rw-rw-   0        0        0      407 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/au_mal_anders_vers2.jcpds
--rw-rw-rw-   0        0        0      521 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/mo.jcpds
--rw-rw-rw-   0        0        0      467 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/nanana.jcpds
--rw-rw-rw-   0        0        0      792 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/pt.jcpds
--rw-rw-rw-   0        0        0     1159 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/re.jcpds
--rw-rw-rw-   0        0        0     1154 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/jcpds/re_K0.jcpds
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/tests/data/lambda/
--rw-rw-rw-   0        0        0      444 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/lambda/L2.poni
--rw-rw-rw-   0        0        0     2445 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/pattern_001.chi
--rw-rw-rw-   0        0        0    45335 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/pattern_001.xy
--rw-rw-rw-   0        0        0    45335 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/pattern_002.xy
--rw-rw-rw-   0        0        0     1966 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/test.cif
--rw-rw-rw-   0        0        0     1007 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/data/wrong_file_format.txt
--rw-rw-rw-   0        0        0     2375 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/ehook.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/tests/functional_tests/
--rw-rw-rw-   0        0        0     1026 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/__init__.py
--rw-rw-rw-   0        0        0    38294 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_functional_JcpdsEditor.py
--rw-rw-rw-   0        0        0    32794 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_functional_integration.py
--rw-rw-rw-   0        0        0     3468 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_img_bg.py
--rw-rw-rw-   0        0        0    30892 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_save_and_load_project.py
--rw-rw-rw-   0        0        0     2999 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_scripts.py
--rw-rw-rw-   0        0        0     3580 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/functional_tests/test_userinterface.py
--rw-rw-rw-   0        0        0       51 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/pytest.ini
--rw-rw-rw-   0        0        0     2028 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/run_tests.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/tests/unit_tests/
--rw-rw-rw-   0        0        0     1022 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/__init__.py
--rw-rw-rw-   0        0        0     5167 2022-11-23 13:04:29.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_BatchModel.py
--rw-rw-rw-   0        0        0    25584 2022-11-23 13:04:29.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_CalibrationModel.py
--rw-rw-rw-   0        0        0    12241 2022-11-23 13:04:29.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_DioptasModel.py
--rw-rw-rw-   0        0        0     4566 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_FileNameIterator.py
--rw-rw-rw-   0        0        0     4456 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_HelperModule.py
--rw-rw-rw-   0        0        0    14782 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_ImgCorrections.py
--rw-rw-rw-   0        0        0    13253 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_ImgModel.py
--rw-rw-rw-   0        0        0     4938 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_Jcpds.py
--rw-rw-rw-   0        0        0     7203 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_MaskModel.py
--rw-rw-rw-   0        0        0     3103 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_NewFileInDirectoryWatcher.py
--rw-rw-rw-   0        0        0     2378 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_OverlayModel.py
--rw-rw-rw-   0        0        0     7916 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_Pattern.py
--rw-rw-rw-   0        0        0     3044 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_PatternModel.py
--rw-rw-rw-   0        0        0     4236 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_PhaseModel.py
--rw-rw-rw-   0        0        0     3639 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_background_extraction.py
--rw-rw-rw-   0        0        0      418 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_calc.py
--rw-rw-rw-   0        0        0     5274 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/unit_tests/test_cif.py
--rw-rw-rw-   0        0        0     2720 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/utility.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/tests/widget_tests/
--rw-rw-rw-   0        0        0     1022 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/widget_tests/__init__.py
--rw-rw-rw-   0        0        0     1914 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/widget_tests/test_BatchSurfaceWidget.py
--rw-rw-rw-   0        0        0     3163 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/widget_tests/test_ConfigurationWidget.py
--rw-rw-rw-   0        0        0     4857 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/tests/widget_tests/test_JcpdsEditorWidget.py
--rw-rw-rw-   0        0        0      181 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas/version.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/widgets/
--rw-rw-rw-   0        0        0    38362 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/CalibrationWidget.py
--rw-rw-rw-   0        0        0     5872 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/ConfigurationWidget.py
--rw-rw-rw-   0        0        0    11395 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/CustomWidgets.py
--rw-rw-rw-   0        0        0     6578 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/EpicsWidgets.py
--rw-rw-rw-   0        0        0     7647 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/MainWidget.py
--rw-rw-rw-   0        0        0     7408 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/MaskWidget.py
--rw-rw-rw-   0        0        0     8680 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/UtilityWidgets.py
--rw-rw-rw-   0        0        0     1024 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/widgets/integration/
--rw-rw-rw-   0        0        0    26457 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/BatchWidget.py
--rw-rw-rw-   0        0        0    10160 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/CustomWidgets.py
--rw-rw-rw-   0        0        0    22518 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/JcpdsEditorWidget.py
--rw-rw-rw-   0        0        0    20329 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/widgets/integration/control/
--rw-rw-rw-   0        0        0     9136 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/BackgroundWidget.py
--rw-rw-rw-   0        0        0    10595 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/CorrectionsWidget.py
--rw-rw-rw-   0        0        0     3473 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/ImageWidget.py
--rw-rw-rw-   0        0        0     7487 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/OptionsWidget.py
--rw-rw-rw-   0        0        0    15920 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/OverlayWidget.py
--rw-rw-rw-   0        0        0     2703 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/PatternWidget.py
--rw-rw-rw-   0        0        0    13461 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/PhaseWidget.py
--rw-rw-rw-   0        0        0     7658 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/control/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/widgets/integration/display/
--rw-rw-rw-   0        0        0     5566 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/display/ImgWidget.py
--rw-rw-rw-   0        0        0     6322 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/display/PatternWidget.py
--rw-rw-rw-   0        0        0     2143 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/display/StatusWidget.py
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/integration/display/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/
--rw-rw-rw-   0        0        0     5351 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/Custom3DAxis.py
--rw-rw-rw-   0        0        0    11942 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/ExLegendItem.py
--rw-rw-rw-   0        0        0    13099 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/HistogramLUTItem.py
--rw-rw-rw-   0        0        0    37239 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/ImgWidget.py
--rw-rw-rw-   0        0        0    23990 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/PatternWidget.py
--rw-rw-rw-   0        0        0     7019 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/SurfaceWidget.py
--rw-rw-rw-   0        0        0     1140 2022-11-23 13:02:42.000000 dioptas-0.5.6/dioptas/widgets/plot_widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas.egg-info/
--rw-rw-rw-   0        0        0     1395 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11570 2022-11-23 16:33:40.000000 dioptas-0.5.6/dioptas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-23 16:33:39.000000 dioptas-0.5.6/dioptas.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/docs/
--rw-rw-rw-   0        0        0      630 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/Makefile
--rwxrwxrwx   0        0        0      809 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/docs/source/
--rw-rw-rw-   0        0        0     7209 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/calibration.rst
--rw-rw-rw-   0        0        0     5601 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/conf.py
--rw-rw-rw-   0        0        0     3851 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/configurations_and_projects.rst
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/docs/source/images/
--rw-rw-rw-   0        0        0    21543 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/background_control.png
--rw-rw-rw-   0        0        0    42164 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/background_inspect.png
--rw-rw-rw-   0        0        0    24711 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/cor_control.png
--rw-rw-rw-   0        0        0     1370 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/erase_icon.png
--rw-rw-rw-   0        0        0     5229 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/image_widget_qa.png
--rw-rw-rw-   0        0        0     8803 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/integration_options.png
--rw-rw-rw-   0        0        0   277459 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/integration_view.png
--rw-rw-rw-   0        0        0   308439 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/integration_view_configuration.png
--rw-rw-rw-   0        0        0   476757 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/integration_view_modules.png
--rw-rw-rw-   0        0        0   307151 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/integration_view_project_controls.png
--rw-rw-rw-   0        0        0    39134 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/jcpds_editor.png
--rw-rw-rw-   0        0        0   230677 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/mask_view.png
--rw-rw-rw-   0        0        0      988 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/open_icon.png
--rw-rw-rw-   0        0        0    18513 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/overlay_control.png
--rw-rw-rw-   0        0        0     7865 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/peak_selection.png
--rw-rw-rw-   0        0        0   395077 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/peak_selection2.png
--rw-rw-rw-   0        0        0    18394 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/phase_control.png
--rw-rw-rw-   0        0        0     8244 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/refinement_options.png
--rw-rw-rw-   0        0        0     1351 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/save_icon.png
--rw-rw-rw-   0        0        0    16712 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/images/start_values.png
--rw-rw-rw-   0        0        0      457 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/index.rst
--rw-rw-rw-   0        0        0    19764 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/integration.rst
--rw-rw-rw-   0        0        0     3382 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/introduction.rst
--rw-rw-rw-   0        0        0     2768 2022-11-23 13:02:42.000000 dioptas-0.5.6/docs/source/mask.rst
--rw-rw-rw-   0        0        0    35799 2022-11-23 13:02:42.000000 dioptas-0.5.6/license.txt
--rw-rw-rw-   0        0        0      201 2022-11-23 13:02:42.000000 dioptas-0.5.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-11-23 16:33:41.000000 dioptas-0.5.6/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-23 13:02:42.000000 dioptas-0.5.6/scripts/__init__.py
--rw-rw-rw-   0        0        0      111 2022-11-23 13:02:42.000000 dioptas-0.5.6/scripts/dioptas.py
--rw-rw-rw-   0        0        0    12448 2022-11-23 13:02:42.000000 dioptas-0.5.6/scripts/dioptas_batch.py
--rw-rw-rw-   0        0        0      528 2022-11-23 13:02:42.000000 dioptas-0.5.6/scripts/dropbox_upload.py
--rw-rw-rw-   0        0        0     1904 2022-11-23 16:33:41.000000 dioptas-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      231 2022-11-23 13:02:42.000000 dioptas-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.105954 dioptas-0.5.7/
+-rw-rw-rw-   0        0        0     2615 2021-04-06 18:05:28.000000 dioptas-0.5.7/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.651762 dioptas-0.5.7/.github/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.702546 dioptas-0.5.7/.github/workflows/
+-rw-rw-rw-   0        0        0     2768 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/CI_backend.yml
+-rw-rw-rw-   0        0        0     1999 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/CI_batch.yml
+-rw-rw-rw-   0        0        0     3336 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/CI_frontend.yml
+-rw-rw-rw-   0        0        0     2093 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/CI_functional.yml
+-rw-rw-rw-   0        0        0     2759 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/build_linux.yml
+-rw-rw-rw-   0        0        0     2618 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/build_mac.yml
+-rw-rw-rw-   0        0        0     2484 2023-04-24 14:01:57.000000 dioptas-0.5.7/.github/workflows/build_windows.yml
+-rw-rw-rw-   0        0        0     2648 2023-04-24 14:01:57.000000 dioptas-0.5.7/.gitignore
+-rw-rw-rw-   0        0        0       36 2021-04-06 18:05:28.000000 dioptas-0.5.7/Dioptas.py
+-rw-rw-rw-   0        0        0     6456 2023-04-24 14:01:57.000000 dioptas-0.5.7/Dioptas.spec
+-rw-rw-rw-   0        0        0      154 2023-04-24 14:01:57.000000 dioptas-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3103 2023-04-24 14:21:08.105954 dioptas-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2023-04-24 14:01:57.000000 dioptas-0.5.7/README.md
+-rw-rw-rw-   0        0        0    22914 2023-04-24 14:01:57.000000 dioptas-0.5.7/changelog.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.702546 dioptas-0.5.7/conda_scripts/
+-rw-rw-rw-   0        0        0      983 2021-04-06 18:05:28.000000 dioptas-0.5.7/conda_scripts/construct.yaml
+-rw-rw-rw-   0        0        0       48 2021-04-06 18:05:28.000000 dioptas-0.5.7/conda_scripts/post_install_unix.sh
+-rwxrwxrwx   0        0        0       67 2021-04-06 18:05:28.000000 dioptas-0.5.7/conda_scripts/post_install_windows.bat
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.706546 dioptas-0.5.7/conda_scripts/recipe/
+-rw-rw-rw-   0        0        0     1127 2021-04-06 18:05:28.000000 dioptas-0.5.7/conda_scripts/recipe/meta.yaml
+-rwxrwxrwx   0        0        0     1300 2021-04-06 18:05:28.000000 dioptas-0.5.7/create_executable.bat
+-rw-rw-rw-   0        0        0       69 2021-04-06 18:05:28.000000 dioptas-0.5.7/create_executable.sh
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.714555 dioptas-0.5.7/dioptas/
+-rw-rw-rw-   0        0        0     2393 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/__init__.py
+-rw-rw-rw-   0        0        0     7850 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/_desktop_shortcuts.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.754544 dioptas-0.5.7/dioptas/controller/
+-rw-rw-rw-   0        0        0    36136 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/controller/CalibrationController.py
+-rw-rw-rw-   0        0        0     4745 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/controller/ConfigurationController.py
+-rw-rw-rw-   0        0        0    14690 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/MainController.py
+-rw-rw-rw-   0        0        0    20438 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/MaskController.py
+-rw-rw-rw-   0        0        0     1172 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.766942 dioptas-0.5.7/dioptas/controller/integration/
+-rw-rw-rw-   0        0        0    16627 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/controller/integration/BackgroundController.py
+-rw-rw-rw-   0        0        0    57466 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/controller/integration/BatchController.py
+-rw-rw-rw-   0        0        0    15957 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/CorrectionController.py
+-rw-rw-rw-   0        0        0     9155 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/EpicsController.py
+-rw-rw-rw-   0        0        0    48531 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/controller/integration/ImageController.py
+-rw-rw-rw-   0        0        0     3129 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/controller/integration/IntegrationController.py
+-rw-rw-rw-   0        0        0     6592 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/OptionsController.py
+-rw-rw-rw-   0        0        0    15772 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/OverlayController.py
+-rw-rw-rw-   0        0        0    18707 2022-02-21 14:09:38.000000 dioptas-0.5.7/dioptas/controller/integration/PatternController.py
+-rw-rw-rw-   0        0        0     1577 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/econfig.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.774992 dioptas-0.5.7/dioptas/controller/integration/phase/
+-rw-rw-rw-   0        0        0    18648 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/phase/JcpdsEditorController.py
+-rw-rw-rw-   0        0        0    13863 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/controller/integration/phase/PhaseController.py
+-rw-rw-rw-   0        0        0     5645 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInBatchController.py
+-rw-rw-rw-   0        0        0     5734 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInCakeController.py
+-rw-rw-rw-   0        0        0     6541 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInPatternController.py
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/controller/integration/phase/__init__.py
+-rw-rw-rw-   0        0        0     2882 2021-09-23 13:39:14.000000 dioptas-0.5.7/dioptas/excepthook.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.783682 dioptas-0.5.7/dioptas/model/
+-rw-rw-rw-   0        0        0    14957 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/BatchModel.py
+-rw-rw-rw-   0        0        0    40679 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/CalibrationModel.py
+-rw-rw-rw-   0        0        0    34923 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/Configuration.py
+-rw-rw-rw-   0        0        0    23592 2022-02-21 14:09:38.000000 dioptas-0.5.7/dioptas/model/DioptasModel.py
+-rw-rw-rw-   0        0        0    34785 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/ImgModel.py
+-rw-rw-rw-   0        0        0    11976 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/MaskModel.py
+-rw-rw-rw-   0        0        0     4867 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/OverlayModel.py
+-rw-rw-rw-   0        0        0     6225 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/PatternModel.py
+-rw-rw-rw-   0        0        0    13966 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/PhaseModel.py
+-rw-rw-rw-   0        0        0     1292 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.791690 dioptas-0.5.7/dioptas/model/loader/
+-rw-rw-rw-   0        0        0     1429 2021-06-22 11:05:07.000000 dioptas-0.5.7/dioptas/model/loader/FabioLoader.py
+-rw-rw-rw-   0        0        0     1941 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/model/loader/KaraboLoader.py
+-rw-rw-rw-   0        0        0     4852 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/loader/LambdaLoader.py
+-rw-rw-rw-   0        0        0        0 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/model/loader/__init__.py
+-rw-rw-rw-   0        0        0     2096 2021-06-22 11:05:07.000000 dioptas-0.5.7/dioptas/model/loader/hdf5Loader.py
+-rw-rw-rw-   0        0        0    17952 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/loader/spe.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.808028 dioptas-0.5.7/dioptas/model/util/
+-rw-rw-rw-   0        0        0     2944 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/model/util/BackgroundExtraction.py
+-rw-rw-rw-   0        0        0    14793 2022-09-15 17:48:56.000000 dioptas-0.5.7/dioptas/model/util/HelperModule.py
+-rw-rw-rw-   0        0        0    14920 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/util/ImgCorrection.py
+-rw-rw-rw-   0        0        0     4602 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/NewFileWatcher.py
+-rw-rw-rw-   0        0        0    13833 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/model/util/Pattern.py
+-rw-rw-rw-   0        0        0     1312 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/PeakShapes.py
+-rw-rw-rw-   0        0        0     1164 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/__init__.py
+-rw-rw-rw-   0        0        0     3027 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/model/util/calc.py
+-rw-rw-rw-   0        0        0    24845 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/util/cif.py
+-rw-rw-rw-   0        0        0    29427 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/util/cosmics.py
+-rw-rw-rw-   0        0        0    37847 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/model/util/jcpds.py
+-rw-rw-rw-   0        0        0     2776 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/signal.py
+-rw-rw-rw-   0        0        0     2112 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/smooth_bruckner.f95
+-rw-rw-rw-   0        0        0   795024 2023-04-24 09:23:58.000000 dioptas-0.5.7/dioptas/model/util/smooth_bruckner_cython.c
+-rw-rw-rw-   0        0        0     2542 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/smooth_bruckner_cython.pyx
+-rw-rw-rw-   0        0        0     2119 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/model/util/smooth_bruckner_python.py
+-rw-rw-rw-   0        0        0     1324 2021-09-23 13:36:36.000000 dioptas-0.5.7/dioptas/paths.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.661800 dioptas-0.5.7/dioptas/resources/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.835872 dioptas-0.5.7/dioptas/resources/calibrants/
+-rw-rw-rw-   0        0        0     1427 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/AgBh.D
+-rw-rw-rw-   0        0        0      747 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Al.D
+-rw-rw-rw-   0        0        0      601 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Au.D
+-rw-rw-rw-   0        0        0      711 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/C14H30O.D
+-rw-rw-rw-   0        0        0     1255 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/CeO2.D
+-rw-rw-rw-   0        0        0      749 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Cr2O3.D
+-rw-rw-rw-   0        0        0      276 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/CrOx.D
+-rw-rw-rw-   0        0        0      317 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/CuO.D
+-rw-rw-rw-   0        0        0    41796 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/LaB6.D
+-rw-rw-rw-   0        0        0     2623 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660a.D
+-rw-rw-rw-   0        0        0     2623 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660b.D
+-rw-rw-rw-   0        0        0     2639 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660c.D
+-rw-rw-rw-   0        0        0      720 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/NaCl.D
+-rw-rw-rw-   0        0        0      302 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Ni.D
+-rw-rw-rw-   0        0        0     3492 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/PBBA.D
+-rw-rw-rw-   0        0        0    20758 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si.D
+-rw-rw-rw-   0        0        0      585 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640.D
+-rw-rw-rw-   0        0        0      587 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640a.D
+-rw-rw-rw-   0        0        0      581 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640b.D
+-rw-rw-rw-   0        0        0      580 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640c.D
+-rw-rw-rw-   0        0        0      587 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640d.D
+-rw-rw-rw-   0        0        0      588 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640e.D
+-rw-rw-rw-   0        0        0      852 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/TiO2.D
+-rw-rw-rw-   0        0        0      644 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/ZnO.D
+-rw-rw-rw-   0        0        0     1112 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/alpha_Al2O3.D
+-rw-rw-rw-   0        0        0      960 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/cristobaltite.D
+-rw-rw-rw-   0        0        0      743 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/calibrants/quartz.D
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.839873 dioptas-0.5.7/dioptas/resources/data/
+-rw-rw-rw-   0        0        0     6760 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/data/atomic_scattering_params.json
+-rw-rw-rw-   0        0        0   120293 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/data/periodic_table.json
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.855867 dioptas-0.5.7/dioptas/resources/icons/
+-rw-rw-rw-   0        0        0      199 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/CreateICNS.src
+-rw-rw-rw-   0        0        0   101959 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/arrow_down.ico
+-rw-rw-rw-   0        0        0   101925 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/arrow_up.ico
+-rw-rw-rw-   0        0        0     1741 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/delete.png
+-rw-rw-rw-   0        0        0     3190 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/delete.svg
+-rw-rw-rw-   0        0        0     4908 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/edit.png
+-rw-rw-rw-   0        0        0     3434 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/edit.svg
+-rw-rw-rw-   0        0        0   361999 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/icon.icns
+-rw-rw-rw-   0        0        0    25821 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/icon.ico
+-rw-rw-rw-   0        0        0    58861 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/icon.png
+-rw-rw-rw-   0        0        0    97956 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/icon.svg
+-rw-rw-rw-   0        0        0   168996 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/open.ico
+-rw-rw-rw-   0        0        0   404086 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/reset.ico
+-rw-rw-rw-   0        0        0   203590 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/reset_dark.ico
+-rw-rw-rw-   0        0        0   191481 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/resources/icons/save.ico
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.855867 dioptas-0.5.7/dioptas/resources/style/
+-rw-rw-rw-   0        0        0    11001 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/resources/style/stylesheet.qss
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.859866 dioptas-0.5.7/dioptas/tests/
+-rw-rw-rw-   0        0        0       39 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/.coveragerc
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.863880 dioptas-0.5.7/dioptas/tests/Profiling/
+-rw-rw-rw-   0        0        0     1026 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/Profiling/__init__.py
+-rw-rw-rw-   0        0        0     2534 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/Profiling/profiling_cbn_correction.py
+-rw-rw-rw-   0        0        0     1024 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.883894 dioptas-0.5.7/dioptas/tests/controller_tests/
+-rw-rw-rw-   0        0        0     1022 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/__init__.py
+-rw-rw-rw-   0        0        0     5166 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_BackgroundController.py
+-rw-rw-rw-   0        0        0     9803 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part1.py
+-rw-rw-rw-   0        0        0    10150 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part2.py
+-rw-rw-rw-   0        0        0    11753 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part3.py
+-rw-rw-rw-   0        0        0     3743 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part4.py
+-rw-rw-rw-   0        0        0    14569 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_CalibrationController.py
+-rw-rw-rw-   0        0        0     9930 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_ConfigurationController.py
+-rw-rw-rw-   0        0        0     9044 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_CorrectionController.py
+-rw-rw-rw-   0        0        0     4131 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_EpicsController.py
+-rw-rw-rw-   0        0        0    14367 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_ImageController.py
+-rw-rw-rw-   0        0        0     5237 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_IntegrationBackgroundController.py
+-rw-rw-rw-   0        0        0    10464 2022-02-28 13:18:56.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_IntegrationController.py
+-rw-rw-rw-   0        0        0    13670 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_JcpdsEditorController.py
+-rw-rw-rw-   0        0        0     6221 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_MaskController.py
+-rw-rw-rw-   0        0        0     2656 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_OptionsController.py
+-rw-rw-rw-   0        0        0    16500 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_OverlayController.py
+-rw-rw-rw-   0        0        0     6357 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_PatternController.py
+-rw-rw-rw-   0        0        0    13023 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseController.py
+-rw-rw-rw-   0        0        0     5426 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseInCakeController.py
+-rw-rw-rw-   0        0        0     7717 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseInPatternController.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.896114 dioptas-0.5.7/dioptas/tests/data/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.896114 dioptas-0.5.7/dioptas/tests/data/CbnCorrectionOptimization/
+-rw-rw-rw-   0        0        0      336 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/CbnCorrectionOptimization/LaB6_40keV side.poni
+-rw-rw-rw-   0        0        0      340 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/CeO2_Pilatus1M.poni
+-rw-rw-rw-   0        0        0    52093 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/data/CeO2_Pilatus1M.xy
+-rw-rw-rw-   0        0        0      340 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/CeO2_Pilatus1M_2.poni
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.900117 dioptas-0.5.7/dioptas/tests/data/FileIterator/
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/dummy1_1.txt
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/dummy1_2.txt
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/dummy2_1.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.904177 dioptas-0.5.7/dioptas/tests/data/FileIterator/run1/
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:28.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/run1/dummy_1.txt
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/run1/run_1_evt_2.0.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.904177 dioptas-0.5.7/dioptas/tests/data/FileIterator/run2/
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/run2/dummy_1.txt
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/FileIterator/run2/run_2_evt_2.0.txt
+-rw-rw-rw-   0        0        0      672 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/LaB6_40keV_MarCCD.poni
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.908114 dioptas-0.5.7/dioptas/tests/data/TransferCorrection/
+-rw-rw-rw-   0        0        0      419 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/TransferCorrection/transfer.poni
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.920114 dioptas-0.5.7/dioptas/tests/data/cif/
+-rw-rw-rw-   0        0        0    18720 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/Fe2O3_shelx.cif
+-rw-rw-rw-   0        0        0     3421 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/ICSD_triclinic.cif
+-rw-rw-rw-   0        0        0     3400 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/data/cif/ICSD_triclinic_without_cell_volume.cif
+-rw-rw-rw-   0        0        0     4263 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/amcsd.cif
+-rw-rw-rw-   0        0        0     4491 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/apatite.cif
+-rw-rw-rw-   0        0        0     5657 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/fcc.cif
+-rw-rw-rw-   0        0        0     1856 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/hcp.cif
+-rw-rw-rw-   0        0        0     7033 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/cif/magnesiowustite.cif
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.920114 dioptas-0.5.7/dioptas/tests/data/distortion/
+-rw-rw-rw-   0        0        0     7764 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/distortion/f4mnew.spline
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.937012 dioptas-0.5.7/dioptas/tests/data/jcpds/
+-rw-rw-rw-   0        0        0      941 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/FeGeO3_cpx.jcpds
+-rw-rw-rw-   0        0        0      586 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/ag.jcpds
+-rw-rw-rw-   0        0        0      426 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/ar.jcpds
+-rw-rw-rw-   0        0        0      812 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/au_Anderson.jcpds
+-rw-rw-rw-   0        0        0      325 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/au_mal_anders.jcpds
+-rw-rw-rw-   0        0        0      407 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/au_mal_anders_vers2.jcpds
+-rw-rw-rw-   0        0        0      521 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/mo.jcpds
+-rw-rw-rw-   0        0        0      467 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/nanana.jcpds
+-rw-rw-rw-   0        0        0      792 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/pt.jcpds
+-rw-rw-rw-   0        0        0     1159 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/re.jcpds
+-rw-rw-rw-   0        0        0     1154 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/jcpds/re_K0.jcpds
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.937012 dioptas-0.5.7/dioptas/tests/data/lambda/
+-rw-rw-rw-   0        0        0      444 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/tests/data/lambda/L2.poni
+-rw-rw-rw-   0        0        0     2445 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/pattern_001.chi
+-rw-rw-rw-   0        0        0    45335 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/pattern_001.xy
+-rw-rw-rw-   0        0        0    45335 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/pattern_002.xy
+-rw-rw-rw-   0        0        0     1966 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/test.cif
+-rw-rw-rw-   0        0        0     1007 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/data/wrong_file_format.txt
+-rw-rw-rw-   0        0        0     2375 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/ehook.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.944566 dioptas-0.5.7/dioptas/tests/functional_tests/
+-rw-rw-rw-   0        0        0     1026 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/functional_tests/__init__.py
+-rw-rw-rw-   0        0        0    38294 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_functional_JcpdsEditor.py
+-rw-rw-rw-   0        0        0    32794 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_functional_integration.py
+-rw-rw-rw-   0        0        0     3468 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_img_bg.py
+-rw-rw-rw-   0        0        0    30892 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_save_and_load_project.py
+-rw-rw-rw-   0        0        0     2999 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_scripts.py
+-rw-rw-rw-   0        0        0     3580 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/functional_tests/test_userinterface.py
+-rw-rw-rw-   0        0        0       51 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/pytest.ini
+-rw-rw-rw-   0        0        0     2028 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/run_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.964602 dioptas-0.5.7/dioptas/tests/unit_tests/
+-rw-rw-rw-   0        0        0     1022 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/unit_tests/__init__.py
+-rw-rw-rw-   0        0        0     5240 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_BatchModel.py
+-rw-rw-rw-   0        0        0    22298 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_CalibrationModel.py
+-rw-rw-rw-   0        0        0    11790 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_DioptasModel.py
+-rw-rw-rw-   0        0        0     4090 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_FileNameIterator.py
+-rw-rw-rw-   0        0        0     3980 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_HelperModule.py
+-rw-rw-rw-   0        0        0    14312 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_ImgCorrections.py
+-rw-rw-rw-   0        0        0    11333 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_ImgModel.py
+-rw-rw-rw-   0        0        0     4111 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_Jcpds.py
+-rw-rw-rw-   0        0        0     5787 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_MaskModel.py
+-rw-rw-rw-   0        0        0     2628 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_NewFileInDirectoryWatcher.py
+-rw-rw-rw-   0        0        0     2038 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_OverlayModel.py
+-rw-rw-rw-   0        0        0     6678 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_Pattern.py
+-rw-rw-rw-   0        0        0     2653 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_PatternModel.py
+-rw-rw-rw-   0        0        0     3765 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_PhaseModel.py
+-rw-rw-rw-   0        0        0     3286 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_background_extraction.py
+-rw-rw-rw-   0        0        0      311 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_calc.py
+-rw-rw-rw-   0        0        0     4921 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/unit_tests/test_cif.py
+-rw-rw-rw-   0        0        0     2720 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/tests/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.972868 dioptas-0.5.7/dioptas/tests/widget_tests/
+-rw-rw-rw-   0        0        0     1022 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/widget_tests/__init__.py
+-rw-rw-rw-   0        0        0     1914 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/tests/widget_tests/test_BatchSurfaceWidget.py
+-rw-rw-rw-   0        0        0     3163 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/widget_tests/test_ConfigurationWidget.py
+-rw-rw-rw-   0        0        0     4857 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/tests/widget_tests/test_JcpdsEditorWidget.py
+-rw-rw-rw-   0        0        0      164 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas/version.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.984369 dioptas-0.5.7/dioptas/widgets/
+-rw-rw-rw-   0        0        0    38362 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/CalibrationWidget.py
+-rw-rw-rw-   0        0        0     5872 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/ConfigurationWidget.py
+-rw-rw-rw-   0        0        0    11395 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/CustomWidgets.py
+-rw-rw-rw-   0        0        0     6578 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/EpicsWidgets.py
+-rw-rw-rw-   0        0        0     7647 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/MainWidget.py
+-rw-rw-rw-   0        0        0     7408 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/MaskWidget.py
+-rw-rw-rw-   0        0        0     8680 2021-05-05 10:06:44.000000 dioptas-0.5.7/dioptas/widgets/UtilityWidgets.py
+-rw-rw-rw-   0        0        0     1024 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.988377 dioptas-0.5.7/dioptas/widgets/integration/
+-rw-rw-rw-   0        0        0    26457 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/BatchWidget.py
+-rw-rw-rw-   0        0        0    10160 2022-02-21 14:09:38.000000 dioptas-0.5.7/dioptas/widgets/integration/CustomWidgets.py
+-rw-rw-rw-   0        0        0    22518 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/JcpdsEditorWidget.py
+-rw-rw-rw-   0        0        0    20329 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.996374 dioptas-0.5.7/dioptas/widgets/integration/control/
+-rw-rw-rw-   0        0        0     9136 2022-02-28 14:08:12.000000 dioptas-0.5.7/dioptas/widgets/integration/control/BackgroundWidget.py
+-rw-rw-rw-   0        0        0    10595 2022-02-28 14:08:12.000000 dioptas-0.5.7/dioptas/widgets/integration/control/CorrectionsWidget.py
+-rw-rw-rw-   0        0        0     3473 2022-02-28 14:08:12.000000 dioptas-0.5.7/dioptas/widgets/integration/control/ImageWidget.py
+-rw-rw-rw-   0        0        0     7487 2022-02-28 14:08:12.000000 dioptas-0.5.7/dioptas/widgets/integration/control/OptionsWidget.py
+-rw-rw-rw-   0        0        0    15920 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/control/OverlayWidget.py
+-rw-rw-rw-   0        0        0     2703 2022-02-28 14:08:12.000000 dioptas-0.5.7/dioptas/widgets/integration/control/PatternWidget.py
+-rw-rw-rw-   0        0        0    13461 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/control/PhaseWidget.py
+-rw-rw-rw-   0        0        0     7658 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/integration/control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.996374 dioptas-0.5.7/dioptas/widgets/integration/display/
+-rw-rw-rw-   0        0        0     5566 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/integration/display/ImgWidget.py
+-rw-rw-rw-   0        0        0     6322 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/integration/display/PatternWidget.py
+-rw-rw-rw-   0        0        0     2143 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/integration/display/StatusWidget.py
+-rw-rw-rw-   0        0        0        0 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/integration/display/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.004378 dioptas-0.5.7/dioptas/widgets/plot_widgets/
+-rw-rw-rw-   0        0        0     5351 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/Custom3DAxis.py
+-rw-rw-rw-   0        0        0    11942 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/ExLegendItem.py
+-rw-rw-rw-   0        0        0    13099 2021-11-08 12:42:38.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/HistogramLUTItem.py
+-rw-rw-rw-   0        0        0    37236 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/ImgWidget.py
+-rw-rw-rw-   0        0        0    23990 2023-04-24 14:01:57.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/PatternWidget.py
+-rw-rw-rw-   0        0        0     7019 2022-02-21 14:09:21.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/SurfaceWidget.py
+-rw-rw-rw-   0        0        0     1140 2021-04-06 18:05:29.000000 dioptas-0.5.7/dioptas/widgets/plot_widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.746649 dioptas-0.5.7/dioptas.egg-info/
+-rw-rw-rw-   0        0        0     3103 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14694 2023-04-24 14:21:07.000000 dioptas-0.5.7/dioptas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-24 14:21:04.000000 dioptas-0.5.7/dioptas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.004378 dioptas-0.5.7/docs/
+-rw-rw-rw-   0        0        0      630 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/Makefile
+-rwxrwxrwx   0        0        0      809 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.012378 dioptas-0.5.7/docs/source/
+-rw-rw-rw-   0        0        0     7209 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/calibration.rst
+-rw-rw-rw-   0        0        0     5601 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3851 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/configurations_and_projects.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.041029 dioptas-0.5.7/docs/source/images/
+-rw-rw-rw-   0        0        0    21543 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/background_control.png
+-rw-rw-rw-   0        0        0    42164 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/background_inspect.png
+-rw-rw-rw-   0        0        0    24711 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/cor_control.png
+-rw-rw-rw-   0        0        0     1370 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/erase_icon.png
+-rw-rw-rw-   0        0        0     5229 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/image_widget_qa.png
+-rw-rw-rw-   0        0        0     8803 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/integration_options.png
+-rw-rw-rw-   0        0        0   277459 2021-04-06 18:05:29.000000 dioptas-0.5.7/docs/source/images/integration_view.png
+-rw-rw-rw-   0        0        0   308439 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/integration_view_configuration.png
+-rw-rw-rw-   0        0        0   476757 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/integration_view_modules.png
+-rw-rw-rw-   0        0        0   307151 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/integration_view_project_controls.png
+-rw-rw-rw-   0        0        0    39134 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/jcpds_editor.png
+-rw-rw-rw-   0        0        0   230677 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/mask_view.png
+-rw-rw-rw-   0        0        0      988 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/open_icon.png
+-rw-rw-rw-   0        0        0    18513 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/overlay_control.png
+-rw-rw-rw-   0        0        0     7865 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/peak_selection.png
+-rw-rw-rw-   0        0        0   395077 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/peak_selection2.png
+-rw-rw-rw-   0        0        0    18394 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/phase_control.png
+-rw-rw-rw-   0        0        0     8244 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/refinement_options.png
+-rw-rw-rw-   0        0        0     1351 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/save_icon.png
+-rw-rw-rw-   0        0        0    16712 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/images/start_values.png
+-rw-rw-rw-   0        0        0      457 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0    19764 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/integration.rst
+-rw-rw-rw-   0        0        0     3382 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/introduction.rst
+-rw-rw-rw-   0        0        0     2768 2021-04-06 18:05:30.000000 dioptas-0.5.7/docs/source/mask.rst
+-rw-rw-rw-   0        0        0    35799 2021-04-06 18:05:30.000000 dioptas-0.5.7/license.txt
+-rw-rw-rw-   0        0        0      201 2023-04-24 14:01:57.000000 dioptas-0.5.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.041029 dioptas-0.5.7/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:01:57.000000 dioptas-0.5.7/scripts/__init__.py
+-rw-rw-rw-   0        0        0      111 2023-04-24 14:01:57.000000 dioptas-0.5.7/scripts/dioptas.py
+-rw-rw-rw-   0        0        0    12448 2023-04-24 14:01:57.000000 dioptas-0.5.7/scripts/dioptas_batch.py
+-rw-rw-rw-   0        0        0      528 2021-04-06 18:05:30.000000 dioptas-0.5.7/scripts/dropbox_upload.py
+-rw-rw-rw-   0        0        0     1902 2023-04-24 14:21:08.122248 dioptas-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-04-24 14:01:57.000000 dioptas-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.674159 dioptas-0.5.7/venv/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.674159 dioptas-0.5.7/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.682529 dioptas-0.5.7/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.674159 dioptas-0.5.7/venv/Lib/site-packages/Cython/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.045029 dioptas-0.5.7/venv/Lib/site-packages/Cython/Runtime/
+-rw-rw-rw-   0        0        0     6279 2023-04-24 09:25:43.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Runtime/refnanny.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.053036 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/
+-rw-rw-rw-   0        0        0     4338 2023-04-24 09:25:43.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/CConvert.pyx
+-rw-rw-rw-   0        0        0     1893 2023-04-24 09:25:43.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/CpdefEnums.pyx
+-rw-rw-rw-   0        0        0     6098 2023-04-24 09:25:43.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/CppConvert.pyx
+-rw-rw-rw-   0        0        0    49749 2023-04-24 09:25:43.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/MemoryView.pyx
+-rw-rw-rw-   0        0        0      152 2023-04-24 09:25:44.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/TestCyUtilityLoader.pyx
+-rw-rw-rw-   0        0        0     1595 2023-04-24 09:25:44.000000 dioptas-0.5.7/venv/Lib/site-packages/Cython/Utility/TestCythonScope.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.679525 dioptas-0.5.7/venv/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.678156 dioptas-0.5.7/venv/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.678156 dioptas-0.5.7/venv/Lib/site-packages/numpy/core/tests/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.678156 dioptas-0.5.7/venv/Lib/site-packages/numpy/core/tests/examples/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.053036 dioptas-0.5.7/venv/Lib/site-packages/numpy/core/tests/examples/cython/
+-rw-rw-rw-   0        0        0      647 2023-04-24 09:25:15.000000 dioptas-0.5.7/venv/Lib/site-packages/numpy/core/tests/examples/cython/checks.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.679525 dioptas-0.5.7/venv/Lib/site-packages/numpy/random/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.679525 dioptas-0.5.7/venv/Lib/site-packages/numpy/random/_examples/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.057034 dioptas-0.5.7/venv/Lib/site-packages/numpy/random/_examples/cython/
+-rw-rw-rw-   0        0        0     2368 2023-04-24 09:25:16.000000 dioptas-0.5.7/venv/Lib/site-packages/numpy/random/_examples/cython/extending.pyx
+-rw-rw-rw-   0        0        0     3987 2023-04-24 09:25:16.000000 dioptas-0.5.7/venv/Lib/site-packages/numpy/random/_examples/cython/extending_distributions.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.679525 dioptas-0.5.7/venv/Lib/site-packages/pandas/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.077899 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/
+-rw-rw-rw-   0        0        0    52318 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/algos.pyx
+-rw-rw-rw-   0        0        0     6044 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/arrays.pyx
+-rw-rw-rw-   0        0        0    57931 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/groupby.pyx
+-rw-rw-rw-   0        0        0     4879 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/hashing.pyx
+-rw-rw-rw-   0        0        0     3099 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/hashtable.pyx
+-rw-rw-rw-   0        0        0    42329 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/index.pyx
+-rw-rw-rw-   0        0        0      806 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/indexing.pyx
+-rw-rw-rw-   0        0        0    27622 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/internals.pyx
+-rw-rw-rw-   0        0        0    20247 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/interval.pyx
+-rw-rw-rw-   0        0        0    29012 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/join.pyx
+-rw-rw-rw-   0        0        0    91873 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/lib.pyx
+-rw-rw-rw-   0        0        0    14852 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/missing.pyx
+-rw-rw-rw-   0        0        0     8080 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/ops.pyx
+-rw-rw-rw-   0        0        0     2691 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/ops_dispatch.pyx
+-rw-rw-rw-   0        0        0    73048 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/parsers.pyx
+-rw-rw-rw-   0        0        0     1702 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/properties.pyx
+-rw-rw-rw-   0        0        0     1123 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/reduction.pyx
+-rw-rw-rw-   0        0        0     3530 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/reshape.pyx
+-rw-rw-rw-   0        0        0    21691 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/sparse.pyx
+-rw-rw-rw-   0        0        0     6412 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/testing.pyx
+-rw-rw-rw-   0        0        0    23367 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslib.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.094255 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/
+-rw-rw-rw-   0        0        0      305 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/base.pyx
+-rw-rw-rw-   0        0        0     7202 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/ccalendar.pyx
+-rw-rw-rw-   0        0        0    23975 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/conversion.pyx
+-rw-rw-rw-   0        0        0    15190 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/dtypes.pyx
+-rw-rw-rw-   0        0        0    22376 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/fields.pyx
+-rw-rw-rw-   0        0        0    38995 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/nattype.pyx
+-rw-rw-rw-   0        0        0    20772 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/np_datetime.pyx
+-rw-rw-rw-   0        0        0   147704 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/offsets.pyx
+-rw-rw-rw-   0        0        0    40034 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/parsing.pyx
+-rw-rw-rw-   0        0        0    85119 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/period.pyx
+-rw-rw-rw-   0        0        0    26321 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/strptime.pyx
+-rw-rw-rw-   0        0        0    70395 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/timedeltas.pyx
+-rw-rw-rw-   0        0        0    78268 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/timestamps.pyx
+-rw-rw-rw-   0        0        0    14729 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/timezones.pyx
+-rw-rw-rw-   0        0        0    27789 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/tzconversion.pyx
+-rw-rw-rw-   0        0        0    11648 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/tslibs/vectorized.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.094255 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/window/
+-rw-rw-rw-   0        0        0    64651 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/window/aggregations.pyx
+-rw-rw-rw-   0        0        0     4526 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/window/indexers.pyx
+-rw-rw-rw-   0        0        0     4601 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/_libs/writers.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.679525 dioptas-0.5.7/venv/Lib/site-packages/pandas/io/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.097769 dioptas-0.5.7/venv/Lib/site-packages/pandas/io/sas/
+-rw-rw-rw-   0        0        0     2526 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/io/sas/byteswap.pyx
+-rw-rw-rw-   0        0        0    19701 2023-04-24 09:26:56.000000 dioptas-0.5.7/venv/Lib/site-packages/pandas/io/sas/sas.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:07.683533 dioptas-0.5.7/venv/Lib/site-packages/scipy/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.097769 dioptas-0.5.7/venv/Lib/site-packages/scipy/linalg/
+-rw-rw-rw-   0        0        0    64424 2023-04-24 09:25:49.000000 dioptas-0.5.7/venv/Lib/site-packages/scipy/linalg/cython_blas.pyx
+-rw-rw-rw-   0        0        0   697453 2023-04-24 09:25:49.000000 dioptas-0.5.7/venv/Lib/site-packages/scipy/linalg/cython_lapack.pyx
+drwxrwxrwx   0        0        0        0 2023-04-24 14:21:08.105954 dioptas-0.5.7/venv/Lib/site-packages/scipy/special/
+-rw-rw-rw-   0        0        0   877384 2023-04-24 09:25:50.000000 dioptas-0.5.7/venv/Lib/site-packages/scipy/special/_ufuncs.pyx
+-rw-rw-rw-   0        0        0     9415 2023-04-24 09:25:50.000000 dioptas-0.5.7/venv/Lib/site-packages/scipy/special/_ufuncs_cxx.pyx
+-rw-rw-rw-   0        0        0   150528 2023-04-24 09:25:50.000000 dioptas-0.5.7/venv/Lib/site-packages/scipy/special/cython_special.pyx
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dioptas-0.5.6/.gitattributes` & `dioptas-0.5.7/.gitattributes`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/.github/workflows/CI_backend.yml` & `dioptas-0.5.7/.github/workflows/CI_functional.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This is a basic workflow to help you get started with Actions
 
-name: CI_backend
+name: CI_functional
 
 on: [push, pull_request]
 
 jobs:
   test:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
@@ -41,8 +41,11 @@
         pip install pycifrw pandas python-dateutil h5py scikit-image pyqt5 cython future qtpy pyfai lmfit \
                     pyepics extra_data pyinstaller watchdog pyopengl pyopengl-accelerate h5py hdf5plugin pyqtgraph \
                     mock pytest setuptools_scm
 
     - name: Run tests
       shell: bash -l {0}
       run: |
-        py.test dioptas/tests/unit_tests
+        QT_QPA_PLATFORM=offscreen py.test dioptas/tests/functional_tests/test_functional_JcpdsEditor.py
+        QT_QPA_PLATFORM=offscreen py.test dioptas/tests/functional_tests/test_img_bg.py
+        QT_QPA_PLATFORM=offscreen py.test dioptas/tests/functional_tests/test_userinterface.py
+        QT_QPA_PLATFORM=offscreen py.test dioptas/tests/functional_tests/test_functional_integration.py
```

### Comparing `dioptas-0.5.6/.github/workflows/CI_batch.yml` & `dioptas-0.5.7/.github/workflows/CI_batch.yml`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/.github/workflows/CI_frontend.yml` & `dioptas-0.5.7/.github/workflows/CI_frontend.yml`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/.github/workflows/build_linux.yml` & `dioptas-0.5.7/.github/workflows/build_linux.yml`

 * *Files 9% similar despite different names*

```diff
@@ -5,63 +5,60 @@
 on: [push]
 
 # A workflow run is made up of one or more jobs that can run sequentially or in parallel
 jobs:
   build_linux:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
-
+    env:
+      QT_QPA_PLATFORM: offscreen
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
     - uses: actions/checkout@v3
     - run: git fetch --prune --unshallow
 
     - name: Use Miniconda
       uses: s-weigand/setup-conda@v1
 
-    - name: switch to python=3.9 and install pip
-      run: conda install python=3.9 pip -y
+    - name: switch to python=3.10 and install pip
+      run: conda install python=3.10 pip -y
 
     - name: Install Apt Dependencies
       run: |
         sudo apt-get update
         sudo apt-get install libxkbcommon-x11-0 libxkbcommon-x11-dev libxcb-xinerama0  \
         libxkbcommon-dev libfontconfig1-dev libfreetype6-dev libx11-dev libx11-xcb-dev libxext-dev libxfixes-dev \
         libxi-dev libxrender-dev libxcb1-dev libxcb-glx0-dev libxcb-keysyms1-dev libxcb-image0-dev \
         libxcb-shm0-dev libxcb-icccm4-dev libxcb-sync0-dev libxcb-xfixes0-dev libxcb-shape0-dev \
-        libxcb-randr0-dev libxcb-render-util0-dev
+        libxcb-randr0-dev libxcb-render-util0-dev libegl1
 
     - name: Install Pip Dependencies
       run: |
-        pip install pycifrw pandas python-dateutil h5py scikit-image pyqt5 cython future qtpy pyfai lmfit \
-                    pyepics extra_data pyinstaller==5.5 watchdog pyopengl pyopengl-accelerate h5py hdf5plugin \
+        pip install pycifrw pandas python-dateutil h5py scikit-image==0.19.3 pyqt6 cython future qtpy pyfai lmfit \
+                    pyepics extra_data pyinstaller watchdog pyopengl pyopengl-accelerate h5py hdf5plugin \
                     pyqtgraph sharedmem setuptools_scm
+      # we have to use scikit-image==0.19.3 because of a new loading mechanism in 0.20.0 which does currently not work
+      # with pyinstaller
 
     - name: Compile Smooth Bruckner
       run: cythonize -a -i dioptas/model/util/smooth_bruckner_cython.pyx
 
     - name: Create a Version File
       run: python -m setuptools_scm
 
     - name: Run Dioptas from source to test
-      run: xvfb-run python Dioptas.py test
+      run: xvfb-run -e /dev/stdout python Dioptas.py test
         
     - name: Run PyInstaller
       run: bash create_executable.sh
 
-    - name: Clean Up Executable Folder
-      run: |
-        cd dist/Dioptas*
-        rm libQt5Quick.so.5 libQt5Qml.so.5 libQt5Network.so.5 libcrypto.so.1.1 libsqlite3.so.0
-        rm -r imageio
-
     - name: Run Dioptas
       run: |
         cd dist/Dioptas*
-        xvfb-run ./Dioptas test
+        xvfb-run -e /dev/stdout ./Dioptas test
 
     - name: Compress Executable
       run: |
         cd dist
         export DIOPTAS_FOLDER=$(ls | grep Dioptas)
         tar -zcvf $DIOPTAS_FOLDER.tar.gz $DIOPTAS_FOLDER
         du -sh $DIOPTAS_FOLDER.tar.gz
```

### Comparing `dioptas-0.5.6/.github/workflows/build_mac.yml` & `dioptas-0.5.7/.github/workflows/build_mac.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,26 @@
     steps:
     - uses: actions/checkout@v3
     - run: git fetch --prune --unshallow
 
     - name: Use Miniconda
       uses: s-weigand/setup-conda@v1
 
-    - name: switch to python=3.10 and install pip
-      run: conda install python=3.10 pip -y
+    - name: switch to python=3.11 and install pip
+      run: conda install python=3.11 pip -y
+
 
     - name: Install Pip Dependencies
       run: |
-        pip install pycifrw pandas python-dateutil h5py scikit-image pyqt5 future qtpy pyfai lmfit pyepics \
+        pip install pycifrw pandas python-dateutil h5py scikit-image==0.19.3 pyqt6 future qtpy pyfai lmfit pyepics \
                     pyinstaller cython watchdog h5py hdf5plugin pyqtgraph sharedmem \
                     cython setuptools_scm
+      # we have to use scikit-image==0.19.3 because of a new loading mechanism in 0.20.0 which does currently not work
+      # with pyinstaller
+
     - name: Update Pyinstaller Hooks
       run: |
         pip uninstall pyinstaller-hooks-contrib -y
         git clone https://github.com/pyinstaller/pyinstaller-hooks-contrib.git
         cd pyinstaller-hooks-contrib
         python setup.py install
         cd ..
```

### Comparing `dioptas-0.5.6/.github/workflows/build_windows.yml` & `dioptas-0.5.7/.github/workflows/build_windows.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,32 @@
     runs-on: windows-latest
 
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
     - uses: actions/checkout@v3
     - run: git fetch --prune --unshallow
     - name: Setup Python 3.10
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: '3.10'
 
     - name: Use Python Dependency Cache
       id: pip-cache
       uses: actions/cache@v1
       with:
         path: ~\AppData\Local\pip\Cache
         key: ${{ runner.os }}-pip-${{ hashFiles('Dioptas.spec') }}-v3
         restore-keys: |
           ${{ runner.os }}-pip-c3
         
     - name: Install Pip Dependencies
       run: |
-        pip install pycifrw pandas numpy python-dateutil h5py cython scikit-image pyqt5 future qtpy pyfai lmfit pyepics extra_data pyinstaller watchdog pyopengl pyopengl-accelerate h5py hdf5plugin pyqtgraph sharedmem setuptools_scm
+        pip install pycifrw pandas numpy python-dateutil h5py cython scikit-image==0.19.3 pyqt6 future qtpy pyfai lmfit pyepics extra_data pyinstaller watchdog pyopengl pyopengl-accelerate h5py hdf5plugin pyqtgraph sharedmem setuptools_scm
+      # we have to use scikit-image==0.19.3 because of a new loading mechanism in 0.20.0 which does currently not work
+      # with pyinstaller
 
     - name: Compile Smooth Bruckner
       run: cythonize -a -i dioptas\model\util\smooth_bruckner_cython.pyx
 
     - name: Create a Version File
       run: python -m setuptools_scm
```

### Comparing `dioptas-0.5.6/.gitignore` & `dioptas-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/Dioptas.spec` & `dioptas-0.5.7/Dioptas.spec`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/README.md` & `dioptas-0.5.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Maintainer
 ----------
 
 Clemens Prescher (clemens.prescher@gmail.com)
 
 Requirements
 ------------
-    * python 3.7+
+    * python 3.9+
 
 It is known to run on Windows, Mac and Linux. For optimal usage on a Windows machine it should be run with 64 bit
 python. When used with 32 bit Dioptas occasionally crashes because of limited memory allocation possibilities.
 
 Installation
 ------------
```

### Comparing `dioptas-0.5.6/changelog.rst` & `dioptas-0.5.7/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+0.5.7 (stable 24.04.2023)
+-------------------------
+
+New features:
+    - saving in batch window will now also save background subtracted patterns, if enabled in the pattern widget
+    - upgraded dependency pyqt5 to pyqt6 which should result in improvements for high dpi screens
+    - added a new "integrate" button to the batch widget, which will integrate all images in the batch widget
+    - now compatible with python 3.11, whenever possible the created executables are compiled with python 3.11
+    - dropping support for python 3.6, 3.7 and 3.8 and focussing on compatibility with python 3.9, 3.10 and 3.11
+
+
+Bugfixes:
+    - fix numpy float conversion issue due to deprecated numpy.float
+    - reading cif files with missing volume tag will now work correctly and the volume will be calculated from cell
+      parameters (PR #140, thanks to @ScottNotFound)
+
+
 0.5.6 (stable 23.11.2022)
 --------------------------
 
 Removed image files from pypi distribution.
 
 
 0.5.5 (stable 22.11.2022)
```

### Comparing `dioptas-0.5.6/conda_scripts/construct.yaml` & `dioptas-0.5.7/conda_scripts/construct.yaml`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/conda_scripts/recipe/meta.yaml` & `dioptas-0.5.7/conda_scripts/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/create_executable.bat` & `dioptas-0.5.7/create_executable.bat`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/__init__.py` & `dioptas-0.5.7/dioptas/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,14 @@
     __version__ = get_version(root='..', relative_to=__file__)
 
 from .paths import resources_path, calibrants_path, icons_path, data_path, style_path
 from .excepthook import excepthook
 from ._desktop_shortcuts import make_shortcut
 from .controller.MainController import MainController
 
-# Enable scaling for high DPI displays
-if _platform != "linux" or _platform != "linux2":  # does not work correctly on linux
-    QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)
-
 
 def main():
     app = QtWidgets.QApplication([])
     sys.excepthook = excepthook
     print("Dioptas {}".format(__version__))
 
     if _platform == "linux" or _platform == "linux2" or _platform == "win32" or _platform == 'cygwin':
```

### Comparing `dioptas-0.5.6/dioptas/_desktop_shortcuts.py` & `dioptas-0.5.7/dioptas/_desktop_shortcuts.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/CalibrationController.py` & `dioptas-0.5.7/dioptas/controller/CalibrationController.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         if not (0 <= y < shape[1]):
             return
 
         peak_ind = self.widget.peak_num_sb.value()
         if self.widget.automatic_peak_search_rb.isChecked():
             points = self.model.calibration_model.find_peaks_automatic(x, y, peak_ind - 1)
         else:
-            search_size = np.int(self.widget.search_size_sb.value())
+            search_size = int(self.widget.search_size_sb.value())
             points = self.model.calibration_model.find_peak(x, y, search_size, peak_ind - 1)
         if len(points):
             self.plot_points(points)
             if self.widget.automatic_peak_num_inc_cb.checkState():
                 self.widget.peak_num_sb.setValue(peak_ind + 1)
 
     def plot_points(self, points=None):
```

### Comparing `dioptas-0.5.6/dioptas/controller/ConfigurationController.py` & `dioptas-0.5.7/dioptas/controller/ConfigurationController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/MainController.py` & `dioptas-0.5.7/dioptas/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/MaskController.py` & `dioptas-0.5.7/dioptas/controller/MaskController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/__init__.py` & `dioptas-0.5.7/dioptas/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/BackgroundController.py` & `dioptas-0.5.7/dioptas/controller/integration/BackgroundController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/BatchController.py` & `dioptas-0.5.7/dioptas/controller/integration/BatchController.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,15 +837,25 @@
             else:
                 self.model.img_model.blockSignals(True)
                 img_data = self.model.batch_model.data
                 pattern_x = self.model.batch_model.binning
                 for y in range(img_data.shape[0]):
                     pattern_y = img_data[int(y)]
                     self.model.pattern_model.set_pattern(pattern_x, pattern_y)
-                    self.model.current_configuration.save_pattern(f"{name}_{y}{ext}", subtract_background=True)
+                    self.model.current_configuration.save_pattern(f"{name}_{y:03d}{ext}")
+
+                    if self.model.pattern_model.pattern.auto_background_subtraction:
+                        bkg_directory = os.path.join(os.path.dirname(filename), 'bkg_subtracted')
+                        if not os.path.exists(bkg_directory):
+                            os.mkdir(bkg_directory)
+                        bkg_subtracted_name = os.path.join(bkg_directory, os.path.basename(name))
+
+                        self.model.pattern_model.pattern.recalculate_pattern()
+                        self.model.current_configuration.save_pattern(f"{bkg_subtracted_name}_{y:03d}{ext}",
+                                                                      subtract_background=True)
                 self.model.img_model.blockSignals(False)
 
     def img_mouse_click(self, x, y):
         """
         Process mouse click
         """
         y += int(str(self.widget.batch_widget.position_widget.step_series_widget.start_txt.text()))
@@ -934,15 +944,15 @@
         Plot raw image, diffraction pattern and draw lines on the heatmap plot based on given x and y
         """
         img = self.model.batch_model.data
         if img is None:
             return
         x = min(max(x, 0), img.shape[1])
         y = min(max(y, 0), img.shape[0] - 1)
-        self.widget.batch_widget.position_widget.step_series_widget.slider.setValue(y)
+        self.widget.batch_widget.position_widget.step_series_widget.slider.setValue(int(y))
         self.widget.batch_widget.position_widget.step_series_widget.pos_txt.setText(str(int(y)))
         self.plot_image(int(y))
         self.plot_pattern(int(x), int(y))
         start = int(str(self.widget.batch_widget.position_widget.step_series_widget.start_txt.text()))
         self.widget.batch_widget.stack_plot_widget.img_view.horizontal_line.setValue(y - start)
 
     def plot_pattern(self, x, y):
```

### Comparing `dioptas-0.5.6/dioptas/controller/integration/CorrectionController.py` & `dioptas-0.5.7/dioptas/controller/integration/CorrectionController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/EpicsController.py` & `dioptas-0.5.7/dioptas/controller/integration/EpicsController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/ImageController.py` & `dioptas-0.5.7/dioptas/controller/integration/ImageController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/IntegrationController.py` & `dioptas-0.5.7/dioptas/controller/integration/IntegrationController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/OptionsController.py` & `dioptas-0.5.7/dioptas/controller/integration/OptionsController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/OverlayController.py` & `dioptas-0.5.7/dioptas/controller/integration/OverlayController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/PatternController.py` & `dioptas-0.5.7/dioptas/controller/integration/PatternController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/__init__.py` & `dioptas-0.5.7/dioptas/controller/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/econfig.py` & `dioptas-0.5.7/dioptas/controller/integration/econfig.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/phase/JcpdsEditorController.py` & `dioptas-0.5.7/dioptas/controller/integration/phase/JcpdsEditorController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/phase/PhaseController.py` & `dioptas-0.5.7/dioptas/controller/integration/phase/PhaseController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInBatchController.py` & `dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInBatchController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInCakeController.py` & `dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInCakeController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/controller/integration/phase/PhaseInPatternController.py` & `dioptas-0.5.7/dioptas/controller/integration/phase/PhaseInPatternController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/excepthook.py` & `dioptas-0.5.7/dioptas/excepthook.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/BatchModel.py` & `dioptas-0.5.7/dioptas/model/BatchModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,13 +368,15 @@
     match_iterator = pattern.finditer(folder_path)
     new_directory_str = None
     for ind, match in enumerate(list(match_iterator)):
         number_span = match.span()
         left_ind = number_span[0]
         right_ind = number_span[1]
         number = int(folder_path[left_ind:right_ind]) + step
+        if number < 0:
+            number = 0
         new_directory_str = "{left_str}{number:0{len}}{right_str}".format(
             left_str=folder_path[:left_ind],
             number=number,
             len=right_ind - left_ind,
             right_str=folder_path[right_ind:])
     return new_directory_str
```

### Comparing `dioptas-0.5.6/dioptas/model/CalibrationModel.py` & `dioptas-0.5.7/dioptas/model/CalibrationModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         :param float y:
             y-coordinate in pixel - should be from original image (not supersampled y-coordinate)
         :param peak_ind:
             peak/ring index to which the found points will be added
         :return:
             array of points found
         """
-        massif = Massif(self.img_model.img_data)
+        massif = Massif(self.img_model.img_data, median_prefilter=False)
         cur_peak_points = massif.find_peaks((int(np.round(x)), int(np.round(y))), stdout=DummyStdOut())
         if len(cur_peak_points):
             self.points.append(np.array(cur_peak_points))
             self.points_index.append(peak_ind)
         return np.array(cur_peak_points)
 
     def find_peak(self, x, y, search_size, peak_ind):
@@ -182,15 +182,15 @@
         :param algorithm:
             peak search algorithm used. Possible algorithms are 'Massif' and 'Blob'
         :param mask:
             if a mask is used during the process this is provided here as a 2d array for the image.
         """
 
         if algorithm == 'Massif':
-            self.peak_search_algorithm = Massif(self.img_model.img_data)
+            self.peak_search_algorithm = Massif(self.img_model.img_data, median_prefilter=False)
         elif algorithm == 'Blob':
             if mask is not None:
                 self.peak_search_algorithm = BlobDetection(self.img_model.img_data * mask)
             else:
                 self.peak_search_algorithm = BlobDetection(self.img_model.img_data)
             self.peak_search_algorithm.process()
         else:
```

### Comparing `dioptas-0.5.6/dioptas/model/Configuration.py` & `dioptas-0.5.7/dioptas/model/Configuration.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/DioptasModel.py` & `dioptas-0.5.7/dioptas/model/DioptasModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/ImgModel.py` & `dioptas-0.5.7/dioptas/model/ImgModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/MaskModel.py` & `dioptas-0.5.7/dioptas/model/MaskModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/OverlayModel.py` & `dioptas-0.5.7/dioptas/model/OverlayModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/PatternModel.py` & `dioptas-0.5.7/dioptas/model/PatternModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/PhaseModel.py` & `dioptas-0.5.7/dioptas/model/PhaseModel.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/__init__.py` & `dioptas-0.5.7/dioptas/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/loader/FabioLoader.py` & `dioptas-0.5.7/dioptas/model/loader/FabioLoader.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/loader/KaraboLoader.py` & `dioptas-0.5.7/dioptas/model/loader/KaraboLoader.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/loader/LambdaLoader.py` & `dioptas-0.5.7/dioptas/model/loader/LambdaLoader.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/loader/hdf5Loader.py` & `dioptas-0.5.7/dioptas/model/loader/hdf5Loader.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/loader/spe.py` & `dioptas-0.5.7/dioptas/model/loader/spe.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/BackgroundExtraction.py` & `dioptas-0.5.7/dioptas/model/util/BackgroundExtraction.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/HelperModule.py` & `dioptas-0.5.7/dioptas/model/util/HelperModule.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/ImgCorrection.py` & `dioptas-0.5.7/dioptas/model/util/ImgCorrection.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/NewFileWatcher.py` & `dioptas-0.5.7/dioptas/model/util/NewFileWatcher.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/Pattern.py` & `dioptas-0.5.7/dioptas/model/util/Pattern.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/PeakShapes.py` & `dioptas-0.5.7/dioptas/model/util/PeakShapes.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/__init__.py` & `dioptas-0.5.7/dioptas/model/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/calc.py` & `dioptas-0.5.7/dioptas/model/util/calc.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/cif.py` & `dioptas-0.5.7/dioptas/model/util/cif.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import division, unicode_literals
 
 import os
 import itertools
+
 try:
     from urllib import pathname2url
 except ImportError:
     from urllib.request import pathname2url
 
 from math import degrees
 
@@ -342,15 +343,19 @@
         self.b = convert_cif_number_to_float(cif_dictionary['_cell_length_b'])
         self.c = convert_cif_number_to_float(cif_dictionary['_cell_length_c'])
 
         self.alpha = convert_cif_number_to_float(cif_dictionary['_cell_angle_alpha'])
         self.beta = convert_cif_number_to_float(cif_dictionary['_cell_angle_beta'])
         self.gamma = convert_cif_number_to_float(cif_dictionary['_cell_angle_gamma'])
 
-        self.volume = convert_cif_number_to_float(cif_dictionary['_cell_volume'])
+        if '_cell_volume' in cif_dictionary.keys():
+            self.volume = convert_cif_number_to_float(cif_dictionary['_cell_volume'])
+        else:
+            self.volume = calculate_cell_volume(self.a, self.b, self.c,
+                                                np.deg2rad(self.alpha), np.deg2rad(self.beta), np.deg2rad(self.gamma))
 
         if '_symmetry_space_group_name_h-m' in cif_dictionary.keys():
             self.space_group = cif_dictionary['_symmetry_space_group_name_h-m']
         elif '_symmetry_space_group_name_h-m_alt' in cif_dictionary.keys():
             self.space_group = cif_dictionary['_symmetry_space_group_name_h-m_alt']
         else:
             self.space_group = None
@@ -379,15 +384,16 @@
             self.symmetry_operations[i] = self.symmetry_operations[i].replace("/", "./")
 
         self._atom_labels = cif_dictionary['_atom_site_label']
         self._atom_x = [float(convert_cif_number_to_float(s)) for s in cif_dictionary['_atom_site_fract_x']]
         self._atom_y = [float(convert_cif_number_to_float(s)) for s in cif_dictionary['_atom_site_fract_y']]
         self._atom_z = [float(convert_cif_number_to_float(s)) for s in cif_dictionary['_atom_site_fract_z']]
         if '_atom_site_occupancy' in cif_dictionary.keys():
-            self._atom_occupancy = [float(convert_cif_number_to_float(s)) for s in cif_dictionary['_atom_site_occupancy']]
+            self._atom_occupancy = [float(convert_cif_number_to_float(s)) for s in
+                                    cif_dictionary['_atom_site_occupancy']]
         else:
             self._atom_occupancy = [1] * len(self._atom_labels)
 
         # Create a list of 4-tuples, where each tuple is an atom:
         # [ ('Si', 0.4697, 0.0, 0.0),  ('O', 0.4135, 0.2669, 0.1191),  ... ]
         self.atoms = [(self._atom_labels[i], self._atom_x[i], self._atom_y[i], self._atom_z[i],
                        self._atom_occupancy[i]) for i in range(len(self._atom_labels))]
@@ -526,18 +532,18 @@
             self.comments += self.cif_dictionary['_chemical_formula_structural'].replace(" ", "")
         elif self.cif_dictionary.get('_chemical_formula_analytical'):
             self.comments += self.cif_dictionary['_chemical_formula_analytical'].replace(" ", "")
         elif self.cif_dictionary.get('_chemical_formula_sum'):
             self.comments += self.cif_dictionary['_chemical_formula_sum'].replace(" ", "")
 
         if self.cif_dictionary.get('_symmetry_space_group_name_H-M'):
-            if self.comments=='':
+            if self.comments == '':
                 self.comments += self.cif_dictionary.get('_symmetry_space_group_name_H-M').replace(" ", "")
             else:
-                self.comments+= ', ' +self.cif_dictionary.get('_symmetry_space_group_name_H-M').replace(" ", "")
+                self.comments += ', ' + self.cif_dictionary.get('_symmetry_space_group_name_H-M').replace(" ", "")
 
         if self.cif_dictionary.get('_chemical_name_structure_type'):
             self.comments += ' - '
             self.comments += self.cif_dictionary['_chemical_name_structure_type']
             self.comments += ' structure type'
         if self.cif_dictionary.get('_database_code_icsd'):
             self.comments = self.comments.strip()
@@ -547,22 +553,41 @@
                 self.comments += 'ICSD '
             self.comments += self.cif_dictionary['_database_code_icsd']
         elif self.cif_dictionary.get('_database_code_amcsd'):
             if self.comments != '':
                 self.comments += ', amcsd '
             else:
                 self.comments += 'amcsd '
-            self.comments+= self.cif_dictionary['_database_code_amcsd']
+            self.comments += self.cif_dictionary['_database_code_amcsd']
 
 
-def number_between(num, num_low, num_high):
+def number_between(number, low, high):
     """
-    Tests if a number is in between num_low and num_high, whereby num_low and num_high are included  [num_low, num_high]
+    Tests if a number is in between low and high, whereby low and high are included  [low, high]
     :return: Boolean result for the result
     """
-    if num_low <= num <= num_high:
+    if low <= number <= high:
         return True
     return False
 
 
 def convert_cif_number_to_float(cif_number):
     return float(cif_number.split('(')[0])
+
+
+def calculate_cell_volume(a, b, c, alpha, beta, gamma):
+    """
+    Calculates the cell volume using formula: 
+    V = a*b*c*sqrt(1 + 2*cos(alpha)*cos(beta)*cos(gamma)-cos^2(alpha)-cos^2(beta)-cos^2(gamma))
+
+    :param a: lattice parameter a
+    :param b: lattice parameter b
+    :param c: lattice parameter c
+    :param alpha: lattice angle alpha in radians
+    :param beta: lattice angle beta in radians
+    :param gamma: lattice angle gamma in radians
+    :return: cell volume
+    """
+    base = a * b * c
+    part1 = np.cos(alpha) * np.cos(beta) * np.cos(gamma)
+    part2 = np.cos(alpha) ** 2 + np.cos(beta) ** 2 + np.cos(gamma) ** 2
+    return base * np.sqrt(1 + 2 * part1 - part2)
```

### Comparing `dioptas-0.5.6/dioptas/model/util/cosmics.py` & `dioptas-0.5.7/dioptas/model/util/cosmics.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/jcpds.py` & `dioptas-0.5.7/dioptas/model/util/jcpds.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/signal.py` & `dioptas-0.5.7/dioptas/model/util/signal.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/smooth_bruckner.f95` & `dioptas-0.5.7/dioptas/model/util/smooth_bruckner.f95`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/smooth_bruckner_cython.c` & `dioptas-0.5.7/dioptas/model/util/smooth_bruckner_cython.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "dioptas.model.util.smooth_bruckner_cython",
         "sources": [
             "dioptas/model/util/smooth_bruckner_cython.pyx"
@@ -17,16 +17,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -95,15 +95,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -211,15 +211,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -250,15 +250,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -560,35 +560,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1316,26 +1316,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3020,15 +3020,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -4998,15 +4998,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -7301,15 +7301,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -7374,15 +7374,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -15577,15 +15577,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -16933,15 +16933,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -17238,15 +17238,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_dioptas__model__util__smooth_bruckner_cython) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -18384,28 +18384,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -18579,15 +18579,15 @@
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -19404,15 +19404,15 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `dioptas-0.5.6/dioptas/model/util/smooth_bruckner_cython.pyx` & `dioptas-0.5.7/dioptas/model/util/smooth_bruckner_cython.pyx`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/model/util/smooth_bruckner_python.py` & `dioptas-0.5.7/dioptas/model/util/smooth_bruckner_python.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/paths.py` & `dioptas-0.5.7/dioptas/paths.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/AgBh.D` & `dioptas-0.5.7/dioptas/resources/calibrants/AgBh.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Al.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Al.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Au.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Au.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/C14H30O.D` & `dioptas-0.5.7/dioptas/resources/calibrants/C14H30O.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/CeO2.D` & `dioptas-0.5.7/dioptas/resources/calibrants/CeO2.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Cr2O3.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Cr2O3.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/LaB6.D` & `dioptas-0.5.7/dioptas/resources/calibrants/LaB6.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660a.D` & `dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660a.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660b.D` & `dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660b.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/LaB6_SRM660c.D` & `dioptas-0.5.7/dioptas/resources/calibrants/LaB6_SRM660c.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/NaCl.D` & `dioptas-0.5.7/dioptas/resources/calibrants/NaCl.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/PBBA.D` & `dioptas-0.5.7/dioptas/resources/calibrants/PBBA.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640a.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640a.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640b.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640b.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640c.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640c.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640d.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640d.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/Si_SRM640e.D` & `dioptas-0.5.7/dioptas/resources/calibrants/Si_SRM640e.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/TiO2.D` & `dioptas-0.5.7/dioptas/resources/calibrants/TiO2.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/ZnO.D` & `dioptas-0.5.7/dioptas/resources/calibrants/ZnO.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/alpha_Al2O3.D` & `dioptas-0.5.7/dioptas/resources/calibrants/alpha_Al2O3.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/cristobaltite.D` & `dioptas-0.5.7/dioptas/resources/calibrants/cristobaltite.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/calibrants/quartz.D` & `dioptas-0.5.7/dioptas/resources/calibrants/quartz.D`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/data/atomic_scattering_params.json` & `dioptas-0.5.7/dioptas/resources/data/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/data/periodic_table.json` & `dioptas-0.5.7/dioptas/resources/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/arrow_down.ico` & `dioptas-0.5.7/dioptas/resources/icons/arrow_down.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/arrow_up.ico` & `dioptas-0.5.7/dioptas/resources/icons/arrow_up.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/delete.png` & `dioptas-0.5.7/dioptas/resources/icons/delete.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/delete.svg` & `dioptas-0.5.7/dioptas/resources/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/edit.png` & `dioptas-0.5.7/dioptas/resources/icons/edit.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/edit.svg` & `dioptas-0.5.7/dioptas/resources/icons/edit.svg`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/icon.icns` & `dioptas-0.5.7/dioptas/resources/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/icon.ico` & `dioptas-0.5.7/dioptas/resources/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/icon.png` & `dioptas-0.5.7/dioptas/resources/icons/icon.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/icon.svg` & `dioptas-0.5.7/dioptas/resources/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/open.ico` & `dioptas-0.5.7/dioptas/resources/icons/open.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/reset.ico` & `dioptas-0.5.7/dioptas/resources/icons/reset.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/reset_dark.ico` & `dioptas-0.5.7/dioptas/resources/icons/reset_dark.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/icons/save.ico` & `dioptas-0.5.7/dioptas/resources/icons/save.ico`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/resources/style/stylesheet.qss` & `dioptas-0.5.7/dioptas/resources/style/stylesheet.qss`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/Profiling/__init__.py` & `dioptas-0.5.7/dioptas/tests/Profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/Profiling/profiling_cbn_correction.py` & `dioptas-0.5.7/dioptas/tests/Profiling/profiling_cbn_correction.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/__init__.py` & `dioptas-0.5.7/dioptas/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/__init__.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_BackgroundController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_BackgroundController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part1.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# -*- coding: utf-8 -*-
+# Dioptas - GUI program for fast processing of 2D X-ray diffraction data
+# Principal author: Clemens Prescher (clemens.prescher@gmail.com)
+# Copyright (C) 2014-2019 GSECARS, University of Chicago, USA
+# Copyright (C) 2015-2018 Institute for Geology and Mineralogy, University of Cologne, Germany
+# Copyright (C) 2019-2020 DESY, Hamburg, Germany
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import os
 import gc
 import numpy as np
 
 from ..utility import QtTest, MockMouseEvent
 
 from ...widgets.integration import IntegrationWidget
```

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part2.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+# -*- coding: utf-8 -*-
+# Dioptas - GUI program for fast processing of 2D X-ray diffraction data
+# Principal author: Clemens Prescher (clemens.prescher@gmail.com)
+# Copyright (C) 2014-2019 GSECARS, University of Chicago, USA
+# Copyright (C) 2015-2018 Institute for Geology and Mineralogy, University of Cologne, Germany
+# Copyright (C) 2019-2020 DESY, Hamburg, Germany
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import os
 import gc
-import shutil
 from mock import MagicMock
 
 from ..utility import QtTest, click_button
 
 from qtpy import QtWidgets, QtGui
 
 from ...widgets.integration import IntegrationWidget
```

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_BatchController_part3.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_BatchController_part3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# -*- coding: utf-8 -*-
+# Dioptas - GUI program for fast processing of 2D X-ray diffraction data
+# Principal author: Clemens Prescher (clemens.prescher@gmail.com)
+# Copyright (C) 2014-2019 GSECARS, University of Chicago, USA
+# Copyright (C) 2015-2018 Institute for Geology and Mineralogy, University of Cologne, Germany
+# Copyright (C) 2019-2020 DESY, Hamburg, Germany
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import os
 import gc
 import unittest
 from unittest.mock import MagicMock
 
 import numpy as np
 
@@ -146,15 +166,14 @@
             get_partial_value(self.model.batch_model.binning, 20 - 0.5))
 
     def test_click_in_2d_widget_out_of_range_does_not_send_clicked_change(self):
         self.model.clicked_tth_changed.emit = MagicMock()
         self.widget.batch_widget.stack_plot_widget.img_view.mouse_left_clicked.emit(-1, 10)
         self.model.clicked_tth_changed.emit.assert_not_called()
 
-
     def test_clicked_tth_change_signal_changes_line_pos(self):
         self.controller.plot_batch()
 
         # in plot range
         self.model.clicked_tth_changed.emit(12)
         new_line_pos = self.widget.batch_widget.stack_plot_widget.img_view.vertical_line.pos()[0]
         self.assertAlmostEqual(12, get_partial_value(self.model.batch_model.binning, new_line_pos))
@@ -205,7 +224,8 @@
         self.widget.batch_widget.position_widget.step_series_widget.slider.setValue(50)
         self.controller.set_navigation_range((10, 50))
         self.assertEqual(self.widget.batch_widget.position_widget.step_series_widget.start_txt.text(), '10')
         self.assertEqual(self.widget.batch_widget.position_widget.step_series_widget.stop_txt.text(), '50')
         self.assertEqual(self.widget.batch_widget.position_widget.step_series_widget.slider.value(), 50)
 
         # ToDo Test interaction with other controllers: Integration window vertical line. Patterns
+
```

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_CalibrationController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_CalibrationController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_ConfigurationController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_ConfigurationController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_CorrectionController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_CorrectionController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_EpicsController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_EpicsController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_ImageController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_ImageController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_IntegrationBackgroundController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_IntegrationBackgroundController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_IntegrationController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_IntegrationController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_JcpdsEditorController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_JcpdsEditorController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_MaskController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_MaskController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_OptionsController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_OptionsController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_OverlayController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_OverlayController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_PatternController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_PatternController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseInCakeController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseInCakeController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/controller_tests/test_PhaseInPatternController.py` & `dioptas-0.5.7/dioptas/tests/controller_tests/test_PhaseInPatternController.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/CeO2_Pilatus1M.xy` & `dioptas-0.5.7/dioptas/tests/data/CeO2_Pilatus1M.xy`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/LaB6_40keV_MarCCD.poni` & `dioptas-0.5.7/dioptas/tests/data/LaB6_40keV_MarCCD.poni`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/Fe2O3_shelx.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/Fe2O3_shelx.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/ICSD_triclinic.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/ICSD_triclinic.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/amcsd.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/amcsd.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/apatite.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/apatite.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/fcc.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/fcc.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/hcp.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/hcp.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/cif/magnesiowustite.cif` & `dioptas-0.5.7/dioptas/tests/data/cif/magnesiowustite.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/distortion/f4mnew.spline` & `dioptas-0.5.7/dioptas/tests/data/distortion/f4mnew.spline`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/FeGeO3_cpx.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/FeGeO3_cpx.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/ag.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/ag.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/au_Anderson.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/au_Anderson.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/mo.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/mo.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/pt.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/pt.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/re.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/re.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/jcpds/re_K0.jcpds` & `dioptas-0.5.7/dioptas/tests/data/jcpds/re_K0.jcpds`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/pattern_001.chi` & `dioptas-0.5.7/dioptas/tests/data/pattern_001.chi`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/pattern_001.xy` & `dioptas-0.5.7/dioptas/tests/data/pattern_001.xy`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/pattern_002.xy` & `dioptas-0.5.7/dioptas/tests/data/pattern_002.xy`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/test.cif` & `dioptas-0.5.7/dioptas/tests/data/test.cif`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/data/wrong_file_format.txt` & `dioptas-0.5.7/dioptas/tests/data/wrong_file_format.txt`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/ehook.py` & `dioptas-0.5.7/dioptas/tests/ehook.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/__init__.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_functional_JcpdsEditor.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_functional_JcpdsEditor.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_functional_integration.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_functional_integration.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_img_bg.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_img_bg.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_save_and_load_project.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_save_and_load_project.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_scripts.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/functional_tests/test_userinterface.py` & `dioptas-0.5.7/dioptas/tests/functional_tests/test_userinterface.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/run_tests.py` & `dioptas-0.5.7/dioptas/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/__init__.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_FileNameIterator.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_FileNameIterator.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,91 +15,92 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
-import unittest
 
-from ..utility import QtTest
+import pytest
+
 from ...model.util.HelperModule import FileNameIterator
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 
 
-class FileNameIteratorTest(unittest.TestCase):
-    def setUp(self):
-        self.filename_iterator = FileNameIterator()
-
-    def test_get_next_filename_with_existent_file(self):
-        filename = 'image_001.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        new_filename = os.path.basename(self.filename_iterator.get_next_filename())
-        self.assertEqual(new_filename, 'image_002.tif')
-
-    def test_get_next_filename_with_non_existent_file(self):
-        filename = 'image_002.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        self.assertEqual(self.filename_iterator.get_next_filename(), None)
-
-    def test_get_next_filename_with_larger_Step(self):
-        filename = 'image_000.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        new_filename = os.path.basename(self.filename_iterator.get_next_filename(step=2))
-        self.assertEqual(new_filename, 'image_002.tif')
-
-    def test_get_next_filename_with_two_numbers_in_name(self):
-        filename1 = 'image_001w_001.tif'
-        filename2 = 'image_002w_001.tif'
-        file_path1 = os.path.join(data_path, filename1)
-        file_path2 = os.path.join(data_path, filename2)
-
-        open(file_path1, "w")
-        open(file_path2, "w")
-
-        self.filename_iterator.update_filename(file_path1)
-        new_filename = self.filename_iterator.get_next_filename()
-        self.assertEqual(os.path.abspath(new_filename),
-                         os.path.abspath(file_path2))
-
-        os.remove(file_path1)
-        os.remove(file_path2)
-
-        filename1 = 'image_003w_001.tif'
-        filename2 = 'image_003w_002.tif'
-        filename3 = 'image_004w_001.tif'
-
-        file_path1 = os.path.join(data_path, filename1)
-        file_path2 = os.path.join(data_path, filename2)
-        file_path3 = os.path.join(data_path, filename3)
-
-        open(file_path1, "w")
-        open(file_path2, "w")
-        open(file_path3, "w")
-
-        self.filename_iterator.update_filename(file_path1)
-        new_filename = self.filename_iterator.get_next_filename()
-        self.assertEqual(os.path.abspath(new_filename),
-                         os.path.abspath(file_path2))
-
-        os.remove(file_path1)
-        os.remove(file_path2)
-        os.remove(file_path3)
-
-    def test_get_previous_filename_with_existent_file(self):
-        filename = 'image_002.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        new_filename = os.path.basename(self.filename_iterator.get_previous_filename())
-        self.assertEqual(new_filename, 'image_001.tif')
-
-    def test_get_previous_filename_with_non_existent_file(self):
-        filename = 'image_001.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        self.assertEqual(self.filename_iterator.get_previous_filename(), None)
-
-    def test_get_previous_filename_with_larger_Step(self):
-        filename = 'image_003.tif'
-        self.filename_iterator.update_filename(os.path.join(data_path, filename))
-        new_filename = os.path.basename(self.filename_iterator.get_previous_filename(step=2))
-        self.assertEqual(new_filename, 'image_001.tif')
+@pytest.fixture
+def filename_iterator():
+    return FileNameIterator()
+
+
+def test_get_next_filename_with_existent_file(filename_iterator):
+    filename = 'image_001.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    new_filename = os.path.basename(filename_iterator.get_next_filename())
+    assert new_filename == 'image_002.tif'
+
+
+def test_get_next_filename_with_non_existent_file(filename_iterator):
+    filename = 'image_002.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    assert filename_iterator.get_next_filename() is None
+
+
+def test_get_next_filename_with_larger_Step(filename_iterator):
+    filename = 'image_000.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    new_filename = os.path.basename(filename_iterator.get_next_filename(step=2))
+    assert new_filename == 'image_002.tif'
+
+
+def test_get_next_filename_with_two_numbers_in_name(filename_iterator, tmp_path):
+    filename1 = 'image_001w_001.tif'
+    filename2 = 'image_002w_001.tif'
+    file_path1 = os.path.join(tmp_path, filename1)
+    file_path2 = os.path.join(tmp_path, filename2)
+
+    open(file_path1, "w")
+    open(file_path2, "w")
+
+    filename_iterator.update_filename(file_path1)
+    new_filename = filename_iterator.get_next_filename()
+    assert os.path.abspath(new_filename) == os.path.abspath(file_path2)
+
+    os.remove(file_path1)
+    os.remove(file_path2)
+
+    filename1 = 'image_003w_001.tif'
+    filename2 = 'image_003w_002.tif'
+    filename3 = 'image_004w_001.tif'
+
+    file_path1 = os.path.join(tmp_path, filename1)
+    file_path2 = os.path.join(tmp_path, filename2)
+    file_path3 = os.path.join(tmp_path, filename3)
+
+    open(file_path1, "w")
+    open(file_path2, "w")
+    open(file_path3, "w")
+
+    filename_iterator.update_filename(file_path1)
+    new_filename = filename_iterator.get_next_filename()
+    assert os.path.abspath(new_filename) == os.path.abspath(file_path2)
+
+
+def test_get_previous_filename_with_existent_file(filename_iterator):
+    filename = 'image_002.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    new_filename = os.path.basename(filename_iterator.get_previous_filename())
+    assert new_filename == 'image_001.tif'
+
+
+def test_get_previous_filename_with_non_existent_file(filename_iterator):
+    filename = 'image_001.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    assert filename_iterator.get_previous_filename() is None
+
+
+def test_get_previous_filename_with_larger_Step(filename_iterator):
+    filename = 'image_003.tif'
+    filename_iterator.update_filename(os.path.join(data_path, filename))
+    new_filename = os.path.basename(filename_iterator.get_previous_filename(step=2))
+    assert new_filename == 'image_001.tif'
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_HelperModule.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_HelperModule.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,82 +16,89 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import numpy as np
-import unittest
 
 from ...model.util.HelperModule import get_partial_index, FileNameIterator, get_partial_value
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data', 'FileIterator')
 
 
-class HelperModuleTest(unittest.TestCase):
-    def test_get_partial_index(self):
-        data = np.arange(0, 10, 1)
-        value = 2.5
-        self.assertEqual(get_partial_index(data, value), 2.5)
-        self.assertEqual(get_partial_index(data, data[4]), 4)
-
-    def test_get_partial_index_out_of_range(self):
-        data = np.arange(0, 10, 1)
-        self.assertIsNone(get_partial_index(data, -1))
-        self.assertIsNone(get_partial_index(data, 11))
-
-    def test_get_partial_value(self):
-        data = np.arange(2, 11, 2)
-        self.assertEqual(get_partial_value(data, 1.5), 5)
-        self.assertEqual(get_partial_value(data, 0.3), 2+0.3*2)
-
-    def test_get_partial_value_out_of_range(self):
-        data = np.arange(2, 11, 2)
-        self.assertIsNone(get_partial_value(data, -1))
-        self.assertIsNone(get_partial_value(data, 10))
-
-
-    def test_get_next_filename(self):
-        filename = os.path.join(data_path, "dummy1_1.txt")
-        self.file_iterator = FileNameIterator(filename)
-        new_filename = self.file_iterator.get_next_filename(1, filename)
-
-        self.assertEqual(new_filename, os.path.join(data_path, 'dummy1_2.txt'))
-
-    def test_get_next_filename_with_pos(self):
-        filename = os.path.join(data_path, "dummy1_1.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_next_filename(1, filename, pos=1)
-
-        self.assertEqual(new_filename, os.path.join(data_path, 'dummy2_1.txt'))
-
-    def test_get_previous_filename_with_pos(self):
-        filename = os.path.join(data_path, "dummy2_1.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_previous_filename(1, filename, pos=1)
-
-        self.assertEqual(new_filename, os.path.join(data_path, 'dummy1_1.txt'))
-
-    def test_get_next_folder(self):
-        filename = os.path.join(data_path, "run1", "dummy_1.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_next_folder(filename)
-        self.assertEqual(new_filename, os.path.join(data_path, 'run2', "dummy_1.txt"))
-
-    def test_get_previous_folder(self):
-        filename = os.path.join(data_path, "run2", "dummy_1.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_previous_folder(filename)
-        self.assertEqual(new_filename, os.path.join(data_path, 'run1', "dummy_1.txt"))
-
-    def test_get_next_folder_mec(self):
-        filename = os.path.join(data_path, "run1", "run_1_evt_2.0.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_next_folder(filename, mec_mode=True)
-        self.assertEqual(new_filename, os.path.join(data_path, 'run2', "run_2_evt_2.0.txt"))
-
-    def test_get_previous_folder_mec(self):
-        filename = os.path.join(data_path, "run2", "run_2_evt_2.0.txt")
-        self.file_iterator = FileNameIterator()
-        new_filename = self.file_iterator.get_previous_folder(filename, mec_mode=True)
-        self.assertEqual(new_filename, os.path.join(data_path, 'run1', "run_1_evt_2.0.txt"))
+def test_get_partial_index():
+    data = np.arange(0, 10, 1)
+    value = 2.5
+    assert get_partial_index(data, value) == 2.5
+    assert get_partial_index(data, data[4]) == 4
+
+
+def test_get_partial_index_out_of_range():
+    data = np.arange(0, 10, 1)
+    assert get_partial_index(data, -1) is None
+    assert get_partial_index(data, 11) is None
+
+
+def test_get_partial_value():
+    data = np.arange(2, 11, 2)
+    assert get_partial_value(data, 1.5) == 5
+    assert get_partial_value(data, 0.3) == 2 + 0.3 * 2
+
+
+def test_get_partial_value_out_of_range():
+    data = np.arange(2, 11, 2)
+    assert get_partial_value(data, -1) is None
+    assert get_partial_value(data, 10) is None
+
+
+def test_get_next_filename():
+    filename = os.path.join(data_path, "dummy1_1.txt")
+    file_iterator = FileNameIterator(filename)
+    new_filename = file_iterator.get_next_filename(1, filename)
+
+    assert new_filename == os.path.join(data_path, 'dummy1_2.txt')
+
+
+def test_get_next_filename_with_pos():
+    filename = os.path.join(data_path, "dummy1_1.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_next_filename(1, filename, pos=1)
+
+    assert new_filename == os.path.join(data_path, 'dummy2_1.txt')
+
+
+def test_get_previous_filename_with_pos():
+    filename = os.path.join(data_path, "dummy2_1.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_previous_filename(1, filename, pos=1)
+
+    assert new_filename == os.path.join(data_path, 'dummy1_1.txt')
+
+
+def test_get_next_folder():
+    filename = os.path.join(data_path, "run1", "dummy_1.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_next_folder(filename)
+    assert new_filename == os.path.join(data_path, 'run2', "dummy_1.txt")
+
+
+def test_get_previous_folder():
+    filename = os.path.join(data_path, "run2", "dummy_1.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_previous_folder(filename)
+    assert new_filename == os.path.join(data_path, 'run1', "dummy_1.txt")
+
+
+def test_get_next_folder_mec():
+    filename = os.path.join(data_path, "run1", "run_1_evt_2.0.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_next_folder(filename, mec_mode=True)
+    assert new_filename == os.path.join(data_path, 'run2', "run_2_evt_2.0.txt")
+
+
+def test_get_previous_folder_mec():
+    filename = os.path.join(data_path, "run2", "run_2_evt_2.0.txt")
+    file_iterator = FileNameIterator()
+    new_filename = file_iterator.get_previous_folder(filename, mec_mode=True)
+    assert new_filename == os.path.join(data_path, 'run1', "run_1_evt_2.0.txt")
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_ImgCorrections.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_ImgCorrections.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,94 +18,95 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import unittest
 import gc
 
 import numpy as np
+import pytest
 
 from ...model.util.ImgCorrection import ImgCorrectionManager, ImgCorrectionInterface, \
     ObliqueAngleDetectorAbsorptionCorrection
 from ...model.util.ImgCorrection import TransferFunctionCorrection, load_image
 from ..utility import unittest_data_path
 
+from pyFAI.azimuthalIntegrator import AzimuthalIntegrator
+from ...model.util.ImgCorrection import CbnCorrection
+
 
 class DummyCorrection(ImgCorrectionInterface):
     def __init__(self, shape, number=1):
         self._data = np.ones(shape) * number
         self._shape = shape
 
     def get_data(self):
         return self._data
 
     def shape(self):
         return self._shape
 
 
-class ImgCorrectionsUnitTest(unittest.TestCase):
-    def setUp(self):
-        self.corrections = ImgCorrectionManager()
+@pytest.fixture
+def corrections():
+    return ImgCorrectionManager()
 
-    def tearDown(self):
-        del self.corrections
-        gc.collect()
 
-    def test_add_first_matrix_and_detect_shape(self):
-        cor = DummyCorrection((2048, 2048))
+def test_add_first_matrix_and_detect_shape(corrections):
+    cor = DummyCorrection((2048, 2048))
 
-        self.corrections.add(cor)
+    corrections.add(cor)
 
-        self.assertTrue(np.array_equal(cor.get_data(), self.corrections.get_data()))
-        self.assertEqual(self.corrections.shape, (2048, 2048))
+    assert np.array_equal(cor.get_data(), corrections.get_data())
+    assert corrections.shape == (2048, 2048)
 
-    def test_add_several_corrections(self):
-        cor1 = DummyCorrection((2048, 2048), 2)
-        cor2 = DummyCorrection((2048, 2048), 3)
-        cor3 = DummyCorrection((2048, 2048), 5)
 
-        self.corrections.add(cor1)
-        self.corrections.add(cor2)
-        self.corrections.add(cor3)
+def test_add_several_corrections(corrections):
+    cor1 = DummyCorrection((2048, 2048), 2)
+    cor2 = DummyCorrection((2048, 2048), 3)
+    cor3 = DummyCorrection((2048, 2048), 5)
 
-        self.assertEqual(np.mean(self.corrections.get_data()), 2 * 3 * 5)
+    corrections.add(cor1)
+    corrections.add(cor2)
+    corrections.add(cor3)
 
-    def test_delete_corrections_without_names(self):
-        self.assertEqual(self.corrections.get_data(), None)
+    assert np.mean(corrections.get_data()) == 2 * 3 * 5
 
-        self.corrections.add(DummyCorrection((2048, 2048), 3))
-        self.corrections.delete()
-        self.assertEqual(self.corrections.get_data(), None)
 
-        self.corrections.add(DummyCorrection((2048, 2048), 2))
-        self.corrections.add(DummyCorrection((2048, 2048), 3))
+def test_delete_corrections_without_names(corrections):
+    assert corrections.get_data() is None
 
-        self.corrections.delete()
-        self.assertEqual(np.mean(self.corrections.get_data()), 2)
-        self.corrections.delete()
+    corrections.add(DummyCorrection((2048, 2048), 3))
+    corrections.delete()
+    assert corrections.get_data() is None
 
-    def test_delete_corrections_with_names(self):
-        # add two corrections and check if both applied
-        self.corrections.add(DummyCorrection((2048, 2048), 3), "cbn Correction")
-        self.corrections.add(DummyCorrection((2048, 2048), 5), "oblique angle Correction")
-        self.assertEqual(np.mean(self.corrections.get_data()), 3 * 5)
+    corrections.add(DummyCorrection((2048, 2048), 2))
+    corrections.add(DummyCorrection((2048, 2048), 3))
 
-        # delete the first by name
-        self.corrections.delete("cbn Correction")
-        self.assertEqual(np.mean(self.corrections.get_data()), 5)
+    corrections.delete()
+    assert np.mean(corrections.get_data()) == 2
+    corrections.delete()
 
-        # trying to delete non existent name will result in KeyError
-        self.assertRaises(KeyError, self.corrections.delete, "blub")
 
-        # just deleting something, when all corrections have a name will not change anything
-        self.corrections.delete()
-        self.assertEqual(np.mean(self.corrections.get_data()), 5)
+def test_delete_corrections_with_names(corrections):
+    # add two corrections and check if both applied
+    corrections.add(DummyCorrection((2048, 2048), 3), "cbn Correction")
+    corrections.add(DummyCorrection((2048, 2048), 5), "oblique angle Correction")
+    assert np.mean(corrections.get_data()) == 3 * 5
 
+    # delete the first by name
+    corrections.delete("cbn Correction")
+    assert np.mean(corrections.get_data()) == 5
 
-from pyFAI.azimuthalIntegrator import AzimuthalIntegrator
-from ...model.util.ImgCorrection import CbnCorrection
+    # trying to delete non-existent name will result in KeyError
+    with pytest.raises(KeyError):
+        corrections.delete("blub")
+
+    # just deleting something, when all corrections have a name will not change anything
+    corrections.delete()
+    assert np.mean(corrections.get_data()) == 5
 
 
 class CbnCorrectionTest(unittest.TestCase):
     def setUp(self):
         # defining geometry
         image_shape = [2048, 2048]  # pixel
         detector_distance = 200  # mm
@@ -341,11 +342,7 @@
         from ...model.util.HelperModule import rotate_matrix_m90
         img_transformations = [np.fliplr, rotate_matrix_m90]
         self.transfer_correction.set_img_transformations(img_transformations)
 
         transfer_data = self.transfer_correction.get_data()
         self.assertNotEqual(transfer_data, self.original_data)
         self.assertNotEqual(transfer_data, self.response_data)
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_Jcpds.py` & `dioptas-0.5.7/dioptas/tests/widget_tests/test_JcpdsEditorWidget.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,106 +13,88 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import unittest
-import gc
+
 import os
+import unittest
+
+from ..utility import QtTest, QtWidgets
 from ...model.util import jcpds
+from ...widgets.integration.JcpdsEditorWidget import JcpdsEditorWidget
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 jcpds_path = os.path.join(data_path, 'jcpds')
 
 
-class JcpdsUnitTest(unittest.TestCase):
+class JcpdsEditorTest(QtTest):
     def setUp(self):
         self.jcpds = jcpds()
-
-    def tearDown(self):
-        del self.jcpds
-        gc.collect()
-
-    def test_sorting_of_reflections(self):
-        self.jcpds.add_reflection(1, 0, 0, 100, 4.0)
-        self.jcpds.add_reflection(1, 2, 0, 90, 2.0)
-        self.jcpds.add_reflection(2, 2, 0, 23, 3.0)
-        self.jcpds.add_reflection(5, 2, 1, 50, 6.0)
-        self.jcpds.add_reflection(3, 2, 2, 10, 41.0)
-        self.jcpds.add_reflection(4, 3, 0, 30, 1.0)
-        self.jcpds.add_reflection(2, 2, 5, 2, 0.3)
-
-        self.jcpds.sort_reflections_by_h()
-        self.assertEqual(self.jcpds.reflections[0].d0, 4.0)
-        self.assertEqual(self.jcpds.reflections[6].d0, 6.0)
-
-        self.jcpds.sort_reflections_by_k()
-        self.assertEqual(self.jcpds.reflections[0].d0, 4.0)
-        self.assertEqual(self.jcpds.reflections[6].d0, 1.0)
-
-        self.jcpds.sort_reflections_by_l()
-        self.assertEqual(self.jcpds.reflections[0].d0, 4.0)
-        self.assertEqual(self.jcpds.reflections[6].d0, 0.3)
-
-        self.jcpds.sort_reflections_by_intensity()
-        self.assertEqual(self.jcpds.reflections[0].d0, 0.3)
-        self.assertEqual(self.jcpds.reflections[6].d0, 4.0)
-
-        self.jcpds.sort_reflections_by_d()
-        self.assertEqual(self.jcpds.reflections[0].intensity, 2)
-        self.assertEqual(self.jcpds.reflections[6].intensity, 10)
-
-    def test_modified_flag(self):
-        self.assertFalse(self.jcpds.params['modified'])
-        self.jcpds.params['a0'] = 3
-        self.assertTrue(self.jcpds.params['modified'])
-        self.assertEqual(self.jcpds.params['a0'], 3)
-        self.jcpds.modified = False
-
+        self.jcpds.compute_v0()
         self.jcpds.load_file(os.path.join(jcpds_path, 'au_Anderson.jcpds'))
-        self.assertFalse(self.jcpds.params['modified'])
-        self.jcpds.params['k0'] = 200
-        self.assertTrue(self.jcpds.params['modified'])
-        self.assertEqual(os.path.join(jcpds_path, 'au_Anderson.jcpds*'), self.jcpds.filename)
-        self.assertEqual('au_Anderson*', self.jcpds.name)
-
-    def get_reflection_d_spacing(self, reflections, h, k, l):
-        for reflection in reflections:
-            if reflection.h == h and reflection.k == k and reflection.l == l:
-                return reflection.d0
-
-    def test_consistency_d_spacing_calculation(self):
-        # loading a monoclinic jcpds and check if different signs will change the d spacing
-        self.jcpds.load_file(os.path.join(jcpds_path, 'FeGeO3_cpx.jcpds'))
-
-        d1_mon = self.get_reflection_d_spacing(self.jcpds.reflections, 2, 2, 1)
-        d2_mon = self.get_reflection_d_spacing(self.jcpds.reflections, -2, 2, 1)
-
-        self.jcpds.params['symmetry'] = 'TRICLINIC'
-        self.jcpds.compute_d0()
-
-        d1_tri = self.get_reflection_d_spacing(self.jcpds.reflections, 2, 2, 1)
-        d2_tri = self.get_reflection_d_spacing(self.jcpds.reflections, -2, 2, 1)
 
-        self.assertAlmostEqual(d1_mon, d1_tri)
-        self.assertAlmostEqual(d2_mon, d2_tri)
-
-    def test_using_negative_pressures(self):
-        self.jcpds.load_file(os.path.join(jcpds_path, 'au_Anderson.jcpds'))
-        self.jcpds.pressure = -1.
+        self.jcpds_editor_widget = JcpdsEditorWidget()
+        self.jcpds_editor_widget.show_jcpds(self.jcpds, wavelength=0.31)
 
-        self.jcpds.compute_d(-1, 298)
-        self.assertGreater(self.jcpds.params['v'], self.jcpds.params['v0'])
-
-    def test_using_negative_pressures_with_zero_bulk_modulus(self):
-        self.jcpds.load_file(os.path.join(jcpds_path, 're_K0.jcpds'))
-        self.jcpds.pressure = -1.
+    def tearDown(self):
+        del self.jcpds
+        self.jcpds_editor_widget.close()
+        del self.jcpds_editor_widget
 
-        self.jcpds.compute_d(-1, 298)
-        self.assertEqual(self.jcpds.params['v'], self.jcpds.params['v0'])
+    def test_filename_and_comment_are_shown_correctly(self):
+        self.assertEqual(self.jcpds_editor_widget.filename_txt.text(),
+                         self.jcpds.filename)
+        self.assertEqual(self.jcpds_editor_widget.comments_txt.text(),
+                         self.jcpds.params['comments'][0])
+
+    def test_all_lattice_parameters_are_shown_correctly(self):
+        self.assertEqual(self.jcpds_editor_widget.lattice_a_sb.value(),
+                         self.jcpds.params['a0'])
+        self.assertEqual(self.jcpds_editor_widget.lattice_b_sb.value(),
+                         self.jcpds.params['b0'])
+        self.assertEqual(self.jcpds_editor_widget.lattice_c_sb.value(),
+                         self.jcpds.params['c0'])
+        self.assertAlmostEqual(float(str(self.jcpds_editor_widget.lattice_volume_txt.text())),
+                               self.jcpds.params['v0'], delta=0.0001)
+
+        self.assertEqual(float(str(self.jcpds_editor_widget.lattice_eos_a_txt.text())),
+                         self.jcpds.params['a'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.lattice_eos_b_txt.text())),
+                         self.jcpds.params['b'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.lattice_eos_c_txt.text())),
+                         self.jcpds.params['c'])
+
+        self.assertEqual(self.jcpds_editor_widget.lattice_alpha_sb.value(),
+                         self.jcpds.params['alpha'])
+        self.assertEqual(self.jcpds_editor_widget.lattice_beta_sb.value(),
+                         self.jcpds.params['beta0'])
+        self.assertEqual(self.jcpds_editor_widget.lattice_gamma_sb.value(),
+                         self.jcpds.params['gamma0'])
+
+        self.assertEqual(self.jcpds_editor_widget.lattice_ab_sb.value(),
+                         self.jcpds.params['a0'] / float(self.jcpds.params['b0']))
+        self.assertEqual(self.jcpds_editor_widget.lattice_ca_sb.value(),
+                         1)
+        self.assertEqual(self.jcpds_editor_widget.lattice_cb_sb.value(),
+                         1)
+
+    def test_all_eos_parameters_are_shown_correctly(self):
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_K_txt.text())),
+                         self.jcpds.params['k0'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_Kp_txt.text())),
+                         self.jcpds.params['k0p0'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_alphaT_txt.text())),
+                         self.jcpds.params['alpha_t0'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_dalphadT_txt.text())),
+                         self.jcpds.params['d_alpha_dt'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_dKdT_txt.text())),
+                         self.jcpds.params['dk0dt'])
+        self.assertEqual(float(str(self.jcpds_editor_widget.eos_dKpdT_txt.text())),
+                         self.jcpds.params['dk0pdt'])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_MaskModel.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_MaskModel.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,171 +14,166 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
-import gc
 import os
 import numpy as np
-from math import sqrt, atan2, cos, sin
+from math import cos, sin
+
+import pytest
 from qtpy import QtCore
 
 from ...model.MaskModel import MaskModel
 
-from ..utility import delete_if_exists
-
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 
 
-class MaskModelTest(unittest.TestCase):
-    def setUp(self):
-        self.mask_model = MaskModel()
-        self.img = np.zeros((10, 10))
-        self.mask_model.set_dimension(self.img.shape)
-
-    def tearDown(self):
-        delete_if_exists(os.path.join(data_path, "test_save.mask"))
-        del self.mask_model
-        del self.img
-        gc.collect()
-
-    def test_growing_masks(self):
-        self.mask_model._mask_data[4, 4] = 1
-        self.mask_model._mask_data[0, 0] = 1
-        self.mask_model._mask_data[0, 9] = 1
-        self.mask_model._mask_data[9, 9] = 1
-        self.mask_model._mask_data[9, 0] = 1
-
-        self.mask_model.grow()
-
-        # tests corners
-        self.assertEqual(self.mask_model._mask_data[0, 1], 1)
-        self.assertEqual(self.mask_model._mask_data[1, 1], 1)
-        self.assertEqual(self.mask_model._mask_data[1, 0], 1)
-
-        self.assertEqual(self.mask_model._mask_data[0, 8], 1)
-        self.assertEqual(self.mask_model._mask_data[1, 8], 1)
-        self.assertEqual(self.mask_model._mask_data[1, 9], 1)
-
-        self.assertEqual(self.mask_model._mask_data[8, 0], 1)
-        self.assertEqual(self.mask_model._mask_data[8, 1], 1)
-        self.assertEqual(self.mask_model._mask_data[9, 1], 1)
-
-        self.assertEqual(self.mask_model._mask_data[8, 8], 1)
-        self.assertEqual(self.mask_model._mask_data[8, 9], 1)
-        self.assertEqual(self.mask_model._mask_data[9, 8], 1)
-
-        # tests center
-        self.assertEqual(self.mask_model._mask_data[3, 3], 1)
-        self.assertEqual(self.mask_model._mask_data[4, 3], 1)
-        self.assertEqual(self.mask_model._mask_data[5, 3], 1)
-
-        self.assertEqual(self.mask_model._mask_data[3, 5], 1)
-        self.assertEqual(self.mask_model._mask_data[4, 5], 1)
-        self.assertEqual(self.mask_model._mask_data[5, 5], 1)
-
-        self.assertEqual(self.mask_model._mask_data[3, 4], 1)
-        self.assertEqual(self.mask_model._mask_data[5, 4], 1)
-
-    def test_shrink_mask(self):
-        self.mask_model._mask_data[4, 4] = 1
-        self.mask_model._mask_data[0, 0] = 1
-        self.mask_model._mask_data[0, 9] = 1
-        self.mask_model._mask_data[9, 9] = 1
-        self.mask_model._mask_data[9, 0] = 1
-
-        self.before_mask = np.copy(self.mask_model._mask_data)
-        self.mask_model.grow()
-        self.mask_model.shrink()
-
-        self.assertTrue(np.array_equal(self.before_mask, self.mask_model._mask_data))
-
-        self.mask_model.clear_mask()
-
-        self.mask_model._mask_data[4, 4] = 1
-        self.mask_model._mask_data[5, 4] = 1
-        self.mask_model._mask_data[5, 5] = 1
-        self.mask_model._mask_data[4, 5] = 1
-        self.mask_model.shrink()
-
-        self.assertEqual(np.sum(self.mask_model._mask_data), 0)
-
-    def test_saving_and_loading(self):
-        self.mask_model.mask_ellipse(1024, 1024, 100, 100)
-        self.mask_model.set_dimension((2048, 2048))
-
-        mask_array = np.copy(self.mask_model.get_img())
-
-        filename = os.path.join(data_path, 'dummy.mask')
-
-        self.mask_model.save_mask(filename)
-        self.mask_model.load_mask(filename)
-
-        self.assertTrue(np.array_equal(mask_array, self.mask_model.get_img()))
-        os.remove(filename)
-
-    def test_use_roi(self):
-        self.mask_model.roi = [0, 2, 0, 2]
-
-        self.assertTrue(np.array_equal(self.mask_model.get_mask()[0:3, 0:3],
-                                       np.array([[0, 0, 1],
-                                                 [0, 0, 1],
-                                                 [1, 1, 1]]))
-                        )
-
-    def test_save_mask(self):
-        self.mask_model.mask_below_threshold(self.img, 1)
-        self.mask_model.save_mask(os.path.join(data_path, "test_save.mask"))
-
-        self.assertTrue(os.path.exists(os.path.join(data_path, "test_save.mask")))
-
-    def test_find_center_of_circle_from_three_points(self):
-        x0 = 2.0
-        y0 = 3.5
-        r = 1.2
-        phi1 = 0.1
-        phi2 = 1.3
-        phi3 = 6.0
-        p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
-        p2 = QtCore.QPointF(x0 + r * cos(phi2), y0 + r * sin(phi2))
-        p3 = QtCore.QPointF(x0 + r * cos(phi3), y0 + r * sin(phi3))
-        # p1 = (x0 + r * cos(phi1), y0 + r * sin(phi1))
-        # p2 = (x0 + r * cos(phi2), y0 + r * sin(phi2))
-        # p3 = (x0 + r * cos(phi3), y0 + r * sin(phi3))
-        self.mask_model.find_center_of_circle_from_three_points(p1, p2, p3)
-        self.assertAlmostEqual(x0, self.mask_model.center_for_arc.x(), 6)
-        self.assertAlmostEqual(y0, self.mask_model.center_for_arc.y(), 6)
-
-    def test_find_radius_of_circle_from_center_and_point(self):
-        x0 = 2.0
-        y0 = 3.5
-        p0 = QtCore.QPointF(x0, y0)
-        r = 1.2
-        phi1 = 0.1
-        p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
-        rcalc = self.mask_model.find_radius_of_circle_from_center_and_point(p0, p1)
-        self.assertEqual(r, rcalc)
-
-    def test_find_n_points_on_arc_from_three_points(self):
-        n = 50
-        x0 = 2.0
-        y0 = 3.5
-        p0 = QtCore.QPointF(x0, y0)
-        r = 1.2
-        width = 0
-
-        phi1 = 0.1
-        phi2 = 1.3
-        phi3 = -0.2
-        p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
-        p2 = QtCore.QPointF(x0 + r * cos(phi2), y0 + r * sin(phi2))
-        p3 = QtCore.QPointF(x0 + r * cos(phi3), y0 + r * sin(phi3))
-
-        n_angles = self.mask_model.find_n_angles_on_arc_from_three_points_around_p0(p0, p1, p2, p3, n)
-        n_points = self.mask_model.calc_arc_points_from_angles(p0, r, width, n_angles)
-        for p in n_points:
-            rcalc = self.mask_model.find_radius_of_circle_from_center_and_point(p0, p)
-            self.assertAlmostEqual(r, rcalc, 5)
+@pytest.fixture
+def mask_model():
+    mask_model = MaskModel()
+    mask_model.set_dimension((10, 10))
+    return mask_model
+
+
+def test_growing_masks(mask_model):
+    mask_model._mask_data[4, 4] = 1
+    mask_model._mask_data[0, 0] = 1
+    mask_model._mask_data[0, 9] = 1
+    mask_model._mask_data[9, 9] = 1
+    mask_model._mask_data[9, 0] = 1
+
+    mask_model.grow()
+
+    # tests corners
+    assert mask_model._mask_data[0, 1] == 1
+    assert mask_model._mask_data[1, 1] == 1
+    assert mask_model._mask_data[1, 0] == 1
+
+    assert mask_model._mask_data[0, 8] == 1
+    assert mask_model._mask_data[1, 8] == 1
+    assert mask_model._mask_data[1, 9] == 1
+
+    assert mask_model._mask_data[8, 0] == 1
+    assert mask_model._mask_data[8, 1] == 1
+    assert mask_model._mask_data[9, 1] == 1
+
+    assert mask_model._mask_data[8, 8] == 1
+    assert mask_model._mask_data[8, 9] == 1
+    assert mask_model._mask_data[9, 8] == 1
+
+    # tests center
+    assert mask_model._mask_data[3, 3] == 1
+    assert mask_model._mask_data[4, 3] == 1
+    assert mask_model._mask_data[5, 3] == 1
+
+    assert mask_model._mask_data[3, 5] == 1
+    assert mask_model._mask_data[4, 5] == 1
+    assert mask_model._mask_data[5, 5] == 1
+
+    assert mask_model._mask_data[3, 4] == 1
+    assert mask_model._mask_data[5, 4] == 1
+
+
+def test_shrink_mask(mask_model):
+    mask_model._mask_data[4, 4] = 1
+    mask_model._mask_data[0, 0] = 1
+    mask_model._mask_data[0, 9] = 1
+    mask_model._mask_data[9, 9] = 1
+    mask_model._mask_data[9, 0] = 1
+
+    before_mask = np.copy(mask_model._mask_data)
+    mask_model.grow()
+    mask_model.shrink()
+
+    assert np.array_equal(before_mask, mask_model._mask_data)
+
+    mask_model.clear_mask()
+
+    mask_model._mask_data[4, 4] = 1
+    mask_model._mask_data[5, 4] = 1
+    mask_model._mask_data[5, 5] = 1
+    mask_model._mask_data[4, 5] = 1
+    mask_model.shrink()
+
+    assert np.sum(mask_model._mask_data) == 0
+
+
+def test_saving_and_loading(mask_model, tmp_path):
+    mask_model.mask_ellipse(1024, 1024, 100, 100)
+    mask_model.set_dimension((2048, 2048))
+
+    mask_array = np.copy(mask_model.get_img())
+
+    filename = os.path.join(tmp_path, 'dummy.mask')
+
+    mask_model.save_mask(filename)
+    mask_model.load_mask(filename)
+
+    assert np.array_equal(mask_array, mask_model.get_img())
+
+
+def test_use_roi(mask_model):
+    mask_model.roi = [0, 2, 0, 2]
+
+    assert np.array_equal(mask_model.get_mask()[0:3, 0:3],
+                          np.array([[0, 0, 1],
+                                    [0, 0, 1],
+                                    [1, 1, 1]]))
+
+
+def test_save_mask(mask_model, tmp_path):
+    mask_model.mask_below_threshold(np.zeros(shape=(10, 10)), 1)
+    mask_model.save_mask(os.path.join(tmp_path, "test_save.mask"))
+
+    assert os.path.exists(os.path.join(tmp_path, "test_save.mask"))
+
+
+def test_find_center_of_circle_from_three_points(mask_model):
+    x0 = 2.0
+    y0 = 3.5
+    r = 1.2
+    phi1 = 0.1
+    phi2 = 1.3
+    phi3 = 6.0
+    p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
+    p2 = QtCore.QPointF(x0 + r * cos(phi2), y0 + r * sin(phi2))
+    p3 = QtCore.QPointF(x0 + r * cos(phi3), y0 + r * sin(phi3))
+    mask_model.find_center_of_circle_from_three_points(p1, p2, p3)
+    assert pytest.approx(x0) == mask_model.center_for_arc.x()
+    assert pytest.approx(y0) == mask_model.center_for_arc.y()
+
+
+def test_find_radius_of_circle_from_center_and_point(mask_model):
+    x0 = 2.0
+    y0 = 3.5
+    p0 = QtCore.QPointF(x0, y0)
+    r = 1.2
+    phi1 = 0.1
+    p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
+    rcalc = mask_model.find_radius_of_circle_from_center_and_point(p0, p1)
+    assert r == rcalc
+
+
+def test_find_n_points_on_arc_from_three_points(mask_model):
+    n = 50
+    x0 = 2.0
+    y0 = 3.5
+    p0 = QtCore.QPointF(x0, y0)
+    r = 1.2
+    width = 0
+
+    phi1 = 0.1
+    phi2 = 1.3
+    phi3 = -0.2
+    p1 = QtCore.QPointF(x0 + r * cos(phi1), y0 + r * sin(phi1))
+    p2 = QtCore.QPointF(x0 + r * cos(phi2), y0 + r * sin(phi2))
+    p3 = QtCore.QPointF(x0 + r * cos(phi3), y0 + r * sin(phi3))
+
+    n_angles = mask_model.find_n_angles_on_arc_from_three_points_around_p0(p0, p1, p2, p3, n)
+    n_points = mask_model.calc_arc_points_from_angles(p0, r, width, n_angles)
+    for p in n_points:
+        rcalc = mask_model.find_radius_of_circle_from_center_and_point(p0, p)
+        assert r == pytest.approx(rcalc, abs=1e-6)
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_OverlayModel.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_OverlayModel.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,43 +14,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
 import os
 import numpy as np
-from numpy.testing import assert_array_almost_equal
-
-from ...model.util import Pattern
+import pytest
 from ...model.OverlayModel import OverlayModel
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 
 
-class OverlayModelTest(unittest.TestCase):
-    def setUp(self):
-        self.x = np.linspace(0.1, 15, 100)
-        self.y = np.sin(self.x)
-        self.pattern = Pattern(self.x, self.y)
-        self.overlay_model = OverlayModel()
-
-    def test_add_overlay(self):
-        x_overlay = np.linspace(0, 10)
-        y_overlay = np.linspace(0, 100)
-        self.overlay_model.add_overlay(x_overlay, y_overlay, "dummy")
-
-        self.assertEqual(len(self.overlay_model.overlays), 1)
-        new_overlay = self.overlay_model.get_overlay(0)
-        self.assertEqual(new_overlay.name, "dummy")
-        assert_array_almost_equal(new_overlay.x, x_overlay)
-        assert_array_almost_equal(new_overlay.y, y_overlay)
-
-    def test_add_overlay_from_file(self):
-        filename = os.path.join(data_path, 'pattern_001.xy')
-        self.overlay_model.add_overlay_file(filename)
+@pytest.fixture
+def overlay_model():
+    return OverlayModel()
+
+
+def test_add_overlay(overlay_model: OverlayModel):
+    x_overlay = np.linspace(0, 10)
+    y_overlay = np.linspace(0, 100)
+    overlay_model.add_overlay(x_overlay, y_overlay, "dummy")
+
+    assert len(overlay_model.overlays) == 1
+    new_overlay = overlay_model.get_overlay(0)
+    assert new_overlay.name == "dummy"
+    assert np.array_equal(new_overlay.x, x_overlay)
+    assert np.array_equal(new_overlay.y, y_overlay)
+
+
+def test_add_overlay_from_file(overlay_model: OverlayModel):
+    filename = os.path.join(data_path, 'pattern_001.xy')
+    overlay_model.add_overlay_file(filename)
 
-        self.assertEqual(len(self.overlay_model.overlays), 1)
-        self.assertEqual(self.overlay_model.get_overlay(0).name, ''.join(os.path.basename(filename).split('.')[0:-1]))
+    assert len(overlay_model.overlays) == 1
+    assert overlay_model.get_overlay(0).name == ''.join(os.path.basename(filename).split('.')[0:-1])
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_Pattern.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_Pattern.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,220 +13,213 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-import unittest
 import os
-
 import numpy as np
+import pytest
+from pytest import approx
 
 from ...model.util.Pattern import BkgNotInRangeError
 from ...model.util import Pattern
 from ...model.util.PeakShapes import gaussian
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 
 
-class PatternTest(unittest.TestCase):
-    def array_almost_equal(self, array1, array2, places=7):
-        self.assertAlmostEqual(np.sum(array1 - array2), 0, places=places)
-
-    def array_not_almost_equal(self, array1, array2, places=7):
-        self.assertNotAlmostEqual(np.sum(array1 - array2), 0, places=places)
-
-    def test_loading_chi_file(self):
-        spec = Pattern()
-        x, y = spec.data
-
-        spec.load(os.path.join(data_path, 'pattern_001.chi'))
-        new_x, new_y = spec.data
-
-        self.assertNotEqual(len(x), len(new_x))
-        self.assertNotEqual(len(y), len(new_y))
-
-    def test_loading_invalid_file(self):
-        spec = Pattern()
-        self.assertEqual(-1, spec.load(os.path.join(data_path, 'wrong_file_format.txt')))
-
-    def test_saving_a_file(self):
-        x = np.linspace(-5, 5, 100)
-        y = x ** 2
-        spec = Pattern(x, y)
-        filename = os.path.join(data_path, "test.dat")
-        spec.save(filename)
-
-        spec2 = Pattern()
-        spec2.load(filename)
-
-        spec2_x, spec2_y = spec2.data
-        self.array_almost_equal(spec2_x, x)
-        self.array_almost_equal(spec2_y, y)
-
-        os.remove(filename)
-
-    def test_plus_and_minus_operators(self):
-        x = np.linspace(0, 10, 100)
-        pattern1 = Pattern(x, np.sin(x))
-        pattern2 = Pattern(x, np.sin(x))
-
-        pattern3 = pattern1 + pattern2
-        self.assertTrue(np.array_equal(pattern3.y, np.sin(x) * 2))
-        self.assertTrue(np.array_equal(pattern2.original_y, np.sin(x) * 1))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-
-        pattern3 = pattern1 + pattern1
-        self.assertTrue(np.array_equal(pattern3.y, np.sin(x) * 2))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-
-        pattern3 = pattern2 - pattern1
-        self.assertTrue(np.array_equal(pattern3.y, np.sin(x) * 0))
-        self.assertTrue(np.array_equal(pattern2.original_y, np.sin(x) * 1))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-
-        pattern3 = pattern1 - pattern1
-        self.assertTrue(np.array_equal(pattern3.y, np.sin(x) * 0))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-        self.assertTrue(np.array_equal(pattern1.original_y, np.sin(x) * 1))
-
-    def test_plus_and_minus_operators_with_different_shapes(self):
-        x = np.linspace(0, 10, 1000)
-        x2 = np.linspace(0, 12, 1300)
-        pattern1 = Pattern(x, np.sin(x))
-        pattern2 = Pattern(x2, np.sin(x2))
-
-        pattern3 = pattern1 + pattern2
-        self.array_almost_equal(pattern3.x, pattern1._original_x)
-        self.array_almost_equal(pattern3.y, pattern1._original_y * 2, 2)
-
-        pattern3 = pattern1 + pattern1
-        self.array_almost_equal(pattern3.y, np.sin(x) * 2, 2)
-
-        pattern3 = pattern1 - pattern2
-        self.array_almost_equal(pattern3.y, np.sin(x) * 0, 2)
-
-        pattern3 = pattern1 - pattern1
-        self.array_almost_equal(pattern3.y, np.sin(x) * 0, 2)
-
-    def test_multiply_with_scalar_operator(self):
-        x = np.linspace(0, 10, 100)
-        pattern1 = 2 * Pattern(x, np.sin(x))
-
-        pattern2 = 2 * Pattern(x, np.sin(x))
-
-        self.assertTrue(np.array_equal(pattern2.y, np.sin(x) * 2))
-
-    def test_using_background_pattern(self):
-        x = np.linspace(-5, 5, 100)
-        pattern_y = x ** 2
-        bkg_y = x
+def test_loading_chi_file():
+    spec = Pattern()
+    x, y = spec.data
 
-        spec = Pattern(x, pattern_y)
-        background_pattern = Pattern(x, bkg_y)
+    spec.load(os.path.join(data_path, 'pattern_001.chi'))
+    new_x, new_y = spec.data
 
-        spec.background_pattern = background_pattern
-        new_x, new_y = spec.data
+    assert len(x) != len(new_x)
+    assert len(y) != len(new_y)
 
-        self.array_almost_equal(new_x, x)
-        self.array_almost_equal(new_y, pattern_y - bkg_y)
 
-    def test_using_background_pattern_with_different_spacing(self):
-        x = np.linspace(-5, 5, 100)
-        pattern_y = x ** 2
-        x_bkg = np.linspace(-5, 5, 99)
-        bkg_y = x_bkg
+def test_loading_invalid_file():
+    pattern = Pattern()
+    assert -1 == pattern.load(os.path.join(data_path, 'wrong_file_format.txt'))
 
-        spec = Pattern(x, pattern_y)
-        background_pattern = Pattern(x_bkg, bkg_y)
 
-        spec.background_pattern = background_pattern
-        new_x, new_y = spec.data
+def test_saving_a_file(tmp_path):
+    x = np.linspace(-5, 5, 100)
+    y = x ** 2
+    pattern = Pattern(x, y)
+    filename = os.path.join(tmp_path, "test.dat")
+    pattern.save(filename)
+
+    pattern2 = Pattern()
+    pattern2.load(filename)
+
+    pattern2_x, pattern2_y = pattern2.data
+    assert pattern2_x == pytest.approx(x)
+    assert pattern2_y == pytest.approx(y)
+
+
+def test_plus_and_minus_operators():
+    x = np.linspace(0, 10, 100)
+    pattern1 = Pattern(x, np.sin(x))
+    pattern2 = Pattern(x, np.sin(x))
+
+    pattern3 = pattern1 + pattern2
+    assert np.array_equal(pattern3.y, np.sin(x) * 2)
+    assert np.array_equal(pattern2.original_y, np.sin(x) * 1)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+
+    pattern3 = pattern1 + pattern1
+    assert np.array_equal(pattern3.y, np.sin(x) * 2)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+
+    pattern3 = pattern2 - pattern1
+    assert np.array_equal(pattern3.y, np.sin(x) * 0)
+    assert np.array_equal(pattern2.original_y, np.sin(x) * 1)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+
+    pattern3 = pattern1 - pattern1
+    assert np.array_equal(pattern3.y, np.sin(x) * 0)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+    assert np.array_equal(pattern1.original_y, np.sin(x) * 1)
+
+
+def test_plus_and_minus_operators_with_different_shapes():
+    x = np.linspace(0, 10, 1000)
+    x2 = np.linspace(0, 12, 1300)
+    pattern1 = Pattern(x, np.sin(x))
+    pattern2 = Pattern(x2, np.sin(x2))
+
+    pattern3 = pattern1 + pattern2
+    assert pattern3.x == approx(pattern1._original_x)
+    assert pattern3.y == approx(pattern1._original_y * 2, abs=1e-4)
+
+    pattern3 = pattern1 + pattern1
+    assert pattern3.y == approx(np.sin(x) * 2, abs=1e-4)
 
-        self.array_almost_equal(new_x, x)
-        self.array_almost_equal(new_y, pattern_y - x)
+    pattern3 = pattern1 - pattern2
+    assert pattern3.y == approx(np.sin(x) * 0, abs=1e-4)
 
-    def test_background_out_of_range_throws_error(self):
-        x1 = np.linspace(0, 10)
-        x2 = np.linspace(-10, -1)
+    pattern3 = pattern1 - pattern1
+    assert pattern3.y == approx(np.sin(x) * 0, abs=1e-4)
 
-        spec = Pattern(x1, x1)
-        background_pattern = Pattern(x2, x2)
 
-        with self.assertRaises(BkgNotInRangeError):
-            spec.background_pattern = background_pattern
+def test_multiply_with_scalar_operator():
+    x = np.linspace(0, 10, 100)
+    pattern = 2 * Pattern(x, np.sin(x))
+    assert np.array_equal(pattern.y, np.sin(x) * 2)
+
+
+def test_using_background_pattern():
+    x = np.linspace(-5, 5, 100)
+    pattern_y = x ** 2
+    bkg_y = x
+
+    spec = Pattern(x, pattern_y)
+    background_pattern = Pattern(x, bkg_y)
+
+    spec.background_pattern = background_pattern
+    new_x, new_y = spec.data
+
+    assert np.array_equal(new_x, x)
+    assert np.array_equal(new_y, pattern_y - bkg_y)
+
+
+def test_using_background_pattern_with_different_spacing():
+    x = np.linspace(-5, 5, 100)
+    pattern_y = x ** 2
+    x_bkg = np.linspace(-5, 5, 99)
+    bkg_y = x_bkg
+
+    spec = Pattern(x, pattern_y)
+    background_pattern = Pattern(x_bkg, bkg_y)
+
+    spec.background_pattern = background_pattern
+    new_x, new_y = spec.data
+
+    assert np.array_equal(new_x, x)
+    assert np.array_equal(new_y, pattern_y - x)
+
+
+def test_background_out_of_range_throws_error():
+    x1 = np.linspace(0, 10)
+    x2 = np.linspace(-10, -1)
+
+    spec = Pattern(x1, x1)
+    background_pattern = Pattern(x2, x2)
+
+    with pytest.raises(BkgNotInRangeError):
+        spec.background_pattern = background_pattern
+
 
-    def test_automatic_background_subtraction(self):
-        x = np.linspace(0, 24, 2500)
-        y = np.zeros(x.shape)
+def test_automatic_background_subtraction():
+    x = np.linspace(0, 24, 2500)
+    y = np.zeros(x.shape)
 
-        peaks = [
-            [10, 3, 0.1],
-            [12, 4, 0.1],
-            [12, 6, 0.1],
-        ]
-        for peak in peaks:
-            y += gaussian(x, peak[0], peak[1], peak[2])
-        y_bkg = x * 0.4 + 5.0
-        y_measurement = y + y_bkg
+    peaks = [
+        [10, 3, 0.1],
+        [12, 4, 0.1],
+        [12, 6, 0.1],
+    ]
+    for peak in peaks:
+        y += gaussian(x, peak[0], peak[1], peak[2])
+    y_bkg = x * 0.4 + 5.0
+    y_measurement = y + y_bkg
 
-        pattern = Pattern(x, y_measurement)
+    pattern = Pattern(x, y_measurement)
 
-        auto_background_subtraction_parameters = [2, 50, 50]
-        pattern.set_auto_background_subtraction(auto_background_subtraction_parameters)
+    auto_background_subtraction_parameters = [2, 50, 50]
+    pattern.set_auto_background_subtraction(auto_background_subtraction_parameters)
 
-        x_spec, y_spec = pattern.data
+    x_spec, y_spec = pattern.data
 
-        self.array_almost_equal(y_spec, y)
+    assert y_spec == approx(y, abs=1e-4)
 
-    def test_automatic_background_subtraction_with_roi(self):
-        x = np.linspace(0, 24, 2500)
-        y = np.zeros(x.shape)
 
-        peaks = [
-            [10, 3, 0.1],
-            [12, 4, 0.1],
-            [12, 6, 0.1],
-        ]
-        for peak in peaks:
-            y += gaussian(x, peak[0], peak[1], peak[2])
-        y_bkg = x * 0.4 + 5.0
-        y_measurement = y + y_bkg
+def test_automatic_background_subtraction_with_roi():
+    x = np.linspace(0, 24, 2500)
+    y = np.zeros(x.shape)
 
-        roi = [1, 23]
+    peaks = [
+        [10, 3, 0.1],
+        [12, 4, 0.1],
+        [12, 6, 0.1],
+    ]
+    for peak in peaks:
+        y += gaussian(x, peak[0], peak[1], peak[2])
+    y_bkg = x * 0.4 + 5.0
+    y_measurement = y + y_bkg
 
-        pattern = Pattern(x, y_measurement)
+    roi = [1, 23]
 
-        auto_background_subtraction_parameters = [2, 50, 50]
-        pattern.set_auto_background_subtraction(auto_background_subtraction_parameters, roi)
+    pattern = Pattern(x, y_measurement)
 
-        x_spec, y_spec = pattern.data
+    auto_background_subtraction_parameters = [2, 50, 50]
+    pattern.set_auto_background_subtraction(auto_background_subtraction_parameters, roi)
 
-        self.assertGreater(x_spec[0], roi[0])
-        self.assertLess(x_spec[-1], roi[1])
+    x_spec, y_spec = pattern.data
 
-        # self.array_almost_equal(y_spec, y)
+    assert x_spec[0] > roi[0]
+    assert x_spec[-1] < roi[1]
 
-    def test_setting_new_data(self):
-        spec = Pattern()
-        x = np.linspace(0, 10)
-        y = np.sin(x)
-        spec.data = x, y
 
-        new_x, new_y = spec.data
-        self.array_almost_equal(new_x, x)
-        self.array_almost_equal(new_y, y)
+def test_setting_new_data():
+    spec = Pattern()
+    x = np.linspace(0, 10)
+    y = np.sin(x)
+    spec.data = x, y
 
-    def test_using_len(self):
-        x = np.linspace(0, 10, 234)
-        y = x ** 2
-        spec = Pattern(x, y)
+    new_x, new_y = spec.data
+    assert np.array_equal(new_x, x)
+    assert np.array_equal(new_y, y)
 
-        self.assertEqual(len(spec), 234)
 
+def test_using_len():
+    x = np.linspace(0, 10, 234)
+    y = x ** 2
+    spec = Pattern(x, y)
 
-if __name__ == '__main__':
-    unittest.main()
+    assert len(spec) == 234
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_PatternModel.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_PatternModel.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,64 +14,62 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import unittest
+import pytest
+from pytest import approx
 import os
 import numpy as np
-from numpy.testing import assert_array_almost_equal
 
-from ...model.PatternModel import Pattern, PatternModel
+from ...model.PatternModel import PatternModel
 from ...model.util.PeakShapes import gaussian
 
 unittest_path = os.path.dirname(__file__)
 data_path = os.path.join(unittest_path, '../data')
 
 
-class PatternModelTest(unittest.TestCase):
-    def setUp(self):
-        self.x = np.linspace(0.1, 15, 100)
-        self.y = np.sin(self.x)
-        self.pattern = Pattern(self.x, self.y)
-        self.pattern_model = PatternModel()
-
-    def test_set_pattern(self):
-        self.pattern_model.set_pattern(self.x, self.y, 'hoho')
-        assert_array_almost_equal(self.pattern_model.get_pattern().x, self.x)
-        assert_array_almost_equal(self.pattern_model.get_pattern().y, self.y)
-        self.assertEqual(self.pattern_model.get_pattern().name, 'hoho')
-
-    def test_load_pattern(self):
-        self.pattern_model.load_pattern(os.path.join(data_path, 'pattern_001.xy'))
-        self.assertEqual(self.pattern_model.get_pattern().name, 'pattern_001')
-        self.assertNotEqual(len(self.x), len(self.pattern_model.get_pattern().x))
-        self.assertNotEqual(len(self.y), len(self.pattern_model.get_pattern().y))
-
-    def test_auto_background_subtraction(self):
-        x = np.linspace(0, 24, 2500)
-        y = np.zeros(x.shape)
-
-        peaks = [
-            [10, 3, 0.1],
-            [12, 4, 0.1],
-            [12, 6, 0.1],
-        ]
-        for peak in peaks:
-            y += gaussian(x, peak[0], peak[1], peak[2])
-        y_bkg = x * 0.4 + 5.0
-        y_measurement = y + y_bkg
-
-        self.pattern_model.set_pattern(x, y_measurement)
-
-        auto_background_subtraction_parameters = [2, 50, 50]
-        self.pattern_model.set_auto_background_subtraction(auto_background_subtraction_parameters)
+@pytest.fixture
+def pattern_model():
+    return PatternModel()
 
-        x_spec, y_spec = self.pattern_model.pattern.data
 
-        self.assertAlmostEqual(np.sum(y_spec - y), 0)
+def test_set_pattern(pattern_model: PatternModel):
+    x = np.linspace(0.1, 15, 100)
+    y = np.sin(x)
+    pattern_model.set_pattern(x, y, 'hoho')
+    assert pattern_model.get_pattern().x == approx(x)
+    assert pattern_model.get_pattern().y == approx(y)
+    assert pattern_model.get_pattern().name == 'hoho'
 
 
-if __name__ == '__main__':
-    unittest.main()
+def test_load_pattern(pattern_model: PatternModel):
+    pattern_model.load_pattern(os.path.join(data_path, 'pattern_001.xy'))
+    assert pattern_model.get_pattern().name == 'pattern_001'
+    assert len(pattern_model.get_pattern().x) > 101
+    assert len(pattern_model.get_pattern().y) > 101
+
+
+def test_auto_background_subtraction(pattern_model: PatternModel):
+    x = np.linspace(0, 24, 2500)
+    y = np.zeros(x.shape)
+
+    peaks = [
+        [10, 3, 0.1],
+        [12, 4, 0.1],
+        [12, 6, 0.1],
+    ]
+    for peak in peaks:
+        y += gaussian(x, peak[0], peak[1], peak[2])
+    y_bkg = x * 0.4 + 5.0
+    y_measurement = y + y_bkg
+
+    pattern_model.set_pattern(x, y_measurement)
+
+    auto_background_subtraction_parameters = [2, 50, 50]
+    pattern_model.set_auto_background_subtraction(auto_background_subtraction_parameters)
+
+    x_spec, y_spec = pattern_model.pattern.data
+
+    assert np.sum(y_spec - y) == approx(0, abs=1e-9)
```

### Comparing `dioptas-0.5.6/dioptas/tests/unit_tests/test_background_extraction.py` & `dioptas-0.5.7/dioptas/tests/unit_tests/test_background_extraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,91 +13,82 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import unittest
+
 import numpy as np
+from pytest import approx
 
 from ...model.util import extract_background
 from ...model.util.PeakShapes import gaussian
 
 
-class TestBackgroundExtraction(unittest.TestCase):
+def test_simple_linear_background_with_single_peak():
+    """ We produce a Gaussian peak on a linear background, and test if the background subtraction algorithm
+    can find the correct background.
+    """
+
+    peaks = [[10, 3, 0.1]]
+
+    x, y_data, y_bkg = generate_pattern(peaks)
+
+    # combination
+    y_measurement = y_data + y_bkg
+
+    y_extracted_bkg = extract_background(x, y_measurement, 1)
+    assert np.sum(y_data - (y_measurement - y_extracted_bkg)) == approx(0, abs=1e-7)
+
+
+def test_simple_linear_background_with_multiple_peaks():
+    """ We produce several Gaussian peaks on top of a linear background and test if the background subtraction
+    algorithm can find the correct background.
     """
-    Tests the Background extraction module in the model.util package
+    peaks = [
+        [10, 3, 0.05],
+        [12, 6, 0.05],
+        [12, 9, 0.05],
+    ]
+
+    x, y_data, y_bkg = generate_pattern(peaks)
+
+    # combination
+    y_measurement = y_data + y_bkg
+
+    y_extracted_bkg = extract_background(x, y_measurement, 0.3)
+    assert np.sum(y_data - (y_measurement - y_extracted_bkg)) == approx(0, abs=1e-7)
+
+
+def test_simple_linear_background_with_multiple_close_peaks():
+    """ We produce several close overlapping peaks on top of a linear background and check whether the background
+    algorithm finds the correct background
+    """
+
+    peaks = [
+        [10, 3, 0.1],
+        [12, 3.1, 0.1],
+        [12, 3.4, 0.1],
+    ]
+    x, y_data, y_bkg = generate_pattern(peaks)
+
+    # combination
+    y_measurement = y_data + y_bkg
+
+    y_extracted_bkg = extract_background(x, y_measurement, 1)
+    assert np.sum(y_data - (y_measurement - y_extracted_bkg)) == approx(0, abs=1e-7)
+
+
+def generate_pattern(peaks):
+    """ Generates a pattern with the given peaks. Peaks is a list of lists, where each list contains the
+    parameters of a single peak. The parameters are [position, width, intensity]
     """
-    def test_simple_linear_background_with_single_peak(self):
-        """
-        Here we produce a Gaussian peak on a linear background, and test if the background subtraction algorithm
-        can find the correct background.
-        """
-
-        # Gaussian
-        x = np.linspace(0, 25, 2500)
-        y_data = gaussian(x, 10, 3, 0.1)
-
-        # linear background
-        y_bkg = x * 0.4 + 5.0
-
-        # combination
-        y_measurement = y_data + y_bkg
-
-        y_extracted_bkg = extract_background(x, y_measurement, 1)
-        self.assertAlmostEqual(np.sum(y_data - (y_measurement - y_extracted_bkg)), 0)
-
-    def test_simple_linear_background_with_multiple_peaks(self):
-        """
-        Here we produce several Gaussian peaks on top of a linear background and test if the background subtraction
-        algorithm can find the correct background.
-        """
-
-        # produce peaks
-        x = np.linspace(0, 24, 2500)
-        y_data = np.zeros(x.shape)
-
-        peaks = [
-            [10, 3, 0.05],
-            [12, 6, 0.05],
-            [12, 9, 0.05],
-        ]
-        for peak in peaks:
-            y_data += gaussian(x, peak[0], peak[1], peak[2])
-
-
-        # linear background
-        y_bkg = x * 0.4 + 5.0
-
-        # combination
-        y_measurement = y_data + y_bkg
-
-        y_extracted_bkg = extract_background(x, y_measurement, 0.3)
-        self.assertAlmostEqual(np.sum(y_data - (y_measurement - y_extracted_bkg)), 0)
-
-    def test_simple_linear_background_with_multiple_close_peaks(self):
-        """
-        Here we produce several close overlapping peaks on top of a linear background and check whether the background
-        algorithm finds the correct background
-        """
-
-        # produce peaks
-        x = np.linspace(0, 24, 2500)
-        y_data = np.zeros(x.shape)
-
-        peaks = [
-            [10, 3, 0.1],
-            [12, 3.1, 0.1],
-            [12, 3.4, 0.1],
-        ]
-        for peak in peaks:
-            y_data += gaussian(x, peak[0], peak[1], peak[2])
+    x = np.linspace(0, 24, 2500)
+    y_data = np.zeros(x.shape)
 
-        # background
-        y_bkg = x * 0.4 + 5.0
+    for peak in peaks:
+        y_data += gaussian(x, peak[0], peak[1], peak[2])
 
-        # combination
-        y_measurement = y_data + y_bkg
+    y_bkg = x * 0.4 + 5.0
 
-        y_extracted_bkg = extract_background(x, y_measurement, 1)
-        self.assertAlmostEqual(np.sum(y_data - (y_measurement - y_extracted_bkg)), 0)
+    return x, y_data, y_bkg
```

### Comparing `dioptas-0.5.6/dioptas/tests/utility.py` & `dioptas-0.5.7/dioptas/tests/utility.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/widget_tests/__init__.py` & `dioptas-0.5.7/dioptas/tests/widget_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/widget_tests/test_BatchSurfaceWidget.py` & `dioptas-0.5.7/dioptas/tests/widget_tests/test_BatchSurfaceWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/tests/widget_tests/test_ConfigurationWidget.py` & `dioptas-0.5.7/dioptas/tests/widget_tests/test_ConfigurationWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/CalibrationWidget.py` & `dioptas-0.5.7/dioptas/widgets/CalibrationWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/ConfigurationWidget.py` & `dioptas-0.5.7/dioptas/widgets/ConfigurationWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/CustomWidgets.py` & `dioptas-0.5.7/dioptas/widgets/CustomWidgets.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/EpicsWidgets.py` & `dioptas-0.5.7/dioptas/widgets/EpicsWidgets.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/MainWidget.py` & `dioptas-0.5.7/dioptas/widgets/MainWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/MaskWidget.py` & `dioptas-0.5.7/dioptas/widgets/MaskWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/UtilityWidgets.py` & `dioptas-0.5.7/dioptas/widgets/UtilityWidgets.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/__init__.py` & `dioptas-0.5.7/dioptas/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/BatchWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/BatchWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/CustomWidgets.py` & `dioptas-0.5.7/dioptas/widgets/integration/CustomWidgets.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/JcpdsEditorWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/JcpdsEditorWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/__init__.py` & `dioptas-0.5.7/dioptas/widgets/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/BackgroundWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/BackgroundWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/CorrectionsWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/CorrectionsWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/ImageWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/ImageWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/OptionsWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/OptionsWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/OverlayWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/OverlayWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/PatternWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/PatternWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/PhaseWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/PhaseWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/control/__init__.py` & `dioptas-0.5.7/dioptas/widgets/integration/control/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/display/ImgWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/display/ImgWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/display/PatternWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/display/PatternWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/integration/display/StatusWidget.py` & `dioptas-0.5.7/dioptas/widgets/integration/display/StatusWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/Custom3DAxis.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/Custom3DAxis.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/ExLegendItem.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/ExLegendItem.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/HistogramLUTItem.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/HistogramLUTItem.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/ImgWidget.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/ImgWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         # most of this code is copied behavior of left click mouse drag from the original code
         ev.accept()
         pos = ev.pos()
         lastPos = ev.lastPos()
         dif = pos - lastPos
         dif *= -1
         ## Ignore axes if mouse is disabled
-        mouseEnabled = np.array(self.img_view_box.state['mouseEnabled'], dtype=np.float)
+        mouseEnabled = np.array(self.img_view_box.state['mouseEnabled'], dtype=float)
         mask = mouseEnabled.copy()
         if axis is not None:
             mask[1 - axis] = 0.0
 
         if ev.button() == QtCore.Qt.RightButton or \
                 (ev.button() == QtCore.Qt.LeftButton and \
                  ev.modifiers() & QtCore.Qt.ControlModifier):
```

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/PatternWidget.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/PatternWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/SurfaceWidget.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/SurfaceWidget.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/dioptas/widgets/plot_widgets/__init__.py` & `dioptas-0.5.7/dioptas/widgets/plot_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/Makefile` & `dioptas-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/make.bat` & `dioptas-0.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/calibration.rst` & `dioptas-0.5.7/docs/source/calibration.rst`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/conf.py` & `dioptas-0.5.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/configurations_and_projects.rst` & `dioptas-0.5.7/docs/source/configurations_and_projects.rst`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/background_control.png` & `dioptas-0.5.7/docs/source/images/background_control.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/background_inspect.png` & `dioptas-0.5.7/docs/source/images/background_inspect.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/cor_control.png` & `dioptas-0.5.7/docs/source/images/cor_control.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/erase_icon.png` & `dioptas-0.5.7/docs/source/images/erase_icon.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/image_widget_qa.png` & `dioptas-0.5.7/docs/source/images/image_widget_qa.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/integration_options.png` & `dioptas-0.5.7/docs/source/images/integration_options.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/integration_view.png` & `dioptas-0.5.7/docs/source/images/integration_view.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/integration_view_configuration.png` & `dioptas-0.5.7/docs/source/images/integration_view_configuration.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/integration_view_modules.png` & `dioptas-0.5.7/docs/source/images/integration_view_modules.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/integration_view_project_controls.png` & `dioptas-0.5.7/docs/source/images/integration_view_project_controls.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/jcpds_editor.png` & `dioptas-0.5.7/docs/source/images/jcpds_editor.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/mask_view.png` & `dioptas-0.5.7/docs/source/images/mask_view.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/open_icon.png` & `dioptas-0.5.7/docs/source/images/open_icon.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/overlay_control.png` & `dioptas-0.5.7/docs/source/images/overlay_control.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/peak_selection.png` & `dioptas-0.5.7/docs/source/images/peak_selection.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/peak_selection2.png` & `dioptas-0.5.7/docs/source/images/peak_selection2.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/phase_control.png` & `dioptas-0.5.7/docs/source/images/phase_control.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/refinement_options.png` & `dioptas-0.5.7/docs/source/images/refinement_options.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/save_icon.png` & `dioptas-0.5.7/docs/source/images/save_icon.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/images/start_values.png` & `dioptas-0.5.7/docs/source/images/start_values.png`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/integration.rst` & `dioptas-0.5.7/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/introduction.rst` & `dioptas-0.5.7/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/docs/source/mask.rst` & `dioptas-0.5.7/docs/source/mask.rst`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/license.txt` & `dioptas-0.5.7/license.txt`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/scripts/dioptas_batch.py` & `dioptas-0.5.7/scripts/dioptas_batch.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/scripts/dropbox_upload.py` & `dioptas-0.5.7/scripts/dropbox_upload.py`

 * *Files identical despite different names*

### Comparing `dioptas-0.5.6/setup.cfg` & `dioptas-0.5.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,117 +3,117 @@
 00000020: 7269 7074 696f 6e20 3d20 4755 4920 7072  ription = GUI pr
 00000030: 6f67 7261 6d20 666f 7220 7265 6475 6374  ogram for reduct
 00000040: 696f 6e20 616e 6420 6578 706c 6f72 6174  ion and explorat
 00000050: 696f 6e20 6f66 2032 4420 582d 7261 7920  ion of 2D X-ray 
 00000060: 6469 6666 7261 6374 696f 6e20 6461 7461  diffraction data
 00000070: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000080: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-00000090: 452e 7273 740d 0a6c 6f6e 675f 6465 7363  E.rst..long_desc
-000000a0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000b0: 7479 7065 203d 2074 6578 742f 782d 7273  type = text/x-rs
-000000c0: 740d 0a61 7574 686f 7220 3d20 436c 656d  t..author = Clem
-000000d0: 656e 7320 5072 6573 6368 6572 0d0a 6175  ens Prescher..au
-000000e0: 7468 6f72 5f65 6d61 696c 203d 2063 6c65  thor_email = cle
-000000f0: 6d65 6e73 2e70 7265 7363 6865 7240 676d  mens.prescher@gm
-00000100: 6169 6c2e 636f 6d0d 0a75 726c 203d 2068  ail.com..url = h
-00000110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000120: 6d2f 4469 6f70 7461 732f 4469 6f70 7461  m/Dioptas/Diopta
-00000130: 730d 0a6c 6963 656e 7365 203d 2047 504c  s..license = GPL
-00000140: 2d33 2e30 0d0a 706c 6174 666f 726d 7320  -3.0..platforms 
-00000150: 3d20 616e 790d 0a63 6c61 7373 6966 6965  = any..classifie
-00000160: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-00000170: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-00000180: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-00000190: 626c 650d 0a09 496e 7465 6e64 6564 2041  ble...Intended A
-000001a0: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-000001b0: 6365 2f52 6573 6561 7263 680d 0a09 546f  ce/Research...To
-000001c0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000001d0: 632f 456e 6769 6e65 6572 696e 670d 0a09  c/Engineering...
-000001e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001f0: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
-00000200: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00000210: 6365 6e73 6520 7633 2028 4750 4c76 3329  cense v3 (GPLv3)
-00000220: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000230: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000240: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
-00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000260: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-00000270: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000280: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000290: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
-000002a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002b0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000002c0: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
-000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002e0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-000002f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000300: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000310: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000330: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
-00000360: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
-00000370: 2043 5079 7468 6f6e 0d0a 6b65 7977 6f72   CPython..keywor
-00000380: 6473 203d 2078 2d72 6179 2064 6966 6672  ds = x-ray diffr
-00000390: 6163 7469 6f6e 2c20 7379 6e63 6872 6f74  action, synchrot
-000003a0: 726f 6e2c 2068 6967 6820 7072 6573 7375  ron, high pressu
-000003b0: 7265 2c20 6772 6170 6869 6361 6c20 7573  re, graphical us
-000003c0: 6572 2069 6e74 6572 6661 6365 0d0a 7072  er interface..pr
-000003d0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-000003e0: 536f 7572 6365 203d 2068 7474 7073 3a2f  Source = https:/
-000003f0: 2f67 6974 6875 622e 636f 6d2f 6469 6f70  /github.com/diop
-00000400: 7461 732f 6469 6f70 7461 730d 0a09 4368  tas/dioptas...Ch
-00000410: 616e 6765 6c6f 6720 3d20 6874 7470 733a  angelog = https:
-00000420: 2f2f 6769 7468 7562 2e63 6f6d 2f44 696f  //github.com/Dio
-00000430: 7074 6173 2f44 696f 7074 6173 2f62 6c6f  ptas/Dioptas/blo
-00000440: 622f 6465 7665 6c6f 702f 6368 616e 6765  b/develop/change
-00000450: 6c6f 672e 7273 740d 0a09 446f 6375 6d65  log.rst...Docume
-00000460: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-00000470: 2f2f 6469 6f70 7461 732e 7265 6164 7468  //dioptas.readth
-00000480: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-00000490: 6c65 2f0d 0a09 5472 6163 6b65 7220 3d20  le/...Tracker = 
-000004a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000004b0: 6f6d 2f44 696f 7074 6173 2f44 696f 7074  om/Dioptas/Diopt
-000004c0: 6173 2f69 7373 7565 730d 0a0d 0a5b 6f70  as/issues....[op
-000004d0: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
-000004e0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-000004f0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000500: 370d 0a73 6574 7570 5f72 6571 7569 7265  7..setup_require
-00000510: 7320 3d20 0d0a 0973 6574 7570 746f 6f6c  s = ...setuptool
-00000520: 735f 7363 6d0d 0a09 6379 7468 6f6e 0d0a  s_scm...cython..
-00000530: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000540: 203d 200d 0a09 6379 7468 6f6e 0d0a 0965   = ...cython...e
-00000550: 7874 7261 5f64 6174 610d 0a09 6675 7475  xtra_data...futu
-00000560: 7265 0d0a 0968 3570 790d 0a09 6864 6635  re...h5py...hdf5
-00000570: 706c 7567 696e 0d0a 096c 6d66 6974 0d0a  plugin...lmfit..
-00000580: 0970 616e 6461 730d 0a09 7073 7574 696c  .pandas...psutil
-00000590: 0d0a 0970 7963 6966 7277 0d0a 0970 7974  ...pycifrw...pyt
-000005a0: 686f 6e2d 6461 7465 7574 696c 0d0a 0970  hon-dateutil...p
-000005b0: 7969 6e73 7461 6c6c 6572 0d0a 0970 7971  yinstaller...pyq
-000005c0: 7435 0d0a 0970 7966 6169 0d0a 0970 7971  t5...pyfai...pyq
-000005d0: 7467 7261 7068 0d0a 0971 7470 790d 0a09  tgraph...qtpy...
-000005e0: 7363 696b 6974 2d69 6d61 6765 0d0a 0973  scikit-image...s
-000005f0: 6861 7265 646d 656d 0d0a 0977 6174 6368  haredmem...watch
-00000600: 646f 670d 0a0d 0a5b 6f70 7469 6f6e 732e  dog....[options.
-00000610: 7061 636b 6167 655f 6461 7461 5d0d 0a64  package_data]..d
-00000620: 696f 7074 6173 203d 200d 0a09 7265 736f  ioptas = ...reso
-00000630: 7572 6365 732f 7374 796c 652f 2a0d 0a09  urces/style/*...
-00000640: 7265 736f 7572 6365 732f 6361 6c69 6272  resources/calibr
-00000650: 616e 7473 2f2a 0d0a 0972 6573 6f75 7263  ants/*...resourc
-00000660: 6573 2f64 6174 612f 2a0d 0a09 7265 736f  es/data/*...reso
-00000670: 7572 6365 732f 6963 6f6e 732f 2a0d 0a09  urces/icons/*...
-00000680: 5f5f 7665 7273 696f 6e5f 5f0d 0a0d 0a5b  __version__....[
-00000690: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-000006a0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000006b0: 6372 6970 7473 203d 200d 0a09 6469 6f70  cripts = ...diop
-000006c0: 7461 7320 3d20 7363 7269 7074 733a 6469  tas = scripts:di
-000006d0: 6f70 7461 732e 6d61 696e 0d0a 0964 696f  optas.main...dio
-000006e0: 7074 6173 5f62 6174 6368 203d 2073 6372  ptas_batch = scr
-000006f0: 6970 7473 3a64 696f 7074 6173 5f62 6174  ipts:dioptas_bat
-00000700: 6368 2e6d 6169 6e0d 0a0d 0a5b 636f 7665  ch.main....[cove
-00000710: 7261 6765 3a72 756e 5d0d 0a6f 6d69 7420  rage:run]..omit 
-00000720: 3d20 0d0a 095f 7665 7273 696f 6e2e 7079  = ..._version.py
-00000730: 0d0a 0964 696f 7074 6173 2f74 6573 7473  ...dioptas/tests
-00000740: 2f2a 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  /*....[egg_info]
-00000750: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000760: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000090: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+000000a0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000b0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+000000c0: 6f77 6e0d 0a61 7574 686f 7220 3d20 436c  own..author = Cl
+000000d0: 656d 656e 7320 5072 6573 6368 6572 0d0a  emens Prescher..
+000000e0: 6175 7468 6f72 5f65 6d61 696c 203d 2063  author_email = c
+000000f0: 6c65 6d65 6e73 2e70 7265 7363 6865 7240  lemens.prescher@
+00000100: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
+00000110: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000120: 636f 6d2f 4469 6f70 7461 732f 4469 6f70  com/Dioptas/Diop
+00000130: 7461 730d 0a6c 6963 656e 7365 203d 2047  tas..license = G
+00000140: 504c 2d33 2e30 0d0a 706c 6174 666f 726d  PL-3.0..platform
+00000150: 7320 3d20 616e 790d 0a63 6c61 7373 6966  s = any..classif
+00000160: 6965 7273 203d 200d 0a09 4465 7665 6c6f  iers = ...Develo
+00000170: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000180: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+00000190: 7461 626c 650d 0a09 496e 7465 6e64 6564  table...Intended
+000001a0: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+000001b0: 656e 6365 2f52 6573 6561 7263 680d 0a09  ence/Research...
+000001c0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
+000001d0: 6669 632f 456e 6769 6e65 6572 696e 670d  fic/Engineering.
+000001e0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001f0: 2041 7070 726f 7665 6420 3a3a 2047 4e55   Approved :: GNU
+00000200: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+00000210: 4c69 6365 6e73 6520 7633 2028 4750 4c76  License v3 (GPLv
+00000220: 3329 0d0a 094f 7065 7261 7469 6e67 2053  3)...Operating S
+00000230: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000240: 7065 6e64 656e 740d 0a09 5072 6f67 7261  pendent...Progra
+00000250: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000260: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000290: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
+000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002c0: 332e 370d 0a09 5072 6f67 7261 6d6d 696e  3.7...Programmin
+000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002e0: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
+000002f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000300: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000310: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
+00000320: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000330: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+00000340: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000350: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000360: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
+00000370: 3a3a 2043 5079 7468 6f6e 0d0a 6b65 7977  :: CPython..keyw
+00000380: 6f72 6473 203d 2078 2d72 6179 2064 6966  ords = x-ray dif
+00000390: 6672 6163 7469 6f6e 2c20 7379 6e63 6872  fraction, synchr
+000003a0: 6f74 726f 6e2c 2068 6967 6820 7072 6573  otron, high pres
+000003b0: 7375 7265 2c20 6772 6170 6869 6361 6c20  sure, graphical 
+000003c0: 7573 6572 2069 6e74 6572 6661 6365 0d0a  user interface..
+000003d0: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
+000003e0: 0a09 536f 7572 6365 203d 2068 7474 7073  ..Source = https
+000003f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6469  ://github.com/di
+00000400: 6f70 7461 732f 6469 6f70 7461 730d 0a09  optas/dioptas...
+00000410: 4368 616e 6765 6c6f 6720 3d20 6874 7470  Changelog = http
+00000420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f44  s://github.com/D
+00000430: 696f 7074 6173 2f44 696f 7074 6173 2f62  ioptas/Dioptas/b
+00000440: 6c6f 622f 6465 7665 6c6f 702f 6368 616e  lob/develop/chan
+00000450: 6765 6c6f 672e 7273 740d 0a09 446f 6375  gelog.rst...Docu
+00000460: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
+00000470: 733a 2f2f 6469 6f70 7461 732e 7265 6164  s://dioptas.read
+00000480: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00000490: 6162 6c65 2f0d 0a09 5472 6163 6b65 7220  able/...Tracker 
+000004a0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000004b0: 2e63 6f6d 2f44 696f 7074 6173 2f44 696f  .com/Dioptas/Dio
+000004c0: 7074 6173 2f69 7373 7565 730d 0a0d 0a5b  ptas/issues....[
+000004d0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+000004e0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000004f0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000500: 332e 370d 0a73 6574 7570 5f72 6571 7569  3.7..setup_requi
+00000510: 7265 7320 3d20 0d0a 0973 6574 7570 746f  res = ...setupto
+00000520: 6f6c 735f 7363 6d0d 0a09 6379 7468 6f6e  ols_scm...cython
+00000530: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000540: 6573 203d 200d 0a09 6379 7468 6f6e 0d0a  es = ...cython..
+00000550: 0965 7874 7261 5f64 6174 610d 0a09 6675  .extra_data...fu
+00000560: 7475 7265 0d0a 0968 3570 790d 0a09 6864  ture...h5py...hd
+00000570: 6635 706c 7567 696e 0d0a 096c 6d66 6974  f5plugin...lmfit
+00000580: 0d0a 0970 616e 6461 730d 0a09 7073 7574  ...pandas...psut
+00000590: 696c 0d0a 0970 7963 6966 7277 0d0a 0970  il...pycifrw...p
+000005a0: 7974 686f 6e2d 6461 7465 7574 696c 0d0a  ython-dateutil..
+000005b0: 0970 7971 7436 0d0a 0970 7966 6169 3e3d  .pyqt6...pyfai>=
+000005c0: 3230 3233 2e31 2e30 0d0a 0970 7971 7467  2023.1.0...pyqtg
+000005d0: 7261 7068 0d0a 0971 7470 790d 0a09 7363  raph...qtpy...sc
+000005e0: 696b 6974 2d69 6d61 6765 0d0a 0973 6861  ikit-image...sha
+000005f0: 7265 646d 656d 0d0a 0977 6174 6368 646f  redmem...watchdo
+00000600: 670d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  g....[options.pa
+00000610: 636b 6167 655f 6461 7461 5d0d 0a64 696f  ckage_data]..dio
+00000620: 7074 6173 203d 200d 0a09 7265 736f 7572  ptas = ...resour
+00000630: 6365 732f 7374 796c 652f 2a0d 0a09 7265  ces/style/*...re
+00000640: 736f 7572 6365 732f 6361 6c69 6272 616e  sources/calibran
+00000650: 7473 2f2a 0d0a 0972 6573 6f75 7263 6573  ts/*...resources
+00000660: 2f64 6174 612f 2a0d 0a09 7265 736f 7572  /data/*...resour
+00000670: 6365 732f 6963 6f6e 732f 2a0d 0a09 5f5f  ces/icons/*...__
+00000680: 7665 7273 696f 6e5f 5f0d 0a0d 0a5b 6f70  version__....[op
+00000690: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000006a0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000006b0: 6970 7473 203d 200d 0a09 6469 6f70 7461  ipts = ...diopta
+000006c0: 7320 3d20 7363 7269 7074 733a 6469 6f70  s = scripts:diop
+000006d0: 7461 732e 6d61 696e 0d0a 0964 696f 7074  tas.main...diopt
+000006e0: 6173 5f62 6174 6368 203d 2073 6372 6970  as_batch = scrip
+000006f0: 7473 3a64 696f 7074 6173 5f62 6174 6368  ts:dioptas_batch
+00000700: 2e6d 6169 6e0d 0a0d 0a5b 636f 7665 7261  .main....[covera
+00000710: 6765 3a72 756e 5d0d 0a6f 6d69 7420 3d20  ge:run]..omit = 
+00000720: 0d0a 095f 7665 7273 696f 6e2e 7079 0d0a  ..._version.py..
+00000730: 0964 696f 7074 6173 2f74 6573 7473 2f2a  .dioptas/tests/*
+00000740: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000750: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000760: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```


# Comparing `tmp/dfm_tools-0.10.55.tar.gz` & `tmp/dfm_tools-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfm_tools-0.10.55.tar", last modified: Sun Apr 23 21:19:24 2023, max compression
+gzip compressed data, was "dfm_tools-0.11.0.tar", last modified: Sun Apr 23 22:49:21 2023, max compression
```

## Comparing `dfm_tools-0.10.55.tar` & `dfm_tools-0.11.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:19:24.848843 dfm_tools-0.10.55/
--rw-rw-rw-   0        0        0    35823 2021-05-31 08:26:08.000000 dfm_tools-0.10.55/LICENSE
--rw-rw-rw-   0        0        0     4083 2023-04-23 21:19:24.849848 dfm_tools-0.10.55/PKG-INFO
--rw-rw-rw-   0        0        0     3375 2023-04-23 21:13:27.000000 dfm_tools-0.10.55/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 21:19:24.820848 dfm_tools-0.10.55/dfm_tools/
--rw-rw-rw-   0        0        0      883 2023-04-23 21:17:19.000000 dfm_tools-0.10.55/dfm_tools/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-04-14 22:09:00.000000 dfm_tools-0.10.55/dfm_tools/bathymetry.py
--rw-rw-rw-   0        0        0     3057 2023-04-23 20:55:04.000000 dfm_tools-0.10.55/dfm_tools/deprecated.py
--rw-rw-rw-   0        0        0    17438 2023-04-23 11:04:48.000000 dfm_tools-0.10.55/dfm_tools/download.py
--rw-rw-rw-   0        0        0     3782 2023-03-31 16:31:41.000000 dfm_tools-0.10.55/dfm_tools/energy_dissipation.py
--rw-rw-rw-   0        0        0      140 2023-04-14 22:09:00.000000 dfm_tools-0.10.55/dfm_tools/errors.py
--rw-rw-rw-   0        0        0    29334 2023-04-23 20:55:04.000000 dfm_tools-0.10.55/dfm_tools/get_nc.py
--rw-rw-rw-   0        0        0     9989 2023-04-23 20:55:04.000000 dfm_tools-0.10.55/dfm_tools/get_nc_helpers.py
--rw-rw-rw-   0        0        0    18721 2023-04-17 18:50:52.000000 dfm_tools-0.10.55/dfm_tools/hydrolib_helpers.py
--rw-rw-rw-   0        0        0    32675 2023-04-14 22:09:00.000000 dfm_tools-0.10.55/dfm_tools/interpolate_grid2bnd.py
--rw-rw-rw-   0        0        0     1078 2023-04-14 22:09:00.000000 dfm_tools-0.10.55/dfm_tools/linebuilder.py
--rw-rw-rw-   0        0        0    10474 2023-04-22 20:53:18.000000 dfm_tools-0.10.55/dfm_tools/meshkernel_helpers.py
--rw-rw-rw-   0        0        0    13442 2023-04-22 20:53:18.000000 dfm_tools-0.10.55/dfm_tools/modelbuilder.py
--rw-rw-rw-   0        0        0    24633 2023-03-31 19:02:03.000000 dfm_tools-0.10.55/dfm_tools/modplot.py
--rw-rw-rw-   0        0        0     7628 2023-04-23 20:55:04.000000 dfm_tools-0.10.55/dfm_tools/regulargrid.py
--rw-rw-rw-   0        0        0    24710 2023-03-31 02:51:40.000000 dfm_tools-0.10.55/dfm_tools/streamplot_COPY.py
--rw-rw-rw-   0        0        0    28001 2023-04-20 11:36:35.000000 dfm_tools-0.10.55/dfm_tools/xarray_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:19:24.840840 dfm_tools-0.10.55/dfm_tools.egg-info/
--rw-rw-rw-   0        0        0     4083 2023-04-23 21:19:24.000000 dfm_tools-0.10.55/dfm_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-04-23 21:19:24.000000 dfm_tools-0.10.55/dfm_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:19:24.000000 dfm_tools-0.10.55/dfm_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-05-31 08:41:23.000000 dfm_tools-0.10.55/dfm_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      363 2023-04-23 21:19:24.000000 dfm_tools-0.10.55/dfm_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-23 21:19:24.000000 dfm_tools-0.10.55/dfm_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1804 2023-04-23 21:19:24.852958 dfm_tools-0.10.55/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-01-24 21:20:28.000000 dfm_tools-0.10.55/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:19:24.846845 dfm_tools-0.10.55/tests/
--rw-rw-rw-   0        0        0       40 2021-05-31 08:26:08.000000 dfm_tools-0.10.55/tests/__init__.py
--rw-rw-rw-   0        0        0    20154 2023-04-23 20:12:33.000000 dfm_tools-0.10.55/tests/test_dfm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/dfm_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17127 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/energy_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28771 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9793 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/get_nc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18353 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32206 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/linebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13218 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23929 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/modplot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/regulargrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27467 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/xarray_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/dfm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-04-23 22:49:21.437927 dfm_tools-0.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19768 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/tests/test_dfm_tools.py
```

### Comparing `dfm_tools-0.10.55/PKG-INFO` & `dfm_tools-0.11.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-Metadata-Version: 2.1
-Name: dfm_tools
-Version: 0.10.55
-Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
-Home-page: https://github.com/Deltares/dfm_tools
-Author: Jelmer Veenstra
-Author-email: Jelmer.Veenstra@Deltares.nl
-License: GNU General Public License v3 (GPLv3)
-Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: complete
-
-[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
-[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
-[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
-[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
-[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
-
-dfm_tools
-=========
-
-A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
-
-Information and examples
---------
-- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
-- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
-
-
-Installation
---------
-- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
-- open Anaconda prompt
-- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
-- ``conda activate dfm_tools_env``
-- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
-- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
-- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
-- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
-- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
+Metadata-Version: 2.1
+Name: dfm_tools
+Version: 0.11.0
+Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
+Home-page: https://github.com/Deltares/dfm_tools
+Author: Jelmer Veenstra
+Author-email: Jelmer.Veenstra@Deltares.nl
+License: GNU General Public License v3 (GPLv3)
+Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: complete
+
+[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
+[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
+[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
+[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
+[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+
+dfm_tools
+=========
+
+A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
+
+Information and examples
+--------
+- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
+- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
+- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
+- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
+- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
+
+Installation basics
+--------
+- latest release: ``pip install dfm_tools`` (excludes ``cartopy`` since it is only installable via conda)
+
+Installation recommendation
+--------
+- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
+- open Anaconda prompt
+- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
+- ``conda activate dfm_tools_env``
+- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
+- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
+- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
+- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
+- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
```

### Comparing `dfm_tools-0.10.55/README.md` & `dfm_tools-0.11.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
-[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
-[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
-[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
-[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
-
-dfm_tools
-=========
-
-A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
-
-Information and examples
---------
-- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
-- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
-
-
-Installation
---------
-- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
-- open Anaconda prompt
-- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
-- ``conda activate dfm_tools_env``
-- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
-- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
-- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
-- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
-- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
+[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
+[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
+[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
+[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
+[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+
+dfm_tools
+=========
+
+A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
+
+Information and examples
+--------
+- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
+- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
+- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
+- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
+- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
+
+Installation basics
+--------
+- latest release: ``pip install dfm_tools`` (excludes ``cartopy`` since it is only installable via conda)
+
+Installation recommendation
+--------
+- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
+- open Anaconda prompt
+- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
+- ``conda activate dfm_tools_env``
+- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
+- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
+- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
+- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
+- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
```

### Comparing `dfm_tools-0.10.55/dfm_tools/__init__.py` & `dfm_tools-0.11.0/dfm_tools/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-.. include:: ../README.md
-"""
-
-__author__ = """Jelmer Veenstra"""
-__email__ = 'jelmer.veenstra@deltares.nl'
-__version__ = '0.10.55'
-
-from dfm_tools.deprecated import *
-from dfm_tools.errors import *
-from dfm_tools.download import *
-from dfm_tools.get_nc import *
-from dfm_tools.get_nc_helpers import *
-from dfm_tools.hydrolib_helpers import *
-from dfm_tools.meshkernel_helpers import *
-from dfm_tools.interpolate_grid2bnd import *
-from dfm_tools.linebuilder import *
-from dfm_tools.modplot import *
-from dfm_tools.regulargrid import *
-from dfm_tools.xarray_helpers import *
-from dfm_tools.energy_dissipation import *
-from dfm_tools.bathymetry import *
-#from dfm_tools.modelbuilder import * #commented since we do not want to expose these functions with hardcoded parameters
-
-import warnings
-warnings.filterwarnings('always',category=DeprecationWarning)
+"""
+.. include:: ../README.md
+"""
+
+__author__ = """Jelmer Veenstra"""
+__email__ = 'jelmer.veenstra@deltares.nl'
+__version__ = '0.11.0'
+
+from dfm_tools.deprecated import *
+from dfm_tools.errors import *
+from dfm_tools.download import *
+from dfm_tools.get_nc import *
+from dfm_tools.get_nc_helpers import *
+from dfm_tools.hydrolib_helpers import *
+from dfm_tools.meshkernel_helpers import *
+from dfm_tools.interpolate_grid2bnd import *
+from dfm_tools.linebuilder import *
+from dfm_tools.modplot import *
+from dfm_tools.regulargrid import *
+from dfm_tools.xarray_helpers import *
+from dfm_tools.energy_dissipation import *
+from dfm_tools.bathymetry import *
+#from dfm_tools.modelbuilder import * #commented since we do not want to expose these functions with hardcoded parameters
+
+import warnings
+warnings.filterwarnings('always',category=DeprecationWarning)
```

### Comparing `dfm_tools-0.10.55/dfm_tools/bathymetry.py` & `dfm_tools-0.11.0/dfm_tools/bathymetry.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon May 31 17:17:09 2021
-
-@author: veenstra
-"""
-
-import numpy as np
-
-
-def write_bathy_toasc(filename_asc,lon_sel_ext,lat_sel_ext,elev_sel_ext,asc_fmt='%9.2f',nodata_val=32767):
-
-    print('writing to asc file')
-    if elev_sel_ext.shape != (lat_sel_ext.shape[0], lon_sel_ext.shape[0]):
-        raise ValueError('resulting shape of elev_sel_ext %s is not consistent with lat_sel_ext/lon_sel_ext vars %s'%(elev_sel_ext.shape,(lat_sel_ext.shape[0], lon_sel_ext.shape[0])))
-    if isinstance(elev_sel_ext,np.ma.core.MaskedArray): #masked has to be filled in order for the nans to be visible
-        elev_sel_ext = elev_sel_ext.filled(np.nan)
-    if np.isnan(elev_sel_ext).sum()>0:
-        elev_sel_ext = elev_sel_ext.copy()
-        elev_sel_ext[np.isnan(elev_sel_ext)] = nodata_val
-        print('replaced nan values with %d'%(nodata_val))
-    resinv_lonlat = np.round(1/np.diff(lon_sel_ext[:2]),2)
-    resinv_lat = np.round(1/np.diff(lat_sel_ext[:2]),2)
-    if resinv_lonlat!=resinv_lat:
-        raise ValueError('inconsistent resolution over lat/lon')
-    
-    with open(filename_asc,'w') as file_asc:
-        file_asc.write('ncols         %d\n'%(elev_sel_ext.shape[1]))
-        file_asc.write('nrows         %d\n'%(elev_sel_ext.shape[0]))
-        file_asc.write('xllcenter     %13.8f\n'%(lon_sel_ext[0]))
-        file_asc.write('yllcenter     %13.8f\n'%(lat_sel_ext[0]))
-        file_asc.write('cellsize      %16.11f\n'%(1/resinv_lonlat))
-        #file_asc.write('NODATA_value  %d\n'%(nodata_val))
-        file_asc.write('NODATA_value  '+asc_fmt%(nodata_val)+'\n')
-    with open(filename_asc,'a') as file_asc:
-        np.savetxt(file_asc,np.flip(elev_sel_ext,axis=0),fmt=asc_fmt)
-    print('...finished')
-
+# -*- coding: utf-8 -*-
+"""
+Created on Mon May 31 17:17:09 2021
+
+@author: veenstra
+"""
+
+import numpy as np
+
+
+def write_bathy_toasc(filename_asc,lon_sel_ext,lat_sel_ext,elev_sel_ext,asc_fmt='%9.2f',nodata_val=32767):
+
+    print('writing to asc file')
+    if elev_sel_ext.shape != (lat_sel_ext.shape[0], lon_sel_ext.shape[0]):
+        raise ValueError('resulting shape of elev_sel_ext %s is not consistent with lat_sel_ext/lon_sel_ext vars %s'%(elev_sel_ext.shape,(lat_sel_ext.shape[0], lon_sel_ext.shape[0])))
+    if isinstance(elev_sel_ext,np.ma.core.MaskedArray): #masked has to be filled in order for the nans to be visible
+        elev_sel_ext = elev_sel_ext.filled(np.nan)
+    if np.isnan(elev_sel_ext).sum()>0:
+        elev_sel_ext = elev_sel_ext.copy()
+        elev_sel_ext[np.isnan(elev_sel_ext)] = nodata_val
+        print('replaced nan values with %d'%(nodata_val))
+    resinv_lonlat = np.round(1/np.diff(lon_sel_ext[:2]),2)
+    resinv_lat = np.round(1/np.diff(lat_sel_ext[:2]),2)
+    if resinv_lonlat!=resinv_lat:
+        raise ValueError('inconsistent resolution over lat/lon')
+    
+    with open(filename_asc,'w') as file_asc:
+        file_asc.write('ncols         %d\n'%(elev_sel_ext.shape[1]))
+        file_asc.write('nrows         %d\n'%(elev_sel_ext.shape[0]))
+        file_asc.write('xllcenter     %13.8f\n'%(lon_sel_ext[0]))
+        file_asc.write('yllcenter     %13.8f\n'%(lat_sel_ext[0]))
+        file_asc.write('cellsize      %16.11f\n'%(1/resinv_lonlat))
+        #file_asc.write('NODATA_value  %d\n'%(nodata_val))
+        file_asc.write('NODATA_value  '+asc_fmt%(nodata_val)+'\n')
+    with open(filename_asc,'a') as file_asc:
+        np.savetxt(file_asc,np.flip(elev_sel_ext,axis=0),fmt=asc_fmt)
+    print('...finished')
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/deprecated.py` & `dfm_tools-0.11.0/dfm_tools/deprecated.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Apr 23 22:42:27 2023
-
-@author: veenstra
-"""
-
-
-def plot_background(ax=None, projection=None, google_style='satellite', resolution=1, features=None, nticks=6, latlon_format=False, gridlines=False, **kwargs):
-    raise DeprecationWarning('dfmt.plot_background() is deprecated, use contextily and cartopy instead like in https://github.com/Deltares/dfm_tools/blob/main/tests/examples_workinprogress/workinprogress_cartopy_satellite_coastlines.py')
-
-
-def get_ugrid_verts(data_xr_map):
-    """
-    getting ugrid verts from xugrid mapfile.
-    """
-    raise DeprecationWarning('dfmt.get_ugrid_verts() is deprecated, use uds.grid.face_node_coordinates instead (https://github.com/Deltares/xugrid/issues/48)')
-
-
-def scatter_to_regulargrid(xcoords, ycoords, values, ncellx=None, ncelly=None, reg_x_vec=None, reg_y_vec=None, method='nearest', maskland_dist=None):
-    raise DeprecationWarning('dfm_tools.regulargrid.scatter_to_regulargrid() is deprecated, use ds = dfmt.rasterize_ugrid(uds) instead')
-
-
-def get_varnamefromattrs(data_xr, varname):
-    raise DeprecationWarning('dfmt.get_varnamefromattrs() will be deprecated in a future version of dfm_tools, ds=dfmt.rename_waqvars(ds) is a more convenient alternative')
-
-
-class Polygon:
-    def __init__(self, data, name, comments):
-        raise DeprecationWarning('the function dfm_tools.polygon.Polygon() is deprecated, please use the new hydrolib alternative.')
-        
-    def fromfile(self, file_pol, pd_output=False, tekmap_output=False):
-        raise DeprecationWarning('the function dfm_tools.polygon.Polygon.fromfile() is deprecated, please use the new hydrolib alternative. Example script: https://github.com/Deltares/dfm_tools/blob/main/tests/examples/preprocess_hydrolib_readwritepol.py')
-
-
-def write_bcfile(filename, datablocks, metadatas, refdate=None, tzone=0, float_format='%6.2f'):
-    raise DeprecationWarning('the function dfm_tools.io.bc.write_bcfile() is deprecated, please use the new hydrolib alternative. Example script: dfm_tools/tests/examples/CMEMS_interpolate_example.py')
-
-
-def read_bcfile(filename, converttime=False):
-    raise DeprecationWarning('the function dfm_tools.io.bc.read_bcfile() is deprecated, please use the new hydrolib alternative. Example script: dfm_tools/tests/examples/hydrolib_readbc.py')
-
-
-def write_timfile(filename, datablock, header, converttime=False, refdate=None, float_format='%6.2f'):
-    raise DeprecationWarning('the function dfm_tools.write_timfile() is deprecated, please use the new hydrolib alternative: https://github.com/Deltares/dfm_tools/blob/301-convert-timmodel-to-pandasdataframe/tests/examples/preprocess_hydrolib_readtim.py.')
-
-
-def read_timfile(filename, converttime=False, refdate=None):
-    raise DeprecationWarning('the function dfm_tools.read_timfile() is deprecated, please use the new hydrolib alternative: https://github.com/Deltares/dfm_tools/blob/301-convert-timmodel-to-pandasdataframe/tests/examples/preprocess_hydrolib_readtim.py.')
-
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Apr 23 22:42:27 2023
+
+@author: veenstra
+"""
+
+
+def plot_background(ax=None, projection=None, google_style='satellite', resolution=1, features=None, nticks=6, latlon_format=False, gridlines=False, **kwargs):
+    raise DeprecationWarning('dfmt.plot_background() is deprecated, use contextily and cartopy instead like in https://github.com/Deltares/dfm_tools/blob/main/tests/examples_workinprogress/workinprogress_cartopy_satellite_coastlines.py')
+
+
+def get_ugrid_verts(data_xr_map):
+    """
+    getting ugrid verts from xugrid mapfile.
+    """
+    raise DeprecationWarning('dfmt.get_ugrid_verts() is deprecated, use uds.grid.face_node_coordinates instead (https://github.com/Deltares/xugrid/issues/48)')
+
+
+def scatter_to_regulargrid(xcoords, ycoords, values, ncellx=None, ncelly=None, reg_x_vec=None, reg_y_vec=None, method='nearest', maskland_dist=None):
+    raise DeprecationWarning('dfm_tools.regulargrid.scatter_to_regulargrid() is deprecated, use ds = dfmt.rasterize_ugrid(uds) instead')
+
+
+def get_varnamefromattrs(data_xr, varname):
+    raise DeprecationWarning('dfmt.get_varnamefromattrs() will be deprecated in a future version of dfm_tools, ds=dfmt.rename_waqvars(ds) is a more convenient alternative')
+
+
+class Polygon:
+    def __init__(self, data, name, comments):
+        raise DeprecationWarning('the function dfm_tools.polygon.Polygon() is deprecated, please use the new hydrolib alternative.')
+        
+    def fromfile(self, file_pol, pd_output=False, tekmap_output=False):
+        raise DeprecationWarning('the function dfm_tools.polygon.Polygon.fromfile() is deprecated, please use the new hydrolib alternative. Example script: https://github.com/Deltares/dfm_tools/blob/main/tests/examples/preprocess_hydrolib_readwritepol.py')
+
+
+def write_bcfile(filename, datablocks, metadatas, refdate=None, tzone=0, float_format='%6.2f'):
+    raise DeprecationWarning('the function dfm_tools.io.bc.write_bcfile() is deprecated, please use the new hydrolib alternative. Example script: dfm_tools/tests/examples/CMEMS_interpolate_example.py')
+
+
+def read_bcfile(filename, converttime=False):
+    raise DeprecationWarning('the function dfm_tools.io.bc.read_bcfile() is deprecated, please use the new hydrolib alternative. Example script: dfm_tools/tests/examples/hydrolib_readbc.py')
+
+
+def write_timfile(filename, datablock, header, converttime=False, refdate=None, float_format='%6.2f'):
+    raise DeprecationWarning('the function dfm_tools.write_timfile() is deprecated, please use the new hydrolib alternative: https://github.com/Deltares/dfm_tools/blob/301-convert-timmodel-to-pandasdataframe/tests/examples/preprocess_hydrolib_readtim.py.')
+
+
+def read_timfile(filename, converttime=False, refdate=None):
+    raise DeprecationWarning('the function dfm_tools.read_timfile() is deprecated, please use the new hydrolib alternative: https://github.com/Deltares/dfm_tools/blob/301-convert-timmodel-to-pandasdataframe/tests/examples/preprocess_hydrolib_readtim.py.')
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/download.py` & `dfm_tools-0.11.0/dfm_tools/download.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,311 +1,311 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Oct 18 15:09:26 2022
-
-@author: veenstra
-"""
-
-import os
-import pandas as pd
-from pathlib import Path
-import xarray as xr
-from pydap.client import open_url
-from pydap.cas.get_cookies import setup_session
-import warnings
-from dfm_tools.errors import OutOfRangeError
-import cdsapi
-import cftime
-
-
-def download_ERA5(varkey,
-                  longitude_min, longitude_max, latitude_min, latitude_max, 
-                  date_min, date_max,
-                  dir_output='.', overwrite=False):
-    
-    #TODO: describe something about the .cdsapirc file
-    #TODO: make this function cdsapi generic, instead of ERA5 hardcoded (make flexible for product_type/name/name_output) (variables_dict is not used actively anymore, so this is possible)
-    
-    c = cdsapi.Client() # import cdsapi and create a Client instance # https://cds.climate.copernicus.eu/api-how-to
-    
-    #dictionary with ERA5 variables #this is not actively used
-    variables_dict = {'ssr':'surface_net_solar_radiation',
-                      'sst':'sea_surface_temperature',
-                      'strd':'surface_thermal_radiation_downwards',
-                      'slhf':'surface_latent_heat_flux',
-                      'sshf':'surface_sensible_heat_flux',
-                      'str':'surface_net_thermal_radiation',
-                      'chnk':'charnock',
-                      'd2m':'2m_dewpoint_temperature',
-                      't2m':'2m_temperature',
-                      'tcc':'total_cloud_cover',
-                      'msl':'mean_sea_level_pressure',
-                      'u10':'10m_u_component_of_wind',
-                      'u10n':'10m_u_component_of_neutral_wind',
-                      'v10':'10m_v_component_of_wind',
-                      'v10n':'10m_v_component_of_neutral_wind',
-                      'mer':'mean_evaporation_rate',
-                      'mtpr':'mean_total_precipitation_rate',
-                      }
-    if varkey not in variables_dict.keys(): #TODO: how to get list of available vars? mean_sea_level_pressure and msl both return a dataset with msl varkey, but standard_name air_pressure_at_mean_sea_level returns an error
-        raise KeyError(f'"{varkey}" not available, choose from: {list(variables_dict.keys())}')
-    
-    period_range = pd.period_range(date_min,date_max,freq='M')
-    print(f'retrieving data from {period_range[0]} to {period_range[-1]} (freq={period_range.freq})')
-    
-    for date in period_range:
-        name_output = f'era5_{varkey}_{date.strftime("%Y-%m")}.nc'
-        file_out = Path(dir_output,name_output)
-        if file_out.is_file() and not overwrite:
-            print(f'"{name_output}" found and overwrite=False, continuing.')
-            continue
-        print (f'retrieving ERA5 data for variable "{varkey}" and month {date.strftime("%Y-%m")} (YYYY-MM)')
-
-        request_dict = {'product_type':'reanalysis',
-                        'variable':variables_dict[varkey],
-                        'year':date.strftime('%Y'),
-                        'month':date.strftime('%m'),
-                        #'month':[f'{x:02d}' for x in range(1,12+1)], #all months, but instead retrieving per month
-                        'day':[f'{x:02d}' for x in range(1,31+1)], #all days
-                        'time':[f'{x:02d}:00' for x in range(0,23+1)], #all times/hours
-                        'area':[latitude_max,longitude_min,latitude_min,longitude_max], # north, west, south, east. default: global - option not available through the Climate Data Store (CDS) web interface (for cmip data)
-                        #'grid': [1.0, 1.0], # latitude/longitude grid: east-west (longitude) and north-south resolution (latitude). default: 0.25 x 0.25 - option not available through the Climate Data Store (CDS) web interface
-                        'format':'netcdf'}
-        
-        c.retrieve(name='reanalysis-era5-single-levels', request=request_dict, target=file_out)
-
-
-def download_CMEMS(varkey,
-                   longitude_min, longitude_max, latitude_min, latitude_max, 
-                   date_min, date_max, freq='D',
-                   dir_output='.', file_prefix='', overwrite=False,
-                   credentials=None):
-
-    date_min = pd.Timestamp(date_min)-pd.Timedelta(days=1) #CMEMS has daily noon values (not midnight), so subtract one day from date_min to cover desired time extent
-    
-    if 'my_datemax' not in globals(): #set multiyear date_max (my_datemax) as global variable, so it only has to be retreived once per download run (otherwise once per variable)
-        print('retrieving enddate of multiyear CMEMS dataset')
-        dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m' #assuming here that physchem and bio reanalyisus/multiyear datasets have the same enddate, this seems safe
-        ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
-        my_times = ds.time.to_series()
-        global my_datemax
-        my_datemax = my_times.iloc[-1]
-
-    if pd.Timestamp(date_max) <= my_datemax:
-        product = 'reanalysis'
-    elif pd.Timestamp(date_min) > my_datemax:
-        product = 'analysisforecast'
-    else:
-        raise ValueError(f'Requested timerange is {date_min} to {date_max}. Currently, it is only possible to query periods before OR after the multiyear/reanalysis enddate ({my_datemax}).')
-    
-    Path(dir_output).mkdir(parents=True, exist_ok=True)
-    if varkey in ['bottomT','tob','mlotst','siconc','sithick','so','thetao','uo','vo','usi','vsi','zos']: #for physchem
-        if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
-            if varkey=='bottomT': #rename old to new anfc varname (still called bottomT in reanalysis)
-                varkey = 'tob'
-            if varkey in ['uo','vo']:
-                varkey_name = 'phy-cur'
-            elif varkey in ['so','thetao']:
-                varkey_name = 'phy-'+varkey
-            else:
-                varkey_name = 'phy'
-            dataset_url = f'https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_{varkey_name}_anfc_0.083deg_P1D-m'#.html' #TODO: also PT6H-i timeresolution available but not for all variables and not for reanalysis
-        else: #reanalysis: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/description
-            dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m'
-    else: #for bio
-        if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
-            dataset_url = 'https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily' #contains ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
-        else: #https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/description
-            dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m' #contains ['chl','no3','nppv','o2','po4','si']
-    
-    download_OPeNDAP(dataset_url=dataset_url,
-                     credentials=credentials, #credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'
-                     varkey=varkey,
-                     longitude_min=longitude_min, longitude_max=longitude_max, latitude_min=latitude_min, latitude_max=latitude_max,
-                     date_min=date_min, date_max=date_max,
-                     dir_output=dir_output, file_prefix=file_prefix, overwrite=overwrite)
-
-
-def open_OPeNDAP_xr(dataset_url, credentials=None):
-    """
-    How to get the opendap dataset_url (CMEMS example):
-        - https://data.marine.copernicus.eu/products
-        - go to the data access tab of a product, e.g.: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
-        - click the opendap link of the dataset of your choice
-        - copy the dataset_url from the adress bar (excl .html), e.g.: https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
-        
-        Example multiyear phys/chem:
-            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
-            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
-            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
-        Example multiyear bio:
-            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/services
-            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m
-            ['chl','no3','nppv','o2','po4','si']
-        Example forecast phys/chem:
-            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_PHY_001_024/services
-            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-phy-001-024
-            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
-        Example forecast bio:
-            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_BIO_001_028/services
-            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily
-            ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
-    
-    How to get the opendap dataset_url (HYCOM example):
-        - https://www.hycom.org/dataserver
-        - Select a product and search for THREDDS, e.g.: https://www.hycom.org/dataserver/gofs-3pt1/analysis
-        - find an opendap dataset_url, it depends per product/run where to find it.
-        Some examples:
-            https://tds.hycom.org/thredds/dodsC/GLBu0.08/expt_19.1/2010
-            https://tds.hycom.org/thredds/dodsC/GLBy0.08/expt_93.0
-
-    """
-    
-    def copernicusmarine_datastore(dataset_url, username, password):
-        #https://help.marine.copernicus.eu/en/articles/5182598-how-to-consume-the-opendap-api-and-cas-sso-using-python
-        cas_url = 'https://cmems-cas.cls.fr/cas/login'
-        session = setup_session(cas_url, username, password)
-        cookies_dict = session.cookies.get_dict()
-        if 'CASTGC' not in cookies_dict.keys():
-            raise KeyError('CASTGC key missing from session cookies_dict, probably authentication failure')
-        session.cookies.set("CASTGC", cookies_dict['CASTGC'])
-        #TODO: add check for wrong dataset_id (now always "AttributeError: You cannot set the charset when no content-type is defined")
-        DAP_dataset = open_url(dataset_url, session=session)#, user_charset='utf-8') # TODO: user_charset needs PyDAP >= v3.3.0 see https://github.com/pydap/pydap/pull/223/commits 
-        data_store = xr.backends.PydapDataStore(DAP_dataset)
-        return data_store
-    
-    if isinstance(dataset_url,list):
-        dataset_url_one = dataset_url[0]
-    else:
-        dataset_url_one = dataset_url
-    
-    if 'cmems-du.eu' in dataset_url_one:
-        if isinstance(dataset_url,list):
-            raise TypeError('list not supported by opendap method used for cmems')
-        
-        #parse credentials to username/password #TODO: now CMEMS specific, make more generic
-        if credentials is None:
-            file_credentials = f'{os.path.expanduser("~")}/CMEMS_credentials.txt'
-            if not os.path.exists(file_credentials):
-                raise FileNotFoundError(f'credentials argument not supplied and file_credentials not available ({file_credentials})')
-            with open(file_credentials) as fc:
-                username = fc.readline().strip()
-                password = fc.readline().strip()
-        else:
-            username,password = credentials
-
-        print(f'opening pydap connection to opendap dataset: {dataset_url}.html')
-        data_store = copernicusmarine_datastore(dataset_url=dataset_url, username=username, password=password)
-        print('xarray opening opendap dataset')
-        data_xr = xr.open_dataset(data_store)
-    elif 'hycom.org' in dataset_url_one:
-        if isinstance(dataset_url,list):
-            print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
-            data_xr = xr.open_mfdataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar'."
-        else:
-            print(f'xarray opening opendap dataset: {dataset_url}.html')
-            data_xr = xr.open_dataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar
-        data_xr['time'] = cftime.num2date(data_xr.time,units=data_xr.time.units,calendar=data_xr.time.calendar)
-        data_xr = data_xr.rename({'lon':'longitude','lat':'latitude'})
-    else:
-        print(f'unspecified dataset_url, might fail: {dataset_url}')
-        if isinstance(dataset_url,list):
-            print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
-            data_xr = xr.open_mfdataset(dataset_url)
-        else:
-            print(f'xarray opening opendap dataset: {dataset_url}.html')
-            data_xr = xr.open_dataset(dataset_url)
-        if 'lon' in data_xr.dims:
-            data_xr = data_xr.rename({'lon':'longitude','lat':'latitude'})
-        
-    return data_xr
-
-
-def download_OpenDAP_gettimes(dataset_url,credentials=None):
-    ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
-    ds_time = ds.time.to_series()
-    return ds_time
-
-
-def download_OPeNDAP(dataset_url,
-                     varkey,
-                     longitude_min, longitude_max, latitude_min, latitude_max, 
-                     date_min, date_max, freq='D',
-                     dir_output='.', file_prefix='', overwrite=False,
-                     credentials=None):
-    """
-    
-
-    Parameters
-    ----------
-    dataset_url : TYPE
-        DESCRIPTION.
-    varkey : TYPE
-        DESCRIPTION.
-    longitude_min : TYPE
-        DESCRIPTION.
-    longitude_max : TYPE
-        DESCRIPTION.
-    latitude_min : TYPE
-        DESCRIPTION.
-    latitude_max : TYPE
-        DESCRIPTION.
-    date_min : TYPE
-        DESCRIPTION.
-    date_max : TYPE
-        DESCRIPTION.
-    freq : TYPE, optional
-        DESCRIPTION. The default is 'D'.
-    dir_output : TYPE, optional
-        DESCRIPTION. The default is '.'.
-    file_prefix : TYPE, optional
-        DESCRIPTION. The default is ''.
-    overwrite : TYPE, optional
-        DESCRIPTION. The default is False.
-    credentials : TYPE, optional
-        for CMEMS: credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'. The default is None.
-
-    Raises
-    ------
-    KeyError
-        DESCRIPTION.
-    OutOfRangeError
-        DESCRIPTION.
-
-    Returns
-    -------
-    None.
-
-    """
-    
-    data_xr = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
-    
-    print(f'xarray subsetting data (variable \'{varkey}\' and lon/lat extents)')
-    if varkey not in data_xr.data_vars:
-        raise KeyError(f'"{varkey}" not found in dataset, available are: {list(data_xr.data_vars)}')
-    data_xr_var = data_xr[[varkey]]
-    data_xr_var = data_xr_var.sel(longitude=slice(longitude_min,longitude_max), #TODO: add depth selection?
-                                  latitude=slice(latitude_min,latitude_max))
-    data_xr_times = data_xr_var.time.to_series()
-    print(f'available time range in dataset from {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
-    period_range = pd.period_range(date_min,date_max,freq=freq)
-    
-    #check if date_min/date_max are available in dataset
-    if not (data_xr_times.index[0] <= period_range[0].to_timestamp() <= data_xr_times.index[-1]):
-        raise OutOfRangeError(f'date_min ({period_range[0]}) is outside available time range in dataset: {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
-    if not (data_xr_times.index[0] <= period_range[-1].to_timestamp() <= data_xr_times.index[-1]):
-        raise OutOfRangeError(f'date_max ({period_range[-1]}) is outside available time range in dataset: {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
-    
-    for date in period_range:
-        date_str = str(date)
-        name_output = f'{file_prefix}{varkey}_{date_str}.nc'
-        file_out = Path(dir_output,name_output)
-        if file_out.is_file() and not overwrite:
-            print(f'"{name_output}" found and overwrite=False, continuing.')
-            continue
-        
-        print(f'xarray subsetting data per {period_range.freq}: {date_str}')
-        data_xr_var_seltime = data_xr_var.sel(time=slice(date_str,date_str)) #+' 12:00:00', 
-        
-        print(f'xarray writing netcdf file: {name_output}')
-        data_xr_var_seltime.to_netcdf(os.path.join(dir_output,name_output)) #TODO: add chunks={'time':1} or only possible with opening?
-        data_xr_var_seltime.close()
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Oct 18 15:09:26 2022
+
+@author: veenstra
+"""
+
+import os
+import pandas as pd
+from pathlib import Path
+import xarray as xr
+from pydap.client import open_url
+from pydap.cas.get_cookies import setup_session
+import warnings
+from dfm_tools.errors import OutOfRangeError
+import cdsapi
+import cftime
+
+
+def download_ERA5(varkey,
+                  longitude_min, longitude_max, latitude_min, latitude_max, 
+                  date_min, date_max,
+                  dir_output='.', overwrite=False):
+    
+    #TODO: describe something about the .cdsapirc file
+    #TODO: make this function cdsapi generic, instead of ERA5 hardcoded (make flexible for product_type/name/name_output) (variables_dict is not used actively anymore, so this is possible)
+    
+    c = cdsapi.Client() # import cdsapi and create a Client instance # https://cds.climate.copernicus.eu/api-how-to
+    
+    #dictionary with ERA5 variables #this is not actively used
+    variables_dict = {'ssr':'surface_net_solar_radiation',
+                      'sst':'sea_surface_temperature',
+                      'strd':'surface_thermal_radiation_downwards',
+                      'slhf':'surface_latent_heat_flux',
+                      'sshf':'surface_sensible_heat_flux',
+                      'str':'surface_net_thermal_radiation',
+                      'chnk':'charnock',
+                      'd2m':'2m_dewpoint_temperature',
+                      't2m':'2m_temperature',
+                      'tcc':'total_cloud_cover',
+                      'msl':'mean_sea_level_pressure',
+                      'u10':'10m_u_component_of_wind',
+                      'u10n':'10m_u_component_of_neutral_wind',
+                      'v10':'10m_v_component_of_wind',
+                      'v10n':'10m_v_component_of_neutral_wind',
+                      'mer':'mean_evaporation_rate',
+                      'mtpr':'mean_total_precipitation_rate',
+                      }
+    if varkey not in variables_dict.keys(): #TODO: how to get list of available vars? mean_sea_level_pressure and msl both return a dataset with msl varkey, but standard_name air_pressure_at_mean_sea_level returns an error
+        raise KeyError(f'"{varkey}" not available, choose from: {list(variables_dict.keys())}')
+    
+    period_range = pd.period_range(date_min,date_max,freq='M')
+    print(f'retrieving data from {period_range[0]} to {period_range[-1]} (freq={period_range.freq})')
+    
+    for date in period_range:
+        name_output = f'era5_{varkey}_{date.strftime("%Y-%m")}.nc'
+        file_out = Path(dir_output,name_output)
+        if file_out.is_file() and not overwrite:
+            print(f'"{name_output}" found and overwrite=False, continuing.')
+            continue
+        print (f'retrieving ERA5 data for variable "{varkey}" and month {date.strftime("%Y-%m")} (YYYY-MM)')
+
+        request_dict = {'product_type':'reanalysis',
+                        'variable':variables_dict[varkey],
+                        'year':date.strftime('%Y'),
+                        'month':date.strftime('%m'),
+                        #'month':[f'{x:02d}' for x in range(1,12+1)], #all months, but instead retrieving per month
+                        'day':[f'{x:02d}' for x in range(1,31+1)], #all days
+                        'time':[f'{x:02d}:00' for x in range(0,23+1)], #all times/hours
+                        'area':[latitude_max,longitude_min,latitude_min,longitude_max], # north, west, south, east. default: global - option not available through the Climate Data Store (CDS) web interface (for cmip data)
+                        #'grid': [1.0, 1.0], # latitude/longitude grid: east-west (longitude) and north-south resolution (latitude). default: 0.25 x 0.25 - option not available through the Climate Data Store (CDS) web interface
+                        'format':'netcdf'}
+        
+        c.retrieve(name='reanalysis-era5-single-levels', request=request_dict, target=file_out)
+
+
+def download_CMEMS(varkey,
+                   longitude_min, longitude_max, latitude_min, latitude_max, 
+                   date_min, date_max, freq='D',
+                   dir_output='.', file_prefix='', overwrite=False,
+                   credentials=None):
+
+    date_min = pd.Timestamp(date_min)-pd.Timedelta(days=1) #CMEMS has daily noon values (not midnight), so subtract one day from date_min to cover desired time extent
+    
+    if 'my_datemax' not in globals(): #set multiyear date_max (my_datemax) as global variable, so it only has to be retreived once per download run (otherwise once per variable)
+        print('retrieving enddate of multiyear CMEMS dataset')
+        dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m' #assuming here that physchem and bio reanalyisus/multiyear datasets have the same enddate, this seems safe
+        ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+        my_times = ds.time.to_series()
+        global my_datemax
+        my_datemax = my_times.iloc[-1]
+
+    if pd.Timestamp(date_max) <= my_datemax:
+        product = 'reanalysis'
+    elif pd.Timestamp(date_min) > my_datemax:
+        product = 'analysisforecast'
+    else:
+        raise ValueError(f'Requested timerange is {date_min} to {date_max}. Currently, it is only possible to query periods before OR after the multiyear/reanalysis enddate ({my_datemax}).')
+    
+    Path(dir_output).mkdir(parents=True, exist_ok=True)
+    if varkey in ['bottomT','tob','mlotst','siconc','sithick','so','thetao','uo','vo','usi','vsi','zos']: #for physchem
+        if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
+            if varkey=='bottomT': #rename old to new anfc varname (still called bottomT in reanalysis)
+                varkey = 'tob'
+            if varkey in ['uo','vo']:
+                varkey_name = 'phy-cur'
+            elif varkey in ['so','thetao']:
+                varkey_name = 'phy-'+varkey
+            else:
+                varkey_name = 'phy'
+            dataset_url = f'https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_{varkey_name}_anfc_0.083deg_P1D-m'#.html' #TODO: also PT6H-i timeresolution available but not for all variables and not for reanalysis
+        else: #reanalysis: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/description
+            dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m'
+    else: #for bio
+        if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
+            dataset_url = 'https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily' #contains ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
+        else: #https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/description
+            dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m' #contains ['chl','no3','nppv','o2','po4','si']
+    
+    download_OPeNDAP(dataset_url=dataset_url,
+                     credentials=credentials, #credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'
+                     varkey=varkey,
+                     longitude_min=longitude_min, longitude_max=longitude_max, latitude_min=latitude_min, latitude_max=latitude_max,
+                     date_min=date_min, date_max=date_max,
+                     dir_output=dir_output, file_prefix=file_prefix, overwrite=overwrite)
+
+
+def open_OPeNDAP_xr(dataset_url, credentials=None):
+    """
+    How to get the opendap dataset_url (CMEMS example):
+        - https://data.marine.copernicus.eu/products
+        - go to the data access tab of a product, e.g.: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
+        - click the opendap link of the dataset of your choice
+        - copy the dataset_url from the adress bar (excl .html), e.g.: https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
+        
+        Example multiyear phys/chem:
+            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
+            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
+            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
+        Example multiyear bio:
+            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/services
+            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m
+            ['chl','no3','nppv','o2','po4','si']
+        Example forecast phys/chem:
+            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_PHY_001_024/services
+            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-phy-001-024
+            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
+        Example forecast bio:
+            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_BIO_001_028/services
+            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily
+            ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
+    
+    How to get the opendap dataset_url (HYCOM example):
+        - https://www.hycom.org/dataserver
+        - Select a product and search for THREDDS, e.g.: https://www.hycom.org/dataserver/gofs-3pt1/analysis
+        - find an opendap dataset_url, it depends per product/run where to find it.
+        Some examples:
+            https://tds.hycom.org/thredds/dodsC/GLBu0.08/expt_19.1/2010
+            https://tds.hycom.org/thredds/dodsC/GLBy0.08/expt_93.0
+
+    """
+    
+    def copernicusmarine_datastore(dataset_url, username, password):
+        #https://help.marine.copernicus.eu/en/articles/5182598-how-to-consume-the-opendap-api-and-cas-sso-using-python
+        cas_url = 'https://cmems-cas.cls.fr/cas/login'
+        session = setup_session(cas_url, username, password)
+        cookies_dict = session.cookies.get_dict()
+        if 'CASTGC' not in cookies_dict.keys():
+            raise KeyError('CASTGC key missing from session cookies_dict, probably authentication failure')
+        session.cookies.set("CASTGC", cookies_dict['CASTGC'])
+        #TODO: add check for wrong dataset_id (now always "AttributeError: You cannot set the charset when no content-type is defined")
+        DAP_dataset = open_url(dataset_url, session=session)#, user_charset='utf-8') # TODO: user_charset needs PyDAP >= v3.3.0 see https://github.com/pydap/pydap/pull/223/commits 
+        data_store = xr.backends.PydapDataStore(DAP_dataset)
+        return data_store
+    
+    if isinstance(dataset_url,list):
+        dataset_url_one = dataset_url[0]
+    else:
+        dataset_url_one = dataset_url
+    
+    if 'cmems-du.eu' in dataset_url_one:
+        if isinstance(dataset_url,list):
+            raise TypeError('list not supported by opendap method used for cmems')
+        
+        #parse credentials to username/password #TODO: now CMEMS specific, make more generic
+        if credentials is None:
+            file_credentials = f'{os.path.expanduser("~")}/CMEMS_credentials.txt'
+            if not os.path.exists(file_credentials):
+                raise FileNotFoundError(f'credentials argument not supplied and file_credentials not available ({file_credentials})')
+            with open(file_credentials) as fc:
+                username = fc.readline().strip()
+                password = fc.readline().strip()
+        else:
+            username,password = credentials
+
+        print(f'opening pydap connection to opendap dataset: {dataset_url}.html')
+        data_store = copernicusmarine_datastore(dataset_url=dataset_url, username=username, password=password)
+        print('xarray opening opendap dataset')
+        data_xr = xr.open_dataset(data_store)
+    elif 'hycom.org' in dataset_url_one:
+        if isinstance(dataset_url,list):
+            print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
+            data_xr = xr.open_mfdataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar'."
+        else:
+            print(f'xarray opening opendap dataset: {dataset_url}.html')
+            data_xr = xr.open_dataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar
+        data_xr['time'] = cftime.num2date(data_xr.time,units=data_xr.time.units,calendar=data_xr.time.calendar)
+        data_xr = data_xr.rename({'lon':'longitude','lat':'latitude'})
+    else:
+        print(f'unspecified dataset_url, might fail: {dataset_url}')
+        if isinstance(dataset_url,list):
+            print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
+            data_xr = xr.open_mfdataset(dataset_url)
+        else:
+            print(f'xarray opening opendap dataset: {dataset_url}.html')
+            data_xr = xr.open_dataset(dataset_url)
+        if 'lon' in data_xr.dims:
+            data_xr = data_xr.rename({'lon':'longitude','lat':'latitude'})
+        
+    return data_xr
+
+
+def download_OpenDAP_gettimes(dataset_url,credentials=None):
+    ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+    ds_time = ds.time.to_series()
+    return ds_time
+
+
+def download_OPeNDAP(dataset_url,
+                     varkey,
+                     longitude_min, longitude_max, latitude_min, latitude_max, 
+                     date_min, date_max, freq='D',
+                     dir_output='.', file_prefix='', overwrite=False,
+                     credentials=None):
+    """
+    
+
+    Parameters
+    ----------
+    dataset_url : TYPE
+        DESCRIPTION.
+    varkey : TYPE
+        DESCRIPTION.
+    longitude_min : TYPE
+        DESCRIPTION.
+    longitude_max : TYPE
+        DESCRIPTION.
+    latitude_min : TYPE
+        DESCRIPTION.
+    latitude_max : TYPE
+        DESCRIPTION.
+    date_min : TYPE
+        DESCRIPTION.
+    date_max : TYPE
+        DESCRIPTION.
+    freq : TYPE, optional
+        DESCRIPTION. The default is 'D'.
+    dir_output : TYPE, optional
+        DESCRIPTION. The default is '.'.
+    file_prefix : TYPE, optional
+        DESCRIPTION. The default is ''.
+    overwrite : TYPE, optional
+        DESCRIPTION. The default is False.
+    credentials : TYPE, optional
+        for CMEMS: credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'. The default is None.
+
+    Raises
+    ------
+    KeyError
+        DESCRIPTION.
+    OutOfRangeError
+        DESCRIPTION.
+
+    Returns
+    -------
+    None.
+
+    """
+    
+    data_xr = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+    
+    print(f'xarray subsetting data (variable \'{varkey}\' and lon/lat extents)')
+    if varkey not in data_xr.data_vars:
+        raise KeyError(f'"{varkey}" not found in dataset, available are: {list(data_xr.data_vars)}')
+    data_xr_var = data_xr[[varkey]]
+    data_xr_var = data_xr_var.sel(longitude=slice(longitude_min,longitude_max), #TODO: add depth selection?
+                                  latitude=slice(latitude_min,latitude_max))
+    data_xr_times = data_xr_var.time.to_series()
+    print(f'available time range in dataset from {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
+    period_range = pd.period_range(date_min,date_max,freq=freq)
+    
+    #check if date_min/date_max are available in dataset
+    if not (data_xr_times.index[0] <= period_range[0].to_timestamp() <= data_xr_times.index[-1]):
+        raise OutOfRangeError(f'date_min ({period_range[0]}) is outside available time range in dataset: {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
+    if not (data_xr_times.index[0] <= period_range[-1].to_timestamp() <= data_xr_times.index[-1]):
+        raise OutOfRangeError(f'date_max ({period_range[-1]}) is outside available time range in dataset: {data_xr_times.index[0]} to {data_xr_times.index[-1]}')
+    
+    for date in period_range:
+        date_str = str(date)
+        name_output = f'{file_prefix}{varkey}_{date_str}.nc'
+        file_out = Path(dir_output,name_output)
+        if file_out.is_file() and not overwrite:
+            print(f'"{name_output}" found and overwrite=False, continuing.')
+            continue
+        
+        print(f'xarray subsetting data per {period_range.freq}: {date_str}')
+        data_xr_var_seltime = data_xr_var.sel(time=slice(date_str,date_str)) #+' 12:00:00', 
+        
+        print(f'xarray writing netcdf file: {name_output}')
+        data_xr_var_seltime.to_netcdf(os.path.join(dir_output,name_output)) #TODO: add chunks={'time':1} or only possible with opening?
+        data_xr_var_seltime.close()
```

### Comparing `dfm_tools-0.10.55/dfm_tools/energy_dissipation.py` & `dfm_tools-0.11.0/dfm_tools/energy_dissipation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Dec  8 22:07:22 2022
-
-@author: veenstra
-"""
-import datetime as dt
-from dask.diagnostics import ProgressBar
-
-
-def compute_energy_dissipation(data_xr_map,file_ED_computed):
-    """
-    Example:
-        data_xr_map = dfmt.open_partitioned_dataset(file_nc_map,chunks={'time':100}) #TODO: important to have time>1, otherwise time-mean floods memory (100-200 seems optimal for GTSM 1month, but memory still floods so 1 year would probably be impossible).
-        data_xr_map = data_xr_map.sel(time=slice('2014-01-01','2014-02-01'))
-        dfmt.compute_energy_dissipation(data_xr_map,file_ED_computed)
-
-    
-    TODO: clean up these comments
-    
-    Stel de bodemwrijving is (tau_x,tau_y) dan is het verlies aan energie in W/m^2
-    E_loss = tau_x*u_x + tau_y*u_y
-    
-    Voor Chezy geldt (zo uit mijn hoofd):
-    tau_x = - (rho*g)/(C^2) u_x * sqrt(u_x^2+u_y^2)
-    tau_y = - (rho*g)/(C^2) u_y * sqrt(u_x^2+u_y^2)
-    
-    En gecombineerd
-    E_loss = - (rho*g)/(C^2) * (u_x^2+u_y^2)^(3/2)
-    
-    Approximation: using velocities in cell centers, this is averaged but easiest
-    
-    E_loss(area) = sum_cells [ - (rho*g)/(C^2) * (sqrt(u_x^2+u_y^2))^3 ] * cell_area
-    
-    Dit is dan voor een tijdstip. Ik zou middelen over een iets langere periode zodat het de variatie over het getij verdwijnt, want de waarde is bij springtij waarschijnlijk groter.
-
-    """
-    rho = 1020 #kg/m3
-    g = 9.81 #m/s2
-    
-    attrs_ED = {'long_name':'energy dissipation','units':'W'}    
-    attrs_ED_pm2 = {'long_name':'energy dissipation','units':'W/m^2'}    
-    attrs_ED_areasum = {'long_name':'area-sum energy dissipation', 'units':'W'}
-    attrs_ED_timemean = {'long_name':'springneaptide-mean energy dissipation', 'units': 'W'}
-    attrs_ED_pm2_timemean = {'long_name':'springneaptide-mean energy dissipation', 'units':'Wm^2'}
-    
-    print('>> compute energyloss from C/u/area: ',end='')
-    dtstart = dt.datetime.now()
-    data_ucmag = data_xr_map.mesh2d_ucmag #m/s
-    data_czs = data_xr_map.mesh2d_czs #m0.5s-1
-    data_czs = data_czs.where(data_czs!=0) #0 will result in inf energyloss, so replace by nan
-    data_ba = data_xr_map.mesh2d_flowelem_ba #m2
-    data_xr_map['ED'] = ((rho*g)/(data_czs**2) * data_ucmag**3 * data_ba).assign_attrs(attrs_ED) #equation: (kg/m3)*(m/s2)/(m/s2)*(m3/s3)*m2 = kg/s3*m2 = W = J/s
-    data_xr_map['ED_pm2'] = (data_xr_map['ED'] / data_ba).assign_attrs(attrs_ED_pm2) #TODO: maybe include ba instead of supplying _pm2 separately?
-    
-    #TODO: check da.sum(split_every=4): https://github.com/dask/dask/issues/883. Does not seem to work: "TypeError: nansum() got an unexpected keyword argument 'split_every'"
-    #TODO: chunking: float32 = 32 bits = 4 bytes >> use this to calculate chunking sizes (100-200MB per chunk is optimal)
-    data_xr_map['ED_areasum'] = data_xr_map.ED.sum(dim='mesh2d_nFaces').assign_attrs(attrs_ED_areasum)
-    data_xr_map['ED_timemean'] = data_xr_map.ED.mean(dim='time').assign_attrs(attrs_ED_timemean)
-    data_xr_map['ED_pm2_timemean'] = data_xr_map.ED_pm2.mean(dim='time').assign_attrs(attrs_ED_pm2_timemean)
-    
-    
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    data_xr_map_computed = data_xr_map[['mesh2d_flowelem_ba','ED_areasum','ED_timemean','ED_pm2_timemean']] #has to contain some var with cells (not only ED_areasum), otherwise ugrid accessor is not valid
-    #data_xr_map_computed.ED_timemean.data.visualize() #does not yet work >> visualizes tasks of dask array
-    
-    print('>> compute and save data_xr_map_computed to netcdf: ')
-    with ProgressBar():
-        data_xr_map_computed.ugrid.to_netcdf(file_ED_computed)
-    
-    data_xr_map_computed.close()
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Dec  8 22:07:22 2022
+
+@author: veenstra
+"""
+import datetime as dt
+from dask.diagnostics import ProgressBar
+
+
+def compute_energy_dissipation(data_xr_map,file_ED_computed):
+    """
+    Example:
+        data_xr_map = dfmt.open_partitioned_dataset(file_nc_map,chunks={'time':100}) #TODO: important to have time>1, otherwise time-mean floods memory (100-200 seems optimal for GTSM 1month, but memory still floods so 1 year would probably be impossible).
+        data_xr_map = data_xr_map.sel(time=slice('2014-01-01','2014-02-01'))
+        dfmt.compute_energy_dissipation(data_xr_map,file_ED_computed)
+
+    
+    TODO: clean up these comments
+    
+    Stel de bodemwrijving is (tau_x,tau_y) dan is het verlies aan energie in W/m^2
+    E_loss = tau_x*u_x + tau_y*u_y
+    
+    Voor Chezy geldt (zo uit mijn hoofd):
+    tau_x = - (rho*g)/(C^2) u_x * sqrt(u_x^2+u_y^2)
+    tau_y = - (rho*g)/(C^2) u_y * sqrt(u_x^2+u_y^2)
+    
+    En gecombineerd
+    E_loss = - (rho*g)/(C^2) * (u_x^2+u_y^2)^(3/2)
+    
+    Approximation: using velocities in cell centers, this is averaged but easiest
+    
+    E_loss(area) = sum_cells [ - (rho*g)/(C^2) * (sqrt(u_x^2+u_y^2))^3 ] * cell_area
+    
+    Dit is dan voor een tijdstip. Ik zou middelen over een iets langere periode zodat het de variatie over het getij verdwijnt, want de waarde is bij springtij waarschijnlijk groter.
+
+    """
+    rho = 1020 #kg/m3
+    g = 9.81 #m/s2
+    
+    attrs_ED = {'long_name':'energy dissipation','units':'W'}    
+    attrs_ED_pm2 = {'long_name':'energy dissipation','units':'W/m^2'}    
+    attrs_ED_areasum = {'long_name':'area-sum energy dissipation', 'units':'W'}
+    attrs_ED_timemean = {'long_name':'springneaptide-mean energy dissipation', 'units': 'W'}
+    attrs_ED_pm2_timemean = {'long_name':'springneaptide-mean energy dissipation', 'units':'Wm^2'}
+    
+    print('>> compute energyloss from C/u/area: ',end='')
+    dtstart = dt.datetime.now()
+    data_ucmag = data_xr_map.mesh2d_ucmag #m/s
+    data_czs = data_xr_map.mesh2d_czs #m0.5s-1
+    data_czs = data_czs.where(data_czs!=0) #0 will result in inf energyloss, so replace by nan
+    data_ba = data_xr_map.mesh2d_flowelem_ba #m2
+    data_xr_map['ED'] = ((rho*g)/(data_czs**2) * data_ucmag**3 * data_ba).assign_attrs(attrs_ED) #equation: (kg/m3)*(m/s2)/(m/s2)*(m3/s3)*m2 = kg/s3*m2 = W = J/s
+    data_xr_map['ED_pm2'] = (data_xr_map['ED'] / data_ba).assign_attrs(attrs_ED_pm2) #TODO: maybe include ba instead of supplying _pm2 separately?
+    
+    #TODO: check da.sum(split_every=4): https://github.com/dask/dask/issues/883. Does not seem to work: "TypeError: nansum() got an unexpected keyword argument 'split_every'"
+    #TODO: chunking: float32 = 32 bits = 4 bytes >> use this to calculate chunking sizes (100-200MB per chunk is optimal)
+    data_xr_map['ED_areasum'] = data_xr_map.ED.sum(dim='mesh2d_nFaces').assign_attrs(attrs_ED_areasum)
+    data_xr_map['ED_timemean'] = data_xr_map.ED.mean(dim='time').assign_attrs(attrs_ED_timemean)
+    data_xr_map['ED_pm2_timemean'] = data_xr_map.ED_pm2.mean(dim='time').assign_attrs(attrs_ED_pm2_timemean)
+    
+    
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    data_xr_map_computed = data_xr_map[['mesh2d_flowelem_ba','ED_areasum','ED_timemean','ED_pm2_timemean']] #has to contain some var with cells (not only ED_areasum), otherwise ugrid accessor is not valid
+    #data_xr_map_computed.ED_timemean.data.visualize() #does not yet work >> visualizes tasks of dask array
+    
+    print('>> compute and save data_xr_map_computed to netcdf: ')
+    with ProgressBar():
+        data_xr_map_computed.ugrid.to_netcdf(file_ED_computed)
+    
+    data_xr_map_computed.close()
```

### Comparing `dfm_tools-0.10.55/dfm_tools/get_nc.py` & `dfm_tools-0.11.0/dfm_tools/get_nc.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,563 +1,563 @@
-# -*- coding: utf-8 -*-
-"""
-dfm_tools are post-processing tools for Delft3D FM
-Copyright (C) 2020 Deltares. All rights reserved.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  if not, see <http://www.gnu.org/licenses/>.
-
-All names, logos, and references to "Deltares" are registered trademarks of
-Stichting Deltares and remain full property of Stichting Deltares at all times.
-All rights reserved.
-
-
-INFORMATION
-This script is part of dfm_tools: https://github.com/openearth/dfm_tools
-Check the README.rst on github for other available functions
-Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
-Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
-
-Created on Fri Feb 14 12:45:11 2020
-
-@author: veenstra
-"""
-
-import numpy as np
-import datetime as dt
-import re
-import xugrid as xu
-import xarray as xr
-import matplotlib.pyplot as plt
-from dfm_tools.xarray_helpers import get_vertical_dimensions, Dataset_varswithdim
-import netCDF4
-
-
-def calc_dist_pythagoras(x1,x2,y1,y2):
-    distance = np.sqrt((x2 - x1)**2 + (y2 - y1)**2)
-    return distance
-
-
-def calc_dist_haversine(lon1,lon2,lat1,lat2):
-    """
-    calculates distance between lat/lon coordinates in meters
-    https://community.esri.com/t5/coordinate-reference-systems-blog/distance-on-a-sphere-the-haversine-formula/ba-p/902128
-    """
-    # convert to radians
-    lon1_rad = np.deg2rad(lon1)
-    lon2_rad = np.deg2rad(lon2)
-    lat1_rad = np.deg2rad(lat1)
-    lat2_rad = np.deg2rad(lat2)
-    
-    # apply formulae
-    a = np.sin((lat2_rad-lat1_rad)/2)**2 + np.cos(lat1_rad) * np.cos(lat2_rad) * np.sin((lon2_rad-lon1_rad)/2)**2
-    c = 2 * np.arctan2( np.sqrt(a), np.sqrt(1-a) )
-    R = 6371000
-    distance = R * c
-    if np.isnan(distance).any():
-        raise ValueError('nan encountered in calc_dist_latlon distance')
-    return distance
-
-
-def intersect_edges_withsort(uds,edges): #TODO: move sorting to xugrid? https://deltares.github.io/xugrid/api/xugrid.Ugrid2d.intersect_edges.html
-    
-    edge_index, face_index, intersections = uds.grid.intersect_edges(edges) #TODO: is fast, but maybe speed can be increased with bounding box?
-    
-    #ordering of face_index is wrong (visible with cb3 with long line_array), so sort on distance from startpoint (in x/y units)
-    
-    #compute distance from start of line to start of each linepart
-    edge_len = np.linalg.norm(edges[:,1] - edges[:,0], axis=1)
-    edge_len_cum = np.cumsum(edge_len)
-    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
-    
-    #compute distance from start to lineparts to start of line (via line)
-    startcoord_linepart = edges[edge_index,0,:]
-    dist_tostart_linepart = np.linalg.norm(intersections[:,0,:] - startcoord_linepart, axis=1)
-    dist_tostart_line = dist_tostart_linepart + edge_len_cum0[edge_index]
-    
-    #sorting on distance
-    id_sorted = np.argsort(dist_tostart_line)
-    edge_index = edge_index[id_sorted]
-    face_index = face_index[id_sorted]
-    intersections = intersections[id_sorted]
-    return edge_index, face_index, intersections
-
-
-def get_xzcoords_onintersection(uds, face_index, crs_dist_starts, crs_dist_stops):
-    #TODO: remove hardcoding of variable names
-    if 'time' in uds.dims: #TODO: maybe make time dependent grid?
-        raise Exception('time dimension present in uds, provide uds.isel(time=timestep) instead. This is necessary to retrieve correct waterlevel or fullgrid output')
-    
-    dimn_layer, dimn_interfaces = get_vertical_dimensions(uds)
-    gridname = uds.grid.name
-    
-    #construct fullgrid info (zcc/zw) for 3D models
-    if dimn_layer in uds.dims:
-        uds = reconstruct_zw_zcc(uds)
-
-    #drop all variables that do not contain a face dimension, then select only all sliced faceidx
-    xu_facedim = uds.grid.face_dimension
-    face_index_xr = xr.DataArray(face_index,dims=('ncrossed_faces'))
-    uds = Dataset_varswithdim(uds,dimname=xu_facedim) #TODO: is there an xugrid alternative?
-    uds_sel = uds.sel({xu_facedim:face_index_xr})
-    
-    # take zvals_interface
-    if dimn_layer in uds_sel.dims: #3D model
-        nlay = uds.dims[dimn_layer]
-        zvals_interface_filled = uds_sel[f'{gridname}_flowelem_zw'].bfill(dim=dimn_interfaces) #fill nan values (below bed) with equal values
-        zvals_interface = zvals_interface_filled.to_numpy().T #transpose to make in line with 2D sigma dataset
-    else: #2D model, no layers
-        nlay = 1
-        data_frommap_wl3_sel = uds_sel[f'{gridname}_s1'].to_numpy() #TODO: add escape for missing wl/bl vars
-        data_frommap_bl_sel = uds_sel[f'{gridname}_flowelem_bl'].to_numpy()
-        zvals_interface = np.linspace(data_frommap_bl_sel,data_frommap_wl3_sel,nlay+1)
-
-    #derive crs_verts
-    crs_dist_starts_matrix = np.repeat(crs_dist_starts[np.newaxis],nlay,axis=0)
-    crs_dist_stops_matrix = np.repeat(crs_dist_stops[np.newaxis],nlay,axis=0)
-    crs_verts_x_all = np.array([[crs_dist_starts_matrix.ravel(),crs_dist_stops_matrix.ravel(),crs_dist_stops_matrix.ravel(),crs_dist_starts_matrix.ravel()]]).T
-    crs_verts_z_all = np.ma.array([zvals_interface[1:,:].ravel(),zvals_interface[1:,:].ravel(),zvals_interface[:-1,:].ravel(),zvals_interface[:-1,:].ravel()]).T[:,:,np.newaxis]
-    crs_verts = np.ma.concatenate([crs_verts_x_all, crs_verts_z_all], axis=2)
-    
-    #define grid
-    shape_crs_grid = crs_verts[:,:,0].shape
-    shape_crs_flat = crs_verts[:,:,0].ravel().shape
-    xr_crs_grid = xu.Ugrid2d(node_x=crs_verts[:,:,0].ravel(),
-                             node_y=crs_verts[:,:,1].ravel(),
-                             fill_value=-1,
-                             face_node_connectivity=np.arange(shape_crs_flat[0]).reshape(shape_crs_grid),
-                             )
-
-    #define dataset
-    if dimn_layer in uds_sel.dims:
-        crs_plotdata_clean = uds_sel.stack({xr_crs_grid.face_dimension:[dimn_layer,'ncrossed_faces']},create_index=False)
-    else: #2D: still make sure xr_crs_grid.face_dimension is created, using stack since .rename() gives "UserWarning: rename 'ncrossed_faces' to 'mesh2d_nFaces' does not create an index anymore."
-        crs_plotdata_clean = uds_sel.stack({xr_crs_grid.face_dimension:['ncrossed_faces']},create_index=False)
-                    
-    #combine into xugrid
-    xr_crs_ugrid = xu.UgridDataset(crs_plotdata_clean, grids=[xr_crs_grid])
-    return xr_crs_ugrid
-
-
-def polyline_mapslice(uds:xu.UgridDataset, line_array:np.array, calcdist_fromlatlon:bool = None) -> xu.UgridDataset:
-    """
-    Slice trough mapdata, combine: intersect_edges_withsort, calculation of distances and conversion to ugrid dataset.
-
-    Parameters
-    ----------
-    uds : xu.UgridDataset
-        DESCRIPTION.
-    line_array : np.array
-        DESCRIPTION.
-    calcdist_fromlatlon : bool, optional
-        DESCRIPTION. The default is None.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    xr_crs_ugrid : xu.UgridDataset
-        DESCRIPTION.
-
-    """
-    
-    #compute intersection coordinates of crossings between edges and faces and their respective indices
-    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
-    edge_index, face_index, intersections = intersect_edges_withsort(uds=uds, edges=edges)
-    if len(edge_index) == 0:
-        raise ValueError('polyline does not cross mapdata')
-    
-    #auto determine if cartesian/sperical distance should be computed
-    if calcdist_fromlatlon is None:
-        if hasattr(uds,'projected_coordinate_system'):
-            calcdist_fromlatlon = False
-        elif hasattr(uds,'wgs84'):
-            calcdist_fromlatlon = True
-        else:
-            raise KeyError('To auto determine calcdist_fromlatlon, a variable "projected_coordinate_system" or "wgs84" is required, please provide calcdist_fromlatlon=True/False yourself.')
-    if calcdist_fromlatlon:
-        calc_dist = calc_dist_haversine
-    else:
-        calc_dist = calc_dist_pythagoras
-    
-    #compute pyt/haversine start/stop distances for all intersections
-    edge_len = calc_dist(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
-    edge_len_cum = np.cumsum(edge_len)
-    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
-    crs_dist_starts = calc_dist(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
-    crs_dist_stops  = calc_dist(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
-    
-    #derive vertices from cross section (distance from first point)
-    xr_crs_ugrid = get_xzcoords_onintersection(uds=uds, face_index=face_index, crs_dist_starts=crs_dist_starts, crs_dist_stops=crs_dist_stops)
-    
-    return xr_crs_ugrid
-
-
-def get_formula_terms(uds, varn_contains):
-    """
-    get formula_terms for zw/zcc reconstruction, convert to list and then to dict. This can be done for layer/interface (via varn_contains)
-    """
-    osz_varnames = list(uds.filter_by_attrs(formula_terms=lambda v: v is not None).variables) #names of variables containing attribute "formula_terms"
-    osz_varnames_contains = [x for x in osz_varnames if varn_contains in x] #TODO: to get the layer/interface ocean_*_coordinate. Not too pretty, but it works
-    if len(osz_varnames_contains) != 1: #should be 1 exactly, none is the case in zlayer models
-        raise ValueError(f'no or more than one {varn_contains} variable found with formula_terms attribute: {osz_varnames}')
-    osz_varn = osz_varnames_contains[0]
-    osz_formulaterms = uds[osz_varn].attrs['formula_terms']
-    tokens = re.split('[:\\s]+', osz_formulaterms)
-    osz_formulaterms_dict = dict(zip(tokens[::2], tokens[1::2]))
-    return osz_formulaterms_dict
-
-
-def reconstruct_zw_zcc_fromsigma(uds):
-    """
-    reconstruct full grid output (time/face-varying z-values) for sigma model, necessary for slicing sigmamodel on depth value
-    based on https://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_sigma_coordinate
-    """
-    osz_formulaterms_int_dict = get_formula_terms(uds,varn_contains='interface')
-    osz_formulaterms_lay_dict = get_formula_terms(uds,varn_contains='layer')
-    
-    uds_eta = uds[osz_formulaterms_int_dict['eta']] #mesh2d_s1
-    uds_depth = uds[osz_formulaterms_int_dict['depth']] #mesh2d_bldepth in new output, mesh2d_waterdepth in old output (see comment below)
-    if uds_depth.attrs['standard_name'] == 'sea_floor_depth_below_sea_surface': # previously the waterdepth instead of negative bedlevel was coupled via the formula_terms in sigmamodels (was fixed in OSS 140982 / 29-3-2022)
-        uds_depth = -uds['mesh2d_flowelem_bl'] # assuming this variable is available, which is not guaranteed
-    uds_sigma_int = uds[osz_formulaterms_int_dict['sigma']] #mesh2d_interface_sigma
-    uds_sigma_lay = uds[osz_formulaterms_lay_dict['sigma']] #mesh2d_layer_sigma
-    
-    uds['mesh2d_flowelem_zw'] = uds_eta + uds_sigma_int*(uds_depth+uds_eta)
-    uds['mesh2d_flowelem_zcc'] = uds_eta + uds_sigma_lay*(uds_depth+uds_eta)
-    
-    uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
-    return uds
-
-
-def reconstruct_zw_zcc_fromz(data_xr_map):
-    """
-    reconstruct full grid output (time/face-varying z-values) for zvalue model. Necessary when extracting values with zdepth w.r.t. waterlevel/bedlevel
-    #TODO: gives spotty result for 0/0.1m w.r.t. bedlevel for Grevelingen zmodel
-    #TODO: remove hardcoding of varnames (assuming wl/bl variables are available)
-    #TODO: center values are clipped to waterlevel+bedlevel, so the center values of the top+bottom layer are currently incorrect
-    """
-    
-    dimn_layer, dimn_interfaces = get_vertical_dimensions(data_xr_map)
-    
-    data_frommap_wl_sel = data_xr_map['mesh2d_s1']
-    data_frommap_z0_sel = data_frommap_wl_sel*0
-    data_frommap_bl_sel = data_xr_map['mesh2d_flowelem_bl']
-    
-    zvals_cen_zval = data_xr_map['mesh2d_layer_z'] #no clipping for zcenter values, since otherwise interp will fail
-    data_xr_map['mesh2d_flowelem_zcc'] = (data_frommap_z0_sel+zvals_cen_zval).clip(min=data_frommap_bl_sel, max=data_frommap_wl_sel)
-
-    zvals_interface_zval = data_xr_map['mesh2d_interface_z'] #clipping for zinterface values, to make sure layer interfaces are also at water/bed level
-    data_xr_map['mesh2d_flowelem_zw'] = (data_frommap_z0_sel+zvals_interface_zval).clip(min=data_frommap_bl_sel, max=data_frommap_wl_sel)
-    bool_notoplayer_int = zvals_interface_zval<zvals_interface_zval.isel({dimn_interfaces:-1})
-    bool_int_abovewl = zvals_interface_zval>data_frommap_wl_sel
-    data_xr_map['mesh2d_flowelem_zw'] = data_xr_map['mesh2d_flowelem_zw'].where(bool_notoplayer_int | bool_int_abovewl, other=data_frommap_wl_sel) #zvalues of top layer_interfaces that are lower than wl are replaced by wl
-    
-    data_xr_map = data_xr_map.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
-    return data_xr_map
-
-
-def reconstruct_zw_zcc_fromzsigma(uds):
-    """
-    reconstruct full grid output (time/face-varying z-values) for zsigmavalue model without full grid output. Implemented in https://issuetracker.deltares.nl/browse/UNST-5477
-    based on https://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_sigma_over_z_coordinate
-    #TODO: center values are clipped to bedlevel, so the center values of the bottom layer are currently incorrect
-    """
-    
-    #TODO: default fillvalues are not automatically parsed to nan, so doing it manually: https://github.com/pydata/xarray/issues/2742
-    fillvals = netCDF4.default_fillvals
-    
-    osz_formulaterms_int_dict = get_formula_terms(uds,varn_contains='interface')
-    osz_formulaterms_lay_dict = get_formula_terms(uds,varn_contains='layer')
-    
-    uds_eta = uds[osz_formulaterms_int_dict['eta']] #mesh2d_s1
-    uds_depth = uds[osz_formulaterms_int_dict['depth']] #mesh2d_bldepth: positive version of mesh2d_flowelem_bl, but this one is always in file
-    uds_depth_c = uds[osz_formulaterms_int_dict['depth_c']] #mesh2d_sigmazdepth
-    uds_zlev_int = uds[osz_formulaterms_int_dict['zlev']] #mesh2d_interface_z
-    uds_zlev_int = uds_zlev_int.where(uds_zlev_int!=fillvals['f8'])
-    uds_sigma_int = uds[osz_formulaterms_int_dict['sigma']] #mesh2d_interface_sigma
-    uds_sigma_int = uds_sigma_int.where(uds_sigma_int!=fillvals['f8'])
-    uds_zlev_lay = uds[osz_formulaterms_lay_dict['zlev']] #mesh2d_layer_z
-    uds_zlev_lay = uds_zlev_lay.where(uds_zlev_lay!=fillvals['f8'])
-    uds_sigma_lay = uds[osz_formulaterms_lay_dict['sigma']] #mesh2d_layer_sigma
-    uds_sigma_lay = uds_sigma_lay.where(uds_sigma_lay!=fillvals['f8'])
-    
-    # for levels k where sigma(k) has a defined value and zlev(k) is not defined:
-    # z(n,k,j,i) = eta(n,j,i) + sigma(k)*(min(depth_c,depth(j,i))+eta(n,j,i))
-    zw_sigmapart = uds_eta + uds_sigma_int*(uds_depth.clip(max=uds_depth_c)+uds_eta)
-    zcc_sigmapart = uds_eta + uds_sigma_lay*(uds_depth.clip(max=uds_depth_c)+uds_eta)
-    # for levels k where zlev(k) has a defined value and sigma(k) is not defined: 
-    # z(n,k,j,i) = zlev(k)
-    zw_zpart = uds_zlev_int.clip(min=-uds_depth) #added clipping of zvalues with bedlevel
-    zcc_zpart = uds_zlev_lay.clip(min=-uds_depth) #added clipping of zvalues with bedlevel
-    uds['mesh2d_flowelem_zw'] = zw_sigmapart.fillna(zw_zpart)
-    uds['mesh2d_flowelem_zcc'] = zcc_sigmapart.fillna(zcc_zpart)
-    
-    uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
-    return uds
-
-
-def reconstruct_zw_zcc(ds):
-    dimn_layer, dimn_interfaces = get_vertical_dimensions(ds)
-    
-    if dimn_layer is not None: #D-FlowFM mapfile
-        gridname = ds.grid.name
-        varname_zint = f'{gridname}_flowelem_zw'
-    elif 'laydim' in ds.dims: #D-FlowFM hisfile
-        varname_zint = 'zcoordinate_w'
-    
-    #reconstruct zw/zcc variables (if not in file) and treat as fullgrid mapfile from here
-    if varname_zint in ds.variables: #fullgrid info already available, so continuing
-        print(f'zw/zcc (fullgrid) values already present in Dataset in variable {varname_zint}')
-    elif len(ds.filter_by_attrs(standard_name='ocean_sigma_z_coordinate')) != 0:
-        print('zsigma-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
-        ds = reconstruct_zw_zcc_fromzsigma(ds)
-    elif 'mesh2d_layer_sigma' in ds.variables: #TODO: var with standard_name='ocean_sigma_coordinate' available?
-        print('sigma-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
-        ds = reconstruct_zw_zcc_fromsigma(ds)
-    elif 'mesh2d_layer_z' in ds.variables:
-        print('z-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
-        ds = reconstruct_zw_zcc_fromz(ds)
-    else:
-        raise KeyError('layers present, but unknown layertype, expected one of variables: mesh2d_flowelem_zw, mesh2d_layer_sigma, mesh2d_layer_z')
-    return ds
-
-    
-def get_Dataset_atdepths(data_xr:xu.UgridDataset, depths, reference:str ='z0'):    
-    """
-    Lazily depth-slice a dataset with layers. Performance can be increased by using a subset of variables or subsetting the dataset in any dimension.
-    This can be done for instance with ds.isel(time=-1) or uds.ugrid.sel(x=slice(),y=slice()) to subset a ugrid dataset in space.
-    The return dataset only contains the sliced variables.
-    
-    Parameters
-    ----------
-    data_xr : xu.UgridDataset
-        has to be Dataset (not a DataArray), otherwise mesh2d_flowelem_zw etc are not available (interface z values)
-        in case of zsigma/sigma layers (or fullgrid), it is advisable to .sel()/.isel() the time dimension first, because that is less computationally heavy
-    depths : TYPE
-        int/float or list/array of int/float. Depths w.r.t. reference level. If reference=='waterlevel', depth>0 returns only nans. If reference=='bedlevel', depth<0 returns only nans. Depths are sorted and only uniques are kept.
-    reference : str, optional
-        compute depth w.r.t. z0/waterlevel/bed. The default is 'z0'.
-    zlayer_z0_selnearest : bool, optional
-        Use xr.interp() to interpolate zlayer model to z-value. Only possible for reference='z' (not 'waterlevel' or 'bedlevel'). Only used if "mesh2d_layer_z" is present (zlayer model)
-        This is faster but results in values interpolated between zcc (z cell centers), so it is different than slicing.. The default is False.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    xu.UgridDataset
-        Dataset with the depth-sliced variables.
-
-    """
-    
-    depth_vardimname = f'depth_from_{reference}'
-    
-    dimn_layer, dimn_interfaces = get_vertical_dimensions(data_xr)
-    
-    if dimn_layer is not None: #D-FlowFM mapfile
-        gridname = data_xr.grid.name
-        varname_zint = f'{gridname}_flowelem_zw'
-        dimname_layc = dimn_layer
-        dimname_layw = dimn_interfaces
-        varname_wl = f'{gridname}_s1'
-        varname_bl = f'{gridname}_flowelem_bl'
-    elif 'laydim' in data_xr.dims: #D-FlowFM hisfile
-        varname_zint = 'zcoordinate_w'
-        dimname_layc = 'laydim'
-        dimname_layw = 'laydimw'
-        varname_wl = 'waterlevel'
-        varname_bl = 'bedlevel'
-    else:
-        print(UserWarning('depth/layer dimension not found, probably 2D model, returning input Dataset')) #TODO: this can also be at depth, since slice will put parts of model dry (and allnan if below wl or below bl). Implement this
-        return data_xr #early return
-    
-    if not isinstance(data_xr,(xr.Dataset,xu.UgridDataset)):
-        raise TypeError(f'data_xr_map should be of type xr.Dataset, but is {type(data_xr)}')
-    
-    #create depth xr.DataArray
-    if isinstance(depths,(float,int)):
-        depth_dims = ()
-    else:
-        depths = np.unique(depths) #array of unique+sorted floats/ints
-        depth_dims = (depth_vardimname)
-    depths_xr = xr.DataArray(depths,dims=depth_dims,attrs={'units':'m',
-                                                           'reference':f'model_{reference}',
-                                                           'positive':'up'}) #TODO: make more in line with CMEMS etc
-    
-    #potentially construct fullgrid info (zcc/zw)
-    data_xr = reconstruct_zw_zcc(data_xr)
-    
-    #correct reference level
-    if reference=='z0':
-        zw_reference = data_xr[varname_zint]
-    elif reference=='waterlevel':
-        if varname_wl not in data_xr.variables:
-            raise KeyError(f'get_Dataset_atdepths() called with reference=waterlevel, but {varname_wl} variable not present')
-        data_wl = data_xr[varname_wl]
-        zw_reference = data_xr[varname_zint] - data_wl
-    elif reference=='bedlevel':
-        if varname_bl not in data_xr.variables:
-            raise KeyError(f'get_Dataset_atdepths() called with reference=bedlevel, but {varname_bl} variable not present') #TODO: in case of zsigma/sigma it can also be -mesh2d_bldepth
-        data_bl = data_xr[varname_bl]
-        zw_reference = data_xr[varname_zint] - data_bl
-    else:
-        raise KeyError(f'unknown reference "{reference}" (possible are z0, waterlevel and bedlevel') #TODO: make enum?
-    
-    print('>> subsetting data on fixed depth in fullgrid z-data: ',end='')
-    dtstart = dt.datetime.now()
-    
-    #get layerbool via z-interface value (zw), check which celltop-interfaces are above/on depth and which which cellbottom-interfaces are below/on depth
-    bool_topinterface_abovedepth = zw_reference.isel({dimname_layw:slice(1,None)}) >= depths_xr
-    bool_botinterface_belowdepth = zw_reference.isel({dimname_layw:slice(None,-1)}) <= depths_xr
-    bool_topbotinterface_arounddepth = bool_topinterface_abovedepth & bool_botinterface_belowdepth #this bool also automatically excludes all values below bed and above wl
-    bool_topbotinterface_arounddepth = bool_topbotinterface_arounddepth.rename({dimname_layw:dimname_layc}) #correct dimname for interfaces to centers
-    
-    #subset variables that have no, time, face and/or layer dims, slice only variables with all three dims (and add to subset)
-    bool_dims = [x for x in bool_topbotinterface_arounddepth.dims if x!=depth_vardimname] #exclude depth_vardimname (present if multiple depths supplied), since it is not present in pre-slice variables
-    variables_toslice = [var for var in data_xr.data_vars if set(bool_dims).issubset(data_xr[var].dims)]
-    
-    #actual slicing with .where().max()
-    ds_atdepths = data_xr[variables_toslice].where(bool_topbotinterface_arounddepth).max(dim=dimname_layc,keep_attrs=True) #set all layers but one to nan, followed by an arbitrary reduce (max in this case) #TODO: check if attributes should be passed/altered
-    #TODO: suppress warning (upon plotting/load/etc): "C:\Users\veenstra\Anaconda3\envs\dfm_tools_env\lib\site-packages\dask\array\reductions.py:640: RuntimeWarning: All-NaN slice encountered" >> already merged in xarray: https://github.com/dask/dask/pull/9916
-    ds_atdepths = ds_atdepths.drop_dims([dimname_layw,dimname_layc],errors='ignore') #dropping interface dim if it exists, since it does not correspond to new depths dim
-    
-    #add depth as coordinate var
-    ds_atdepths[depth_vardimname] = depths_xr
-    ds_atdepths = ds_atdepths.set_coords([depth_vardimname])
-    
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    return ds_atdepths
-
-
-def rasterize_ugrid(uds:xu.UgridDataset, ds_like:xr.Dataset = None, resolution:float = None):
-    """
-    Rasterizing ugrid dataset to regular dataset. ds_like has higher priority than `resolution`. If both are not passed, a raster is generated of at least 200x200
-    inspired by xugrid.plot.imshow and xugrid.ugrid.ugrid2d.rasterize/rasterize_like.
-
-
-    Parameters
-    ----------
-    uds : xu.UgridDataset
-        DESCRIPTION.
-    ds_like : xr.Dataset, optional
-        xr.Dataset with ed x and y variables to interpolate uds to. The default is None.
-    resolution : float, optional
-        Only used if ds_like is not supplied. The default is None.
-    
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds : TYPE
-        DESCRIPTION.
-
-    """
-    #TODO: maybe put part of code in xugrid (https://github.com/Deltares/xugrid/issues/31)
-    #TODO: vars can also be rasterized with uds_facevars[var].ugrid.rasterize(resolution), but is not efficient. Wait for uds.rasterize() method: https://github.com/Deltares/xugrid/issues/61
-    if not isinstance(uds,xu.core.wrap.UgridDataset):
-        raise TypeError(f'rasterize_ugrid expected xu.core.wrap.UgridDataset, got {type(uds)} instead')
-    
-    grid = uds.grid
-    xu_facedim = uds.grid.face_dimension
-    uds_facevars = Dataset_varswithdim(uds,xu_facedim)
-    
-    if ds_like is not None:
-        regx = ds_like.x
-        regy = ds_like.y
-    else:
-        xmin, ymin, xmax, ymax = grid.bounds
-        dx = xmax - xmin
-        dy = ymax - ymin
-        if resolution is None: # check if a rasterization resolution is passed, otherwise default to 200 raster cells otherwise for the smallest axis.
-            resolution = min(dx, dy) / 200
-        d = abs(resolution)
-        regx = np.arange(xmin + 0.5 * d, xmax, d)
-        regy = np.arange(ymin + 0.5 * d, ymax, d)
-    
-    regx, regy, index = grid.rasterize_like(x=regx,y=regy) #TODO: this can be used to steer rasterization, eg with xstart/ystart/xres/yres
-    index_da = xr.DataArray(index,dims=('y','x'))
-    
-    print(f'>> rasterizing ugrid dataset with {len(uds_facevars.data_vars)} face variables to shape={index_da.shape}: ',end='')
-    dtstart = dt.datetime.now()
-    ds = uds_facevars.isel({xu_facedim:index_da})
-    ds = ds.where(index_da != grid.fill_value)
-    ds['x'] = xr.DataArray(regx,dims='x')
-    ds['y'] = xr.DataArray(regy,dims='y')
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    return ds
-
-
-def plot_ztdata(data_xr_sel, varname, ax=None, only_contour=False, **kwargs):
-    """
-    
-
-    Parameters
-    ----------
-    data_xr : TYPE
-        DESCRIPTION.
-    varname : TYPE
-        DESCRIPTION.
-    ax : matplotlib.axes._subplots.AxesSubplot, optional
-        the figure axis. The default is None.
-    only_contour : bool, optional
-        Wheter to plot contour lines of the dataset. The default is False.
-    **kwargs : TYPE
-        properties to give on to the pcolormesh function.
-    
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    pc : matplotlib.collections.QuadMesh
-        DESCRIPTION.
-    
-    """
-    
-    if not ax: ax=plt.gca()
-    
-    if len(data_xr_sel[varname].shape) != 2:
-        raise ValueError(f'ERROR: unexpected number of dimensions in requested squeezed variable ({data_xr_sel[varname].shape}), first use data_xr.isel(stations=int) to select a single station') #TODO: can also have a different cause, improve message/testing?
-    
-    #repair zvalues at wl/wl (filling nans and clipping to wl/bl). bfill replaces nan values with last valid value, this is necessary to enable pcolormesh to work. clip forces data to be within bl/wl
-    #TODO: put clip in preproces_hisnc to make plotting easier?
-    data_xr_sel['zcoordinate_c'] = data_xr_sel['zcoordinate_c'].bfill(dim='laydim').clip(min=data_xr_sel.bedlevel,max=data_xr_sel.waterlevel)
-    data_xr_sel['zcoordinate_w'] = data_xr_sel['zcoordinate_w'].bfill(dim='laydimw').clip(min=data_xr_sel.bedlevel,max=data_xr_sel.waterlevel)
-    
-    # generate 2 2d grids for the x & y bounds (you can also give one 2D array as input in case of eg time varying z coordinates)
-    data_fromhis_zcor = data_xr_sel['zcoordinate_w'].to_numpy() 
-    data_fromhis_zcor = np.concatenate([data_fromhis_zcor,data_fromhis_zcor[[-1],:]],axis=0)
-    time_np = data_xr_sel.time.to_numpy()
-    time_cor = np.concatenate([time_np,time_np[[-1]]])
-    time_mesh_cor = np.tile(time_cor,(data_fromhis_zcor.shape[-1],1)).T
-    if only_contour:
-        pc = data_xr_sel[varname].plot.contour(ax=ax, x='time', y='zcoordinate_c', **kwargs)
-    else:
-        #pc = data_xr_sel[varname].plot.pcolormesh(ax=ax, x='time', y='zcoordinate_w', **kwargs) #TODO: not possible to put center values on interfaces, so more difficult approach needed
-        pc = ax.pcolormesh(time_mesh_cor, data_fromhis_zcor, data_xr_sel[varname], **kwargs)
-   
-    return pc
-
+# -*- coding: utf-8 -*-
+"""
+dfm_tools are post-processing tools for Delft3D FM
+Copyright (C) 2020 Deltares. All rights reserved.
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  if not, see <http://www.gnu.org/licenses/>.
+
+All names, logos, and references to "Deltares" are registered trademarks of
+Stichting Deltares and remain full property of Stichting Deltares at all times.
+All rights reserved.
+
+
+INFORMATION
+This script is part of dfm_tools: https://github.com/openearth/dfm_tools
+Check the README.rst on github for other available functions
+Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
+Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
+
+Created on Fri Feb 14 12:45:11 2020
+
+@author: veenstra
+"""
+
+import numpy as np
+import datetime as dt
+import re
+import xugrid as xu
+import xarray as xr
+import matplotlib.pyplot as plt
+from dfm_tools.xarray_helpers import get_vertical_dimensions, Dataset_varswithdim
+import netCDF4
+
+
+def calc_dist_pythagoras(x1,x2,y1,y2):
+    distance = np.sqrt((x2 - x1)**2 + (y2 - y1)**2)
+    return distance
+
+
+def calc_dist_haversine(lon1,lon2,lat1,lat2):
+    """
+    calculates distance between lat/lon coordinates in meters
+    https://community.esri.com/t5/coordinate-reference-systems-blog/distance-on-a-sphere-the-haversine-formula/ba-p/902128
+    """
+    # convert to radians
+    lon1_rad = np.deg2rad(lon1)
+    lon2_rad = np.deg2rad(lon2)
+    lat1_rad = np.deg2rad(lat1)
+    lat2_rad = np.deg2rad(lat2)
+    
+    # apply formulae
+    a = np.sin((lat2_rad-lat1_rad)/2)**2 + np.cos(lat1_rad) * np.cos(lat2_rad) * np.sin((lon2_rad-lon1_rad)/2)**2
+    c = 2 * np.arctan2( np.sqrt(a), np.sqrt(1-a) )
+    R = 6371000
+    distance = R * c
+    if np.isnan(distance).any():
+        raise ValueError('nan encountered in calc_dist_latlon distance')
+    return distance
+
+
+def intersect_edges_withsort(uds,edges): #TODO: move sorting to xugrid? https://deltares.github.io/xugrid/api/xugrid.Ugrid2d.intersect_edges.html
+    
+    edge_index, face_index, intersections = uds.grid.intersect_edges(edges) #TODO: is fast, but maybe speed can be increased with bounding box?
+    
+    #ordering of face_index is wrong (visible with cb3 with long line_array), so sort on distance from startpoint (in x/y units)
+    
+    #compute distance from start of line to start of each linepart
+    edge_len = np.linalg.norm(edges[:,1] - edges[:,0], axis=1)
+    edge_len_cum = np.cumsum(edge_len)
+    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
+    
+    #compute distance from start to lineparts to start of line (via line)
+    startcoord_linepart = edges[edge_index,0,:]
+    dist_tostart_linepart = np.linalg.norm(intersections[:,0,:] - startcoord_linepart, axis=1)
+    dist_tostart_line = dist_tostart_linepart + edge_len_cum0[edge_index]
+    
+    #sorting on distance
+    id_sorted = np.argsort(dist_tostart_line)
+    edge_index = edge_index[id_sorted]
+    face_index = face_index[id_sorted]
+    intersections = intersections[id_sorted]
+    return edge_index, face_index, intersections
+
+
+def get_xzcoords_onintersection(uds, face_index, crs_dist_starts, crs_dist_stops):
+    #TODO: remove hardcoding of variable names
+    if 'time' in uds.dims: #TODO: maybe make time dependent grid?
+        raise Exception('time dimension present in uds, provide uds.isel(time=timestep) instead. This is necessary to retrieve correct waterlevel or fullgrid output')
+    
+    dimn_layer, dimn_interfaces = get_vertical_dimensions(uds)
+    gridname = uds.grid.name
+    
+    #construct fullgrid info (zcc/zw) for 3D models
+    if dimn_layer in uds.dims:
+        uds = reconstruct_zw_zcc(uds)
+
+    #drop all variables that do not contain a face dimension, then select only all sliced faceidx
+    xu_facedim = uds.grid.face_dimension
+    face_index_xr = xr.DataArray(face_index,dims=('ncrossed_faces'))
+    uds = Dataset_varswithdim(uds,dimname=xu_facedim) #TODO: is there an xugrid alternative?
+    uds_sel = uds.sel({xu_facedim:face_index_xr})
+    
+    # take zvals_interface
+    if dimn_layer in uds_sel.dims: #3D model
+        nlay = uds.dims[dimn_layer]
+        zvals_interface_filled = uds_sel[f'{gridname}_flowelem_zw'].bfill(dim=dimn_interfaces) #fill nan values (below bed) with equal values
+        zvals_interface = zvals_interface_filled.to_numpy().T #transpose to make in line with 2D sigma dataset
+    else: #2D model, no layers
+        nlay = 1
+        data_frommap_wl3_sel = uds_sel[f'{gridname}_s1'].to_numpy() #TODO: add escape for missing wl/bl vars
+        data_frommap_bl_sel = uds_sel[f'{gridname}_flowelem_bl'].to_numpy()
+        zvals_interface = np.linspace(data_frommap_bl_sel,data_frommap_wl3_sel,nlay+1)
+
+    #derive crs_verts
+    crs_dist_starts_matrix = np.repeat(crs_dist_starts[np.newaxis],nlay,axis=0)
+    crs_dist_stops_matrix = np.repeat(crs_dist_stops[np.newaxis],nlay,axis=0)
+    crs_verts_x_all = np.array([[crs_dist_starts_matrix.ravel(),crs_dist_stops_matrix.ravel(),crs_dist_stops_matrix.ravel(),crs_dist_starts_matrix.ravel()]]).T
+    crs_verts_z_all = np.ma.array([zvals_interface[1:,:].ravel(),zvals_interface[1:,:].ravel(),zvals_interface[:-1,:].ravel(),zvals_interface[:-1,:].ravel()]).T[:,:,np.newaxis]
+    crs_verts = np.ma.concatenate([crs_verts_x_all, crs_verts_z_all], axis=2)
+    
+    #define grid
+    shape_crs_grid = crs_verts[:,:,0].shape
+    shape_crs_flat = crs_verts[:,:,0].ravel().shape
+    xr_crs_grid = xu.Ugrid2d(node_x=crs_verts[:,:,0].ravel(),
+                             node_y=crs_verts[:,:,1].ravel(),
+                             fill_value=-1,
+                             face_node_connectivity=np.arange(shape_crs_flat[0]).reshape(shape_crs_grid),
+                             )
+
+    #define dataset
+    if dimn_layer in uds_sel.dims:
+        crs_plotdata_clean = uds_sel.stack({xr_crs_grid.face_dimension:[dimn_layer,'ncrossed_faces']},create_index=False)
+    else: #2D: still make sure xr_crs_grid.face_dimension is created, using stack since .rename() gives "UserWarning: rename 'ncrossed_faces' to 'mesh2d_nFaces' does not create an index anymore."
+        crs_plotdata_clean = uds_sel.stack({xr_crs_grid.face_dimension:['ncrossed_faces']},create_index=False)
+                    
+    #combine into xugrid
+    xr_crs_ugrid = xu.UgridDataset(crs_plotdata_clean, grids=[xr_crs_grid])
+    return xr_crs_ugrid
+
+
+def polyline_mapslice(uds:xu.UgridDataset, line_array:np.array, calcdist_fromlatlon:bool = None) -> xu.UgridDataset:
+    """
+    Slice trough mapdata, combine: intersect_edges_withsort, calculation of distances and conversion to ugrid dataset.
+
+    Parameters
+    ----------
+    uds : xu.UgridDataset
+        DESCRIPTION.
+    line_array : np.array
+        DESCRIPTION.
+    calcdist_fromlatlon : bool, optional
+        DESCRIPTION. The default is None.
+
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    xr_crs_ugrid : xu.UgridDataset
+        DESCRIPTION.
+
+    """
+    
+    #compute intersection coordinates of crossings between edges and faces and their respective indices
+    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
+    edge_index, face_index, intersections = intersect_edges_withsort(uds=uds, edges=edges)
+    if len(edge_index) == 0:
+        raise ValueError('polyline does not cross mapdata')
+    
+    #auto determine if cartesian/sperical distance should be computed
+    if calcdist_fromlatlon is None:
+        if hasattr(uds,'projected_coordinate_system'):
+            calcdist_fromlatlon = False
+        elif hasattr(uds,'wgs84'):
+            calcdist_fromlatlon = True
+        else:
+            raise KeyError('To auto determine calcdist_fromlatlon, a variable "projected_coordinate_system" or "wgs84" is required, please provide calcdist_fromlatlon=True/False yourself.')
+    if calcdist_fromlatlon:
+        calc_dist = calc_dist_haversine
+    else:
+        calc_dist = calc_dist_pythagoras
+    
+    #compute pyt/haversine start/stop distances for all intersections
+    edge_len = calc_dist(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
+    edge_len_cum = np.cumsum(edge_len)
+    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
+    crs_dist_starts = calc_dist(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
+    crs_dist_stops  = calc_dist(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
+    
+    #derive vertices from cross section (distance from first point)
+    xr_crs_ugrid = get_xzcoords_onintersection(uds=uds, face_index=face_index, crs_dist_starts=crs_dist_starts, crs_dist_stops=crs_dist_stops)
+    
+    return xr_crs_ugrid
+
+
+def get_formula_terms(uds, varn_contains):
+    """
+    get formula_terms for zw/zcc reconstruction, convert to list and then to dict. This can be done for layer/interface (via varn_contains)
+    """
+    osz_varnames = list(uds.filter_by_attrs(formula_terms=lambda v: v is not None).variables) #names of variables containing attribute "formula_terms"
+    osz_varnames_contains = [x for x in osz_varnames if varn_contains in x] #TODO: to get the layer/interface ocean_*_coordinate. Not too pretty, but it works
+    if len(osz_varnames_contains) != 1: #should be 1 exactly, none is the case in zlayer models
+        raise ValueError(f'no or more than one {varn_contains} variable found with formula_terms attribute: {osz_varnames}')
+    osz_varn = osz_varnames_contains[0]
+    osz_formulaterms = uds[osz_varn].attrs['formula_terms']
+    tokens = re.split('[:\\s]+', osz_formulaterms)
+    osz_formulaterms_dict = dict(zip(tokens[::2], tokens[1::2]))
+    return osz_formulaterms_dict
+
+
+def reconstruct_zw_zcc_fromsigma(uds):
+    """
+    reconstruct full grid output (time/face-varying z-values) for sigma model, necessary for slicing sigmamodel on depth value
+    based on https://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_sigma_coordinate
+    """
+    osz_formulaterms_int_dict = get_formula_terms(uds,varn_contains='interface')
+    osz_formulaterms_lay_dict = get_formula_terms(uds,varn_contains='layer')
+    
+    uds_eta = uds[osz_formulaterms_int_dict['eta']] #mesh2d_s1
+    uds_depth = uds[osz_formulaterms_int_dict['depth']] #mesh2d_bldepth in new output, mesh2d_waterdepth in old output (see comment below)
+    if uds_depth.attrs['standard_name'] == 'sea_floor_depth_below_sea_surface': # previously the waterdepth instead of negative bedlevel was coupled via the formula_terms in sigmamodels (was fixed in OSS 140982 / 29-3-2022)
+        uds_depth = -uds['mesh2d_flowelem_bl'] # assuming this variable is available, which is not guaranteed
+    uds_sigma_int = uds[osz_formulaterms_int_dict['sigma']] #mesh2d_interface_sigma
+    uds_sigma_lay = uds[osz_formulaterms_lay_dict['sigma']] #mesh2d_layer_sigma
+    
+    uds['mesh2d_flowelem_zw'] = uds_eta + uds_sigma_int*(uds_depth+uds_eta)
+    uds['mesh2d_flowelem_zcc'] = uds_eta + uds_sigma_lay*(uds_depth+uds_eta)
+    
+    uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
+    return uds
+
+
+def reconstruct_zw_zcc_fromz(data_xr_map):
+    """
+    reconstruct full grid output (time/face-varying z-values) for zvalue model. Necessary when extracting values with zdepth w.r.t. waterlevel/bedlevel
+    #TODO: gives spotty result for 0/0.1m w.r.t. bedlevel for Grevelingen zmodel
+    #TODO: remove hardcoding of varnames (assuming wl/bl variables are available)
+    #TODO: center values are clipped to waterlevel+bedlevel, so the center values of the top+bottom layer are currently incorrect
+    """
+    
+    dimn_layer, dimn_interfaces = get_vertical_dimensions(data_xr_map)
+    
+    data_frommap_wl_sel = data_xr_map['mesh2d_s1']
+    data_frommap_z0_sel = data_frommap_wl_sel*0
+    data_frommap_bl_sel = data_xr_map['mesh2d_flowelem_bl']
+    
+    zvals_cen_zval = data_xr_map['mesh2d_layer_z'] #no clipping for zcenter values, since otherwise interp will fail
+    data_xr_map['mesh2d_flowelem_zcc'] = (data_frommap_z0_sel+zvals_cen_zval).clip(min=data_frommap_bl_sel, max=data_frommap_wl_sel)
+
+    zvals_interface_zval = data_xr_map['mesh2d_interface_z'] #clipping for zinterface values, to make sure layer interfaces are also at water/bed level
+    data_xr_map['mesh2d_flowelem_zw'] = (data_frommap_z0_sel+zvals_interface_zval).clip(min=data_frommap_bl_sel, max=data_frommap_wl_sel)
+    bool_notoplayer_int = zvals_interface_zval<zvals_interface_zval.isel({dimn_interfaces:-1})
+    bool_int_abovewl = zvals_interface_zval>data_frommap_wl_sel
+    data_xr_map['mesh2d_flowelem_zw'] = data_xr_map['mesh2d_flowelem_zw'].where(bool_notoplayer_int | bool_int_abovewl, other=data_frommap_wl_sel) #zvalues of top layer_interfaces that are lower than wl are replaced by wl
+    
+    data_xr_map = data_xr_map.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
+    return data_xr_map
+
+
+def reconstruct_zw_zcc_fromzsigma(uds):
+    """
+    reconstruct full grid output (time/face-varying z-values) for zsigmavalue model without full grid output. Implemented in https://issuetracker.deltares.nl/browse/UNST-5477
+    based on https://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_sigma_over_z_coordinate
+    #TODO: center values are clipped to bedlevel, so the center values of the bottom layer are currently incorrect
+    """
+    
+    #TODO: default fillvalues are not automatically parsed to nan, so doing it manually: https://github.com/pydata/xarray/issues/2742
+    fillvals = netCDF4.default_fillvals
+    
+    osz_formulaterms_int_dict = get_formula_terms(uds,varn_contains='interface')
+    osz_formulaterms_lay_dict = get_formula_terms(uds,varn_contains='layer')
+    
+    uds_eta = uds[osz_formulaterms_int_dict['eta']] #mesh2d_s1
+    uds_depth = uds[osz_formulaterms_int_dict['depth']] #mesh2d_bldepth: positive version of mesh2d_flowelem_bl, but this one is always in file
+    uds_depth_c = uds[osz_formulaterms_int_dict['depth_c']] #mesh2d_sigmazdepth
+    uds_zlev_int = uds[osz_formulaterms_int_dict['zlev']] #mesh2d_interface_z
+    uds_zlev_int = uds_zlev_int.where(uds_zlev_int!=fillvals['f8'])
+    uds_sigma_int = uds[osz_formulaterms_int_dict['sigma']] #mesh2d_interface_sigma
+    uds_sigma_int = uds_sigma_int.where(uds_sigma_int!=fillvals['f8'])
+    uds_zlev_lay = uds[osz_formulaterms_lay_dict['zlev']] #mesh2d_layer_z
+    uds_zlev_lay = uds_zlev_lay.where(uds_zlev_lay!=fillvals['f8'])
+    uds_sigma_lay = uds[osz_formulaterms_lay_dict['sigma']] #mesh2d_layer_sigma
+    uds_sigma_lay = uds_sigma_lay.where(uds_sigma_lay!=fillvals['f8'])
+    
+    # for levels k where sigma(k) has a defined value and zlev(k) is not defined:
+    # z(n,k,j,i) = eta(n,j,i) + sigma(k)*(min(depth_c,depth(j,i))+eta(n,j,i))
+    zw_sigmapart = uds_eta + uds_sigma_int*(uds_depth.clip(max=uds_depth_c)+uds_eta)
+    zcc_sigmapart = uds_eta + uds_sigma_lay*(uds_depth.clip(max=uds_depth_c)+uds_eta)
+    # for levels k where zlev(k) has a defined value and sigma(k) is not defined: 
+    # z(n,k,j,i) = zlev(k)
+    zw_zpart = uds_zlev_int.clip(min=-uds_depth) #added clipping of zvalues with bedlevel
+    zcc_zpart = uds_zlev_lay.clip(min=-uds_depth) #added clipping of zvalues with bedlevel
+    uds['mesh2d_flowelem_zw'] = zw_sigmapart.fillna(zw_zpart)
+    uds['mesh2d_flowelem_zcc'] = zcc_sigmapart.fillna(zcc_zpart)
+    
+    uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
+    return uds
+
+
+def reconstruct_zw_zcc(ds):
+    dimn_layer, dimn_interfaces = get_vertical_dimensions(ds)
+    
+    if dimn_layer is not None: #D-FlowFM mapfile
+        gridname = ds.grid.name
+        varname_zint = f'{gridname}_flowelem_zw'
+    elif 'laydim' in ds.dims: #D-FlowFM hisfile
+        varname_zint = 'zcoordinate_w'
+    
+    #reconstruct zw/zcc variables (if not in file) and treat as fullgrid mapfile from here
+    if varname_zint in ds.variables: #fullgrid info already available, so continuing
+        print(f'zw/zcc (fullgrid) values already present in Dataset in variable {varname_zint}')
+    elif len(ds.filter_by_attrs(standard_name='ocean_sigma_z_coordinate')) != 0:
+        print('zsigma-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
+        ds = reconstruct_zw_zcc_fromzsigma(ds)
+    elif 'mesh2d_layer_sigma' in ds.variables: #TODO: var with standard_name='ocean_sigma_coordinate' available?
+        print('sigma-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
+        ds = reconstruct_zw_zcc_fromsigma(ds)
+    elif 'mesh2d_layer_z' in ds.variables:
+        print('z-layer model, computing zw/zcc (fullgrid) values and treat as fullgrid model from here')
+        ds = reconstruct_zw_zcc_fromz(ds)
+    else:
+        raise KeyError('layers present, but unknown layertype, expected one of variables: mesh2d_flowelem_zw, mesh2d_layer_sigma, mesh2d_layer_z')
+    return ds
+
+    
+def get_Dataset_atdepths(data_xr:xu.UgridDataset, depths, reference:str ='z0'):    
+    """
+    Lazily depth-slice a dataset with layers. Performance can be increased by using a subset of variables or subsetting the dataset in any dimension.
+    This can be done for instance with ds.isel(time=-1) or uds.ugrid.sel(x=slice(),y=slice()) to subset a ugrid dataset in space.
+    The return dataset only contains the sliced variables.
+    
+    Parameters
+    ----------
+    data_xr : xu.UgridDataset
+        has to be Dataset (not a DataArray), otherwise mesh2d_flowelem_zw etc are not available (interface z values)
+        in case of zsigma/sigma layers (or fullgrid), it is advisable to .sel()/.isel() the time dimension first, because that is less computationally heavy
+    depths : TYPE
+        int/float or list/array of int/float. Depths w.r.t. reference level. If reference=='waterlevel', depth>0 returns only nans. If reference=='bedlevel', depth<0 returns only nans. Depths are sorted and only uniques are kept.
+    reference : str, optional
+        compute depth w.r.t. z0/waterlevel/bed. The default is 'z0'.
+    zlayer_z0_selnearest : bool, optional
+        Use xr.interp() to interpolate zlayer model to z-value. Only possible for reference='z' (not 'waterlevel' or 'bedlevel'). Only used if "mesh2d_layer_z" is present (zlayer model)
+        This is faster but results in values interpolated between zcc (z cell centers), so it is different than slicing.. The default is False.
+
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    xu.UgridDataset
+        Dataset with the depth-sliced variables.
+
+    """
+    
+    depth_vardimname = f'depth_from_{reference}'
+    
+    dimn_layer, dimn_interfaces = get_vertical_dimensions(data_xr)
+    
+    if dimn_layer is not None: #D-FlowFM mapfile
+        gridname = data_xr.grid.name
+        varname_zint = f'{gridname}_flowelem_zw'
+        dimname_layc = dimn_layer
+        dimname_layw = dimn_interfaces
+        varname_wl = f'{gridname}_s1'
+        varname_bl = f'{gridname}_flowelem_bl'
+    elif 'laydim' in data_xr.dims: #D-FlowFM hisfile
+        varname_zint = 'zcoordinate_w'
+        dimname_layc = 'laydim'
+        dimname_layw = 'laydimw'
+        varname_wl = 'waterlevel'
+        varname_bl = 'bedlevel'
+    else:
+        print(UserWarning('depth/layer dimension not found, probably 2D model, returning input Dataset')) #TODO: this can also be at depth, since slice will put parts of model dry (and allnan if below wl or below bl). Implement this
+        return data_xr #early return
+    
+    if not isinstance(data_xr,(xr.Dataset,xu.UgridDataset)):
+        raise TypeError(f'data_xr_map should be of type xr.Dataset, but is {type(data_xr)}')
+    
+    #create depth xr.DataArray
+    if isinstance(depths,(float,int)):
+        depth_dims = ()
+    else:
+        depths = np.unique(depths) #array of unique+sorted floats/ints
+        depth_dims = (depth_vardimname)
+    depths_xr = xr.DataArray(depths,dims=depth_dims,attrs={'units':'m',
+                                                           'reference':f'model_{reference}',
+                                                           'positive':'up'}) #TODO: make more in line with CMEMS etc
+    
+    #potentially construct fullgrid info (zcc/zw)
+    data_xr = reconstruct_zw_zcc(data_xr)
+    
+    #correct reference level
+    if reference=='z0':
+        zw_reference = data_xr[varname_zint]
+    elif reference=='waterlevel':
+        if varname_wl not in data_xr.variables:
+            raise KeyError(f'get_Dataset_atdepths() called with reference=waterlevel, but {varname_wl} variable not present')
+        data_wl = data_xr[varname_wl]
+        zw_reference = data_xr[varname_zint] - data_wl
+    elif reference=='bedlevel':
+        if varname_bl not in data_xr.variables:
+            raise KeyError(f'get_Dataset_atdepths() called with reference=bedlevel, but {varname_bl} variable not present') #TODO: in case of zsigma/sigma it can also be -mesh2d_bldepth
+        data_bl = data_xr[varname_bl]
+        zw_reference = data_xr[varname_zint] - data_bl
+    else:
+        raise KeyError(f'unknown reference "{reference}" (possible are z0, waterlevel and bedlevel') #TODO: make enum?
+    
+    print('>> subsetting data on fixed depth in fullgrid z-data: ',end='')
+    dtstart = dt.datetime.now()
+    
+    #get layerbool via z-interface value (zw), check which celltop-interfaces are above/on depth and which which cellbottom-interfaces are below/on depth
+    bool_topinterface_abovedepth = zw_reference.isel({dimname_layw:slice(1,None)}) >= depths_xr
+    bool_botinterface_belowdepth = zw_reference.isel({dimname_layw:slice(None,-1)}) <= depths_xr
+    bool_topbotinterface_arounddepth = bool_topinterface_abovedepth & bool_botinterface_belowdepth #this bool also automatically excludes all values below bed and above wl
+    bool_topbotinterface_arounddepth = bool_topbotinterface_arounddepth.rename({dimname_layw:dimname_layc}) #correct dimname for interfaces to centers
+    
+    #subset variables that have no, time, face and/or layer dims, slice only variables with all three dims (and add to subset)
+    bool_dims = [x for x in bool_topbotinterface_arounddepth.dims if x!=depth_vardimname] #exclude depth_vardimname (present if multiple depths supplied), since it is not present in pre-slice variables
+    variables_toslice = [var for var in data_xr.data_vars if set(bool_dims).issubset(data_xr[var].dims)]
+    
+    #actual slicing with .where().max()
+    ds_atdepths = data_xr[variables_toslice].where(bool_topbotinterface_arounddepth).max(dim=dimname_layc,keep_attrs=True) #set all layers but one to nan, followed by an arbitrary reduce (max in this case) #TODO: check if attributes should be passed/altered
+    #TODO: suppress warning (upon plotting/load/etc): "C:\Users\veenstra\Anaconda3\envs\dfm_tools_env\lib\site-packages\dask\array\reductions.py:640: RuntimeWarning: All-NaN slice encountered" >> already merged in xarray: https://github.com/dask/dask/pull/9916
+    ds_atdepths = ds_atdepths.drop_dims([dimname_layw,dimname_layc],errors='ignore') #dropping interface dim if it exists, since it does not correspond to new depths dim
+    
+    #add depth as coordinate var
+    ds_atdepths[depth_vardimname] = depths_xr
+    ds_atdepths = ds_atdepths.set_coords([depth_vardimname])
+    
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    return ds_atdepths
+
+
+def rasterize_ugrid(uds:xu.UgridDataset, ds_like:xr.Dataset = None, resolution:float = None):
+    """
+    Rasterizing ugrid dataset to regular dataset. ds_like has higher priority than `resolution`. If both are not passed, a raster is generated of at least 200x200
+    inspired by xugrid.plot.imshow and xugrid.ugrid.ugrid2d.rasterize/rasterize_like.
+
+
+    Parameters
+    ----------
+    uds : xu.UgridDataset
+        DESCRIPTION.
+    ds_like : xr.Dataset, optional
+        xr.Dataset with ed x and y variables to interpolate uds to. The default is None.
+    resolution : float, optional
+        Only used if ds_like is not supplied. The default is None.
+    
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds : TYPE
+        DESCRIPTION.
+
+    """
+    #TODO: maybe put part of code in xugrid (https://github.com/Deltares/xugrid/issues/31)
+    #TODO: vars can also be rasterized with uds_facevars[var].ugrid.rasterize(resolution), but is not efficient. Wait for uds.rasterize() method: https://github.com/Deltares/xugrid/issues/61
+    if not isinstance(uds,xu.core.wrap.UgridDataset):
+        raise TypeError(f'rasterize_ugrid expected xu.core.wrap.UgridDataset, got {type(uds)} instead')
+    
+    grid = uds.grid
+    xu_facedim = uds.grid.face_dimension
+    uds_facevars = Dataset_varswithdim(uds,xu_facedim)
+    
+    if ds_like is not None:
+        regx = ds_like.x
+        regy = ds_like.y
+    else:
+        xmin, ymin, xmax, ymax = grid.bounds
+        dx = xmax - xmin
+        dy = ymax - ymin
+        if resolution is None: # check if a rasterization resolution is passed, otherwise default to 200 raster cells otherwise for the smallest axis.
+            resolution = min(dx, dy) / 200
+        d = abs(resolution)
+        regx = np.arange(xmin + 0.5 * d, xmax, d)
+        regy = np.arange(ymin + 0.5 * d, ymax, d)
+    
+    regx, regy, index = grid.rasterize_like(x=regx,y=regy) #TODO: this can be used to steer rasterization, eg with xstart/ystart/xres/yres
+    index_da = xr.DataArray(index,dims=('y','x'))
+    
+    print(f'>> rasterizing ugrid dataset with {len(uds_facevars.data_vars)} face variables to shape={index_da.shape}: ',end='')
+    dtstart = dt.datetime.now()
+    ds = uds_facevars.isel({xu_facedim:index_da})
+    ds = ds.where(index_da != grid.fill_value)
+    ds['x'] = xr.DataArray(regx,dims='x')
+    ds['y'] = xr.DataArray(regy,dims='y')
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    return ds
+
+
+def plot_ztdata(data_xr_sel, varname, ax=None, only_contour=False, **kwargs):
+    """
+    
+
+    Parameters
+    ----------
+    data_xr : TYPE
+        DESCRIPTION.
+    varname : TYPE
+        DESCRIPTION.
+    ax : matplotlib.axes._subplots.AxesSubplot, optional
+        the figure axis. The default is None.
+    only_contour : bool, optional
+        Wheter to plot contour lines of the dataset. The default is False.
+    **kwargs : TYPE
+        properties to give on to the pcolormesh function.
+    
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    pc : matplotlib.collections.QuadMesh
+        DESCRIPTION.
+    
+    """
+    
+    if not ax: ax=plt.gca()
+    
+    if len(data_xr_sel[varname].shape) != 2:
+        raise ValueError(f'ERROR: unexpected number of dimensions in requested squeezed variable ({data_xr_sel[varname].shape}), first use data_xr.isel(stations=int) to select a single station') #TODO: can also have a different cause, improve message/testing?
+    
+    #repair zvalues at wl/wl (filling nans and clipping to wl/bl). bfill replaces nan values with last valid value, this is necessary to enable pcolormesh to work. clip forces data to be within bl/wl
+    #TODO: put clip in preproces_hisnc to make plotting easier?
+    data_xr_sel['zcoordinate_c'] = data_xr_sel['zcoordinate_c'].bfill(dim='laydim').clip(min=data_xr_sel.bedlevel,max=data_xr_sel.waterlevel)
+    data_xr_sel['zcoordinate_w'] = data_xr_sel['zcoordinate_w'].bfill(dim='laydimw').clip(min=data_xr_sel.bedlevel,max=data_xr_sel.waterlevel)
+    
+    # generate 2 2d grids for the x & y bounds (you can also give one 2D array as input in case of eg time varying z coordinates)
+    data_fromhis_zcor = data_xr_sel['zcoordinate_w'].to_numpy() 
+    data_fromhis_zcor = np.concatenate([data_fromhis_zcor,data_fromhis_zcor[[-1],:]],axis=0)
+    time_np = data_xr_sel.time.to_numpy()
+    time_cor = np.concatenate([time_np,time_np[[-1]]])
+    time_mesh_cor = np.tile(time_cor,(data_fromhis_zcor.shape[-1],1)).T
+    if only_contour:
+        pc = data_xr_sel[varname].plot.contour(ax=ax, x='time', y='zcoordinate_c', **kwargs)
+    else:
+        #pc = data_xr_sel[varname].plot.pcolormesh(ax=ax, x='time', y='zcoordinate_w', **kwargs) #TODO: not possible to put center values on interfaces, so more difficult approach needed
+        pc = ax.pcolormesh(time_mesh_cor, data_fromhis_zcor, data_xr_sel[varname], **kwargs)
+   
+    return pc
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/get_nc_helpers.py` & `dfm_tools-0.11.0/dfm_tools/get_nc_helpers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-# -*- coding: utf-8 -*-
-"""
-dfm_tools are post-processing tools for Delft3D FM
-Copyright (C) 2020 Deltares. All rights reserved.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  if not, see <http://www.gnu.org/licenses/>.
-
-All names, logos, and references to "Deltares" are registered trademarks of
-Stichting Deltares and remain full property of Stichting Deltares at all times.
-All rights reserved.
-
-
-INFORMATION
-This script is part of dfm_tools: https://github.com/openearth/dfm_tools
-Check the README.rst on github for other available functions
-Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
-Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
-
-Created on Fri Feb 14 12:43:19 2020
-
-@author: veenstra
-
-helper functions for functions in get_nc.py
-"""
-
-import xarray as xr
-import xugrid as xu
-import pandas as pd
-import warnings
-
-
-def get_ncvarproperties(data_xr):
-    if not isinstance(data_xr,(xr.Dataset,xu.UgridDataset)):
-        raise TypeError('data_xr should be of type xr.Dataset or xu.UgridDataset')
-    
-    nc_varkeys = data_xr.variables.mapping.keys()
-    
-    list_varattrs_pd = []
-    for varkey in nc_varkeys:
-        varattrs_pd = pd.DataFrame({varkey:data_xr.variables.mapping[varkey].attrs}).T
-        varattrs_pd[['shape','dimensions']] = 2*[''] #set dtype as str (float will raise an error when putting tuple in there)
-        varattrs_pd.at[varkey,'shape'] = data_xr[varkey].shape
-        varattrs_pd.at[varkey,'dimensions'] = data_xr.variables[varkey].dims
-        varattrs_pd.loc[varkey,'dtype'] = data_xr.variables[varkey].dtype
-        list_varattrs_pd.append(varattrs_pd)
-    
-    vars_pd = pd.concat(list_varattrs_pd,axis=0)
-    vars_pd[vars_pd.isnull()] = '' #avoid nan values
-    
-    data_xr.close()
-
-    return vars_pd
-
-
-def rename_waqvars(ds:(xr.Dataset,xu.UgridDataset)):
-    """
-    Rename all water quality variables in a dataset (like mesh2d_water_quality_output_24) to their long_name attribute (like mesh2d_DOscore)
-    
-    Parameters
-    ----------
-    ds : (xr.Dataset,xu.UgridDataset)
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds : TYPE
-        DESCRIPTION.
-
-    """
-    #TODO: results also in variable "mesh2d_Water quality mass balance areas" (with spaces), report in FM issue (remove spaces from long_name attr)
-    
-    if hasattr(ds,'grid'): #append gridname (e.g. mesh2d) in case of mapfile
-        varn_prepend = f'{ds.grid.name}_'
-    else:
-        varn_prepend = ''
-    list_waqvars = [i for i in ds.data_vars if 'water_quality_' in i] #water_quality_output and water_quality_stat
-    rename_dict = {waqvar:varn_prepend+ds[waqvar].attrs['long_name'] for waqvar in list_waqvars}
-    
-    if len(rename_dict) == 0: #early return to silence "FutureWarning: The default dtype for empty Series will be 'object' instead of 'float64' in a future version. Specify a dtype explicitly to silence this warning."
-        return ds
-    
-    #prevent renaming duplicate long_names
-    rename_pd = pd.Series(rename_dict)
-    if rename_pd.duplicated().sum():
-        duplicated_pd = rename_pd.loc[rename_pd.duplicated(keep=False)]
-        print(UserWarning(f'duplicate long_name attributes found with dfmt.rename_waqvars(), renaming only first variable:\n{duplicated_pd}'))
-        rename_dict = rename_pd.loc[~rename_pd.duplicated()].to_dict()
-    
-    ds = ds.rename(rename_dict)
-    return ds
-
-
-def rename_fouvars(ds:(xr.Dataset,xu.UgridDataset), drop_tidal_times:bool = True):
-    """
-    Rename all fourier variables in a dataset (like mesh2d_fourier033_amp) to a unique name containing gridname/quantity/analysistype/tstart/tstop
-    
-    Parameters
-    ----------
-    ds : (xr.Dataset,xu.UgridDataset)
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds : TYPE
-        DESCRIPTION.
-
-    """
-    
-    file_freqs = 'https://raw.githubusercontent.com/Deltares/hatyan/main/hatyan/data/data_foreman_frequencies.txt' #TODO: fix hatyan dependency (MSQM and M1 were also added, but file is not used by hatyan, so might disappear one day)
-    freqs_pd = pd.read_csv(file_freqs,names=['freq','dependents'],delim_whitespace=True,comment='#')
-    freqs_pd['angfreq'] = freqs_pd['freq'] * 360 #deg/hr
-    
-    gridname = ds.grid.name
-    list_fouvars = [i for i in ds.data_vars if '_fourier' in i] #water_quality_output and water_quality_stat
-    
-    rename_dict = {}
-    for fouvar in list_fouvars:
-        fouvar_attrs_lower = {k.lower():v for k,v in ds[fouvar].attrs.items()}
-        fouvar_lowerattrs = ds[fouvar].assign_attrs(fouvar_attrs_lower) #to avoid case issues
-        
-        #quantity
-        long_name = fouvar_lowerattrs.attrs['long_name']
-        long_name_noprefix = long_name.split(': ')[1]
-        quantity_long = long_name_noprefix.split(',')[0]
-        quantity_dict = {'water level':'s1', #dict based on https://svn.oss.deltares.nl/repos/delft3d/trunk/src/engines_gpl/dflowfm/packages/dflowfm_kernel/src/dflowfm_kernel/prepost/fourier_analysis.f90
-                         #'energy head':'s1', #TODO: duplicate namfun/dictvalue is not convenient
-                         'wind speed':'ws',
-                         'U-component of cell-centre velocity':'ux',
-                         'V-component of cell-centre velocity':'uy',
-                         'U-component velocity, column average':'uxa',
-                         'V-component velocity, column average':'uya',
-                         'velocity magnitude':'uc',
-                         #'':'r1', #TODO: unclear which namfun/dictvalue corresponds (trim(namcon(gdfourier%fconno(ifou))))
-                         'velocity':'u1',
-                         'unit discharge':'qx',
-                         'bed stress':'ta',
-                         'freeboard':'fb',
-                         'waterdepth_on_ground':'wdog',
-                         'volume_on_ground':'vog',
-                         'discharge through flow link':'q1',
-                         'water level at flow link':'su1',
-                         'temperature':'tem', #not clear from fourier_analysis.f90, ct in user manual C.13
-                         'salt':'sal', #not clear from fourier_analysis.f90, cs in user manual C.13
-                         }
-        if quantity_long not in quantity_dict.keys():
-            raise KeyError(f'quantity_dict does not yet contain quantity for: {quantity_long}')
-        quantity = quantity_dict[quantity_long]
-        
-        #analysistype
-        istidal = False
-        if hasattr(fouvar_lowerattrs,'frequency_degrees_per_hour'):
-            if fouvar_lowerattrs.attrs['frequency_degrees_per_hour'] > 0: #wl mean with numcyc=0 has frequency attribute (wl min with numcyc=0 does not)
-                istidal = True #for tidal components with frequency >0
-        
-        if istidal: #for tidal analysistype
-            tidepart = fouvar.split('_')[-1] # amp/phs
-            freq = fouvar_lowerattrs.attrs['frequency_degrees_per_hour']
-            compidx_closestfreq = (freqs_pd['angfreq'] - freq).abs().argmin()
-            compname = freqs_pd.index[compidx_closestfreq] #M2/NU2
-            analysistype = tidepart+compname
-            warnings.warn(UserWarning('tidal components found in foufile, matching frequency with online list to get component names, which might go wrong. Also, be aware that v0 and knfac columns from fourier inputfile are not available in fourier output, so it is not clear whether to correct for these.'))
-        else: #for all other quantities
-            fouvar_splitted = fouvar.split('_')
-            analysistype = ''.join(fouvar_splitted[2:]) #min/max/mean. min_depth/max_depth etc are converted to mindepth/maxdepth
-            
-        #tstart/tstop
-        refdate = pd.Timestamp(str(fouvar_lowerattrs.attrs['reference_date_in_yyyymmdd']))
-        if hasattr(fouvar_lowerattrs,'starttime_fourier_analysis_in_minutes_since_reference_date'):
-            tstart_min = fouvar_lowerattrs.attrs['starttime_fourier_analysis_in_minutes_since_reference_date']
-            tstop_min = fouvar_lowerattrs.attrs['stoptime_fourier_analysis_in_minutes_since_reference_date']
-        elif hasattr(fouvar_lowerattrs,'starttime_min_max_analysis_in_minutes_since_reference_date'):
-            tstart_min = fouvar_lowerattrs.attrs['starttime_min_max_analysis_in_minutes_since_reference_date']
-            tstop_min = fouvar_lowerattrs.attrs['stoptime_min_max_analysis_in_minutes_since_reference_date']
-        else:
-            raise AttributeError(f'starttime/stoptime attribute not found in fouvar:\n{fouvar_lowerattrs.attrs}')
-        tstart_str = (refdate + pd.Timedelta(minutes=tstart_min)).strftime('%Y%m%d%H%M%S')
-        tstop_str = (refdate + pd.Timedelta(minutes=tstop_min)).strftime('%Y%m%d%H%M%S')
-        
-        rename_dict[fouvar] = f'{gridname}_{quantity}_{analysistype}_{tstart_str}_{tstop_str}'
-        if istidal and drop_tidal_times:
-            rename_dict[fouvar] = f'{gridname}_{quantity}_{analysistype}' #TODO: might cause conflicting variable names if one component is analysed for multiple periods or if component is not defined in frequency list. Add duplicate check like rename_waqvars() that provides some basic info for debugging.
-    
-    ds = ds.rename(rename_dict)
-    return ds
-
+# -*- coding: utf-8 -*-
+"""
+dfm_tools are post-processing tools for Delft3D FM
+Copyright (C) 2020 Deltares. All rights reserved.
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  if not, see <http://www.gnu.org/licenses/>.
+
+All names, logos, and references to "Deltares" are registered trademarks of
+Stichting Deltares and remain full property of Stichting Deltares at all times.
+All rights reserved.
+
+
+INFORMATION
+This script is part of dfm_tools: https://github.com/openearth/dfm_tools
+Check the README.rst on github for other available functions
+Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
+Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
+
+Created on Fri Feb 14 12:43:19 2020
+
+@author: veenstra
+
+helper functions for functions in get_nc.py
+"""
+
+import xarray as xr
+import xugrid as xu
+import pandas as pd
+import warnings
+
+
+def get_ncvarproperties(data_xr):
+    if not isinstance(data_xr,(xr.Dataset,xu.UgridDataset)):
+        raise TypeError('data_xr should be of type xr.Dataset or xu.UgridDataset')
+    
+    nc_varkeys = data_xr.variables.mapping.keys()
+    
+    list_varattrs_pd = []
+    for varkey in nc_varkeys:
+        varattrs_pd = pd.DataFrame({varkey:data_xr.variables.mapping[varkey].attrs}).T
+        varattrs_pd[['shape','dimensions']] = 2*[''] #set dtype as str (float will raise an error when putting tuple in there)
+        varattrs_pd.at[varkey,'shape'] = data_xr[varkey].shape
+        varattrs_pd.at[varkey,'dimensions'] = data_xr.variables[varkey].dims
+        varattrs_pd.loc[varkey,'dtype'] = data_xr.variables[varkey].dtype
+        list_varattrs_pd.append(varattrs_pd)
+    
+    vars_pd = pd.concat(list_varattrs_pd,axis=0)
+    vars_pd[vars_pd.isnull()] = '' #avoid nan values
+    
+    data_xr.close()
+
+    return vars_pd
+
+
+def rename_waqvars(ds:(xr.Dataset,xu.UgridDataset)):
+    """
+    Rename all water quality variables in a dataset (like mesh2d_water_quality_output_24) to their long_name attribute (like mesh2d_DOscore)
+    
+    Parameters
+    ----------
+    ds : (xr.Dataset,xu.UgridDataset)
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds : TYPE
+        DESCRIPTION.
+
+    """
+    #TODO: results also in variable "mesh2d_Water quality mass balance areas" (with spaces), report in FM issue (remove spaces from long_name attr)
+    
+    if hasattr(ds,'grid'): #append gridname (e.g. mesh2d) in case of mapfile
+        varn_prepend = f'{ds.grid.name}_'
+    else:
+        varn_prepend = ''
+    list_waqvars = [i for i in ds.data_vars if 'water_quality_' in i] #water_quality_output and water_quality_stat
+    rename_dict = {waqvar:varn_prepend+ds[waqvar].attrs['long_name'] for waqvar in list_waqvars}
+    
+    if len(rename_dict) == 0: #early return to silence "FutureWarning: The default dtype for empty Series will be 'object' instead of 'float64' in a future version. Specify a dtype explicitly to silence this warning."
+        return ds
+    
+    #prevent renaming duplicate long_names
+    rename_pd = pd.Series(rename_dict)
+    if rename_pd.duplicated().sum():
+        duplicated_pd = rename_pd.loc[rename_pd.duplicated(keep=False)]
+        print(UserWarning(f'duplicate long_name attributes found with dfmt.rename_waqvars(), renaming only first variable:\n{duplicated_pd}'))
+        rename_dict = rename_pd.loc[~rename_pd.duplicated()].to_dict()
+    
+    ds = ds.rename(rename_dict)
+    return ds
+
+
+def rename_fouvars(ds:(xr.Dataset,xu.UgridDataset), drop_tidal_times:bool = True):
+    """
+    Rename all fourier variables in a dataset (like mesh2d_fourier033_amp) to a unique name containing gridname/quantity/analysistype/tstart/tstop
+    
+    Parameters
+    ----------
+    ds : (xr.Dataset,xu.UgridDataset)
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds : TYPE
+        DESCRIPTION.
+
+    """
+    
+    file_freqs = 'https://raw.githubusercontent.com/Deltares/hatyan/main/hatyan/data/data_foreman_frequencies.txt' #TODO: fix hatyan dependency (MSQM and M1 were also added, but file is not used by hatyan, so might disappear one day)
+    freqs_pd = pd.read_csv(file_freqs,names=['freq','dependents'],delim_whitespace=True,comment='#')
+    freqs_pd['angfreq'] = freqs_pd['freq'] * 360 #deg/hr
+    
+    gridname = ds.grid.name
+    list_fouvars = [i for i in ds.data_vars if '_fourier' in i] #water_quality_output and water_quality_stat
+    
+    rename_dict = {}
+    for fouvar in list_fouvars:
+        fouvar_attrs_lower = {k.lower():v for k,v in ds[fouvar].attrs.items()}
+        fouvar_lowerattrs = ds[fouvar].assign_attrs(fouvar_attrs_lower) #to avoid case issues
+        
+        #quantity
+        long_name = fouvar_lowerattrs.attrs['long_name']
+        long_name_noprefix = long_name.split(': ')[1]
+        quantity_long = long_name_noprefix.split(',')[0]
+        quantity_dict = {'water level':'s1', #dict based on https://svn.oss.deltares.nl/repos/delft3d/trunk/src/engines_gpl/dflowfm/packages/dflowfm_kernel/src/dflowfm_kernel/prepost/fourier_analysis.f90
+                         #'energy head':'s1', #TODO: duplicate namfun/dictvalue is not convenient
+                         'wind speed':'ws',
+                         'U-component of cell-centre velocity':'ux',
+                         'V-component of cell-centre velocity':'uy',
+                         'U-component velocity, column average':'uxa',
+                         'V-component velocity, column average':'uya',
+                         'velocity magnitude':'uc',
+                         #'':'r1', #TODO: unclear which namfun/dictvalue corresponds (trim(namcon(gdfourier%fconno(ifou))))
+                         'velocity':'u1',
+                         'unit discharge':'qx',
+                         'bed stress':'ta',
+                         'freeboard':'fb',
+                         'waterdepth_on_ground':'wdog',
+                         'volume_on_ground':'vog',
+                         'discharge through flow link':'q1',
+                         'water level at flow link':'su1',
+                         'temperature':'tem', #not clear from fourier_analysis.f90, ct in user manual C.13
+                         'salt':'sal', #not clear from fourier_analysis.f90, cs in user manual C.13
+                         }
+        if quantity_long not in quantity_dict.keys():
+            raise KeyError(f'quantity_dict does not yet contain quantity for: {quantity_long}')
+        quantity = quantity_dict[quantity_long]
+        
+        #analysistype
+        istidal = False
+        if hasattr(fouvar_lowerattrs,'frequency_degrees_per_hour'):
+            if fouvar_lowerattrs.attrs['frequency_degrees_per_hour'] > 0: #wl mean with numcyc=0 has frequency attribute (wl min with numcyc=0 does not)
+                istidal = True #for tidal components with frequency >0
+        
+        if istidal: #for tidal analysistype
+            tidepart = fouvar.split('_')[-1] # amp/phs
+            freq = fouvar_lowerattrs.attrs['frequency_degrees_per_hour']
+            compidx_closestfreq = (freqs_pd['angfreq'] - freq).abs().argmin()
+            compname = freqs_pd.index[compidx_closestfreq] #M2/NU2
+            analysistype = tidepart+compname
+            warnings.warn(UserWarning('tidal components found in foufile, matching frequency with online list to get component names, which might go wrong. Also, be aware that v0 and knfac columns from fourier inputfile are not available in fourier output, so it is not clear whether to correct for these.'))
+        else: #for all other quantities
+            fouvar_splitted = fouvar.split('_')
+            analysistype = ''.join(fouvar_splitted[2:]) #min/max/mean. min_depth/max_depth etc are converted to mindepth/maxdepth
+            
+        #tstart/tstop
+        refdate = pd.Timestamp(str(fouvar_lowerattrs.attrs['reference_date_in_yyyymmdd']))
+        if hasattr(fouvar_lowerattrs,'starttime_fourier_analysis_in_minutes_since_reference_date'):
+            tstart_min = fouvar_lowerattrs.attrs['starttime_fourier_analysis_in_minutes_since_reference_date']
+            tstop_min = fouvar_lowerattrs.attrs['stoptime_fourier_analysis_in_minutes_since_reference_date']
+        elif hasattr(fouvar_lowerattrs,'starttime_min_max_analysis_in_minutes_since_reference_date'):
+            tstart_min = fouvar_lowerattrs.attrs['starttime_min_max_analysis_in_minutes_since_reference_date']
+            tstop_min = fouvar_lowerattrs.attrs['stoptime_min_max_analysis_in_minutes_since_reference_date']
+        else:
+            raise AttributeError(f'starttime/stoptime attribute not found in fouvar:\n{fouvar_lowerattrs.attrs}')
+        tstart_str = (refdate + pd.Timedelta(minutes=tstart_min)).strftime('%Y%m%d%H%M%S')
+        tstop_str = (refdate + pd.Timedelta(minutes=tstop_min)).strftime('%Y%m%d%H%M%S')
+        
+        rename_dict[fouvar] = f'{gridname}_{quantity}_{analysistype}_{tstart_str}_{tstop_str}'
+        if istidal and drop_tidal_times:
+            rename_dict[fouvar] = f'{gridname}_{quantity}_{analysistype}' #TODO: might cause conflicting variable names if one component is analysed for multiple periods or if component is not defined in frequency list. Add duplicate check like rename_waqvars() that provides some basic info for debugging.
+    
+    ds = ds.rename(rename_dict)
+    return ds
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/hydrolib_helpers.py` & `dfm_tools-0.11.0/dfm_tools/hydrolib_helpers.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,368 +1,368 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Aug 23 13:36:44 2022
-
-@author: veenstra
-"""
-
-import pandas as pd
-import cftime
-import numpy as np
-import xarray as xr
-from cftime import date2num
-import hydrolib.core.dflowfm as hcdfm
-import warnings
-import datetime as dt
-
-
-def Dataset_to_T3D(datablock_xr):
-    """
-    convert an xarray.DataArray (is one data_var) or an xarray.Dataset (with one or two data_vars) with time and depth dimension to a hydrolib T3D object
-    """
-    
-    if not isinstance(datablock_xr,(xr.DataArray,xr.Dataset)):
-        raise TypeError(f'expected xarray.DataArray or xarray.Dataset, not {type(datablock_xr)}')
-        
-    vector = False
-    if isinstance(datablock_xr,xr.DataArray):
-        data_xr_var0 = datablock_xr
-    elif isinstance(datablock_xr,xr.Dataset):
-        data_vars = list(datablock_xr.data_vars)
-        data_xr_var0 = datablock_xr[data_vars[0]]
-        if len(data_vars)==2:
-            if not pd.Series(data_vars).isin(['ux','uy']).all():
-                raise Exception(f'Dataset with 2 data_vars should contain only ux/uy data_vars, but contains {data_vars}')
-            vector = True
-            data_xr_var1 = datablock_xr[data_vars[1]]
-        elif len(data_vars) > 2:
-            raise ValueError(f'Dataset should contain 1 or 2 data_vars, but contains {len(data_vars)} variables')
-    
-    #ffill/bfill nan data along over depth dimension (corresponds to vertical extrapolation)
-    data_xr_var0 = data_xr_var0.bfill(dim='depth').ffill(dim='depth')
-    if vector:
-        data_xr_var1 = data_xr_var1.bfill(dim='depth').ffill(dim='depth')
-    
-    #TODO: clean up these first lines of code and add description to docstring?
-    locationname = data_xr_var0.attrs['locationname']
-    refdate_str = data_xr_var0.time.encoding['units']
-    
-    if not set(data_xr_var0.dims).issubset(set(('time','depth'))): #check if both time and depth dimensions are present
-        raise ValueError(f"data_var in provided data_xr has dimensions {data_xr_var0.dims} while ('time','depth') is expected")
-    
-    #get depth variable and values
-    depth_array = data_xr_var0['depth'].to_numpy()
-    
-    #get datablock and concatenate with relative time data
-    if vector:
-        data_xr_var0_np = data_xr_var0.to_numpy()
-        data_xr_var1_np = data_xr_var1.to_numpy()
-        datablock_np = np.stack((data_xr_var0_np,data_xr_var1_np),2).reshape(data_xr_var0_np.shape[0],-1) #merge data with alternating rows
-    else:
-        datablock_np = data_xr_var0.to_numpy()
-    
-    timevar_sel_rel = date2num(pd.DatetimeIndex(data_xr_var0.time.to_numpy()).to_pydatetime(),units=refdate_str,calendar='standard')
-    datablock_incltime = np.concatenate([timevar_sel_rel[:,np.newaxis],datablock_np],axis=1)
-    
-    # Each .bc file can contain 1 or more timeseries, in this case one for each support point
-    verticalpositions_idx = np.arange(data_xr_var0['depth'].size)+1
-    if vector: #vector T3D object
-        QUP_quan_list = [hcdfm.QuantityUnitPair(quantity=quan, unit=data_xr_var0.attrs['units'], vertpositionindex=iVP) for iVP in verticalpositions_idx for quan in data_vars]
-        QUP_quan_vector = hcdfm.VectorQuantityUnitPairs(vectorname='uxuyadvectionvelocitybnd', #TODO: vectorname from global attr? (then also support other vectors which is not necessary)
-                                                  elementname=data_vars,
-                                                  quantityunitpair=QUP_quan_list)
-        quantityunitpair = [hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str)]+[QUP_quan_vector]
-    else: #normal T3D object
-        QUP_quan_list = [hcdfm.QuantityUnitPair(quantity=data_xr_var0.name, unit=data_xr_var0.attrs['units'], vertpositionindex=iVP) for iVP in verticalpositions_idx]
-        quantityunitpair=[hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str)]+QUP_quan_list
-    
-    T3D_object = hcdfm.T3D(name=locationname,
-                           #offset=0,
-                           #factor=1,
-                           vertpositions=depth_array.tolist(),
-                           vertinterpolation='linear', #TODO: make these parameters user defined (via attrs)
-                           vertPositionType='ZDatum',
-                           quantityunitpair=quantityunitpair,
-                           timeinterpolation='linear',
-                           datablock=datablock_incltime.tolist(),
-                           )
-    
-    return T3D_object
-
-
-def Dataset_to_TimeSeries(datablock_xr):
-    """
-    convert an xarray.DataArray or xarray.Dataset with time dimension to a hydrolib TimeSeries object
-    """
-    if not isinstance(datablock_xr,(xr.DataArray,xr.Dataset)):
-        raise TypeError(f'Dataset_to_TimeSeries expects xr.DataArray or xr.Dataset, not {type(datablock_xr)}')
-    
-    if isinstance(datablock_xr,xr.Dataset): #convert Dataset to DataArray
-        data_vars = list(datablock_xr.data_vars)
-        if len(data_vars)!=1:
-            raise ValueError('more than one variable supplied in Dataset, not yet possible') #TODO: add support for multiple quantities and for vectors
-        datablock_xr = datablock_xr[data_vars[0]]
-    
-    #TODO: clean up these first lines of code and add description to docstring?
-    locationname = datablock_xr.attrs['locationname']
-    bcvarname = datablock_xr.name
-    refdate_str = datablock_xr.time.encoding['units']
-    
-    if datablock_xr.dims != ('time',):
-        raise ValueError(f"datablock_xr provided to DataArray_to_TimeSeries has dimensions {datablock_xr.dims} while ('time') is expected")
-    
-    #get datablock and concatenate with relative time data
-    datablock_np = datablock_xr.to_numpy()[:,np.newaxis]
-    timevar_sel_rel = date2num(pd.DatetimeIndex(datablock_xr.time.to_numpy()).to_pydatetime(),units=refdate_str,calendar='standard')
-    datablock_incltime = np.concatenate([timevar_sel_rel[:,np.newaxis],datablock_np],axis=1)
-    
-    # Each .bc file can contain 1 or more timeseries, in this case one for each support point
-    TimeSeries_object = hcdfm.TimeSeries(name=locationname,
-                                         quantityunitpair=[hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str),
-                                                           hcdfm.QuantityUnitPair(quantity=bcvarname, unit=datablock_xr.attrs['units'])],
-                                         timeinterpolation='linear', #TODO: make userdefined via attrs?
-                                         datablock=datablock_incltime.tolist(), 
-                                         )
-    return TimeSeries_object
-
-
-def Dataset_to_Astronomic(datablock_xr):
-    """
-    convert an xarray.Dataset (with amplitude and phase data_vars) to a hydrolib Astronomic object
-    
-    """
-    if not isinstance(datablock_xr,xr.Dataset):
-        raise TypeError(f'Dataset_to_Astronomic expects xr.Dataset, not {type(datablock_xr)}')
-    
-    data_vars = list(datablock_xr.data_vars)
-    if 'amplitude' not in data_vars or 'phase_new' not in data_vars:
-        raise KeyError('amplitude and/or phase_new not in input xr.Dataset')
-
-    #TODO: clean up these first lines of code and add description to docstring?
-    locationname = datablock_xr['amplitude'].attrs['locationname']
-        
-    #get datablock and concatenate with component names
-    datablock_np_cna = datablock_xr['compnames'].to_numpy()[:,np.newaxis]
-    datablock_np_amp = datablock_xr['amplitude'].to_numpy()[:,np.newaxis]
-    datablock_np_phs = datablock_xr['phase_new'].to_numpy()[:,np.newaxis]
-    datablock_inclcomp = np.concatenate([datablock_np_cna,datablock_np_amp,datablock_np_phs],axis=1)
-    
-    Astronomic_object = hcdfm.Astronomic(name=locationname,
-                                         quantityunitpair=[hcdfm.QuantityUnitPair(quantity="astronomic component", unit='-'),
-                                                           hcdfm.QuantityUnitPair(quantity='waterlevelbnd amplitude', unit=datablock_xr['amplitude'].attrs['units']),
-                                                           hcdfm.QuantityUnitPair(quantity='waterlevelbnd phase', unit=datablock_xr['phase'].attrs['units'])],
-                                         datablock=datablock_inclcomp.tolist(), 
-                                         )
-    return Astronomic_object
-
-
-def DataFrame_to_PolyObject(poly_pd,name,content=None):
-    """
-    convert a pandas dataframe with x/y columns (and optional others like z/data/comment) to a hydrolib PolyObject
-    """
-    if 'z' in poly_pd.columns:
-        nondata_cols = ['x','y','z']
-    else:
-        nondata_cols = ['x','y']
-    poly_pd_xy = poly_pd[nondata_cols]
-    poly_pd_data = pd.DataFrame({'data':poly_pd.drop(nondata_cols,axis=1).values.tolist()})
-    poly_pd_polyobj = pd.concat([poly_pd_xy,poly_pd_data],axis=1)
-    pointsobj_list = poly_pd_polyobj.T.apply(dict).tolist() #TODO: maybe faster with list iteration
-    polyobject = hcdfm.PolyObject(metadata={'name':name,'n_rows':poly_pd.shape[0],'n_columns':poly_pd.shape[1]}, points=pointsobj_list)
-    if content is not None:
-        polyobject.description = {'content':content}
-    return polyobject
-
-
-def DataFrame_to_TimModel(tim_pd, refdate:(dt.datetime, pd.Timestamp, str)):
-    """
-    converts data from tim_pd to TimModel and puts all headers as comments. Ignores the index, assumes first column is time in minutes since a refdate.
-    """
-    #TODO: add conversion from datetimes in index to minutes, maybe drop minutes column upon reading? First await https://github.com/Deltares/HYDROLIB-core/issues/511
-    
-    refdate_pd = pd.Timestamp(refdate)
-    
-    data_tim = tim_pd.values.tolist()
-    times_tim = ((tim_pd.index - refdate_pd).total_seconds()/60).tolist()
-    dict_tim = [hcdfm.TimRecord(time=t,data=d) for t,d in zip(times_tim,data_tim)]
-    
-    comments_datacols = tim_pd.columns.tolist()
-    comments = [tim_pd.index.name] + comments_datacols
-    for iC, comment in enumerate(comments):
-        comments[iC] = f'COLUMN {iC+1}: {comment}'
-    timmodel = hcdfm.TimModel(timeseries=dict_tim, comments=comments)
-    
-    return timmodel
-
-
-def forcinglike_to_Dataset(forcingobj, convertnan=False): #TODO: would be convenient to have this as a method of ForcingModel objects (Timeseries/T3D/etc): https://github.com/Deltares/HYDROLIB-core/issues/307
-    """
-    convert a hydrolib forcing like object (like Timeseries, T3D, Harmonic, etc) to an xarray Dataset with one or more variables.
-    
-    convertnan: convert depths with the same values over time as the deepest layer to nan (these were created with .bfill() or .ffill()).
-    """
-    
-    #check if forcingmodel instead of T3D/TimeSeries is provided
-    if isinstance(forcingobj, hcdfm.ForcingModel):
-        raise TypeError('instead of supplying a ForcingModel, provide a ForcingObject (Timeseries/T3D etc), by doing something like ForcingModel.forcing[0]')
-    
-    allowed_instances = (hcdfm.T3D, hcdfm.TimeSeries, hcdfm.Astronomic)
-    if not isinstance(forcingobj, allowed_instances):
-        raise TypeError(f'supplied input is not one of: {allowed_instances}')
-    
-    if isinstance(forcingobj, hcdfm.Astronomic):
-        var_quantity_list = [x.quantity for x in forcingobj.quantityunitpair[1:]]
-        var_unit = [x.unit for x in forcingobj.quantityunitpair[1:]]
-    elif hasattr(forcingobj.quantityunitpair[1],'elementname'): #T3D with vector quantity
-        var_quantity_list = forcingobj.quantityunitpair[1].elementname
-        var_unit_one = forcingobj.quantityunitpair[1].quantityunitpair[0].unit
-        var_unit = [var_unit_one,var_unit_one]
-    else: #non-vector TimeSeries or T3D
-        var_quantity_list = [forcingobj.quantityunitpair[1].quantity]
-        var_unit = [forcingobj.quantityunitpair[1].unit]
-    nquan = len(var_quantity_list)
-    
-    if isinstance(forcingobj, hcdfm.T3D):
-        dims = ('time','depth')
-    elif isinstance(forcingobj, hcdfm.TimeSeries):
-        dims = ('time')
-    elif isinstance(forcingobj, hcdfm.Astronomic):
-        dims = ('astronomic_component')
-    
-    datablock_all = np.array(forcingobj.datablock)
-    datablock_data = datablock_all[:,1:] #select all columns except first one (which is the time column)
-    if isinstance(forcingobj, hcdfm.Astronomic):
-        datablock_data = datablock_data.astype(float) #convert str to float in case of "astronomic component"
-    
-    data_xr = xr.Dataset()
-    for iQ, var_quantity in enumerate(var_quantity_list):
-        datablock_data_onequan = datablock_data[:,iQ::nquan]
-        datablock_data_onequan = datablock_data_onequan.squeeze() #drop dimensions of len 1 in case of 1 dimension, eg "waterlevelbnd" (first subsetting over depth dimension)
-        
-        data_xr_var = xr.DataArray(datablock_data_onequan, name=var_quantity, dims=dims)
-        if 'depth' in dims:
-            data_xr_var['depth'] = forcingobj.vertpositions
-            #data_xr_var['depth'].attrs['positive'] == 'up' #TODO: maybe add this attribute
-            if convertnan: #convert ffilled/bfilled values back to nan
-                deepestlayeridx = data_xr_var.depth.to_numpy().argmin()
-                if deepestlayeridx==0: #sorted from deep to shallow layers
-                    bool_nandepths = (data_xr_var==data_xr_var.shift(depth=-1)).all(dim='time')
-                else: #sorted from shallow to deep layers
-                    bool_nandepths = (data_xr_var==data_xr_var.shift(depth=1)).all(dim='time')
-                data_xr_var = data_xr_var.where(~bool_nandepths)
-        if 'time' in dims:
-            time_unit = forcingobj.quantityunitpair[0].unit.lower()
-            data_xr_var['time'] = cftime.num2pydate(datablock_all[:,0], units=time_unit)
-            data_xr_var['time'].encoding['units'] = time_unit #check tz conversion if eg '+01:00' is present in time_unit
-            data_xr_var['time'].encoding['calendar'] = 'standard'
-        if 'astronomic_component' in dims:
-            data_xr_var['astronomic_component'] = datablock_all[:,0]
-        
-        #add attributes
-        data_xr_var.attrs['source'] = 'hydrolib-core object converted to xarray.Dataset with dfm_tools.xarray_helpers.forcinglike_to_Dataset()'
-        data_xr_var.attrs['locationname'] = forcingobj.name
-        data_xr_var.attrs['units'] = var_unit[iQ]
-        forcingobj_keys = forcingobj.__dict__.keys()
-        for key in forcingobj_keys: #['comments','name','function','offset','factor','vertinterpolation','vertpositiontype','timeinterpolation']: 
-            if key in ['datablock','quantityunitpair','vertpositions']: #skipping these since they are in the DataArray already
-                continue
-            data_xr_var.attrs[key] = str(forcingobj.__dict__[key])
-        
-        #add DataArray to Dataset
-        data_xr[var_quantity] = data_xr_var
-    
-    return data_xr
-
-
-def pointlike_to_DataFrame(pointlike,drop_emptycols=True):
-    """
-    convert a hydrolib object with points (like PolyObject, XYZModel and possibly others) to a pandas DataFrame.
-
-    Parameters
-    ----------
-    pointlike : TYPE
-        Hydrolib-core object with point objects.
-
-    Returns
-    -------
-    pointlike_pd : TYPE
-        DESCRIPTION.
-    drop_emptycols : bool, optional
-        Drop empty (all-nan) columns automatically, like the z-column in ldb file. The default is True.
-    
-    Example:
-        polyfile_object = PolyFile(file_pli)
-        data_pol_pd_list = [pointlike_to_DataFrame(polyobj) for polyobj in polyfile_object.objects]
-
-    """
-    
-    pointlike_pd = pd.DataFrame([dict(p) for p in pointlike.points])
-    if 'data' in pointlike_pd.columns:
-        datavals_pd = pd.DataFrame([p.data for p in pointlike.points])
-        pointlike_pd = pd.concat([pointlike_pd.drop(['data'],axis=1), datavals_pd],axis=1)
-        
-    if drop_emptycols:
-        pointlike_pd = pointlike_pd.dropna(axis=1).copy()
-        
-    return pointlike_pd
-
-
-def parse_xy_to_datetime(pointlike_pd):
-    datatimevals_pdstr = (pointlike_pd['x'].astype(int).apply(lambda x:f'{x:08d}') +
-                          pointlike_pd['y'].astype(int).apply(lambda x:f'{x:06d}'))
-    pointlike_pd.index = pd.to_datetime(datatimevals_pdstr)
-    pointlike_pd_timeidx = pointlike_pd.drop(['x','y'],axis=1)
-    
-    return pointlike_pd_timeidx
-
-
-def TimModel_to_DataFrame(data_tim:hcdfm.TimModel, parse_column_labels:bool = True, refdate:(dt.datetime, pd.Timestamp, str) = None):
-    """
-    
-
-    Parameters
-    ----------
-    data_tim : hcdfm.TimModel
-        DESCRIPTION.
-    parse_column_labels : bool, optional
-        Parse column labels from comments. This might fail since there is no standard way of prescribing the columns in the comments. The default is True.
-    refdate : (dt.datetime, pd.Timestamp, str, int, float), optional
-        DESCRIPTION. The default is None.
-
-    Returns
-    -------
-    tim_pd : TYPE
-        DESCRIPTION.
-
-    """
-    #convert to pandas dataframe
-    timevals_pd = pd.Index([p.time for p in data_tim.timeseries])
-    tim_pd = pd.DataFrame([p.data for p in data_tim.timeseries],index=timevals_pd)
-    tim_pd.columns += 2 #make column numbers 1-based, but first column is already in index so start with 2
-    tim_pd.index.name = 'time in minutes'
-    
-    if parse_column_labels:
-        #replace column labels with the ones in comments
-        tim_pd_columns = tim_pd.columns.tolist()
-        for line in data_tim.comments:
-            if 'column' in line.lower() and ':' in line: #assume ":" is separator. Remove casing to be able to check for Column/COLUMN/column in string
-                sep = ':'
-            elif 'column' in line.lower() and '=' in line: #assume "=" is separator. Remove casing to be able to check for Column/COLUMN/column in string
-                sep = '='
-            else:
-                continue
-            line_split = line.split(sep)
-            colnum = line_split[0].lower().replace('column','').strip()
-            if colnum.isnumeric():
-                comment_str = ':'.join(line_split[1:]).strip()
-                if colnum==1: #time column is now in index, overwrite index name
-                    tim_pd.index.name = comment_str
-                else:
-                    tim_pd_columns[int(colnum)-2] = comment_str
-        tim_pd.columns = tim_pd_columns
-    
-    if refdate:
-        refdate_pd = pd.Timestamp(refdate)
-        tim_pd.index = refdate_pd + pd.to_timedelta(tim_pd.index,unit='minutes')
-    
-    return tim_pd
-
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Aug 23 13:36:44 2022
+
+@author: veenstra
+"""
+
+import pandas as pd
+import cftime
+import numpy as np
+import xarray as xr
+from cftime import date2num
+import hydrolib.core.dflowfm as hcdfm
+import warnings
+import datetime as dt
+
+
+def Dataset_to_T3D(datablock_xr):
+    """
+    convert an xarray.DataArray (is one data_var) or an xarray.Dataset (with one or two data_vars) with time and depth dimension to a hydrolib T3D object
+    """
+    
+    if not isinstance(datablock_xr,(xr.DataArray,xr.Dataset)):
+        raise TypeError(f'expected xarray.DataArray or xarray.Dataset, not {type(datablock_xr)}')
+        
+    vector = False
+    if isinstance(datablock_xr,xr.DataArray):
+        data_xr_var0 = datablock_xr
+    elif isinstance(datablock_xr,xr.Dataset):
+        data_vars = list(datablock_xr.data_vars)
+        data_xr_var0 = datablock_xr[data_vars[0]]
+        if len(data_vars)==2:
+            if not pd.Series(data_vars).isin(['ux','uy']).all():
+                raise Exception(f'Dataset with 2 data_vars should contain only ux/uy data_vars, but contains {data_vars}')
+            vector = True
+            data_xr_var1 = datablock_xr[data_vars[1]]
+        elif len(data_vars) > 2:
+            raise ValueError(f'Dataset should contain 1 or 2 data_vars, but contains {len(data_vars)} variables')
+    
+    #ffill/bfill nan data along over depth dimension (corresponds to vertical extrapolation)
+    data_xr_var0 = data_xr_var0.bfill(dim='depth').ffill(dim='depth')
+    if vector:
+        data_xr_var1 = data_xr_var1.bfill(dim='depth').ffill(dim='depth')
+    
+    #TODO: clean up these first lines of code and add description to docstring?
+    locationname = data_xr_var0.attrs['locationname']
+    refdate_str = data_xr_var0.time.encoding['units']
+    
+    if not set(data_xr_var0.dims).issubset(set(('time','depth'))): #check if both time and depth dimensions are present
+        raise ValueError(f"data_var in provided data_xr has dimensions {data_xr_var0.dims} while ('time','depth') is expected")
+    
+    #get depth variable and values
+    depth_array = data_xr_var0['depth'].to_numpy()
+    
+    #get datablock and concatenate with relative time data
+    if vector:
+        data_xr_var0_np = data_xr_var0.to_numpy()
+        data_xr_var1_np = data_xr_var1.to_numpy()
+        datablock_np = np.stack((data_xr_var0_np,data_xr_var1_np),2).reshape(data_xr_var0_np.shape[0],-1) #merge data with alternating rows
+    else:
+        datablock_np = data_xr_var0.to_numpy()
+    
+    timevar_sel_rel = date2num(pd.DatetimeIndex(data_xr_var0.time.to_numpy()).to_pydatetime(),units=refdate_str,calendar='standard')
+    datablock_incltime = np.concatenate([timevar_sel_rel[:,np.newaxis],datablock_np],axis=1)
+    
+    # Each .bc file can contain 1 or more timeseries, in this case one for each support point
+    verticalpositions_idx = np.arange(data_xr_var0['depth'].size)+1
+    if vector: #vector T3D object
+        QUP_quan_list = [hcdfm.QuantityUnitPair(quantity=quan, unit=data_xr_var0.attrs['units'], vertpositionindex=iVP) for iVP in verticalpositions_idx for quan in data_vars]
+        QUP_quan_vector = hcdfm.VectorQuantityUnitPairs(vectorname='uxuyadvectionvelocitybnd', #TODO: vectorname from global attr? (then also support other vectors which is not necessary)
+                                                  elementname=data_vars,
+                                                  quantityunitpair=QUP_quan_list)
+        quantityunitpair = [hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str)]+[QUP_quan_vector]
+    else: #normal T3D object
+        QUP_quan_list = [hcdfm.QuantityUnitPair(quantity=data_xr_var0.name, unit=data_xr_var0.attrs['units'], vertpositionindex=iVP) for iVP in verticalpositions_idx]
+        quantityunitpair=[hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str)]+QUP_quan_list
+    
+    T3D_object = hcdfm.T3D(name=locationname,
+                           #offset=0,
+                           #factor=1,
+                           vertpositions=depth_array.tolist(),
+                           vertinterpolation='linear', #TODO: make these parameters user defined (via attrs)
+                           vertPositionType='ZDatum',
+                           quantityunitpair=quantityunitpair,
+                           timeinterpolation='linear',
+                           datablock=datablock_incltime.tolist(),
+                           )
+    
+    return T3D_object
+
+
+def Dataset_to_TimeSeries(datablock_xr):
+    """
+    convert an xarray.DataArray or xarray.Dataset with time dimension to a hydrolib TimeSeries object
+    """
+    if not isinstance(datablock_xr,(xr.DataArray,xr.Dataset)):
+        raise TypeError(f'Dataset_to_TimeSeries expects xr.DataArray or xr.Dataset, not {type(datablock_xr)}')
+    
+    if isinstance(datablock_xr,xr.Dataset): #convert Dataset to DataArray
+        data_vars = list(datablock_xr.data_vars)
+        if len(data_vars)!=1:
+            raise ValueError('more than one variable supplied in Dataset, not yet possible') #TODO: add support for multiple quantities and for vectors
+        datablock_xr = datablock_xr[data_vars[0]]
+    
+    #TODO: clean up these first lines of code and add description to docstring?
+    locationname = datablock_xr.attrs['locationname']
+    bcvarname = datablock_xr.name
+    refdate_str = datablock_xr.time.encoding['units']
+    
+    if datablock_xr.dims != ('time',):
+        raise ValueError(f"datablock_xr provided to DataArray_to_TimeSeries has dimensions {datablock_xr.dims} while ('time') is expected")
+    
+    #get datablock and concatenate with relative time data
+    datablock_np = datablock_xr.to_numpy()[:,np.newaxis]
+    timevar_sel_rel = date2num(pd.DatetimeIndex(datablock_xr.time.to_numpy()).to_pydatetime(),units=refdate_str,calendar='standard')
+    datablock_incltime = np.concatenate([timevar_sel_rel[:,np.newaxis],datablock_np],axis=1)
+    
+    # Each .bc file can contain 1 or more timeseries, in this case one for each support point
+    TimeSeries_object = hcdfm.TimeSeries(name=locationname,
+                                         quantityunitpair=[hcdfm.QuantityUnitPair(quantity="time", unit=refdate_str),
+                                                           hcdfm.QuantityUnitPair(quantity=bcvarname, unit=datablock_xr.attrs['units'])],
+                                         timeinterpolation='linear', #TODO: make userdefined via attrs?
+                                         datablock=datablock_incltime.tolist(), 
+                                         )
+    return TimeSeries_object
+
+
+def Dataset_to_Astronomic(datablock_xr):
+    """
+    convert an xarray.Dataset (with amplitude and phase data_vars) to a hydrolib Astronomic object
+    
+    """
+    if not isinstance(datablock_xr,xr.Dataset):
+        raise TypeError(f'Dataset_to_Astronomic expects xr.Dataset, not {type(datablock_xr)}')
+    
+    data_vars = list(datablock_xr.data_vars)
+    if 'amplitude' not in data_vars or 'phase_new' not in data_vars:
+        raise KeyError('amplitude and/or phase_new not in input xr.Dataset')
+
+    #TODO: clean up these first lines of code and add description to docstring?
+    locationname = datablock_xr['amplitude'].attrs['locationname']
+        
+    #get datablock and concatenate with component names
+    datablock_np_cna = datablock_xr['compnames'].to_numpy()[:,np.newaxis]
+    datablock_np_amp = datablock_xr['amplitude'].to_numpy()[:,np.newaxis]
+    datablock_np_phs = datablock_xr['phase_new'].to_numpy()[:,np.newaxis]
+    datablock_inclcomp = np.concatenate([datablock_np_cna,datablock_np_amp,datablock_np_phs],axis=1)
+    
+    Astronomic_object = hcdfm.Astronomic(name=locationname,
+                                         quantityunitpair=[hcdfm.QuantityUnitPair(quantity="astronomic component", unit='-'),
+                                                           hcdfm.QuantityUnitPair(quantity='waterlevelbnd amplitude', unit=datablock_xr['amplitude'].attrs['units']),
+                                                           hcdfm.QuantityUnitPair(quantity='waterlevelbnd phase', unit=datablock_xr['phase'].attrs['units'])],
+                                         datablock=datablock_inclcomp.tolist(), 
+                                         )
+    return Astronomic_object
+
+
+def DataFrame_to_PolyObject(poly_pd,name,content=None):
+    """
+    convert a pandas dataframe with x/y columns (and optional others like z/data/comment) to a hydrolib PolyObject
+    """
+    if 'z' in poly_pd.columns:
+        nondata_cols = ['x','y','z']
+    else:
+        nondata_cols = ['x','y']
+    poly_pd_xy = poly_pd[nondata_cols]
+    poly_pd_data = pd.DataFrame({'data':poly_pd.drop(nondata_cols,axis=1).values.tolist()})
+    poly_pd_polyobj = pd.concat([poly_pd_xy,poly_pd_data],axis=1)
+    pointsobj_list = poly_pd_polyobj.T.apply(dict).tolist() #TODO: maybe faster with list iteration
+    polyobject = hcdfm.PolyObject(metadata={'name':name,'n_rows':poly_pd.shape[0],'n_columns':poly_pd.shape[1]}, points=pointsobj_list)
+    if content is not None:
+        polyobject.description = {'content':content}
+    return polyobject
+
+
+def DataFrame_to_TimModel(tim_pd, refdate:(dt.datetime, pd.Timestamp, str)):
+    """
+    converts data from tim_pd to TimModel and puts all headers as comments. Ignores the index, assumes first column is time in minutes since a refdate.
+    """
+    #TODO: add conversion from datetimes in index to minutes, maybe drop minutes column upon reading? First await https://github.com/Deltares/HYDROLIB-core/issues/511
+    
+    refdate_pd = pd.Timestamp(refdate)
+    
+    data_tim = tim_pd.values.tolist()
+    times_tim = ((tim_pd.index - refdate_pd).total_seconds()/60).tolist()
+    dict_tim = [hcdfm.TimRecord(time=t,data=d) for t,d in zip(times_tim,data_tim)]
+    
+    comments_datacols = tim_pd.columns.tolist()
+    comments = [tim_pd.index.name] + comments_datacols
+    for iC, comment in enumerate(comments):
+        comments[iC] = f'COLUMN {iC+1}: {comment}'
+    timmodel = hcdfm.TimModel(timeseries=dict_tim, comments=comments)
+    
+    return timmodel
+
+
+def forcinglike_to_Dataset(forcingobj, convertnan=False): #TODO: would be convenient to have this as a method of ForcingModel objects (Timeseries/T3D/etc): https://github.com/Deltares/HYDROLIB-core/issues/307
+    """
+    convert a hydrolib forcing like object (like Timeseries, T3D, Harmonic, etc) to an xarray Dataset with one or more variables.
+    
+    convertnan: convert depths with the same values over time as the deepest layer to nan (these were created with .bfill() or .ffill()).
+    """
+    
+    #check if forcingmodel instead of T3D/TimeSeries is provided
+    if isinstance(forcingobj, hcdfm.ForcingModel):
+        raise TypeError('instead of supplying a ForcingModel, provide a ForcingObject (Timeseries/T3D etc), by doing something like ForcingModel.forcing[0]')
+    
+    allowed_instances = (hcdfm.T3D, hcdfm.TimeSeries, hcdfm.Astronomic)
+    if not isinstance(forcingobj, allowed_instances):
+        raise TypeError(f'supplied input is not one of: {allowed_instances}')
+    
+    if isinstance(forcingobj, hcdfm.Astronomic):
+        var_quantity_list = [x.quantity for x in forcingobj.quantityunitpair[1:]]
+        var_unit = [x.unit for x in forcingobj.quantityunitpair[1:]]
+    elif hasattr(forcingobj.quantityunitpair[1],'elementname'): #T3D with vector quantity
+        var_quantity_list = forcingobj.quantityunitpair[1].elementname
+        var_unit_one = forcingobj.quantityunitpair[1].quantityunitpair[0].unit
+        var_unit = [var_unit_one,var_unit_one]
+    else: #non-vector TimeSeries or T3D
+        var_quantity_list = [forcingobj.quantityunitpair[1].quantity]
+        var_unit = [forcingobj.quantityunitpair[1].unit]
+    nquan = len(var_quantity_list)
+    
+    if isinstance(forcingobj, hcdfm.T3D):
+        dims = ('time','depth')
+    elif isinstance(forcingobj, hcdfm.TimeSeries):
+        dims = ('time')
+    elif isinstance(forcingobj, hcdfm.Astronomic):
+        dims = ('astronomic_component')
+    
+    datablock_all = np.array(forcingobj.datablock)
+    datablock_data = datablock_all[:,1:] #select all columns except first one (which is the time column)
+    if isinstance(forcingobj, hcdfm.Astronomic):
+        datablock_data = datablock_data.astype(float) #convert str to float in case of "astronomic component"
+    
+    data_xr = xr.Dataset()
+    for iQ, var_quantity in enumerate(var_quantity_list):
+        datablock_data_onequan = datablock_data[:,iQ::nquan]
+        datablock_data_onequan = datablock_data_onequan.squeeze() #drop dimensions of len 1 in case of 1 dimension, eg "waterlevelbnd" (first subsetting over depth dimension)
+        
+        data_xr_var = xr.DataArray(datablock_data_onequan, name=var_quantity, dims=dims)
+        if 'depth' in dims:
+            data_xr_var['depth'] = forcingobj.vertpositions
+            #data_xr_var['depth'].attrs['positive'] == 'up' #TODO: maybe add this attribute
+            if convertnan: #convert ffilled/bfilled values back to nan
+                deepestlayeridx = data_xr_var.depth.to_numpy().argmin()
+                if deepestlayeridx==0: #sorted from deep to shallow layers
+                    bool_nandepths = (data_xr_var==data_xr_var.shift(depth=-1)).all(dim='time')
+                else: #sorted from shallow to deep layers
+                    bool_nandepths = (data_xr_var==data_xr_var.shift(depth=1)).all(dim='time')
+                data_xr_var = data_xr_var.where(~bool_nandepths)
+        if 'time' in dims:
+            time_unit = forcingobj.quantityunitpair[0].unit.lower()
+            data_xr_var['time'] = cftime.num2pydate(datablock_all[:,0], units=time_unit)
+            data_xr_var['time'].encoding['units'] = time_unit #check tz conversion if eg '+01:00' is present in time_unit
+            data_xr_var['time'].encoding['calendar'] = 'standard'
+        if 'astronomic_component' in dims:
+            data_xr_var['astronomic_component'] = datablock_all[:,0]
+        
+        #add attributes
+        data_xr_var.attrs['source'] = 'hydrolib-core object converted to xarray.Dataset with dfm_tools.xarray_helpers.forcinglike_to_Dataset()'
+        data_xr_var.attrs['locationname'] = forcingobj.name
+        data_xr_var.attrs['units'] = var_unit[iQ]
+        forcingobj_keys = forcingobj.__dict__.keys()
+        for key in forcingobj_keys: #['comments','name','function','offset','factor','vertinterpolation','vertpositiontype','timeinterpolation']: 
+            if key in ['datablock','quantityunitpair','vertpositions']: #skipping these since they are in the DataArray already
+                continue
+            data_xr_var.attrs[key] = str(forcingobj.__dict__[key])
+        
+        #add DataArray to Dataset
+        data_xr[var_quantity] = data_xr_var
+    
+    return data_xr
+
+
+def pointlike_to_DataFrame(pointlike,drop_emptycols=True):
+    """
+    convert a hydrolib object with points (like PolyObject, XYZModel and possibly others) to a pandas DataFrame.
+
+    Parameters
+    ----------
+    pointlike : TYPE
+        Hydrolib-core object with point objects.
+
+    Returns
+    -------
+    pointlike_pd : TYPE
+        DESCRIPTION.
+    drop_emptycols : bool, optional
+        Drop empty (all-nan) columns automatically, like the z-column in ldb file. The default is True.
+    
+    Example:
+        polyfile_object = PolyFile(file_pli)
+        data_pol_pd_list = [pointlike_to_DataFrame(polyobj) for polyobj in polyfile_object.objects]
+
+    """
+    
+    pointlike_pd = pd.DataFrame([dict(p) for p in pointlike.points])
+    if 'data' in pointlike_pd.columns:
+        datavals_pd = pd.DataFrame([p.data for p in pointlike.points])
+        pointlike_pd = pd.concat([pointlike_pd.drop(['data'],axis=1), datavals_pd],axis=1)
+        
+    if drop_emptycols:
+        pointlike_pd = pointlike_pd.dropna(axis=1).copy()
+        
+    return pointlike_pd
+
+
+def parse_xy_to_datetime(pointlike_pd):
+    datatimevals_pdstr = (pointlike_pd['x'].astype(int).apply(lambda x:f'{x:08d}') +
+                          pointlike_pd['y'].astype(int).apply(lambda x:f'{x:06d}'))
+    pointlike_pd.index = pd.to_datetime(datatimevals_pdstr)
+    pointlike_pd_timeidx = pointlike_pd.drop(['x','y'],axis=1)
+    
+    return pointlike_pd_timeidx
+
+
+def TimModel_to_DataFrame(data_tim:hcdfm.TimModel, parse_column_labels:bool = True, refdate:(dt.datetime, pd.Timestamp, str) = None):
+    """
+    
+
+    Parameters
+    ----------
+    data_tim : hcdfm.TimModel
+        DESCRIPTION.
+    parse_column_labels : bool, optional
+        Parse column labels from comments. This might fail since there is no standard way of prescribing the columns in the comments. The default is True.
+    refdate : (dt.datetime, pd.Timestamp, str, int, float), optional
+        DESCRIPTION. The default is None.
+
+    Returns
+    -------
+    tim_pd : TYPE
+        DESCRIPTION.
+
+    """
+    #convert to pandas dataframe
+    timevals_pd = pd.Index([p.time for p in data_tim.timeseries])
+    tim_pd = pd.DataFrame([p.data for p in data_tim.timeseries],index=timevals_pd)
+    tim_pd.columns += 2 #make column numbers 1-based, but first column is already in index so start with 2
+    tim_pd.index.name = 'time in minutes'
+    
+    if parse_column_labels:
+        #replace column labels with the ones in comments
+        tim_pd_columns = tim_pd.columns.tolist()
+        for line in data_tim.comments:
+            if 'column' in line.lower() and ':' in line: #assume ":" is separator. Remove casing to be able to check for Column/COLUMN/column in string
+                sep = ':'
+            elif 'column' in line.lower() and '=' in line: #assume "=" is separator. Remove casing to be able to check for Column/COLUMN/column in string
+                sep = '='
+            else:
+                continue
+            line_split = line.split(sep)
+            colnum = line_split[0].lower().replace('column','').strip()
+            if colnum.isnumeric():
+                comment_str = ':'.join(line_split[1:]).strip()
+                if colnum==1: #time column is now in index, overwrite index name
+                    tim_pd.index.name = comment_str
+                else:
+                    tim_pd_columns[int(colnum)-2] = comment_str
+        tim_pd.columns = tim_pd_columns
+    
+    if refdate:
+        refdate_pd = pd.Timestamp(refdate)
+        tim_pd.index = refdate_pd + pd.to_timedelta(tim_pd.index,unit='minutes')
+    
+    return tim_pd
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/interpolate_grid2bnd.py` & `dfm_tools-0.11.0/dfm_tools/interpolate_grid2bnd.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,469 +1,469 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Aug 18 17:39:03 2022
-
-@author: veenstra
-
-"""
-
-import os
-import glob
-import datetime as dt
-import numpy as np
-import pandas as pd
-import xarray as xr
-from pathlib import Path
-from scipy.spatial import KDTree
-import warnings
-import hydrolib.core.dflowfm as hcdfm
-
-from dfm_tools.hydrolib_helpers import Dataset_to_TimeSeries, Dataset_to_T3D, Dataset_to_Astronomic, pointlike_to_DataFrame
-from dfm_tools.errors import OutOfRangeError
-
-
-def get_conversion_dict(ncvarname_updates={}):
-    
-    """
-    get the conversion_dict, optionally with updated ncvarnames
-    conversion_dict.keys() are the dflowfm quantities and the ncvarname the corresponding netcdf variable name/key
-    alternative ncvarnames can be supplied via ncvarname_updates, e.g. get_conversion_dict(ncvarname_updates={'temperaturebnd':'tos'})
-    
-    interpolate_nc_to_bc() renames netcdf variable like this:
-    data_xr = data_xr.rename({ncvarname:quantity})
-    
-    for CMCC:
-    conversion_dict = { # mg/l is the same as g/m3: conversion is phyc in mol/m3 to newvar in g/m3
-                       'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 },
-                       'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 },
-                       'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 },
-                       'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08},
-                       'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0}, # Caution: this empirical relation might not be applicable to your use case
-                       'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 30.97}, # Caution: this empirical relation might not be applicable to your use case
-                       'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0 * (106 / 16)}, # Caution: this empirical relation might not be applicable to your use case
-                       'salinitybnd'         : {'ncvarname': 'sos'},         #'1e-3'
-                       'temperaturebnd'      : {'ncvarname': 'tos'},         #'degC'
-                       'ux'                  : {'ncvarname': 'uo'},          #'m/s'
-                       'uy'                  : {'ncvarname': 'vo'},          #'m/s'
-                       'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
-                       'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
-                       }
-    """
-    # conversion_dict, 
-    conversion_dict = { # mg/l is the same as g/m3: conversion is phyc in mmol/l to newvar in g/m3
-                        'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 / 1000.0}, 
-                        'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 / 1000.0},
-                        'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 / 1000.0},
-                        'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08 / 1000.0},
-                        'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 16. * 14. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 30.97 / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 12. / 1000.0}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndDON'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 3.24 * 2. * 16. * 14. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndDOP'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 1.0 * 2. * 30.97 / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndDOC'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': (199. / 20.) * 3.24 * 2. * 16. * 12. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'tracerbndOpal'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 0.5 * 0.13 * 28.08 / (1000.0)}, # Caution: this empirical relation might not be applicable to your use case
-                        'salinitybnd'         : {'ncvarname': 'so'},          #'1e-3'
-                        'temperaturebnd'      : {'ncvarname': 'thetao'},      #'degC'
-                        'ux'                  : {'ncvarname': 'uo'},          #'m/s'
-                        'uy'                  : {'ncvarname': 'vo'},          #'m/s'
-                        'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
-                        'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
-                        }
-    #do updates
-    for k,v in ncvarname_updates.items():
-        conversion_dict[k]['ncvarname'] = v
-    return conversion_dict
-
-
-def interpolate_tide_to_bc(tidemodel, file_pli, component_list=None, nPoints=None):
-    """
-    """
-    # translate dict from .\hydro_tools\FES\PreProcessing_FES_TideModel_imaginary.m
-    #component_list = ['2N2','LABDA2','MF','MFM','P1','SSA','EPSILON2','M2','MKS2','MU2','Q1','T2','J1','M3','MM','N2','R2','K1','M4','MN4','N4','S1','K2','M6','MS4','NU2','S2','L2','M8','MSF','O1','S4','MSQM','SA']
-    translate_dict = {'LA2':'LABDA2', #TODO: use value instead of key in bc file? Support using value instead of key in const_list also (like line above)
-                      'EPS2':'EPSILON2', 
-                      'Z0':'A0',
-                      'MTM':'MFM', #Needs to be verified
-                      }
-    
-    dir_pattern_dict = {'FES2014': Path(r'P:\metocean-data\licensed\FES2014','*.nc'), #ocean_tide_extrapolated
-                        'FES2012': Path(r'P:\metocean-data\open\FES2012\data','*_FES2012_SLEV.nc'), #is eigenlijk ook licensed
-                        'EOT20': Path(r'P:\metocean-data\open\EOT20\ocean_tides','*_ocean_eot20.nc'),
-                        'GTSM4.1preliminary': Path(r'p:\1230882-emodnet_hrsm\GTSMv3.0EMODnet\EMOD_MichaelTUM_yearcomponents\GTSMv4.1_yeartide_2014_2.20.06\compare_fouhis_fouxyz_v3','gtsmv4.1_2014_*_withfu_v3_rasterized.nc'),
-                        #TODO: add tpxo8 (tpxo9 is also available), catalog: https://opendap.deltares.nl/thredds/catalog/opendap/deltares/delftdashboard/tidemodels/tpxo80/catalog.html
-                        }
-    if tidemodel not in dir_pattern_dict.keys():
-        raise KeyError(f'invalid tidemodel "{tidemodel}", options are: {list(dir_pattern_dict.keys())}')
-    if tidemodel == 'GTSM4.1preliminary':
-        warnings.warn(UserWarning(f'you are using tidemodel "{tidemodel}", beware that the dataset is preliminary so it is still quite coarse and may contain errors. Check your results carefully'))
-    dir_pattern = dir_pattern_dict[tidemodel]
-    
-    if component_list is None:
-        file_list_nc = glob.glob(str(dir_pattern))
-        dir_pattern_basename = os.path.basename(dir_pattern)
-        replace = dir_pattern_basename.split('*')
-        component_list = [os.path.basename(x).replace(replace[0],'').replace(replace[1],'') for x in file_list_nc] #TODO: make this less hard-coded
-    component_list_upper_pd = pd.Series([x.upper() for x in component_list]).replace(translate_dict, regex=True)
-    
-    def extract_component(ds):
-        #https://github.com/pydata/xarray/issues/1380
-        if 'FES2012' in ds.encoding["source"]: #TODO: make more generic with regex, or just add tidemodel argument since they are quite specific
-            compname = os.path.basename(ds.encoding["source"]).replace('_FES2012_SLEV.nc','')
-            ds = ds.sel(lon=ds.lon<360) #drop last instance, since 0 and 360 are both present
-            ds = ds.rename({'Ha':'amplitude','Hg':'phase'})
-        elif 'eot20' in ds.encoding["source"]:
-            compname = os.path.basename(ds.encoding["source"]).replace('_ocean_eot20.nc','')
-            ds = ds.sel(lon=ds.lon<360) #drop last instance, since 0 and 360 are both present
-        elif 'gtsm' in ds.encoding["source"].lower(): #TODO: make less hard coded
-            compname = os.path.basename(ds.encoding["source"]).replace('gtsmv4.1_2014_','').replace('_withfu_v3_rasterized.nc','')
-            ds = ds.rename({f'wl_amp{compname}':'amplitude',f'wl_phs{compname}':'phase'}) #TODO: adjust in rasterized dataset?
-            ds['amplitude'] = ds['amplitude'].assign_attrs({'units':'m'}) #TODO: handle this rasterize function
-            ds['phase'] = ds['phase'].assign_attrs({'units':'degrees'}) #TODO: handle this rasterize function
-            ds = ds.rename({'x':'lon','y':'lat'})
-        else:
-            compname = os.path.basename(ds.encoding["source"]).replace('.nc','')
-        compnumber = [component_list.index(compname)]
-        ds = ds.assign(compno=compnumber)
-        
-        convert_360to180 = (ds['lon'].to_numpy()>180).any()
-        if convert_360to180: # results in large chunks if it is done after concatenation, so do for each file before concatenation
-            ds.coords['lon'] = (ds.coords['lon'] + 180) % 360 - 180
-            ds = ds.sortby('lon')
-        return ds
-    
-    #use open_mfdataset() with preprocess argument to open all requested FES files into one Dataset
-    file_list_nc = [str(dir_pattern).replace('*',comp) for comp in component_list]
-    data_xrsel = xr.open_mfdataset(file_list_nc, combine='nested', concat_dim='compno', preprocess=extract_component)
-    data_xrsel = data_xrsel.rename({'lon':'longitude','lat':'latitude'})
-    
-    #derive uv phase components (using amplitude=1)
-    data_xrsel_phs_rad = np.deg2rad(data_xrsel['phase'])
-    #we need to compute u/v components for the phase to avoid zero-crossing interpolation issues
-    data_xrsel['phase_u'] = 1*np.cos(data_xrsel_phs_rad)
-    data_xrsel['phase_v'] = 1*np.sin(data_xrsel_phs_rad)
-    data_xrsel['compnames'] = xr.DataArray(component_list_upper_pd,dims=('compno')) #TODO: convert to proper string variable
-    
-    #convert cm to m
-    if data_xrsel['amplitude'].attrs['units'] == 'cm':
-        data_xrsel['amplitude'] /= 100
-        data_xrsel['amplitude'].attrs['units'] = 'm'
-    
-    data_interp = interp_regularnc_to_plipoints(data_xr_reg=data_xrsel, file_pli=file_pli, nPoints=nPoints)
-    data_interp['phase_new'] = np.rad2deg(np.arctan2(data_interp['phase_v'],data_interp['phase_u']))
-    
-    ForcingModel_object = plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
-    
-    return ForcingModel_object
-
-
-def open_dataset_extra(dir_pattern, quantity, tstart, tstop, conversion_dict=None, refdate_str=None, reverse_depth=False, chunks=None):
-    
-    if conversion_dict is None:
-        conversion_dict = get_conversion_dict()
-    
-    if quantity=='uxuy': #T3Dvector
-        quantity_list = ['ux','uy']
-    else:
-        quantity_list = [quantity]
-    ncvarname_list = [conversion_dict[quan]['ncvarname'] for quan in quantity_list]
-    
-    #convert tstart/tstop from str/dt.datetime/pd.Timestamp to pd.Timestamp. WARNING: when supplying '05-04-2016', monthfirst is assumed, so 2016-05-04 will be the result (may instead of april).
-    tstart = pd.Timestamp(tstart)
-    tstop = pd.Timestamp(tstop)
-    
-    dir_pattern = [Path(str(dir_pattern).format(ncvarname=ncvarname)) for ncvarname in ncvarname_list]
-    file_list_nc = []
-    for dir_pattern_one in dir_pattern:
-        file_list_nc = file_list_nc + glob.glob(str(dir_pattern_one))
-    list_pattern_names = [x.name for x in dir_pattern]
-    print(f'loading mfdataset of {len(file_list_nc)} files with pattern(s) {list_pattern_names}')
-    
-    try:
-        data_xr = xr.open_mfdataset(file_list_nc, chunks=chunks) #TODO: does chunks argument solve "PerformanceWarning: Slicing is producing a large chunk."? {'time':1} is not a convenient chunking to use for timeseries extraction
-    except xr.MergeError as e: #TODO: this except is necessary for CMCC, ux and uy have different lat/lon values, so renaming those of uy to avoid merging conflict
-        def preprocess_CMCC_uovo(ds):
-            if 'vo_' in os.path.basename(ds.encoding['source']):
-                ds.coords['longitude'] = (ds.coords['longitude'] + 180) % 360 - 180 #normally this is done at convert_360to180, but inconvenient after renaming longitude variable
-                ds = ds.rename({'longitude':'longitude_uy','latitude':'latitude_uy'})
-                ds = ds.drop_vars(['vertices_longitude','vertices_latitude'])
-            return ds
-        print(f'catching "MergeError: {e}" >> WARNING: ux/uy have different latitude/longitude values, making two coordinates sets in Dataset.')
-        data_xr = xr.open_mfdataset(file_list_nc, chunks=chunks, preprocess=preprocess_CMCC_uovo)
-    
-    #TODO: remove this commented code
-    #rename variables with rename_dict derived from conversion_dict. duplicate keys are not possible, so phyc is always renamed to tracerbndOpal (last in conversion_dict)
-    # rename_dict = {v['ncvarname']:k for k,v in conversion_dict.items()}
-    # for ncvarn in data_xr.variables.mapping.keys():
-    #     if ncvarn in rename_dict.keys():
-    #         data_xr = data_xr.rename({ncvarn:rename_dict[ncvarn]})
-
-    #renames ncvarnames to quantity names: proposal lisa, does not support ux/uy
-    # for ncvarn in data_xr.variables.mapping.keys():
-    #     if ncvarn == conversion_dict[quantity]['ncvarname']:
-    #         data_xr = data_xr.rename({ncvarn:quantity})
-    #         print(f'variable {ncvarn} renamed to {quantity}')
-    
-    for k,v in conversion_dict.items():
-        ncvarn = v['ncvarname']
-        if ncvarn in data_xr.variables.mapping.keys() and k in quantity_list: #k in quantity_list so phyc is not always renamed to tracerbndPON1 (first in conversion_dict)
-            data_xr = data_xr.rename({ncvarn:k})
-            print(f'variable {ncvarn} renamed to {k}')
-    
-    #rename dims time/depth/lat/lon/x/y #TODO: this has to be phased out some time, or made as an argument or merged with conversion_dict?
-    rename_dims_dict = {'time_counter':'time', #time_counter instead of time for some CMCC files
-                        'lev':'depth', #depth for CMEMS and many others, but lev for GFDL
-                        'deptht':'depth', #deptht for some CMCC vars
-                        'lon':'longitude','lat':'latitude',
-                        'nav_lon':'longitude','nav_lat':'latitude', #nav_lon/nav_lat for some CMCC vars
-                        'x':'j','y':'i', #x/y instead of j/i for some CMCC vars (non-regulargrid)
-                        }
-    for k,v in rename_dims_dict.items():
-        if k in data_xr.dims and v not in data_xr.dims: 
-            data_xr = data_xr.rename({k:v}) #TODO: can also do this for data_xr_var only?
-            print(f'dimension {k} renamed to {v}')
-    
-    #get calendar and maybe convert_calendar, makes sure that nc_tstart/nc_tstop are of type pd._libs.tslibs.timestamps.Timestamp
-    data_xr_calendar = data_xr['time'].dt.calendar
-    if data_xr_calendar != 'proleptic_gregorian': #this is for instance the case in case of noleap (or 365_days) calendars from GFDL and CMCC
-        units_copy = data_xr['time'].encoding['units']
-        print(f'WARNING: calendar different than proleptic_gregorian found ({data_xr_calendar}), convert_calendar is called so check output carefully. It should be no issue for datasets with a monthly interval.')
-        data_xr = data_xr.convert_calendar('standard') #TODO: does this not result in 29feb nan values in e.g. GFDL model? Check missing argument at https://docs.xarray.dev/en/stable/generated/xarray.Dataset.convert_calendar.html
-        data_xr['time'].encoding['units'] = units_copy #put back dropped units
-    
-    #get timevar and compare requested dates
-    timevar = data_xr['time']
-    xr_tstartstop = pd.to_datetime(timevar.isel(time=[0,-1]).to_series())
-    nc_tstart = xr_tstartstop.index[0]
-    nc_tstop = xr_tstartstop.index[-1]
-    if tstart < nc_tstart:
-        raise OutOfRangeError(f'requested tstart {tstart} outside of available range {nc_tstart} to {nc_tstop}')
-    if tstop > nc_tstop:
-        raise OutOfRangeError(f'requested tstop {tstop} outside of available range {nc_tstart} to {nc_tstop}')
-    
-    #360 to 180 conversion
-    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any() #TODO: replace to_numpy() with load()
-    latlon_ndims = len(data_xr['longitude'].shape)
-    if convert_360to180: #TODO: make more flexible for models that eg pass -180/+180 crossing (add overlap at lon edges).
-        data_xr.coords['longitude'] = (data_xr.coords['longitude'] + 180) % 360 - 180
-        if latlon_ndims==1: #lon/lat has 1 dimension, .sortby() not possible if there are 2 dimensions
-            data_xr = data_xr.sortby(data_xr['longitude'])
-        else: #lon/lat is 2D #TODO: this can be removed
-            print('WARNING: 2D latitude/longitude has more than one dim, continue without .sortby(). This is expected for e.g. CMCC')
-    
-    #retrieve var(s) (after potential longitude conversion) (also selecting relevant times)
-    data_vars = list(data_xr.data_vars)
-    bool_quanavailable = pd.Series(quantity_list).isin(data_vars)
-    if not bool_quanavailable.all():
-        quantity_list_notavailable = pd.Series(quantity_list).loc[~bool_quanavailable].tolist()
-        raise KeyError(f'quantity {quantity_list_notavailable} not found in netcdf, available are: {data_vars}. Try updating conversion_dict to rename these variables.')
-    data_xr_vars = data_xr[quantity_list].sel(time=slice(tstart,tstop))
-    
-    #optional conversion of units. Multiplications or other simple operatiors do not affect performance (dask.array(getitem) becomes dask.array(mul). With more complex operation it is better do do it on the interpolated array.
-    for quan in quantity_list: #TODO: maybe do unit conversion before interp or is that computationally heavy?
-        if 'conversion' in conversion_dict[quan].keys(): #if conversion is present, unit key must also be in conversion_dict
-            print(f'> converting units from [{data_xr_vars[quan].attrs["units"]}] to [{conversion_dict[quan]["unit"]}]')
-            #print(f'attrs are discarded:\n{data_xr_vars[quan].attrs}')
-            data_xr_vars[quan] = data_xr_vars[quan] * conversion_dict[quan]['conversion'] #conversion drops all attributes of which units (which are changed anyway)
-            data_xr_vars[quan].attrs['units'] = conversion_dict[quan]['unit'] #add unit attribute with resulting unit
-    
-    #optional refdate changing
-    if refdate_str is not None:
-        if 'long_name' in data_xr_vars.time.attrs: #for CMEMS it is 'hours since 1950-01-01', which would be wrong now #TODO: consider also removing attrs for depth/varname, since we would like to have salinitybnd/waterlevel instead of Salinity/sea_surface_height in xr plots?
-            del data_xr_vars.time.attrs['long_name']
-        data_xr_vars.time.encoding['units'] = refdate_str
-    
-    if 'depth' in data_xr_vars.coords:
-        #make negative down
-        if 'positive' in data_xr_vars['depth'].attrs.keys():
-            if data_xr_vars['depth'].attrs['positive'] == 'down': #attribute appears in CMEMS, GFDL and CMCC, save to assume presence?
-                data_xr_vars['depth'] = -data_xr_vars['depth']
-        #optional reversing depth dimension for comparison to coastserv
-        if reverse_depth:
-            print('> reversing depth dimension')
-            data_xr_vars = data_xr_vars.reindex({'depth':list(reversed(data_xr_vars['depth']))})
-    
-    return data_xr_vars
-
-
-def interp_regularnc_to_plipoints(data_xr_reg, file_pli, nPoints=None, load=True):
-    """
-    load: interpolation errors are only raised upon loading, so do this per default
-    #TODO: make format of this dataset more in line with existing bnd-nc format and hisfile: https://issuetracker.deltares.nl/browse/UNST-6549
-    """
-    data_xr_var = data_xr_reg #TODO: rename in script
-    
-    #load boundary file
-    polyfile_object = hcdfm.PolyFile(file_pli)
-    
-    #check if polyobj names in plifile are unique
-    polynames_pd = pd.Series([polyobj.metadata.name for polyobj in polyfile_object.objects])
-    if polynames_pd.duplicated().any():
-        raise ValueError(f'Duplicate polyobject names in polyfile {file_pli.name}, this is not allowed:\n{polynames_pd}')
-    
-    #create df of x/y/name of all plipoints in plifile
-    data_pol_list = []
-    for polyobj in polyfile_object.objects:
-        data_pol_pd_one = pointlike_to_DataFrame(polyobj)
-        data_pol_pd_one = data_pol_pd_one.iloc[:nPoints] #only use testset of points per polyobj in polyfile
-        data_pol_pd_one['name'] = pd.Series(data_pol_pd_one.index).apply(lambda x: f'{polyobj.metadata.name}_{x+1:04d}')
-        data_pol_list.append(data_pol_pd_one)
-    data_pol_pd = pd.concat(data_pol_list)
-    
-    da_plipoints = xr.Dataset()
-    da_plipoints['plipoint_x'] = xr.DataArray(data_pol_pd['x'], dims='plipoints')
-    da_plipoints['plipoint_y'] = xr.DataArray(data_pol_pd['y'], dims='plipoints')
-    da_plipoints['plipoint_name'] = xr.DataArray(data_pol_pd['name'].astype('S64'), dims='plipoints').str.decode('utf-8',errors='ignore').str.strip() #TODO: must be possible to do this less complex
-    da_plipoints = da_plipoints.set_coords(['plipoint_x','plipoint_y','plipoint_name'])
-    da_plipoints = da_plipoints.set_index({'plipoints':'plipoint_name'})
-    
-    #interpolation to lat/lon combinations
-    print('> interp mfdataset to all PolyFile points (lat/lon coordinates)')
-    #dtstart = dt.datetime.now()
-    try:
-        data_interp = data_xr_var.interp(longitude=da_plipoints['plipoint_x'], latitude=da_plipoints['plipoint_y'],
-                                         method='linear', 
-                                         kwargs={'bounds_error':True}, #error is only raised upon load(), so when the actual value retrieval happens
-                                         )
-    
-    except ValueError as e: #Dimensions {'latitude', 'longitude'} do not exist. Expected one or more of Frozen({'time': 17, 'depth': 50, 'i': 292, 'j': 362}).
-        #this is for eg CMCC model with multidimensional lat/lon variable
-        #TODO: make nicer, without try except? eg latlon_ndims==1, but not sure if that is always valid >> add nonregular alternative for interp_regularnc_to_plipoints() and set kdtree to 1 (closest value) (uy stuff has to be dropped anyway)
-        #TODO: maybe also spherical coordinate distance calculation instead of cartesian/eucledian
-        #TODO: maybe use .sel(method='nearest'), but "KeyError: "no index found for coordinate 'longitude'""
-        #TODO: interp for 2D also requested: https://github.com/pydata/xarray/issues/2281
-        print(f'ValueError: {e}. Reverting to KDTree instead (nearest neigbour)')
-        data_interp = xr.Dataset()
-        for varone in list(data_xr_var.data_vars):
-            path_lonlat_pd = data_pol_pd[['x','y']]
-            if (varone=='uy') & (len(data_xr_var.data_vars)>1):
-                data_lon_flat = data_xr_var['longitude_uy'].to_numpy().ravel()
-                data_lat_flat = data_xr_var['latitude_uy'].to_numpy().ravel()
-            else:
-                data_lon_flat = data_xr_var['longitude'].to_numpy().ravel()
-                data_lat_flat = data_xr_var['latitude'].to_numpy().ravel()
-            data_lonlat_pd = pd.DataFrame({'x':data_lon_flat,'y':data_lat_flat})
-            #KDTree, finds minimal eucledian distance between points (maybe haversine would be better)
-            tree = KDTree(data_lonlat_pd) #alternatively sklearn.neighbors.BallTree: tree = BallTree(data_lonlat_pd)
-            kdtree_k = 3 #TODO: nearest is probably just as wrong/right as weighted average, but raises error when using 1
-            distance, data_lonlat_idx = tree.query(path_lonlat_pd, k=kdtree_k) #TODO: maybe add outofbounds treshold for distance
-            #data_lonlat_pd.iloc[data_lonlat_idx]
-            idx_i,idx_j = np.divmod(data_lonlat_idx, data_xr_var['longitude'].shape[1]) #get idx i and j by sort of counting over 2D array
-            # import matplotlib.pyplot as plt
-            # fig,ax = plt.subplots()
-            # data_xr_var[varone].isel(time=0,depth=0).plot(ax=ax)
-            # ax.plot(idx_j,idx_i,'xr')
-            da_plipoints['da_idxi'] = xr.DataArray(idx_i, dims=('plipoints','nearestkpoints'))
-            da_plipoints['da_idxj'] = xr.DataArray(idx_j, dims=('plipoints','nearestkpoints'))
-            da_dist = xr.DataArray(distance, dims=('plipoints','nearestkpoints'))
-            da_invdistweight = (1/da_dist)/(1/da_dist).sum(dim='nearestkpoints')
-            da_varone_3k = data_xr_var[varone].isel(i=da_plipoints['da_idxi'],j=da_plipoints['da_idxj'])
-            data_interp[varone] = (da_varone_3k * da_invdistweight).sum(dim='nearestkpoints')
-            data_interp[varone].attrs = data_xr_var[varone].attrs #copy units and other attributes
-    
-    #time_passed = (dt.datetime.now()-dtstart).total_seconds()
-    # print(f'>>time passed: {time_passed:.2f} sec')
-    
-    if not load:
-        return data_interp
-    
-    print(f'> actual extraction of data from netcdf with .load() (for {len(data_pol_pd)} plipoints at once, this might take a while)')
-    dtstart = dt.datetime.now()
-    try:
-        data_interp_loaded = data_interp.load() #loading data for all points at once is more efficient compared to loading data per point in loop 
-    except ValueError as e: #generate a proper error with outofbounds requested coordinates, default is "ValueError: One of the requested xi is out of bounds in dimension 0" #TODO: improve error in xarray
-        lonvar_vals = data_xr_var['longitude'].to_numpy()
-        latvar_vals = data_xr_var['latitude'].to_numpy()
-        data_pol_pd = data_interp[['plipoint_x','plipoint_y']].to_dataframe()
-        bool_reqlon_outbounds = (data_pol_pd['plipoint_x'] <= lonvar_vals.min()) | (data_pol_pd['plipoint_x'] >= lonvar_vals.max())
-        bool_reqlat_outbounds = (data_pol_pd['plipoint_y'] <= latvar_vals.min()) | (data_pol_pd['plipoint_y'] >= latvar_vals.max())
-        reqlatlon_pd = pd.DataFrame({'longitude':data_pol_pd['plipoint_x'],'latitude':data_pol_pd['plipoint_y'],'lon outbounds':bool_reqlon_outbounds,'lat outbounds':bool_reqlat_outbounds})
-        reqlatlon_pd_outbounds = reqlatlon_pd.loc[bool_reqlon_outbounds | bool_reqlat_outbounds]
-        raise ValueError(f'{len(reqlatlon_pd_outbounds)} of requested pli points are out of bounds (valid longitude range {lonvar_vals.min()} to {lonvar_vals.max()}, valid latitude range {latvar_vals.min()} to {latvar_vals.max()}):\n{reqlatlon_pd_outbounds}')
-    time_passed = (dt.datetime.now()-dtstart).total_seconds()
-    print(f'>>time passed: {time_passed:.2f} sec')
-
-    return data_interp_loaded
-
-
-def interp_hisnc_to_plipoints(data_xr_his, file_pli, kdtree_k=3, load=True):
-    """
-    interpolate stations in hisfile to points of polyfile
-    """
-    #KDTree, finds minimal eucledian distance between points (haversine would be better). Alternatively sklearn.neighbors.BallTree: tree = BallTree(data_lonlat_pd)
-    
-    datavars_list = list(data_xr_his.data_vars)
-    if len(datavars_list)>5:
-        print('WARNING: more than 5 data_vars, you might want to subset your data_xr_his')
-    #read hisfile and make KDTree of xy of hisstations
-    hisstations_pd = data_xr_his.stations.to_dataframe() #TODO: add check if stations are strings? (whether preprocess_hisnc was used)
-    tree_nest2 = KDTree(hisstations_pd[['station_x_coordinate','station_y_coordinate']])
-    
-    #read polyfile and query k nearest hisstations (names)
-    polyfile_object = hcdfm.PolyFile(file_pli)
-    data_pol_list = []
-    for polyobj in polyfile_object.objects:
-        data_pol_pd_one = pointlike_to_DataFrame(polyobj)
-        data_pol_pd_one['name'] = pd.Series(data_pol_pd_one.index).apply(lambda x: f'{polyobj.metadata.name}_{x+1:04d}')
-        data_pol_list.append(data_pol_pd_one)
-    data_pol_pd = pd.concat(data_pol_list)
-
-    plicoords_distance2, plicoords_nestpointidx = tree_nest2.query(data_pol_pd[['x','y']], k=kdtree_k)
-    da_plicoords_nestpointidx = xr.DataArray(plicoords_nestpointidx, dims=('plipoints','nearestkpoints'))
-    da_plicoords_nestpointnames = data_xr_his.stations.isel(stations=da_plicoords_nestpointidx)
-    
-    #interpolate hisfile variables to plipoints
-    data_interp = xr.Dataset()
-    data_interp['plipoint_x'] = xr.DataArray(data_pol_pd['x'],dims=('plipoints'))
-    data_interp['plipoint_y'] = xr.DataArray(data_pol_pd['y'],dims=('plipoints'))
-    data_interp['plipoint_name'] = xr.DataArray(data_pol_pd['name'].astype('S64'), dims='plipoints').str.decode('utf-8',errors='ignore').str.strip() #TODO: must be possible to do this less complex
-    data_interp = data_interp.set_coords(['plipoint_x','plipoint_y','plipoint_name'])
-    data_interp = data_interp.set_index({'plipoints':'plipoint_name'})
-    
-    for varone in datavars_list:
-        da_dist = xr.DataArray(plicoords_distance2, dims=('plipoints','nearestkpoints'))
-        da_invdistweight = (1/da_dist)/(1/da_dist).sum(dim='nearestkpoints') #TODO: set weigths for invalid points to 0 (and increase others weights so sum remains 1)
-        data_xr_his_pli_knearest = data_xr_his[varone].sel(stations=da_plicoords_nestpointnames)
-        data_interp[varone] = (data_xr_his_pli_knearest * da_invdistweight).sum(dim='nearestkpoints')
-        data_interp[varone].attrs = data_xr_his[varone].attrs #copy units and other attributes
-        
-    if not load:
-        return data_interp
-    
-    print('loading dataset (might take a while, but increases performance of point loop significantly)')
-    data_interp = data_interp.load()
-    print('done')
-
-    return data_interp
-    
-
-def plipointsDataset_to_ForcingModel(plipointsDataset):
-    quantity_list = list(plipointsDataset.data_vars)
-    npoints = len(plipointsDataset.plipoints)
-    
-    #start conversion to Forcingmodel object
-    print(f'Converting {npoints} plipoints to hcdfm.ForcingModel():',end='')
-    dtstart = dt.datetime.now()
-    ForcingModel_object = hcdfm.ForcingModel()
-    for iP in range(npoints):
-        print(f' {iP+1}',end='')
-        
-        #select data for this point, ffill nans, concatenating time column, constructing T3D/TimeSeries and append to hcdfm.ForcingModel()
-        datablock_xr_onepoint = plipointsDataset.isel(plipoints=iP)
-        plipoint_name = str(datablock_xr_onepoint.plipoints.to_numpy())
-        
-        for quan in quantity_list:
-            datablock_xr_onepoint[quan].attrs['locationname'] = plipoint_name #TODO: is there a nicer way of passing this data?
-            if datablock_xr_onepoint[quan].isnull().all(): # check if all values of plipoint are nan (on land)
-                warnings.warn(UserWarning(f'Plipoint "{plipoint_name}" might be on land since it only contain nan values. Consider altering your plifile or using plipointsDataset.ffill(dim="plipoints").bfill(dim="plipoints"). Nan values replaced with 0 to avoid bc-writing errors')) #TODO: maybe fill along plipoints dimension, but beware on nans in deep water that are filled with neighbours
-                datablock_xr_onepoint[quan] = datablock_xr_onepoint[quan].fillna(0)
-        
-        if 'depth' in plipointsDataset.dims:
-            ts_one = Dataset_to_T3D(datablock_xr_onepoint)
-        elif 'amplitude' in quantity_list:
-            ts_one = Dataset_to_Astronomic(datablock_xr_onepoint)
-        else:
-            ts_one = Dataset_to_TimeSeries(datablock_xr_onepoint)
-        ForcingModel_object.forcing.append(ts_one)
-    print(f'. >> done in {(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    return ForcingModel_object
-
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Aug 18 17:39:03 2022
+
+@author: veenstra
+
+"""
+
+import os
+import glob
+import datetime as dt
+import numpy as np
+import pandas as pd
+import xarray as xr
+from pathlib import Path
+from scipy.spatial import KDTree
+import warnings
+import hydrolib.core.dflowfm as hcdfm
+
+from dfm_tools.hydrolib_helpers import Dataset_to_TimeSeries, Dataset_to_T3D, Dataset_to_Astronomic, pointlike_to_DataFrame
+from dfm_tools.errors import OutOfRangeError
+
+
+def get_conversion_dict(ncvarname_updates={}):
+    
+    """
+    get the conversion_dict, optionally with updated ncvarnames
+    conversion_dict.keys() are the dflowfm quantities and the ncvarname the corresponding netcdf variable name/key
+    alternative ncvarnames can be supplied via ncvarname_updates, e.g. get_conversion_dict(ncvarname_updates={'temperaturebnd':'tos'})
+    
+    interpolate_nc_to_bc() renames netcdf variable like this:
+    data_xr = data_xr.rename({ncvarname:quantity})
+    
+    for CMCC:
+    conversion_dict = { # mg/l is the same as g/m3: conversion is phyc in mol/m3 to newvar in g/m3
+                       'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 },
+                       'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 },
+                       'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 },
+                       'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08},
+                       'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0}, # Caution: this empirical relation might not be applicable to your use case
+                       'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 30.97}, # Caution: this empirical relation might not be applicable to your use case
+                       'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 14.0 * (106 / 16)}, # Caution: this empirical relation might not be applicable to your use case
+                       'salinitybnd'         : {'ncvarname': 'sos'},         #'1e-3'
+                       'temperaturebnd'      : {'ncvarname': 'tos'},         #'degC'
+                       'ux'                  : {'ncvarname': 'uo'},          #'m/s'
+                       'uy'                  : {'ncvarname': 'vo'},          #'m/s'
+                       'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
+                       'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
+                       }
+    """
+    # conversion_dict, 
+    conversion_dict = { # mg/l is the same as g/m3: conversion is phyc in mmol/l to newvar in g/m3
+                        'tracerbndOXY'        : {'ncvarname': 'o2',          'unit': 'g/m3', 'conversion': 32.0 / 1000.0}, 
+                        'tracerbndNO3'        : {'ncvarname': 'no3',         'unit': 'g/m3', 'conversion': 14.0 / 1000.0},
+                        'tracerbndPO4'        : {'ncvarname': 'po4',         'unit': 'g/m3', 'conversion': 30.97 / 1000.0},
+                        'tracerbndSi'         : {'ncvarname': 'si',          'unit': 'g/m3', 'conversion': 28.08 / 1000.0},
+                        'tracerbndPON1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 16. * 14. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndPOP1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 30.97 / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndPOC1'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 2. * 12. / 1000.0}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndDON'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 3.24 * 2. * 16. * 14. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndDOP'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 1.0 * 2. * 30.97 / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndDOC'        : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': (199. / 20.) * 3.24 * 2. * 16. * 12. / (106. * 1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'tracerbndOpal'       : {'ncvarname': 'phyc',        'unit': 'g/m3', 'conversion': 0.5 * 0.13 * 28.08 / (1000.0)}, # Caution: this empirical relation might not be applicable to your use case
+                        'salinitybnd'         : {'ncvarname': 'so'},          #'1e-3'
+                        'temperaturebnd'      : {'ncvarname': 'thetao'},      #'degC'
+                        'ux'                  : {'ncvarname': 'uo'},          #'m/s'
+                        'uy'                  : {'ncvarname': 'vo'},          #'m/s'
+                        'waterlevelbnd'       : {'ncvarname': 'zos'},         #'m' #steric
+                        'tide'                : {'ncvarname': ''},            #'m' #tide (dummy entry)
+                        }
+    #do updates
+    for k,v in ncvarname_updates.items():
+        conversion_dict[k]['ncvarname'] = v
+    return conversion_dict
+
+
+def interpolate_tide_to_bc(tidemodel, file_pli, component_list=None, nPoints=None):
+    """
+    """
+    # translate dict from .\hydro_tools\FES\PreProcessing_FES_TideModel_imaginary.m
+    #component_list = ['2N2','LABDA2','MF','MFM','P1','SSA','EPSILON2','M2','MKS2','MU2','Q1','T2','J1','M3','MM','N2','R2','K1','M4','MN4','N4','S1','K2','M6','MS4','NU2','S2','L2','M8','MSF','O1','S4','MSQM','SA']
+    translate_dict = {'LA2':'LABDA2', #TODO: use value instead of key in bc file? Support using value instead of key in const_list also (like line above)
+                      'EPS2':'EPSILON2', 
+                      'Z0':'A0',
+                      'MTM':'MFM', #Needs to be verified
+                      }
+    
+    dir_pattern_dict = {'FES2014': Path(r'P:\metocean-data\licensed\FES2014','*.nc'), #ocean_tide_extrapolated
+                        'FES2012': Path(r'P:\metocean-data\open\FES2012\data','*_FES2012_SLEV.nc'), #is eigenlijk ook licensed
+                        'EOT20': Path(r'P:\metocean-data\open\EOT20\ocean_tides','*_ocean_eot20.nc'),
+                        'GTSM4.1preliminary': Path(r'p:\1230882-emodnet_hrsm\GTSMv3.0EMODnet\EMOD_MichaelTUM_yearcomponents\GTSMv4.1_yeartide_2014_2.20.06\compare_fouhis_fouxyz_v3','gtsmv4.1_2014_*_withfu_v3_rasterized.nc'),
+                        #TODO: add tpxo8 (tpxo9 is also available), catalog: https://opendap.deltares.nl/thredds/catalog/opendap/deltares/delftdashboard/tidemodels/tpxo80/catalog.html
+                        }
+    if tidemodel not in dir_pattern_dict.keys():
+        raise KeyError(f'invalid tidemodel "{tidemodel}", options are: {list(dir_pattern_dict.keys())}')
+    if tidemodel == 'GTSM4.1preliminary':
+        warnings.warn(UserWarning(f'you are using tidemodel "{tidemodel}", beware that the dataset is preliminary so it is still quite coarse and may contain errors. Check your results carefully'))
+    dir_pattern = dir_pattern_dict[tidemodel]
+    
+    if component_list is None:
+        file_list_nc = glob.glob(str(dir_pattern))
+        dir_pattern_basename = os.path.basename(dir_pattern)
+        replace = dir_pattern_basename.split('*')
+        component_list = [os.path.basename(x).replace(replace[0],'').replace(replace[1],'') for x in file_list_nc] #TODO: make this less hard-coded
+    component_list_upper_pd = pd.Series([x.upper() for x in component_list]).replace(translate_dict, regex=True)
+    
+    def extract_component(ds):
+        #https://github.com/pydata/xarray/issues/1380
+        if 'FES2012' in ds.encoding["source"]: #TODO: make more generic with regex, or just add tidemodel argument since they are quite specific
+            compname = os.path.basename(ds.encoding["source"]).replace('_FES2012_SLEV.nc','')
+            ds = ds.sel(lon=ds.lon<360) #drop last instance, since 0 and 360 are both present
+            ds = ds.rename({'Ha':'amplitude','Hg':'phase'})
+        elif 'eot20' in ds.encoding["source"]:
+            compname = os.path.basename(ds.encoding["source"]).replace('_ocean_eot20.nc','')
+            ds = ds.sel(lon=ds.lon<360) #drop last instance, since 0 and 360 are both present
+        elif 'gtsm' in ds.encoding["source"].lower(): #TODO: make less hard coded
+            compname = os.path.basename(ds.encoding["source"]).replace('gtsmv4.1_2014_','').replace('_withfu_v3_rasterized.nc','')
+            ds = ds.rename({f'wl_amp{compname}':'amplitude',f'wl_phs{compname}':'phase'}) #TODO: adjust in rasterized dataset?
+            ds['amplitude'] = ds['amplitude'].assign_attrs({'units':'m'}) #TODO: handle this rasterize function
+            ds['phase'] = ds['phase'].assign_attrs({'units':'degrees'}) #TODO: handle this rasterize function
+            ds = ds.rename({'x':'lon','y':'lat'})
+        else:
+            compname = os.path.basename(ds.encoding["source"]).replace('.nc','')
+        compnumber = [component_list.index(compname)]
+        ds = ds.assign(compno=compnumber)
+        
+        convert_360to180 = (ds['lon'].to_numpy()>180).any()
+        if convert_360to180: # results in large chunks if it is done after concatenation, so do for each file before concatenation
+            ds.coords['lon'] = (ds.coords['lon'] + 180) % 360 - 180
+            ds = ds.sortby('lon')
+        return ds
+    
+    #use open_mfdataset() with preprocess argument to open all requested FES files into one Dataset
+    file_list_nc = [str(dir_pattern).replace('*',comp) for comp in component_list]
+    data_xrsel = xr.open_mfdataset(file_list_nc, combine='nested', concat_dim='compno', preprocess=extract_component)
+    data_xrsel = data_xrsel.rename({'lon':'longitude','lat':'latitude'})
+    
+    #derive uv phase components (using amplitude=1)
+    data_xrsel_phs_rad = np.deg2rad(data_xrsel['phase'])
+    #we need to compute u/v components for the phase to avoid zero-crossing interpolation issues
+    data_xrsel['phase_u'] = 1*np.cos(data_xrsel_phs_rad)
+    data_xrsel['phase_v'] = 1*np.sin(data_xrsel_phs_rad)
+    data_xrsel['compnames'] = xr.DataArray(component_list_upper_pd,dims=('compno')) #TODO: convert to proper string variable
+    
+    #convert cm to m
+    if data_xrsel['amplitude'].attrs['units'] == 'cm':
+        data_xrsel['amplitude'] /= 100
+        data_xrsel['amplitude'].attrs['units'] = 'm'
+    
+    data_interp = interp_regularnc_to_plipoints(data_xr_reg=data_xrsel, file_pli=file_pli, nPoints=nPoints)
+    data_interp['phase_new'] = np.rad2deg(np.arctan2(data_interp['phase_v'],data_interp['phase_u']))
+    
+    ForcingModel_object = plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
+    
+    return ForcingModel_object
+
+
+def open_dataset_extra(dir_pattern, quantity, tstart, tstop, conversion_dict=None, refdate_str=None, reverse_depth=False, chunks=None):
+    
+    if conversion_dict is None:
+        conversion_dict = get_conversion_dict()
+    
+    if quantity=='uxuy': #T3Dvector
+        quantity_list = ['ux','uy']
+    else:
+        quantity_list = [quantity]
+    ncvarname_list = [conversion_dict[quan]['ncvarname'] for quan in quantity_list]
+    
+    #convert tstart/tstop from str/dt.datetime/pd.Timestamp to pd.Timestamp. WARNING: when supplying '05-04-2016', monthfirst is assumed, so 2016-05-04 will be the result (may instead of april).
+    tstart = pd.Timestamp(tstart)
+    tstop = pd.Timestamp(tstop)
+    
+    dir_pattern = [Path(str(dir_pattern).format(ncvarname=ncvarname)) for ncvarname in ncvarname_list]
+    file_list_nc = []
+    for dir_pattern_one in dir_pattern:
+        file_list_nc = file_list_nc + glob.glob(str(dir_pattern_one))
+    list_pattern_names = [x.name for x in dir_pattern]
+    print(f'loading mfdataset of {len(file_list_nc)} files with pattern(s) {list_pattern_names}')
+    
+    try:
+        data_xr = xr.open_mfdataset(file_list_nc, chunks=chunks) #TODO: does chunks argument solve "PerformanceWarning: Slicing is producing a large chunk."? {'time':1} is not a convenient chunking to use for timeseries extraction
+    except xr.MergeError as e: #TODO: this except is necessary for CMCC, ux and uy have different lat/lon values, so renaming those of uy to avoid merging conflict
+        def preprocess_CMCC_uovo(ds):
+            if 'vo_' in os.path.basename(ds.encoding['source']):
+                ds.coords['longitude'] = (ds.coords['longitude'] + 180) % 360 - 180 #normally this is done at convert_360to180, but inconvenient after renaming longitude variable
+                ds = ds.rename({'longitude':'longitude_uy','latitude':'latitude_uy'})
+                ds = ds.drop_vars(['vertices_longitude','vertices_latitude'])
+            return ds
+        print(f'catching "MergeError: {e}" >> WARNING: ux/uy have different latitude/longitude values, making two coordinates sets in Dataset.')
+        data_xr = xr.open_mfdataset(file_list_nc, chunks=chunks, preprocess=preprocess_CMCC_uovo)
+    
+    #TODO: remove this commented code
+    #rename variables with rename_dict derived from conversion_dict. duplicate keys are not possible, so phyc is always renamed to tracerbndOpal (last in conversion_dict)
+    # rename_dict = {v['ncvarname']:k for k,v in conversion_dict.items()}
+    # for ncvarn in data_xr.variables.mapping.keys():
+    #     if ncvarn in rename_dict.keys():
+    #         data_xr = data_xr.rename({ncvarn:rename_dict[ncvarn]})
+
+    #renames ncvarnames to quantity names: proposal lisa, does not support ux/uy
+    # for ncvarn in data_xr.variables.mapping.keys():
+    #     if ncvarn == conversion_dict[quantity]['ncvarname']:
+    #         data_xr = data_xr.rename({ncvarn:quantity})
+    #         print(f'variable {ncvarn} renamed to {quantity}')
+    
+    for k,v in conversion_dict.items():
+        ncvarn = v['ncvarname']
+        if ncvarn in data_xr.variables.mapping.keys() and k in quantity_list: #k in quantity_list so phyc is not always renamed to tracerbndPON1 (first in conversion_dict)
+            data_xr = data_xr.rename({ncvarn:k})
+            print(f'variable {ncvarn} renamed to {k}')
+    
+    #rename dims time/depth/lat/lon/x/y #TODO: this has to be phased out some time, or made as an argument or merged with conversion_dict?
+    rename_dims_dict = {'time_counter':'time', #time_counter instead of time for some CMCC files
+                        'lev':'depth', #depth for CMEMS and many others, but lev for GFDL
+                        'deptht':'depth', #deptht for some CMCC vars
+                        'lon':'longitude','lat':'latitude',
+                        'nav_lon':'longitude','nav_lat':'latitude', #nav_lon/nav_lat for some CMCC vars
+                        'x':'j','y':'i', #x/y instead of j/i for some CMCC vars (non-regulargrid)
+                        }
+    for k,v in rename_dims_dict.items():
+        if k in data_xr.dims and v not in data_xr.dims: 
+            data_xr = data_xr.rename({k:v}) #TODO: can also do this for data_xr_var only?
+            print(f'dimension {k} renamed to {v}')
+    
+    #get calendar and maybe convert_calendar, makes sure that nc_tstart/nc_tstop are of type pd._libs.tslibs.timestamps.Timestamp
+    data_xr_calendar = data_xr['time'].dt.calendar
+    if data_xr_calendar != 'proleptic_gregorian': #this is for instance the case in case of noleap (or 365_days) calendars from GFDL and CMCC
+        units_copy = data_xr['time'].encoding['units']
+        print(f'WARNING: calendar different than proleptic_gregorian found ({data_xr_calendar}), convert_calendar is called so check output carefully. It should be no issue for datasets with a monthly interval.')
+        data_xr = data_xr.convert_calendar('standard') #TODO: does this not result in 29feb nan values in e.g. GFDL model? Check missing argument at https://docs.xarray.dev/en/stable/generated/xarray.Dataset.convert_calendar.html
+        data_xr['time'].encoding['units'] = units_copy #put back dropped units
+    
+    #get timevar and compare requested dates
+    timevar = data_xr['time']
+    xr_tstartstop = pd.to_datetime(timevar.isel(time=[0,-1]).to_series())
+    nc_tstart = xr_tstartstop.index[0]
+    nc_tstop = xr_tstartstop.index[-1]
+    if tstart < nc_tstart:
+        raise OutOfRangeError(f'requested tstart {tstart} outside of available range {nc_tstart} to {nc_tstop}')
+    if tstop > nc_tstop:
+        raise OutOfRangeError(f'requested tstop {tstop} outside of available range {nc_tstart} to {nc_tstop}')
+    
+    #360 to 180 conversion
+    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any() #TODO: replace to_numpy() with load()
+    latlon_ndims = len(data_xr['longitude'].shape)
+    if convert_360to180: #TODO: make more flexible for models that eg pass -180/+180 crossing (add overlap at lon edges).
+        data_xr.coords['longitude'] = (data_xr.coords['longitude'] + 180) % 360 - 180
+        if latlon_ndims==1: #lon/lat has 1 dimension, .sortby() not possible if there are 2 dimensions
+            data_xr = data_xr.sortby(data_xr['longitude'])
+        else: #lon/lat is 2D #TODO: this can be removed
+            print('WARNING: 2D latitude/longitude has more than one dim, continue without .sortby(). This is expected for e.g. CMCC')
+    
+    #retrieve var(s) (after potential longitude conversion) (also selecting relevant times)
+    data_vars = list(data_xr.data_vars)
+    bool_quanavailable = pd.Series(quantity_list).isin(data_vars)
+    if not bool_quanavailable.all():
+        quantity_list_notavailable = pd.Series(quantity_list).loc[~bool_quanavailable].tolist()
+        raise KeyError(f'quantity {quantity_list_notavailable} not found in netcdf, available are: {data_vars}. Try updating conversion_dict to rename these variables.')
+    data_xr_vars = data_xr[quantity_list].sel(time=slice(tstart,tstop))
+    
+    #optional conversion of units. Multiplications or other simple operatiors do not affect performance (dask.array(getitem) becomes dask.array(mul). With more complex operation it is better do do it on the interpolated array.
+    for quan in quantity_list: #TODO: maybe do unit conversion before interp or is that computationally heavy?
+        if 'conversion' in conversion_dict[quan].keys(): #if conversion is present, unit key must also be in conversion_dict
+            print(f'> converting units from [{data_xr_vars[quan].attrs["units"]}] to [{conversion_dict[quan]["unit"]}]')
+            #print(f'attrs are discarded:\n{data_xr_vars[quan].attrs}')
+            data_xr_vars[quan] = data_xr_vars[quan] * conversion_dict[quan]['conversion'] #conversion drops all attributes of which units (which are changed anyway)
+            data_xr_vars[quan].attrs['units'] = conversion_dict[quan]['unit'] #add unit attribute with resulting unit
+    
+    #optional refdate changing
+    if refdate_str is not None:
+        if 'long_name' in data_xr_vars.time.attrs: #for CMEMS it is 'hours since 1950-01-01', which would be wrong now #TODO: consider also removing attrs for depth/varname, since we would like to have salinitybnd/waterlevel instead of Salinity/sea_surface_height in xr plots?
+            del data_xr_vars.time.attrs['long_name']
+        data_xr_vars.time.encoding['units'] = refdate_str
+    
+    if 'depth' in data_xr_vars.coords:
+        #make negative down
+        if 'positive' in data_xr_vars['depth'].attrs.keys():
+            if data_xr_vars['depth'].attrs['positive'] == 'down': #attribute appears in CMEMS, GFDL and CMCC, save to assume presence?
+                data_xr_vars['depth'] = -data_xr_vars['depth']
+        #optional reversing depth dimension for comparison to coastserv
+        if reverse_depth:
+            print('> reversing depth dimension')
+            data_xr_vars = data_xr_vars.reindex({'depth':list(reversed(data_xr_vars['depth']))})
+    
+    return data_xr_vars
+
+
+def interp_regularnc_to_plipoints(data_xr_reg, file_pli, nPoints=None, load=True):
+    """
+    load: interpolation errors are only raised upon loading, so do this per default
+    #TODO: make format of this dataset more in line with existing bnd-nc format and hisfile: https://issuetracker.deltares.nl/browse/UNST-6549
+    """
+    data_xr_var = data_xr_reg #TODO: rename in script
+    
+    #load boundary file
+    polyfile_object = hcdfm.PolyFile(file_pli)
+    
+    #check if polyobj names in plifile are unique
+    polynames_pd = pd.Series([polyobj.metadata.name for polyobj in polyfile_object.objects])
+    if polynames_pd.duplicated().any():
+        raise ValueError(f'Duplicate polyobject names in polyfile {file_pli.name}, this is not allowed:\n{polynames_pd}')
+    
+    #create df of x/y/name of all plipoints in plifile
+    data_pol_list = []
+    for polyobj in polyfile_object.objects:
+        data_pol_pd_one = pointlike_to_DataFrame(polyobj)
+        data_pol_pd_one = data_pol_pd_one.iloc[:nPoints] #only use testset of points per polyobj in polyfile
+        data_pol_pd_one['name'] = pd.Series(data_pol_pd_one.index).apply(lambda x: f'{polyobj.metadata.name}_{x+1:04d}')
+        data_pol_list.append(data_pol_pd_one)
+    data_pol_pd = pd.concat(data_pol_list)
+    
+    da_plipoints = xr.Dataset()
+    da_plipoints['plipoint_x'] = xr.DataArray(data_pol_pd['x'], dims='plipoints')
+    da_plipoints['plipoint_y'] = xr.DataArray(data_pol_pd['y'], dims='plipoints')
+    da_plipoints['plipoint_name'] = xr.DataArray(data_pol_pd['name'].astype('S64'), dims='plipoints').str.decode('utf-8',errors='ignore').str.strip() #TODO: must be possible to do this less complex
+    da_plipoints = da_plipoints.set_coords(['plipoint_x','plipoint_y','plipoint_name'])
+    da_plipoints = da_plipoints.set_index({'plipoints':'plipoint_name'})
+    
+    #interpolation to lat/lon combinations
+    print('> interp mfdataset to all PolyFile points (lat/lon coordinates)')
+    #dtstart = dt.datetime.now()
+    try:
+        data_interp = data_xr_var.interp(longitude=da_plipoints['plipoint_x'], latitude=da_plipoints['plipoint_y'],
+                                         method='linear', 
+                                         kwargs={'bounds_error':True}, #error is only raised upon load(), so when the actual value retrieval happens
+                                         )
+    
+    except ValueError as e: #Dimensions {'latitude', 'longitude'} do not exist. Expected one or more of Frozen({'time': 17, 'depth': 50, 'i': 292, 'j': 362}).
+        #this is for eg CMCC model with multidimensional lat/lon variable
+        #TODO: make nicer, without try except? eg latlon_ndims==1, but not sure if that is always valid >> add nonregular alternative for interp_regularnc_to_plipoints() and set kdtree to 1 (closest value) (uy stuff has to be dropped anyway)
+        #TODO: maybe also spherical coordinate distance calculation instead of cartesian/eucledian
+        #TODO: maybe use .sel(method='nearest'), but "KeyError: "no index found for coordinate 'longitude'""
+        #TODO: interp for 2D also requested: https://github.com/pydata/xarray/issues/2281
+        print(f'ValueError: {e}. Reverting to KDTree instead (nearest neigbour)')
+        data_interp = xr.Dataset()
+        for varone in list(data_xr_var.data_vars):
+            path_lonlat_pd = data_pol_pd[['x','y']]
+            if (varone=='uy') & (len(data_xr_var.data_vars)>1):
+                data_lon_flat = data_xr_var['longitude_uy'].to_numpy().ravel()
+                data_lat_flat = data_xr_var['latitude_uy'].to_numpy().ravel()
+            else:
+                data_lon_flat = data_xr_var['longitude'].to_numpy().ravel()
+                data_lat_flat = data_xr_var['latitude'].to_numpy().ravel()
+            data_lonlat_pd = pd.DataFrame({'x':data_lon_flat,'y':data_lat_flat})
+            #KDTree, finds minimal eucledian distance between points (maybe haversine would be better)
+            tree = KDTree(data_lonlat_pd) #alternatively sklearn.neighbors.BallTree: tree = BallTree(data_lonlat_pd)
+            kdtree_k = 3 #TODO: nearest is probably just as wrong/right as weighted average, but raises error when using 1
+            distance, data_lonlat_idx = tree.query(path_lonlat_pd, k=kdtree_k) #TODO: maybe add outofbounds treshold for distance
+            #data_lonlat_pd.iloc[data_lonlat_idx]
+            idx_i,idx_j = np.divmod(data_lonlat_idx, data_xr_var['longitude'].shape[1]) #get idx i and j by sort of counting over 2D array
+            # import matplotlib.pyplot as plt
+            # fig,ax = plt.subplots()
+            # data_xr_var[varone].isel(time=0,depth=0).plot(ax=ax)
+            # ax.plot(idx_j,idx_i,'xr')
+            da_plipoints['da_idxi'] = xr.DataArray(idx_i, dims=('plipoints','nearestkpoints'))
+            da_plipoints['da_idxj'] = xr.DataArray(idx_j, dims=('plipoints','nearestkpoints'))
+            da_dist = xr.DataArray(distance, dims=('plipoints','nearestkpoints'))
+            da_invdistweight = (1/da_dist)/(1/da_dist).sum(dim='nearestkpoints')
+            da_varone_3k = data_xr_var[varone].isel(i=da_plipoints['da_idxi'],j=da_plipoints['da_idxj'])
+            data_interp[varone] = (da_varone_3k * da_invdistweight).sum(dim='nearestkpoints')
+            data_interp[varone].attrs = data_xr_var[varone].attrs #copy units and other attributes
+    
+    #time_passed = (dt.datetime.now()-dtstart).total_seconds()
+    # print(f'>>time passed: {time_passed:.2f} sec')
+    
+    if not load:
+        return data_interp
+    
+    print(f'> actual extraction of data from netcdf with .load() (for {len(data_pol_pd)} plipoints at once, this might take a while)')
+    dtstart = dt.datetime.now()
+    try:
+        data_interp_loaded = data_interp.load() #loading data for all points at once is more efficient compared to loading data per point in loop 
+    except ValueError as e: #generate a proper error with outofbounds requested coordinates, default is "ValueError: One of the requested xi is out of bounds in dimension 0" #TODO: improve error in xarray
+        lonvar_vals = data_xr_var['longitude'].to_numpy()
+        latvar_vals = data_xr_var['latitude'].to_numpy()
+        data_pol_pd = data_interp[['plipoint_x','plipoint_y']].to_dataframe()
+        bool_reqlon_outbounds = (data_pol_pd['plipoint_x'] <= lonvar_vals.min()) | (data_pol_pd['plipoint_x'] >= lonvar_vals.max())
+        bool_reqlat_outbounds = (data_pol_pd['plipoint_y'] <= latvar_vals.min()) | (data_pol_pd['plipoint_y'] >= latvar_vals.max())
+        reqlatlon_pd = pd.DataFrame({'longitude':data_pol_pd['plipoint_x'],'latitude':data_pol_pd['plipoint_y'],'lon outbounds':bool_reqlon_outbounds,'lat outbounds':bool_reqlat_outbounds})
+        reqlatlon_pd_outbounds = reqlatlon_pd.loc[bool_reqlon_outbounds | bool_reqlat_outbounds]
+        raise ValueError(f'{len(reqlatlon_pd_outbounds)} of requested pli points are out of bounds (valid longitude range {lonvar_vals.min()} to {lonvar_vals.max()}, valid latitude range {latvar_vals.min()} to {latvar_vals.max()}):\n{reqlatlon_pd_outbounds}')
+    time_passed = (dt.datetime.now()-dtstart).total_seconds()
+    print(f'>>time passed: {time_passed:.2f} sec')
+
+    return data_interp_loaded
+
+
+def interp_hisnc_to_plipoints(data_xr_his, file_pli, kdtree_k=3, load=True):
+    """
+    interpolate stations in hisfile to points of polyfile
+    """
+    #KDTree, finds minimal eucledian distance between points (haversine would be better). Alternatively sklearn.neighbors.BallTree: tree = BallTree(data_lonlat_pd)
+    
+    datavars_list = list(data_xr_his.data_vars)
+    if len(datavars_list)>5:
+        print('WARNING: more than 5 data_vars, you might want to subset your data_xr_his')
+    #read hisfile and make KDTree of xy of hisstations
+    hisstations_pd = data_xr_his.stations.to_dataframe() #TODO: add check if stations are strings? (whether preprocess_hisnc was used)
+    tree_nest2 = KDTree(hisstations_pd[['station_x_coordinate','station_y_coordinate']])
+    
+    #read polyfile and query k nearest hisstations (names)
+    polyfile_object = hcdfm.PolyFile(file_pli)
+    data_pol_list = []
+    for polyobj in polyfile_object.objects:
+        data_pol_pd_one = pointlike_to_DataFrame(polyobj)
+        data_pol_pd_one['name'] = pd.Series(data_pol_pd_one.index).apply(lambda x: f'{polyobj.metadata.name}_{x+1:04d}')
+        data_pol_list.append(data_pol_pd_one)
+    data_pol_pd = pd.concat(data_pol_list)
+
+    plicoords_distance2, plicoords_nestpointidx = tree_nest2.query(data_pol_pd[['x','y']], k=kdtree_k)
+    da_plicoords_nestpointidx = xr.DataArray(plicoords_nestpointidx, dims=('plipoints','nearestkpoints'))
+    da_plicoords_nestpointnames = data_xr_his.stations.isel(stations=da_plicoords_nestpointidx)
+    
+    #interpolate hisfile variables to plipoints
+    data_interp = xr.Dataset()
+    data_interp['plipoint_x'] = xr.DataArray(data_pol_pd['x'],dims=('plipoints'))
+    data_interp['plipoint_y'] = xr.DataArray(data_pol_pd['y'],dims=('plipoints'))
+    data_interp['plipoint_name'] = xr.DataArray(data_pol_pd['name'].astype('S64'), dims='plipoints').str.decode('utf-8',errors='ignore').str.strip() #TODO: must be possible to do this less complex
+    data_interp = data_interp.set_coords(['plipoint_x','plipoint_y','plipoint_name'])
+    data_interp = data_interp.set_index({'plipoints':'plipoint_name'})
+    
+    for varone in datavars_list:
+        da_dist = xr.DataArray(plicoords_distance2, dims=('plipoints','nearestkpoints'))
+        da_invdistweight = (1/da_dist)/(1/da_dist).sum(dim='nearestkpoints') #TODO: set weigths for invalid points to 0 (and increase others weights so sum remains 1)
+        data_xr_his_pli_knearest = data_xr_his[varone].sel(stations=da_plicoords_nestpointnames)
+        data_interp[varone] = (data_xr_his_pli_knearest * da_invdistweight).sum(dim='nearestkpoints')
+        data_interp[varone].attrs = data_xr_his[varone].attrs #copy units and other attributes
+        
+    if not load:
+        return data_interp
+    
+    print('loading dataset (might take a while, but increases performance of point loop significantly)')
+    data_interp = data_interp.load()
+    print('done')
+
+    return data_interp
+    
+
+def plipointsDataset_to_ForcingModel(plipointsDataset):
+    quantity_list = list(plipointsDataset.data_vars)
+    npoints = len(plipointsDataset.plipoints)
+    
+    #start conversion to Forcingmodel object
+    print(f'Converting {npoints} plipoints to hcdfm.ForcingModel():',end='')
+    dtstart = dt.datetime.now()
+    ForcingModel_object = hcdfm.ForcingModel()
+    for iP in range(npoints):
+        print(f' {iP+1}',end='')
+        
+        #select data for this point, ffill nans, concatenating time column, constructing T3D/TimeSeries and append to hcdfm.ForcingModel()
+        datablock_xr_onepoint = plipointsDataset.isel(plipoints=iP)
+        plipoint_name = str(datablock_xr_onepoint.plipoints.to_numpy())
+        
+        for quan in quantity_list:
+            datablock_xr_onepoint[quan].attrs['locationname'] = plipoint_name #TODO: is there a nicer way of passing this data?
+            if datablock_xr_onepoint[quan].isnull().all(): # check if all values of plipoint are nan (on land)
+                warnings.warn(UserWarning(f'Plipoint "{plipoint_name}" might be on land since it only contain nan values. Consider altering your plifile or using plipointsDataset.ffill(dim="plipoints").bfill(dim="plipoints"). Nan values replaced with 0 to avoid bc-writing errors')) #TODO: maybe fill along plipoints dimension, but beware on nans in deep water that are filled with neighbours
+                datablock_xr_onepoint[quan] = datablock_xr_onepoint[quan].fillna(0)
+        
+        if 'depth' in plipointsDataset.dims:
+            ts_one = Dataset_to_T3D(datablock_xr_onepoint)
+        elif 'amplitude' in quantity_list:
+            ts_one = Dataset_to_Astronomic(datablock_xr_onepoint)
+        else:
+            ts_one = Dataset_to_TimeSeries(datablock_xr_onepoint)
+        ForcingModel_object.forcing.append(ts_one)
+    print(f'. >> done in {(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    return ForcingModel_object
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/linebuilder.py` & `dfm_tools-0.11.0/dfm_tools/linebuilder.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Oct  3 13:40:58 2022
-
-@author: veenstra
-"""
-
-import numpy as np
-
-
-class LineBuilder:
-    """
-    https://matplotlib.org/stable/users/explain/event_handling.html
-    """
-    def __init__(self, line):
-        #self.waiting_for_entry = True
-        self.line = line
-        self.xs = list(line.get_xdata())
-        self.ys = list(line.get_ydata())
-        self.cid = line.figure.canvas.mpl_connect('button_press_event', self)
-
-    def __call__(self, event):
-        print('click', event)
-        # if event.inaxes!=self.line.axes:
-        #     print('WARNING: that click was outside the figure axis')
-        #     return
-        # if event.dblclick:
-        #     print('WARNING: double click is interpreted as single click')
-        #     return
-        if event.inaxes!=self.line.axes: return
-        self.xs.append(event.xdata)
-        self.ys.append(event.ydata)
-        self.line_array = np.c_[self.xs, self.ys]
-        self.line.set_data(self.xs, self.ys)
-        self.line.figure.canvas.draw()
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Oct  3 13:40:58 2022
+
+@author: veenstra
+"""
+
+import numpy as np
+
+
+class LineBuilder:
+    """
+    https://matplotlib.org/stable/users/explain/event_handling.html
+    """
+    def __init__(self, line):
+        #self.waiting_for_entry = True
+        self.line = line
+        self.xs = list(line.get_xdata())
+        self.ys = list(line.get_ydata())
+        self.cid = line.figure.canvas.mpl_connect('button_press_event', self)
+
+    def __call__(self, event):
+        print('click', event)
+        # if event.inaxes!=self.line.axes:
+        #     print('WARNING: that click was outside the figure axis')
+        #     return
+        # if event.dblclick:
+        #     print('WARNING: double click is interpreted as single click')
+        #     return
+        if event.inaxes!=self.line.axes: return
+        self.xs.append(event.xdata)
+        self.ys.append(event.ydata)
+        self.line_array = np.c_[self.xs, self.ys]
+        self.line.set_data(self.xs, self.ys)
+        self.line.figure.canvas.draw()
```

### Comparing `dfm_tools-0.10.55/dfm_tools/meshkernel_helpers.py` & `dfm_tools-0.11.0/dfm_tools/meshkernel_helpers.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Apr  6 18:46:35 2023
-
-@author: veenstra
-"""
-
-import xugrid as xu
-import meshkernel
-import xarray as xr
-import datetime as dt
-import hydrolib.core.dflowfm as hcdfm
-import pandas as pd
-from dfm_tools.hydrolib_helpers import pointlike_to_DataFrame
-from dfm_tools import __version__
-import getpass
-import numpy as np
-
-
-def meshkernel_delete_withpol(mk, file_ldb, minpoints=None):
-    print('>> reading+converting ldb: ',end='')
-    dtstart = dt.datetime.now()
-    pol_ldb = hcdfm.PolyFile(file_ldb)
-    pol_ldb_list = [pointlike_to_DataFrame(x) for x in pol_ldb.objects] #TODO: this is quite slow, speed up possible?
-    if minpoints is not None:
-        pol_ldb_list = [x for x in pol_ldb_list if len(x)>minpoints] #filter only large polygons for performance
-    for iP, pol_ldb in enumerate(pol_ldb_list):
-        if not (pol_ldb.iloc[0] == pol_ldb.iloc[-1]).all(): #close the polygon if it is not yet closed
-            pol_ldb_list[iP] = pd.concat([pol_ldb,pol_ldb.iloc[[0]]],axis=0)
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    for iP, pol_del in enumerate(pol_ldb_list): #TODO: also possible without loop? >> geometry_separator=-999.9 so that value can be used to concat polygons. >> use hydrolib poly as input? https://github.com/Deltares/MeshKernelPy/issues/35
-        delete_pol_geom = meshkernel.GeometryList(x_coordinates=pol_del['x'].to_numpy(), y_coordinates=pol_del['y'].to_numpy()) #TODO: .copy()/to_numpy() makes the array contiguous in memory, which is necessary for meshkernel.mesh2d_delete()
-        mk.mesh2d_delete(geometry_list=delete_pol_geom, 
-                         delete_option=meshkernel.DeleteMeshOption(2), #ALL_COMPLETE_FACES/2: Delete all faces of which the complete face is inside the polygon
-                         invert_deletion=False) #TODO: cuts away link that is neccesary, so results in non-orthogonal grid (probably usecase of english channel?)
-
-
-def meshkernel_to_UgridDataset(mk:meshkernel.meshkernel.MeshKernel, remove_noncontiguous:bool = False) -> xr.Dataset:
-    mesh2d_grid3 = mk.mesh2d_get()
-
-    xu_grid = xu.Ugrid2d.from_meshkernel(mesh2d_grid3)
-    
-    #remove non-contiguous grid parts
-    def xugrid_remove_noncontiguous(grid):
-        #based on https://deltares.github.io/xugrid/examples/connectivity.html#connected-components
-        #uses https://docs.scipy.org/doc/scipy/reference/sparse.csgraph.html
-        #TODO: maybe replace with meshkernel?
-        uda = xu.UgridDataArray(
-            xr.DataArray(np.ones(grid.node_face_connectivity.shape[0]), dims=["face"]), grid
-        )
-        labels = uda.ugrid.connected_components()
-        counts = labels.groupby(labels).count()
-        most_frequent_label = counts["group"][np.argmax(counts.data)].item() #find largest contiguous part
-        labels = labels.where(labels == most_frequent_label, drop=True)
-        grid = labels.grid
-        return grid
-    if remove_noncontiguous:
-        xu_grid = xugrid_remove_noncontiguous(xu_grid)
-    
-    #convert to dataset
-    xu_grid_ds = xu_grid.to_dataset()
-    
-    #convert 0-based to 1-based grid for connectivity variables like face_node_connectivity #TODO: FM kernel needs 1-based grid, but it should read the attributes instead. Report this (#ug_get_meshgeom, #12, ierr=0. ** WARNING: Could not read mesh face x-coordinates)
-    ds_idx = xu_grid_ds.filter_by_attrs(start_index=0)
-    for varn_conn in ds_idx.data_vars:
-        xu_grid_ds[varn_conn] += 1
-        xu_grid_ds[varn_conn].attrs["_FillValue"] += 1
-        xu_grid_ds[varn_conn].attrs["start_index"] += 1
-    
-    xu_grid_ds = xu_grid_ds.assign_attrs({#'Conventions': 'CF-1.8 UGRID-1.0 Deltares-0.10', #add Deltares convention (was CF-1.8 UGRID-1.0)
-                                          'institution': 'Deltares',
-                                          'references': 'https://www.deltares.nl',
-                                          'source': f'Created with meshkernel {meshkernel.__version__}, xugrid {xu.__version__} and dfm_tools {__version__}',
-                                          'history': 'Created on %s, %s'%(dt.datetime.now().strftime('%Y-%m-%dT%H:%M:%S%z'),getpass.getuser()), #TODO: add timezone
-                                          })
-    
-    # add attrs (to projected_coordinate_system/wgs84 empty int variable): #TODO: should depend on is_geographic flag in make_basegrid()
-    # attribute_dict = {
-    #     'name': 'WGS84',
-    #     'epsg': np.array([4326], dtype=int),
-    #     'grid_mapping_name': 'Unknown projected',
-    #     'longitude_of_prime_meridian': np.array([0.0], dtype=float),
-    #     'semi_major_axis': np.array([6378137.0], dtype=float),
-    #     'semi_minor_axis': np.array([6356752.314245], dtype=float),
-    #     'inverse_flattening': np.array([6356752.314245], dtype=float),
-    #     'EPSG_code': 'EPSG:4326',
-    #     'value': 'value is equal to EPSG code'}
-    # xu_grid_ds['wgs84'] = xr.DataArray(np.array(0,dtype=int),dims=(),attrs=attribute_dict)
-    
-    xu_grid_uds = xu.UgridDataset(xu_grid_ds)
-    return xu_grid_uds
-
-
-def make_basegrid(lon_min,lon_max,lat_min,lat_max,dx=0.05,dy=0.05,angle=0):
-    print('modelbuilder.make_basegrid()')
-    # create base grid
-    num_columns = int(np.round((lon_max-lon_min)/dx))
-    num_rows = int(np.round((lat_max-lat_min)/dy))
-    
-    make_grid_parameters = meshkernel.MakeGridParameters(num_columns=num_columns,
-                                                         num_rows=num_rows,
-                                                         angle=angle,
-                                                         origin_x=lon_min,
-                                                         origin_y=lat_min,
-                                                         block_size_x=dx,
-                                                         block_size_y=dy)
-    
-    geometry_list = meshkernel.GeometryList(np.empty(0, dtype=np.double), np.empty(0, dtype=np.double)) # A polygon must to be provided. If empty it will not be used. If a polygon is provided it will be used in the generation of the curvilinear grid. The polygon must be closed
-    mk = meshkernel.MeshKernel() #TODO: is_geographic=True was used in modelbuilder, but refinement super slow and raises "MeshKernelError: MeshRefinement::connect_hanging_nodes: The number of non-hanging nodes is neither 3 nor 4."
-    mk.curvilinear_make_uniform(make_grid_parameters, geometry_list) #TODO: make geometry_list argument optional: https://github.com/Deltares/MeshKernelPy/issues/30
-    mk.curvilinear_convert_to_mesh2d() #convert to ugrid/mesh2d
-    
-    return mk
-
-
-def refine_basegrid(mk, data_bathy_sel,min_face_size=0.1):
-    print('modelbuilder.refine_basegrid()')
-    samp_x,samp_y = np.meshgrid(data_bathy_sel.lon.to_numpy(),data_bathy_sel.lat.to_numpy())
-    samp_z = data_bathy_sel.elevation.to_numpy().astype(float) #TODO: without .astype(float), meshkernelpy generates "TypeError: incompatible types, c_short_Array_27120 instance instead of LP_c_double instance": https://github.com/Deltares/MeshKernelPy/issues/31
-    samp_x = samp_x.ravel()
-    samp_y = samp_y.ravel()
-    samp_z = samp_z.ravel()
-    geomlist = meshkernel.GeometryList(x_coordinates=samp_x, y_coordinates=samp_y, values=samp_z) #TODO: does not check if lenghts of input array is equal (samp_z[1:]) https://github.com/Deltares/MeshKernelPy/issues/32
-    
-    #refinement
-    mesh_refinement_parameters = meshkernel.MeshRefinementParameters(refine_intersected=False, #TODO: provide defaults for several arguments, so less arguments are required
-                                                                     use_mass_center_when_refining=False, #TODO: what does this do?
-                                                                     min_face_size=min_face_size, #TODO: size in meters would be more convenient: https://github.com/Deltares/MeshKernelPy/issues/33
-                                                                     refinement_type=meshkernel.RefinementType(1), #Wavecourant/1,
-                                                                     connect_hanging_nodes=True, #set to False to do multiple refinement steps (e.g. for multiple regions)
-                                                                     account_for_samples_outside_face=True, #outsidecell argument for --refine?
-                                                                     max_refinement_iterations=5,
-                                                                     ) #TODO: missing the arguments dtmax (necessary?), hmin (min_face_size but then in meters instead of degrees), smoothiters (currently refinement is patchy along coastlines, goes good in dflowfm exec after additional implementation of HK), spherical 1/0 (necessary?)
-    
-    mk.mesh2d_refine_based_on_samples(samples=geomlist,
-                                       relative_search_radius=0.5, #TODO: bilin interp is preferred, but this is currently not supported (samples have to be ravelled): https://github.com/Deltares/MeshKernelPy/issues/34
-                                       minimum_num_samples=3,
-                                       mesh_refinement_params=mesh_refinement_parameters,
-                                       )
-    
-    return mk
-
-
-def generate_bndpli(lon_min, lon_max, lat_min, lat_max, dlon, dlat, name='bnd'): #TODO: maybe generate with meshkernel?
-
-    vals_lon_ar = np.arange(lon_min, lon_max, dlon)
-    vals_lon = np.linspace(lon_min, lon_max,len(vals_lon_ar))
-    vals_lat_ar = np.arange(lat_min, lat_max, dlat)
-    vals_lat = np.linspace(lat_min, lat_max,len(vals_lat_ar))
-    pli_p1 = np.c_[np.repeat(lon_min,len(vals_lat)),vals_lat]
-    pli_p2 = np.c_[vals_lon,np.repeat(lat_max,len(vals_lon))]
-    pli_p3 = np.c_[np.repeat(lon_max,len(vals_lat)),vals_lat[::-1]]
-    pli_p4 = np.c_[vals_lon[::-1],np.repeat(lat_min,len(vals_lon))]
-    
-    pli_all = np.concatenate([pli_p1[:-1],pli_p2[:-1],pli_p3[:-1],pli_p4[:-1]],axis=0)
-    
-    pli_polyobject = hcdfm.PolyObject(metadata=hcdfm.Metadata(name=name, n_rows=pli_all.shape[0], n_columns=pli_all.shape[1]),
-                                      points=[hcdfm.Point(x=x,y=y,data=[]) for x,y in pli_all])
-    pli_polyfile = hcdfm.PolyFile(objects=[pli_polyobject])
-    return pli_polyfile
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Apr  6 18:46:35 2023
+
+@author: veenstra
+"""
+
+import xugrid as xu
+import meshkernel
+import xarray as xr
+import datetime as dt
+import hydrolib.core.dflowfm as hcdfm
+import pandas as pd
+from dfm_tools.hydrolib_helpers import pointlike_to_DataFrame
+from dfm_tools import __version__
+import getpass
+import numpy as np
+
+
+def meshkernel_delete_withpol(mk, file_ldb, minpoints=None):
+    print('>> reading+converting ldb: ',end='')
+    dtstart = dt.datetime.now()
+    pol_ldb = hcdfm.PolyFile(file_ldb)
+    pol_ldb_list = [pointlike_to_DataFrame(x) for x in pol_ldb.objects] #TODO: this is quite slow, speed up possible?
+    if minpoints is not None:
+        pol_ldb_list = [x for x in pol_ldb_list if len(x)>minpoints] #filter only large polygons for performance
+    for iP, pol_ldb in enumerate(pol_ldb_list):
+        if not (pol_ldb.iloc[0] == pol_ldb.iloc[-1]).all(): #close the polygon if it is not yet closed
+            pol_ldb_list[iP] = pd.concat([pol_ldb,pol_ldb.iloc[[0]]],axis=0)
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    for iP, pol_del in enumerate(pol_ldb_list): #TODO: also possible without loop? >> geometry_separator=-999.9 so that value can be used to concat polygons. >> use hydrolib poly as input? https://github.com/Deltares/MeshKernelPy/issues/35
+        delete_pol_geom = meshkernel.GeometryList(x_coordinates=pol_del['x'].to_numpy(), y_coordinates=pol_del['y'].to_numpy()) #TODO: .copy()/to_numpy() makes the array contiguous in memory, which is necessary for meshkernel.mesh2d_delete()
+        mk.mesh2d_delete(geometry_list=delete_pol_geom, 
+                         delete_option=meshkernel.DeleteMeshOption(2), #ALL_COMPLETE_FACES/2: Delete all faces of which the complete face is inside the polygon
+                         invert_deletion=False) #TODO: cuts away link that is neccesary, so results in non-orthogonal grid (probably usecase of english channel?)
+
+
+def meshkernel_to_UgridDataset(mk:meshkernel.meshkernel.MeshKernel, remove_noncontiguous:bool = False) -> xr.Dataset:
+    mesh2d_grid3 = mk.mesh2d_get()
+
+    xu_grid = xu.Ugrid2d.from_meshkernel(mesh2d_grid3)
+    
+    #remove non-contiguous grid parts
+    def xugrid_remove_noncontiguous(grid):
+        #based on https://deltares.github.io/xugrid/examples/connectivity.html#connected-components
+        #uses https://docs.scipy.org/doc/scipy/reference/sparse.csgraph.html
+        #TODO: maybe replace with meshkernel?
+        uda = xu.UgridDataArray(
+            xr.DataArray(np.ones(grid.node_face_connectivity.shape[0]), dims=["face"]), grid
+        )
+        labels = uda.ugrid.connected_components()
+        counts = labels.groupby(labels).count()
+        most_frequent_label = counts["group"][np.argmax(counts.data)].item() #find largest contiguous part
+        labels = labels.where(labels == most_frequent_label, drop=True)
+        grid = labels.grid
+        return grid
+    if remove_noncontiguous:
+        xu_grid = xugrid_remove_noncontiguous(xu_grid)
+    
+    #convert to dataset
+    xu_grid_ds = xu_grid.to_dataset()
+    
+    #convert 0-based to 1-based grid for connectivity variables like face_node_connectivity #TODO: FM kernel needs 1-based grid, but it should read the attributes instead. Report this (#ug_get_meshgeom, #12, ierr=0. ** WARNING: Could not read mesh face x-coordinates)
+    ds_idx = xu_grid_ds.filter_by_attrs(start_index=0)
+    for varn_conn in ds_idx.data_vars:
+        xu_grid_ds[varn_conn] += 1
+        xu_grid_ds[varn_conn].attrs["_FillValue"] += 1
+        xu_grid_ds[varn_conn].attrs["start_index"] += 1
+    
+    xu_grid_ds = xu_grid_ds.assign_attrs({#'Conventions': 'CF-1.8 UGRID-1.0 Deltares-0.10', #add Deltares convention (was CF-1.8 UGRID-1.0)
+                                          'institution': 'Deltares',
+                                          'references': 'https://www.deltares.nl',
+                                          'source': f'Created with meshkernel {meshkernel.__version__}, xugrid {xu.__version__} and dfm_tools {__version__}',
+                                          'history': 'Created on %s, %s'%(dt.datetime.now().strftime('%Y-%m-%dT%H:%M:%S%z'),getpass.getuser()), #TODO: add timezone
+                                          })
+    
+    # add attrs (to projected_coordinate_system/wgs84 empty int variable): #TODO: should depend on is_geographic flag in make_basegrid()
+    # attribute_dict = {
+    #     'name': 'WGS84',
+    #     'epsg': np.array([4326], dtype=int),
+    #     'grid_mapping_name': 'Unknown projected',
+    #     'longitude_of_prime_meridian': np.array([0.0], dtype=float),
+    #     'semi_major_axis': np.array([6378137.0], dtype=float),
+    #     'semi_minor_axis': np.array([6356752.314245], dtype=float),
+    #     'inverse_flattening': np.array([6356752.314245], dtype=float),
+    #     'EPSG_code': 'EPSG:4326',
+    #     'value': 'value is equal to EPSG code'}
+    # xu_grid_ds['wgs84'] = xr.DataArray(np.array(0,dtype=int),dims=(),attrs=attribute_dict)
+    
+    xu_grid_uds = xu.UgridDataset(xu_grid_ds)
+    return xu_grid_uds
+
+
+def make_basegrid(lon_min,lon_max,lat_min,lat_max,dx=0.05,dy=0.05,angle=0):
+    print('modelbuilder.make_basegrid()')
+    # create base grid
+    num_columns = int(np.round((lon_max-lon_min)/dx))
+    num_rows = int(np.round((lat_max-lat_min)/dy))
+    
+    make_grid_parameters = meshkernel.MakeGridParameters(num_columns=num_columns,
+                                                         num_rows=num_rows,
+                                                         angle=angle,
+                                                         origin_x=lon_min,
+                                                         origin_y=lat_min,
+                                                         block_size_x=dx,
+                                                         block_size_y=dy)
+    
+    geometry_list = meshkernel.GeometryList(np.empty(0, dtype=np.double), np.empty(0, dtype=np.double)) # A polygon must to be provided. If empty it will not be used. If a polygon is provided it will be used in the generation of the curvilinear grid. The polygon must be closed
+    mk = meshkernel.MeshKernel() #TODO: is_geographic=True was used in modelbuilder, but refinement super slow and raises "MeshKernelError: MeshRefinement::connect_hanging_nodes: The number of non-hanging nodes is neither 3 nor 4."
+    mk.curvilinear_make_uniform(make_grid_parameters, geometry_list) #TODO: make geometry_list argument optional: https://github.com/Deltares/MeshKernelPy/issues/30
+    mk.curvilinear_convert_to_mesh2d() #convert to ugrid/mesh2d
+    
+    return mk
+
+
+def refine_basegrid(mk, data_bathy_sel,min_face_size=0.1):
+    print('modelbuilder.refine_basegrid()')
+    samp_x,samp_y = np.meshgrid(data_bathy_sel.lon.to_numpy(),data_bathy_sel.lat.to_numpy())
+    samp_z = data_bathy_sel.elevation.to_numpy().astype(float) #TODO: without .astype(float), meshkernelpy generates "TypeError: incompatible types, c_short_Array_27120 instance instead of LP_c_double instance": https://github.com/Deltares/MeshKernelPy/issues/31
+    samp_x = samp_x.ravel()
+    samp_y = samp_y.ravel()
+    samp_z = samp_z.ravel()
+    geomlist = meshkernel.GeometryList(x_coordinates=samp_x, y_coordinates=samp_y, values=samp_z) #TODO: does not check if lenghts of input array is equal (samp_z[1:]) https://github.com/Deltares/MeshKernelPy/issues/32
+    
+    #refinement
+    mesh_refinement_parameters = meshkernel.MeshRefinementParameters(refine_intersected=False, #TODO: provide defaults for several arguments, so less arguments are required
+                                                                     use_mass_center_when_refining=False, #TODO: what does this do?
+                                                                     min_face_size=min_face_size, #TODO: size in meters would be more convenient: https://github.com/Deltares/MeshKernelPy/issues/33
+                                                                     refinement_type=meshkernel.RefinementType(1), #Wavecourant/1,
+                                                                     connect_hanging_nodes=True, #set to False to do multiple refinement steps (e.g. for multiple regions)
+                                                                     account_for_samples_outside_face=True, #outsidecell argument for --refine?
+                                                                     max_refinement_iterations=5,
+                                                                     ) #TODO: missing the arguments dtmax (necessary?), hmin (min_face_size but then in meters instead of degrees), smoothiters (currently refinement is patchy along coastlines, goes good in dflowfm exec after additional implementation of HK), spherical 1/0 (necessary?)
+    
+    mk.mesh2d_refine_based_on_samples(samples=geomlist,
+                                       relative_search_radius=0.5, #TODO: bilin interp is preferred, but this is currently not supported (samples have to be ravelled): https://github.com/Deltares/MeshKernelPy/issues/34
+                                       minimum_num_samples=3,
+                                       mesh_refinement_params=mesh_refinement_parameters,
+                                       )
+    
+    return mk
+
+
+def generate_bndpli(lon_min, lon_max, lat_min, lat_max, dlon, dlat, name='bnd'): #TODO: maybe generate with meshkernel?
+
+    vals_lon_ar = np.arange(lon_min, lon_max, dlon)
+    vals_lon = np.linspace(lon_min, lon_max,len(vals_lon_ar))
+    vals_lat_ar = np.arange(lat_min, lat_max, dlat)
+    vals_lat = np.linspace(lat_min, lat_max,len(vals_lat_ar))
+    pli_p1 = np.c_[np.repeat(lon_min,len(vals_lat)),vals_lat]
+    pli_p2 = np.c_[vals_lon,np.repeat(lat_max,len(vals_lon))]
+    pli_p3 = np.c_[np.repeat(lon_max,len(vals_lat)),vals_lat[::-1]]
+    pli_p4 = np.c_[vals_lon[::-1],np.repeat(lat_min,len(vals_lon))]
+    
+    pli_all = np.concatenate([pli_p1[:-1],pli_p2[:-1],pli_p3[:-1],pli_p4[:-1]],axis=0)
+    
+    pli_polyobject = hcdfm.PolyObject(metadata=hcdfm.Metadata(name=name, n_rows=pli_all.shape[0], n_columns=pli_all.shape[1]),
+                                      points=[hcdfm.Point(x=x,y=y,data=[]) for x,y in pli_all])
+    pli_polyfile = hcdfm.PolyFile(objects=[pli_polyobject])
+    return pli_polyfile
+
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/modplot.py` & `dfm_tools-0.11.0/dfm_tools/modplot.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,704 +1,704 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 25 15:26:55 2020
-
-@author: Kieran Hunt
-https://github.com/kieranmrhunt/curved-quivers/blob/master/modplot.py
-https://stackoverflow.com/questions/51843313/flow-visualisation-in-python-using-curved-path-following-vectors
-aligned with matplotlib.streamplot and improved by Jelmer Veenstra (30-03-2023), https://github.com/veenstrajelmer
-matplotlib.streamplot available at https://raw.githubusercontent.com/matplotlib/matplotlib/main/lib/matplotlib/streamplot.py
-
-Streamline plotting for 2D vector fields.
-
-"""
-
-import numpy as np
-
-import matplotlib as mpl
-from matplotlib import _api, cm, patches
-import matplotlib.colors as mcolors
-import matplotlib.collections as mcollections
-import matplotlib.lines as mlines
-
-
-__all__ = ['velovect']
-
-
-def velovect(axes, x, y, u, v, density=1, linewidth=None, color=None,
-               cmap=None, norm=None, arrowsize=1, arrowstyle='-|>',
-               transform=None, zorder=None, start_points=None,
-               integration_direction='both',
-               grains=15,
-               broken_streamlines=True):
-    """
-    Draw streamlines of a vector flow.
-
-    Parameters
-    ----------
-    x, y : 1D/2D arrays
-        Evenly spaced strictly increasing arrays to make a grid.  If 2D, all
-        rows of *x* must be equal and all columns of *y* must be equal; i.e.,
-        they must be as if generated by ``np.meshgrid(x_1d, y_1d)``.
-    u, v : 2D arrays
-        *x* and *y*-velocities. The number of rows and columns must match
-        the length of *y* and *x*, respectively.
-    density : float or (float, float)
-        Controls the closeness of streamlines. When ``density = 1``, the domain
-        is divided into a 30x30 grid. *density* linearly scales this grid.
-        Each cell in the grid can have, at most, one traversing streamline.
-        For different densities in each direction, use a tuple
-        (density_x, density_y).
-    linewidth : float or 2D array
-        The width of the streamlines. With a 2D array the line width can be
-        varied across the grid. The array must have the same shape as *u*
-        and *v*.
-    color : color or 2D array
-        The streamline color. If given an array, its values are converted to
-        colors using *cmap* and *norm*.  The array must have the same shape
-        as *u* and *v*.
-    cmap, norm
-        Data normalization and colormapping parameters for *color*; only used
-        if *color* is an array of floats. See `~.Axes.imshow` for a detailed
-        description.
-    arrowsize : float
-        Scaling factor for the arrow size.
-    arrowstyle : str
-        Arrow style specification.
-        See `~matplotlib.patches.FancyArrowPatch`.
-    minlength : float
-        Minimum length of streamline in axes coordinates.
-    start_points : (N, 2) array
-        Coordinates of starting points for the streamlines in data coordinates
-        (the same coordinates as the *x* and *y* arrays).
-    zorder : float
-        The zorder of the streamlines and arrows.
-        Artists with lower zorder values are drawn first.
-    maxlength : float
-        Maximum length of streamline in axes coordinates.
-    integration_direction : {'forward', 'backward', 'both'}, default: 'both'
-        Integrate the streamline in forward, backward or both directions.
-    data : indexable object, optional
-        DATA_PARAMETER_PLACEHOLDER
-    broken_streamlines : boolean, default: True
-        If False, forces streamlines to continue until they
-        leave the plot domain.  If True, they may be terminated if they
-        come too close to another streamline.
-
-    Returns
-    -------
-    StreamplotSet
-        Container object with attributes
- 
-        - ``lines``: `.LineCollection` of streamlines
-
-        - ``arrows``: `.PatchCollection` containing `.FancyArrowPatch`
-          objects representing the arrows half-way along streamlines.
-
-            This container will probably change in the future to allow changes
-            to the colormap, alpha, etc. for both lines and arrows, but these
-            changes should be backward compatible.
-    """
-    grid = Grid(x, y)
-    mask = StreamMask(10)
-    dmap = DomainMap(grid, mask)
-
-    if zorder is None:
-        zorder = mlines.Line2D.zorder
-
-    # default to data coordinates
-    if transform is None:
-        transform = axes.transData
-
-    if color is None:
-        color = axes._get_lines.get_next_color()
-
-    if linewidth is None:
-        linewidth = mpl.rcParams['lines.linewidth']
-
-    line_kw = {}
-    arrow_kw = dict(arrowstyle=arrowstyle, mutation_scale=10 * arrowsize)
-
-    _api.check_in_list(['both', 'forward', 'backward'],
-                       integration_direction=integration_direction)
-
-    #if integration_direction == 'both': #done for magnitude
-    #    maxlength /= 2.
-
-    use_multicolor_lines = isinstance(color, np.ndarray)
-    if use_multicolor_lines:
-        if color.shape != grid.shape:
-            raise ValueError("If 'color' is given, it must match the shape of "
-                             "the (x, y) grid")
-        line_colors = [[]]  # Empty entry allows concatenation of zero arrays.
-        color = np.ma.masked_invalid(color)
-    else:
-        line_kw['color'] = color
-        arrow_kw['color'] = color
-
-    if isinstance(linewidth, np.ndarray):
-        if linewidth.shape != grid.shape:
-            raise ValueError("If 'linewidth' is given, it must match the "
-                             "shape of the (x, y) grid")
-        line_kw['linewidth'] = []
-    else:
-        line_kw['linewidth'] = linewidth
-        arrow_kw['linewidth'] = linewidth
-
-    line_kw['zorder'] = zorder
-    arrow_kw['zorder'] = zorder
-
-    # Sanity checks.
-    if u.shape != grid.shape or v.shape != grid.shape:
-        raise ValueError("'u' and 'v' must match the shape of the (x, y) grid")
-
-    u = np.ma.masked_invalid(u)
-    v = np.ma.masked_invalid(v)
-    magnitude = np.sqrt(u**2 + v**2)
-    magnitude/=np.max(magnitude)
-    if integration_direction == 'both':
-        magnitude /= 2.
-	
-    resolution = density/np.max(grains)
-    integrate = _get_integrator(u, v, dmap, resolution, magnitude, integration_direction)
-
-    trajectories = []    
-   
-    if start_points is None:
-        start_points=_gen_starting_points(x,y,grains)
-    
-    sp2 = np.asanyarray(start_points, dtype=float).copy()
-
-    # Check if start_points are outside the data boundaries
-    for xs, ys in sp2:
-        if not (grid.x_origin <= xs <= grid.x_origin + grid.width and
-                grid.y_origin <= ys <= grid.y_origin + grid.height):
-                raise ValueError(f"Starting point ({xs}, {ys}) outside of "
-                                 "data boundaries")
-
-    # Convert start_points from data to array coords
-    # Shift the seed points from the bottom left of the data so that
-    # data2grid works properly.
-    sp2[:, 0] -= grid.x_origin
-    sp2[:, 1] -= grid.y_origin
-
-    for xs, ys in sp2:
-        xg, yg = dmap.data2grid(xs, ys)
-        # Floating point issues can cause xg, yg to be slightly out of
-        # bounds for xs, ys on the upper boundaries. Because we have
-        # already checked that the starting points are within the original
-        # grid, clip the xg, yg to the grid to work around this issue
-        xg = np.clip(xg, 0, grid.nx - 1)
-        yg = np.clip(yg, 0, grid.ny - 1)
-        
-        t = integrate(xg, yg, broken_streamlines)
-        if t is not None:
-            trajectories.append(t)
-
-    if use_multicolor_lines:
-        if norm is None:
-            norm = mcolors.Normalize(color.min(), color.max())
-        cmap = cm._ensure_cmap(cmap)
-
-    streamlines = []
-    arrows = []
-    for t in trajectories:
-        tgx, tgy = t.T
-        # Rescale from grid-coordinates to data-coordinates.
-        tx, ty = dmap.grid2data(tgx, tgy)
-        tx += grid.x_origin
-        ty += grid.y_origin
-
-        # Create multiple tiny segments if varying width or color is given
-        if isinstance(linewidth, np.ndarray) or use_multicolor_lines:
-            points = np.transpose([tx, ty]).reshape(-1, 1, 2)
-            streamlines.extend(np.hstack([points[:-1], points[1:]]))
-        else:
-            points = np.transpose([tx, ty])
-            streamlines.append(points)
-
-        # Add arrows halfway along each trajectory.
-        s = np.cumsum(np.hypot(np.diff(tx), np.diff(ty)))
-        n = np.searchsorted(s, s[-1])
-        arrow_tail = (tx[n], ty[n])
-        arrow_head = (np.mean(tx[n:n + 2]), np.mean(ty[n:n + 2]))
-
-        if isinstance(linewidth, np.ndarray):
-            line_widths = interpgrid(linewidth, tgx, tgy)[:-1]
-            line_kw['linewidth'].extend(line_widths)
-            arrow_kw['linewidth'] = line_widths[n]
-
-        if use_multicolor_lines:
-            color_values = interpgrid(color, tgx, tgy)[:-1]
-            line_colors.append(color_values)
-            arrow_kw['color'] = cmap(norm(color_values[n]))
-
-        p = patches.FancyArrowPatch(
-            arrow_tail, arrow_head, transform=transform, **arrow_kw)
-        arrows.append(p)
-        
-    lc = mcollections.LineCollection(
-        streamlines, transform=transform, **line_kw)
-    lc.sticky_edges.x[:] = [grid.x_origin, grid.x_origin + grid.width]
-    lc.sticky_edges.y[:] = [grid.y_origin, grid.y_origin + grid.height]
-    if use_multicolor_lines:
-        lc.set_array(np.ma.hstack(line_colors))
-        lc.set_cmap(cmap)
-        lc.set_norm(norm)
-    axes.add_collection(lc)
-
-    ac = mcollections.PatchCollection(arrows)
-    # Adding the collection itself is broken; see #2341.
-    for p in arrows:
-        axes.add_patch(p)
-
-    axes.autoscale_view()
-    stream_container = StreamplotSet(lc, ac)
-    return stream_container
-
-	
-class StreamplotSet:
-
-    def __init__(self, lines, arrows):
-        self.lines = lines
-        self.arrows = arrows
-
-
-# Coordinate definitions
-# ========================
-
-class DomainMap:
-    """
-    Map representing different coordinate systems.
-
-    Coordinate definitions:
-
-    * axes-coordinates goes from 0 to 1 in the domain.
-    * data-coordinates are specified by the input x-y coordinates.
-    * grid-coordinates goes from 0 to N and 0 to M for an N x M grid,
-      where N and M match the shape of the input data.
-    * mask-coordinates goes from 0 to N and 0 to M for an N x M mask,
-      where N and M are user-specified to control the density of streamlines.
-
-    This class also has methods for adding trajectories to the StreamMask.
-    Before adding a trajectory, run `start_trajectory` to keep track of regions
-    crossed by a given trajectory. Later, if you decide the trajectory is bad
-    (e.g., if the trajectory is very short) just call `undo_trajectory`.
-    """
-
-    def __init__(self, grid, mask):
-        self.grid = grid
-        self.mask = mask
-        # Constants for conversion between grid- and mask-coordinates
-        self.x_grid2mask = (mask.nx - 1) / (grid.nx - 1)
-        self.y_grid2mask = (mask.ny - 1) / (grid.ny - 1)
-
-        self.x_mask2grid = 1. / self.x_grid2mask
-        self.y_mask2grid = 1. / self.y_grid2mask
-
-        self.x_data2grid = 1. / grid.dx
-        self.y_data2grid = 1. / grid.dy
-
-    def grid2mask(self, xi, yi):
-        """Return nearest space in mask-coords from given grid-coords."""
-        return round(xi * self.x_grid2mask), round(yi * self.y_grid2mask)
-
-    def mask2grid(self, xm, ym):
-        return xm * self.x_mask2grid, ym * self.y_mask2grid
-
-    def data2grid(self, xd, yd):
-        return xd * self.x_data2grid, yd * self.y_data2grid
-
-    def grid2data(self, xg, yg):
-        return xg / self.x_data2grid, yg / self.y_data2grid
-
-    def start_trajectory(self, xg, yg, broken_streamlines=True):
-        xm, ym = self.grid2mask(xg, yg)
-        self.mask._start_trajectory(xm, ym, broken_streamlines)
-
-    def reset_start_point(self, xg, yg):
-        xm, ym = self.grid2mask(xg, yg)
-        self.mask._current_xy = (xm, ym)
-
-    def update_trajectory(self, xg, yg, broken_streamlines=True):
-        if not self.grid.within_grid(xg, yg):
-            raise InvalidIndexError
-        xm, ym = self.grid2mask(xg, yg)
-        self.mask._update_trajectory(xm, ym, broken_streamlines)
-
-    def undo_trajectory(self):
-        self.mask._undo_trajectory()
-
-
-class Grid:
-    """Grid of data."""
-    def __init__(self, x, y):
-
-        if np.ndim(x) == 1:
-            pass
-        elif np.ndim(x) == 2:
-            x_row = x[0]
-            if not np.allclose(x_row, x):
-                raise ValueError("The rows of 'x' must be equal")
-            x = x_row
-        else:
-            raise ValueError("'x' can have at maximum 2 dimensions")
-
-        if np.ndim(y) == 1:
-            pass
-        elif np.ndim(y) == 2:
-            yt = np.transpose(y)  # Also works for nested lists.
-            y_col = yt[0]
-            if not np.allclose(y_col, yt):
-                raise ValueError("The columns of 'y' must be equal")
-            y = y_col
-        else:
-            raise ValueError("'y' can have at maximum 2 dimensions")
-
-        if not (np.diff(x) > 0).all():
-            raise ValueError("'x' must be strictly increasing")
-        if not (np.diff(y) > 0).all():
-            raise ValueError("'y' must be strictly increasing")
-
-        self.nx = len(x)
-        self.ny = len(y)
-
-        self.dx = x[1] - x[0]
-        self.dy = y[1] - y[0]
-
-        self.x_origin = x[0]
-        self.y_origin = y[0]
-
-        self.width = x[-1] - x[0]
-        self.height = y[-1] - y[0]
-
-        if not np.allclose(np.diff(x), self.width / (self.nx - 1)):
-            raise ValueError("'x' values must be equally spaced")
-        if not np.allclose(np.diff(y), self.height / (self.ny - 1)):
-            raise ValueError("'y' values must be equally spaced")
-
-    @property
-    def shape(self):
-        return self.ny, self.nx
-
-    def within_grid(self, xi, yi):
-        """Return whether (*xi*, *yi*) is a valid index of the grid."""
-        # Note that xi/yi can be floats; so, for example, we can't simply check
-        # `xi < self.nx` since *xi* can be `self.nx - 1 < xi < self.nx`
-        return 0 <= xi <= self.nx - 1 and 0 <= yi <= self.ny - 1
-
-
-class StreamMask:
-    """
-    Mask to keep track of discrete regions crossed by streamlines.
-
-    The resolution of this grid determines the approximate spacing between
-    trajectories. Streamlines are only allowed to pass through zeroed cells:
-    When a streamline enters a cell, that cell is set to 1, and no new
-    streamlines are allowed to enter.
-    """
-
-    def __init__(self, density):
-        try:
-            self.nx, self.ny = (30 * np.broadcast_to(density, 2)).astype(int)
-        except ValueError as err:
-            raise ValueError("'density' must be a scalar or be of length "
-                             "2") from err
-        if self.nx < 0 or self.ny < 0:
-            raise ValueError("'density' must be positive")
-        self._mask = np.zeros((self.ny, self.nx))
-        self.shape = self._mask.shape
-
-        self._current_xy = None
-
-    def __getitem__(self, args):
-        return self._mask[args]
-
-    def _start_trajectory(self, xm, ym, broken_streamlines=True):
-        """Start recording streamline trajectory"""
-        self._traj = []
-        self._update_trajectory(xm, ym, broken_streamlines)
-
-    def _undo_trajectory(self):
-        """Remove current trajectory from mask"""
-        for t in self._traj:
-            self._mask[t] = 0
-
-    def _update_trajectory(self, xm, ym, broken_streamlines=True):
-        """
-        Update current trajectory position in mask.
-
-        If the new position has already been filled, raise `InvalidIndexError`.
-        """
-        if self._current_xy != (xm, ym):
-            if self[ym, xm] == 0:
-                self._traj.append((ym, xm))
-                self._mask[ym, xm] = 1
-                self._current_xy = (xm, ym)
-            else:
-                if broken_streamlines:
-                    raise InvalidIndexError
-                else:
-                    pass
-
-
-class InvalidIndexError(Exception):
-    pass
-
-
-class TerminateTrajectory(Exception):
-    pass
-
-
-# Integrator definitions
-# =======================
-
-def _get_integrator(u, v, dmap, resolution, magnitude, integration_direction):
-
-    # rescale velocity onto grid-coordinates for integrations.
-    u, v = dmap.data2grid(u, v)
-
-    # speed (path length) will be in axes-coordinates
-    u_ax = u / (dmap.grid.nx - 1)
-    v_ax = v / (dmap.grid.ny - 1)
-    speed = np.ma.sqrt(u_ax ** 2 + v_ax ** 2)
-
-    def forward_time(xi, yi):
-        if not dmap.grid.within_grid(xi, yi):
-            raise OutOfBounds
-        ds_dt = interpgrid(speed, xi, yi)
-        if ds_dt == 0:
-            raise TerminateTrajectory()
-        dt_ds = 1. / ds_dt
-        ui = interpgrid(u, xi, yi)
-        vi = interpgrid(v, xi, yi)
-        return ui * dt_ds, vi * dt_ds
-
-    def backward_time(xi, yi):
-        dxi, dyi = forward_time(xi, yi)
-        return -dxi, -dyi
-
-    def integrate(x0, y0, broken_streamlines=True):
-        """
-        Return x, y grid-coordinates of trajectory based on starting point.
-
-        Integrate both forward and backward in time from starting point in
-        grid coordinates.
-
-        Integration is terminated when a trajectory reaches a domain boundary
-        or when it crosses into an already occupied cell in the StreamMask. The
-        resulting trajectory is None if it is shorter than `minlength`.
-        """
-
-        stotal, xy_traj = 0., []
-
-        try:
-            dmap.start_trajectory(x0, y0, broken_streamlines)
-        except InvalidIndexError:
-            return None
-        if integration_direction in ['both', 'backward']:
-            s, xyt = _integrate_rk12(x0, y0, dmap, backward_time, resolution, magnitude,
-                                     broken_streamlines)
-            stotal += s
-            xy_traj += xyt[::-1]
-
-        if integration_direction in ['both', 'forward']:
-            dmap.reset_start_point(x0, y0)
-            s, xyt = _integrate_rk12(x0, y0, dmap, forward_time, resolution, magnitude,
-                                     broken_streamlines)
-            stotal += s
-            xy_traj += xyt[1:]
-
-        if len(xy_traj) > 1:
-            return np.broadcast_arrays(xy_traj, np.empty((1, 2)))[0]
-        else:  # reject short trajectories
-            dmap.undo_trajectory()
-            return None
-
-    return integrate
-
-
-class OutOfBounds(IndexError):
-    pass
-
-
-def _integrate_rk12(x0, y0, dmap, f, resolution, magnitude, broken_streamlines=True):
-    """
-    2nd-order Runge-Kutta algorithm with adaptive step size.
-
-    This method is also referred to as the improved Euler's method, or Heun's
-    method. This method is favored over higher-order methods because:
-
-    1. To get decent looking trajectories and to sample every mask cell
-       on the trajectory we need a small timestep, so a lower order
-       solver doesn't hurt us unless the data is *very* high resolution.
-       In fact, for cases where the user inputs
-       data smaller or of similar grid size to the mask grid, the higher
-       order corrections are negligible because of the very fast linear
-       interpolation used in `interpgrid`.
-
-    2. For high resolution input data (i.e. beyond the mask
-       resolution), we must reduce the timestep. Therefore, an adaptive
-       timestep is more suited to the problem as this would be very hard
-       to judge automatically otherwise.
-
-    This integrator is about 1.5 - 2x as fast as RK4 and RK45 solvers (using
-    similar Python implementations) in most setups.
-    """
-    # This error is below that needed to match the RK4 integrator. It
-    # is set for visual reasons -- too low and corners start
-    # appearing ugly and jagged. Can be tuned.
-    maxerror = 0.003
-
-    # This limit is important (for all integrators) to avoid the
-    # trajectory skipping some mask cells. We could relax this
-    # condition if we use the code which is commented out below to
-    # increment the location gradually. However, due to the efficient
-    # nature of the interpolation, this doesn't boost speed by much
-    # for quite a bit of complexity.
-    maxds = min(1. / dmap.mask.nx, 1. / dmap.mask.ny, 0.1)
-
-    ds = maxds
-    stotal = 0
-    xi = x0
-    yi = y0
-    xyf_traj = []
-    m_total = []
-    
-    while True:
-        try:
-            if dmap.grid.within_grid(xi, yi):
-                xyf_traj.append((xi, yi))
-                m_total.append(interpgrid(magnitude, xi, yi))
-                maxlength = resolution*np.mean(m_total)
-            else:
-                raise OutOfBounds
-
-            # Compute the two intermediate gradients.
-            # f should raise OutOfBounds if the locations given are
-            # outside the grid.
-            k1x, k1y = f(xi, yi)
-            k2x, k2y = f(xi + ds * k1x, yi + ds * k1y)
-
-        except OutOfBounds:
-            # Out of the domain during this step.
-            # Take an Euler step to the boundary to improve neatness
-            # unless the trajectory is currently empty.
-            if xyf_traj:
-                ds, xyf_traj = _euler_step(xyf_traj, dmap, f)
-                stotal += ds
-            break
-        except TerminateTrajectory:
-            break
-
-        dx1 = ds * k1x
-        dy1 = ds * k1y
-        dx2 = ds * 0.5 * (k1x + k2x)
-        dy2 = ds * 0.5 * (k1y + k2y)
-
-        ny, nx = dmap.grid.shape
-        # Error is normalized to the axes coordinates
-        error = np.hypot((dx2 - dx1) / (nx - 1), (dy2 - dy1) / (ny - 1))
-
-        # Only save step if within error tolerance
-        if error < maxerror:
-            xi += dx2
-            yi += dy2
-            try:
-                dmap.update_trajectory(xi, yi, broken_streamlines)
-            except InvalidIndexError:
-                break
-            if stotal + ds > maxlength:
-                break
-            stotal += ds
-
-        # recalculate stepsize based on step error
-        if error == 0:
-            ds = maxds
-        else:
-            ds = min(maxds, 0.85 * ds * (maxerror / error) ** 0.5)
-
-    return stotal, xyf_traj
-
-
-def _euler_step(xyf_traj, dmap, f):
-    """Simple Euler integration step that extends streamline to boundary."""
-    ny, nx = dmap.grid.shape
-    xi, yi = xyf_traj[-1]
-    cx, cy = f(xi, yi)
-    if cx == 0:
-        dsx = np.inf
-    elif cx < 0:
-        dsx = xi / -cx
-    else:
-        dsx = (nx - 1 - xi) / cx
-    if cy == 0:
-        dsy = np.inf
-    elif cy < 0:
-        dsy = yi / -cy
-    else:
-        dsy = (ny - 1 - yi) / cy
-    ds = min(dsx, dsy)
-    xyf_traj.append((xi + cx * ds, yi + cy * ds))
-    return ds, xyf_traj
-
-
-# Utility functions
-# ========================
-
-def interpgrid(a, xi, yi):
-    """Fast 2D, linear interpolation on an integer grid"""
-
-    Ny, Nx = np.shape(a)
-    if isinstance(xi, np.ndarray):
-        x = xi.astype(int)
-        y = yi.astype(int)
-        # Check that xn, yn don't exceed max index
-        xn = np.clip(x + 1, 0, Nx - 1)
-        yn = np.clip(y + 1, 0, Ny - 1)
-    else:
-        x = int(xi)
-        y = int(yi)
-        # conditional is faster than clipping for integers
-        if x == (Nx - 1):
-            xn = x
-        else:
-            xn = x + 1
-        if y == (Ny - 1):
-            yn = y
-        else:
-            yn = y + 1
-
-    a00 = a[y, x]
-    a01 = a[y, xn]
-    a10 = a[yn, x]
-    a11 = a[yn, xn]
-    xt = xi - x
-    yt = yi - y
-    a0 = a00 * (1 - xt) + a01 * xt
-    a1 = a10 * (1 - xt) + a11 * xt
-    ai = a0 * (1 - yt) + a1 * yt
-
-    if not isinstance(xi, np.ndarray):
-        if np.ma.is_masked(ai):
-            raise TerminateTrajectory
-
-    return ai
-
-
-def _gen_starting_points(x,y,grains):
-    if isinstance(grains,tuple):
-        nx, ny = grains
-    elif isinstance(grains,int):
-        nx = ny = grains
-    
-    eps = np.finfo(np.float32).eps
-    
-    tmp_x =  np.linspace(x.min()+eps, x.max()-eps, nx)
-    tmp_y =  np.linspace(y.min()+eps, y.max()-eps, ny)
-    
-    xs = np.tile(tmp_x, ny)
-    ys = np.repeat(tmp_y, nx)
-
-    seed_points = np.array([xs, ys])
-    
-    return seed_points.T
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Mar 25 15:26:55 2020
+
+@author: Kieran Hunt
+https://github.com/kieranmrhunt/curved-quivers/blob/master/modplot.py
+https://stackoverflow.com/questions/51843313/flow-visualisation-in-python-using-curved-path-following-vectors
+aligned with matplotlib.streamplot and improved by Jelmer Veenstra (30-03-2023), https://github.com/veenstrajelmer
+matplotlib.streamplot available at https://raw.githubusercontent.com/matplotlib/matplotlib/main/lib/matplotlib/streamplot.py
+
+Streamline plotting for 2D vector fields.
+
+"""
+
+import numpy as np
+
+import matplotlib as mpl
+from matplotlib import _api, cm, patches
+import matplotlib.colors as mcolors
+import matplotlib.collections as mcollections
+import matplotlib.lines as mlines
+
+
+__all__ = ['velovect']
+
+
+def velovect(axes, x, y, u, v, density=1, linewidth=None, color=None,
+               cmap=None, norm=None, arrowsize=1, arrowstyle='-|>',
+               transform=None, zorder=None, start_points=None,
+               integration_direction='both',
+               grains=15,
+               broken_streamlines=True):
+    """
+    Draw streamlines of a vector flow.
+
+    Parameters
+    ----------
+    x, y : 1D/2D arrays
+        Evenly spaced strictly increasing arrays to make a grid.  If 2D, all
+        rows of *x* must be equal and all columns of *y* must be equal; i.e.,
+        they must be as if generated by ``np.meshgrid(x_1d, y_1d)``.
+    u, v : 2D arrays
+        *x* and *y*-velocities. The number of rows and columns must match
+        the length of *y* and *x*, respectively.
+    density : float or (float, float)
+        Controls the closeness of streamlines. When ``density = 1``, the domain
+        is divided into a 30x30 grid. *density* linearly scales this grid.
+        Each cell in the grid can have, at most, one traversing streamline.
+        For different densities in each direction, use a tuple
+        (density_x, density_y).
+    linewidth : float or 2D array
+        The width of the streamlines. With a 2D array the line width can be
+        varied across the grid. The array must have the same shape as *u*
+        and *v*.
+    color : color or 2D array
+        The streamline color. If given an array, its values are converted to
+        colors using *cmap* and *norm*.  The array must have the same shape
+        as *u* and *v*.
+    cmap, norm
+        Data normalization and colormapping parameters for *color*; only used
+        if *color* is an array of floats. See `~.Axes.imshow` for a detailed
+        description.
+    arrowsize : float
+        Scaling factor for the arrow size.
+    arrowstyle : str
+        Arrow style specification.
+        See `~matplotlib.patches.FancyArrowPatch`.
+    minlength : float
+        Minimum length of streamline in axes coordinates.
+    start_points : (N, 2) array
+        Coordinates of starting points for the streamlines in data coordinates
+        (the same coordinates as the *x* and *y* arrays).
+    zorder : float
+        The zorder of the streamlines and arrows.
+        Artists with lower zorder values are drawn first.
+    maxlength : float
+        Maximum length of streamline in axes coordinates.
+    integration_direction : {'forward', 'backward', 'both'}, default: 'both'
+        Integrate the streamline in forward, backward or both directions.
+    data : indexable object, optional
+        DATA_PARAMETER_PLACEHOLDER
+    broken_streamlines : boolean, default: True
+        If False, forces streamlines to continue until they
+        leave the plot domain.  If True, they may be terminated if they
+        come too close to another streamline.
+
+    Returns
+    -------
+    StreamplotSet
+        Container object with attributes
+ 
+        - ``lines``: `.LineCollection` of streamlines
+
+        - ``arrows``: `.PatchCollection` containing `.FancyArrowPatch`
+          objects representing the arrows half-way along streamlines.
+
+            This container will probably change in the future to allow changes
+            to the colormap, alpha, etc. for both lines and arrows, but these
+            changes should be backward compatible.
+    """
+    grid = Grid(x, y)
+    mask = StreamMask(10)
+    dmap = DomainMap(grid, mask)
+
+    if zorder is None:
+        zorder = mlines.Line2D.zorder
+
+    # default to data coordinates
+    if transform is None:
+        transform = axes.transData
+
+    if color is None:
+        color = axes._get_lines.get_next_color()
+
+    if linewidth is None:
+        linewidth = mpl.rcParams['lines.linewidth']
+
+    line_kw = {}
+    arrow_kw = dict(arrowstyle=arrowstyle, mutation_scale=10 * arrowsize)
+
+    _api.check_in_list(['both', 'forward', 'backward'],
+                       integration_direction=integration_direction)
+
+    #if integration_direction == 'both': #done for magnitude
+    #    maxlength /= 2.
+
+    use_multicolor_lines = isinstance(color, np.ndarray)
+    if use_multicolor_lines:
+        if color.shape != grid.shape:
+            raise ValueError("If 'color' is given, it must match the shape of "
+                             "the (x, y) grid")
+        line_colors = [[]]  # Empty entry allows concatenation of zero arrays.
+        color = np.ma.masked_invalid(color)
+    else:
+        line_kw['color'] = color
+        arrow_kw['color'] = color
+
+    if isinstance(linewidth, np.ndarray):
+        if linewidth.shape != grid.shape:
+            raise ValueError("If 'linewidth' is given, it must match the "
+                             "shape of the (x, y) grid")
+        line_kw['linewidth'] = []
+    else:
+        line_kw['linewidth'] = linewidth
+        arrow_kw['linewidth'] = linewidth
+
+    line_kw['zorder'] = zorder
+    arrow_kw['zorder'] = zorder
+
+    # Sanity checks.
+    if u.shape != grid.shape or v.shape != grid.shape:
+        raise ValueError("'u' and 'v' must match the shape of the (x, y) grid")
+
+    u = np.ma.masked_invalid(u)
+    v = np.ma.masked_invalid(v)
+    magnitude = np.sqrt(u**2 + v**2)
+    magnitude/=np.max(magnitude)
+    if integration_direction == 'both':
+        magnitude /= 2.
+	
+    resolution = density/np.max(grains)
+    integrate = _get_integrator(u, v, dmap, resolution, magnitude, integration_direction)
+
+    trajectories = []    
+   
+    if start_points is None:
+        start_points=_gen_starting_points(x,y,grains)
+    
+    sp2 = np.asanyarray(start_points, dtype=float).copy()
+
+    # Check if start_points are outside the data boundaries
+    for xs, ys in sp2:
+        if not (grid.x_origin <= xs <= grid.x_origin + grid.width and
+                grid.y_origin <= ys <= grid.y_origin + grid.height):
+                raise ValueError(f"Starting point ({xs}, {ys}) outside of "
+                                 "data boundaries")
+
+    # Convert start_points from data to array coords
+    # Shift the seed points from the bottom left of the data so that
+    # data2grid works properly.
+    sp2[:, 0] -= grid.x_origin
+    sp2[:, 1] -= grid.y_origin
+
+    for xs, ys in sp2:
+        xg, yg = dmap.data2grid(xs, ys)
+        # Floating point issues can cause xg, yg to be slightly out of
+        # bounds for xs, ys on the upper boundaries. Because we have
+        # already checked that the starting points are within the original
+        # grid, clip the xg, yg to the grid to work around this issue
+        xg = np.clip(xg, 0, grid.nx - 1)
+        yg = np.clip(yg, 0, grid.ny - 1)
+        
+        t = integrate(xg, yg, broken_streamlines)
+        if t is not None:
+            trajectories.append(t)
+
+    if use_multicolor_lines:
+        if norm is None:
+            norm = mcolors.Normalize(color.min(), color.max())
+        cmap = cm._ensure_cmap(cmap)
+
+    streamlines = []
+    arrows = []
+    for t in trajectories:
+        tgx, tgy = t.T
+        # Rescale from grid-coordinates to data-coordinates.
+        tx, ty = dmap.grid2data(tgx, tgy)
+        tx += grid.x_origin
+        ty += grid.y_origin
+
+        # Create multiple tiny segments if varying width or color is given
+        if isinstance(linewidth, np.ndarray) or use_multicolor_lines:
+            points = np.transpose([tx, ty]).reshape(-1, 1, 2)
+            streamlines.extend(np.hstack([points[:-1], points[1:]]))
+        else:
+            points = np.transpose([tx, ty])
+            streamlines.append(points)
+
+        # Add arrows halfway along each trajectory.
+        s = np.cumsum(np.hypot(np.diff(tx), np.diff(ty)))
+        n = np.searchsorted(s, s[-1])
+        arrow_tail = (tx[n], ty[n])
+        arrow_head = (np.mean(tx[n:n + 2]), np.mean(ty[n:n + 2]))
+
+        if isinstance(linewidth, np.ndarray):
+            line_widths = interpgrid(linewidth, tgx, tgy)[:-1]
+            line_kw['linewidth'].extend(line_widths)
+            arrow_kw['linewidth'] = line_widths[n]
+
+        if use_multicolor_lines:
+            color_values = interpgrid(color, tgx, tgy)[:-1]
+            line_colors.append(color_values)
+            arrow_kw['color'] = cmap(norm(color_values[n]))
+
+        p = patches.FancyArrowPatch(
+            arrow_tail, arrow_head, transform=transform, **arrow_kw)
+        arrows.append(p)
+        
+    lc = mcollections.LineCollection(
+        streamlines, transform=transform, **line_kw)
+    lc.sticky_edges.x[:] = [grid.x_origin, grid.x_origin + grid.width]
+    lc.sticky_edges.y[:] = [grid.y_origin, grid.y_origin + grid.height]
+    if use_multicolor_lines:
+        lc.set_array(np.ma.hstack(line_colors))
+        lc.set_cmap(cmap)
+        lc.set_norm(norm)
+    axes.add_collection(lc)
+
+    ac = mcollections.PatchCollection(arrows)
+    # Adding the collection itself is broken; see #2341.
+    for p in arrows:
+        axes.add_patch(p)
+
+    axes.autoscale_view()
+    stream_container = StreamplotSet(lc, ac)
+    return stream_container
+
+	
+class StreamplotSet:
+
+    def __init__(self, lines, arrows):
+        self.lines = lines
+        self.arrows = arrows
+
+
+# Coordinate definitions
+# ========================
+
+class DomainMap:
+    """
+    Map representing different coordinate systems.
+
+    Coordinate definitions:
+
+    * axes-coordinates goes from 0 to 1 in the domain.
+    * data-coordinates are specified by the input x-y coordinates.
+    * grid-coordinates goes from 0 to N and 0 to M for an N x M grid,
+      where N and M match the shape of the input data.
+    * mask-coordinates goes from 0 to N and 0 to M for an N x M mask,
+      where N and M are user-specified to control the density of streamlines.
+
+    This class also has methods for adding trajectories to the StreamMask.
+    Before adding a trajectory, run `start_trajectory` to keep track of regions
+    crossed by a given trajectory. Later, if you decide the trajectory is bad
+    (e.g., if the trajectory is very short) just call `undo_trajectory`.
+    """
+
+    def __init__(self, grid, mask):
+        self.grid = grid
+        self.mask = mask
+        # Constants for conversion between grid- and mask-coordinates
+        self.x_grid2mask = (mask.nx - 1) / (grid.nx - 1)
+        self.y_grid2mask = (mask.ny - 1) / (grid.ny - 1)
+
+        self.x_mask2grid = 1. / self.x_grid2mask
+        self.y_mask2grid = 1. / self.y_grid2mask
+
+        self.x_data2grid = 1. / grid.dx
+        self.y_data2grid = 1. / grid.dy
+
+    def grid2mask(self, xi, yi):
+        """Return nearest space in mask-coords from given grid-coords."""
+        return round(xi * self.x_grid2mask), round(yi * self.y_grid2mask)
+
+    def mask2grid(self, xm, ym):
+        return xm * self.x_mask2grid, ym * self.y_mask2grid
+
+    def data2grid(self, xd, yd):
+        return xd * self.x_data2grid, yd * self.y_data2grid
+
+    def grid2data(self, xg, yg):
+        return xg / self.x_data2grid, yg / self.y_data2grid
+
+    def start_trajectory(self, xg, yg, broken_streamlines=True):
+        xm, ym = self.grid2mask(xg, yg)
+        self.mask._start_trajectory(xm, ym, broken_streamlines)
+
+    def reset_start_point(self, xg, yg):
+        xm, ym = self.grid2mask(xg, yg)
+        self.mask._current_xy = (xm, ym)
+
+    def update_trajectory(self, xg, yg, broken_streamlines=True):
+        if not self.grid.within_grid(xg, yg):
+            raise InvalidIndexError
+        xm, ym = self.grid2mask(xg, yg)
+        self.mask._update_trajectory(xm, ym, broken_streamlines)
+
+    def undo_trajectory(self):
+        self.mask._undo_trajectory()
+
+
+class Grid:
+    """Grid of data."""
+    def __init__(self, x, y):
+
+        if np.ndim(x) == 1:
+            pass
+        elif np.ndim(x) == 2:
+            x_row = x[0]
+            if not np.allclose(x_row, x):
+                raise ValueError("The rows of 'x' must be equal")
+            x = x_row
+        else:
+            raise ValueError("'x' can have at maximum 2 dimensions")
+
+        if np.ndim(y) == 1:
+            pass
+        elif np.ndim(y) == 2:
+            yt = np.transpose(y)  # Also works for nested lists.
+            y_col = yt[0]
+            if not np.allclose(y_col, yt):
+                raise ValueError("The columns of 'y' must be equal")
+            y = y_col
+        else:
+            raise ValueError("'y' can have at maximum 2 dimensions")
+
+        if not (np.diff(x) > 0).all():
+            raise ValueError("'x' must be strictly increasing")
+        if not (np.diff(y) > 0).all():
+            raise ValueError("'y' must be strictly increasing")
+
+        self.nx = len(x)
+        self.ny = len(y)
+
+        self.dx = x[1] - x[0]
+        self.dy = y[1] - y[0]
+
+        self.x_origin = x[0]
+        self.y_origin = y[0]
+
+        self.width = x[-1] - x[0]
+        self.height = y[-1] - y[0]
+
+        if not np.allclose(np.diff(x), self.width / (self.nx - 1)):
+            raise ValueError("'x' values must be equally spaced")
+        if not np.allclose(np.diff(y), self.height / (self.ny - 1)):
+            raise ValueError("'y' values must be equally spaced")
+
+    @property
+    def shape(self):
+        return self.ny, self.nx
+
+    def within_grid(self, xi, yi):
+        """Return whether (*xi*, *yi*) is a valid index of the grid."""
+        # Note that xi/yi can be floats; so, for example, we can't simply check
+        # `xi < self.nx` since *xi* can be `self.nx - 1 < xi < self.nx`
+        return 0 <= xi <= self.nx - 1 and 0 <= yi <= self.ny - 1
+
+
+class StreamMask:
+    """
+    Mask to keep track of discrete regions crossed by streamlines.
+
+    The resolution of this grid determines the approximate spacing between
+    trajectories. Streamlines are only allowed to pass through zeroed cells:
+    When a streamline enters a cell, that cell is set to 1, and no new
+    streamlines are allowed to enter.
+    """
+
+    def __init__(self, density):
+        try:
+            self.nx, self.ny = (30 * np.broadcast_to(density, 2)).astype(int)
+        except ValueError as err:
+            raise ValueError("'density' must be a scalar or be of length "
+                             "2") from err
+        if self.nx < 0 or self.ny < 0:
+            raise ValueError("'density' must be positive")
+        self._mask = np.zeros((self.ny, self.nx))
+        self.shape = self._mask.shape
+
+        self._current_xy = None
+
+    def __getitem__(self, args):
+        return self._mask[args]
+
+    def _start_trajectory(self, xm, ym, broken_streamlines=True):
+        """Start recording streamline trajectory"""
+        self._traj = []
+        self._update_trajectory(xm, ym, broken_streamlines)
+
+    def _undo_trajectory(self):
+        """Remove current trajectory from mask"""
+        for t in self._traj:
+            self._mask[t] = 0
+
+    def _update_trajectory(self, xm, ym, broken_streamlines=True):
+        """
+        Update current trajectory position in mask.
+
+        If the new position has already been filled, raise `InvalidIndexError`.
+        """
+        if self._current_xy != (xm, ym):
+            if self[ym, xm] == 0:
+                self._traj.append((ym, xm))
+                self._mask[ym, xm] = 1
+                self._current_xy = (xm, ym)
+            else:
+                if broken_streamlines:
+                    raise InvalidIndexError
+                else:
+                    pass
+
+
+class InvalidIndexError(Exception):
+    pass
+
+
+class TerminateTrajectory(Exception):
+    pass
+
+
+# Integrator definitions
+# =======================
+
+def _get_integrator(u, v, dmap, resolution, magnitude, integration_direction):
+
+    # rescale velocity onto grid-coordinates for integrations.
+    u, v = dmap.data2grid(u, v)
+
+    # speed (path length) will be in axes-coordinates
+    u_ax = u / (dmap.grid.nx - 1)
+    v_ax = v / (dmap.grid.ny - 1)
+    speed = np.ma.sqrt(u_ax ** 2 + v_ax ** 2)
+
+    def forward_time(xi, yi):
+        if not dmap.grid.within_grid(xi, yi):
+            raise OutOfBounds
+        ds_dt = interpgrid(speed, xi, yi)
+        if ds_dt == 0:
+            raise TerminateTrajectory()
+        dt_ds = 1. / ds_dt
+        ui = interpgrid(u, xi, yi)
+        vi = interpgrid(v, xi, yi)
+        return ui * dt_ds, vi * dt_ds
+
+    def backward_time(xi, yi):
+        dxi, dyi = forward_time(xi, yi)
+        return -dxi, -dyi
+
+    def integrate(x0, y0, broken_streamlines=True):
+        """
+        Return x, y grid-coordinates of trajectory based on starting point.
+
+        Integrate both forward and backward in time from starting point in
+        grid coordinates.
+
+        Integration is terminated when a trajectory reaches a domain boundary
+        or when it crosses into an already occupied cell in the StreamMask. The
+        resulting trajectory is None if it is shorter than `minlength`.
+        """
+
+        stotal, xy_traj = 0., []
+
+        try:
+            dmap.start_trajectory(x0, y0, broken_streamlines)
+        except InvalidIndexError:
+            return None
+        if integration_direction in ['both', 'backward']:
+            s, xyt = _integrate_rk12(x0, y0, dmap, backward_time, resolution, magnitude,
+                                     broken_streamlines)
+            stotal += s
+            xy_traj += xyt[::-1]
+
+        if integration_direction in ['both', 'forward']:
+            dmap.reset_start_point(x0, y0)
+            s, xyt = _integrate_rk12(x0, y0, dmap, forward_time, resolution, magnitude,
+                                     broken_streamlines)
+            stotal += s
+            xy_traj += xyt[1:]
+
+        if len(xy_traj) > 1:
+            return np.broadcast_arrays(xy_traj, np.empty((1, 2)))[0]
+        else:  # reject short trajectories
+            dmap.undo_trajectory()
+            return None
+
+    return integrate
+
+
+class OutOfBounds(IndexError):
+    pass
+
+
+def _integrate_rk12(x0, y0, dmap, f, resolution, magnitude, broken_streamlines=True):
+    """
+    2nd-order Runge-Kutta algorithm with adaptive step size.
+
+    This method is also referred to as the improved Euler's method, or Heun's
+    method. This method is favored over higher-order methods because:
+
+    1. To get decent looking trajectories and to sample every mask cell
+       on the trajectory we need a small timestep, so a lower order
+       solver doesn't hurt us unless the data is *very* high resolution.
+       In fact, for cases where the user inputs
+       data smaller or of similar grid size to the mask grid, the higher
+       order corrections are negligible because of the very fast linear
+       interpolation used in `interpgrid`.
+
+    2. For high resolution input data (i.e. beyond the mask
+       resolution), we must reduce the timestep. Therefore, an adaptive
+       timestep is more suited to the problem as this would be very hard
+       to judge automatically otherwise.
+
+    This integrator is about 1.5 - 2x as fast as RK4 and RK45 solvers (using
+    similar Python implementations) in most setups.
+    """
+    # This error is below that needed to match the RK4 integrator. It
+    # is set for visual reasons -- too low and corners start
+    # appearing ugly and jagged. Can be tuned.
+    maxerror = 0.003
+
+    # This limit is important (for all integrators) to avoid the
+    # trajectory skipping some mask cells. We could relax this
+    # condition if we use the code which is commented out below to
+    # increment the location gradually. However, due to the efficient
+    # nature of the interpolation, this doesn't boost speed by much
+    # for quite a bit of complexity.
+    maxds = min(1. / dmap.mask.nx, 1. / dmap.mask.ny, 0.1)
+
+    ds = maxds
+    stotal = 0
+    xi = x0
+    yi = y0
+    xyf_traj = []
+    m_total = []
+    
+    while True:
+        try:
+            if dmap.grid.within_grid(xi, yi):
+                xyf_traj.append((xi, yi))
+                m_total.append(interpgrid(magnitude, xi, yi))
+                maxlength = resolution*np.mean(m_total)
+            else:
+                raise OutOfBounds
+
+            # Compute the two intermediate gradients.
+            # f should raise OutOfBounds if the locations given are
+            # outside the grid.
+            k1x, k1y = f(xi, yi)
+            k2x, k2y = f(xi + ds * k1x, yi + ds * k1y)
+
+        except OutOfBounds:
+            # Out of the domain during this step.
+            # Take an Euler step to the boundary to improve neatness
+            # unless the trajectory is currently empty.
+            if xyf_traj:
+                ds, xyf_traj = _euler_step(xyf_traj, dmap, f)
+                stotal += ds
+            break
+        except TerminateTrajectory:
+            break
+
+        dx1 = ds * k1x
+        dy1 = ds * k1y
+        dx2 = ds * 0.5 * (k1x + k2x)
+        dy2 = ds * 0.5 * (k1y + k2y)
+
+        ny, nx = dmap.grid.shape
+        # Error is normalized to the axes coordinates
+        error = np.hypot((dx2 - dx1) / (nx - 1), (dy2 - dy1) / (ny - 1))
+
+        # Only save step if within error tolerance
+        if error < maxerror:
+            xi += dx2
+            yi += dy2
+            try:
+                dmap.update_trajectory(xi, yi, broken_streamlines)
+            except InvalidIndexError:
+                break
+            if stotal + ds > maxlength:
+                break
+            stotal += ds
+
+        # recalculate stepsize based on step error
+        if error == 0:
+            ds = maxds
+        else:
+            ds = min(maxds, 0.85 * ds * (maxerror / error) ** 0.5)
+
+    return stotal, xyf_traj
+
+
+def _euler_step(xyf_traj, dmap, f):
+    """Simple Euler integration step that extends streamline to boundary."""
+    ny, nx = dmap.grid.shape
+    xi, yi = xyf_traj[-1]
+    cx, cy = f(xi, yi)
+    if cx == 0:
+        dsx = np.inf
+    elif cx < 0:
+        dsx = xi / -cx
+    else:
+        dsx = (nx - 1 - xi) / cx
+    if cy == 0:
+        dsy = np.inf
+    elif cy < 0:
+        dsy = yi / -cy
+    else:
+        dsy = (ny - 1 - yi) / cy
+    ds = min(dsx, dsy)
+    xyf_traj.append((xi + cx * ds, yi + cy * ds))
+    return ds, xyf_traj
+
+
+# Utility functions
+# ========================
+
+def interpgrid(a, xi, yi):
+    """Fast 2D, linear interpolation on an integer grid"""
+
+    Ny, Nx = np.shape(a)
+    if isinstance(xi, np.ndarray):
+        x = xi.astype(int)
+        y = yi.astype(int)
+        # Check that xn, yn don't exceed max index
+        xn = np.clip(x + 1, 0, Nx - 1)
+        yn = np.clip(y + 1, 0, Ny - 1)
+    else:
+        x = int(xi)
+        y = int(yi)
+        # conditional is faster than clipping for integers
+        if x == (Nx - 1):
+            xn = x
+        else:
+            xn = x + 1
+        if y == (Ny - 1):
+            yn = y
+        else:
+            yn = y + 1
+
+    a00 = a[y, x]
+    a01 = a[y, xn]
+    a10 = a[yn, x]
+    a11 = a[yn, xn]
+    xt = xi - x
+    yt = yi - y
+    a0 = a00 * (1 - xt) + a01 * xt
+    a1 = a10 * (1 - xt) + a11 * xt
+    ai = a0 * (1 - yt) + a1 * yt
+
+    if not isinstance(xi, np.ndarray):
+        if np.ma.is_masked(ai):
+            raise TerminateTrajectory
+
+    return ai
+
+
+def _gen_starting_points(x,y,grains):
+    if isinstance(grains,tuple):
+        nx, ny = grains
+    elif isinstance(grains,int):
+        nx = ny = grains
+    
+    eps = np.finfo(np.float32).eps
+    
+    tmp_x =  np.linspace(x.min()+eps, x.max()-eps, nx)
+    tmp_y =  np.linspace(y.min()+eps, y.max()-eps, ny)
+    
+    xs = np.tile(tmp_x, ny)
+    ys = np.repeat(tmp_y, nx)
+
+    seed_points = np.array([xs, ys])
+    
+    return seed_points.T
```

### Comparing `dfm_tools-0.10.55/dfm_tools/regulargrid.py` & `dfm_tools-0.11.0/dfm_tools/regulargrid.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-# -*- coding: utf-8 -*-
-"""
-dfm_tools are post-processing tools for Delft3D FM
-Copyright (C) 2020 Deltares. All rights reserved.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  if not, see <http://www.gnu.org/licenses/>.
-
-All names, logos, and references to "Deltares" are registered trademarks of
-Stichting Deltares and remain full property of Stichting Deltares at all times.
-All rights reserved.
-
-
-INFORMATION
-This script is part of dfm_tools: https://github.com/openearth/dfm_tools
-Check the README.rst on github for other available functions
-Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
-Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
-
-Created on Sun Mar 22 08:41:00 2020
-
-@author: veenstra
-"""
-
-import warnings
-import numpy as np
-
-
-def center2corner(cen):
-    
-    warnings.warn(DeprecationWarning('center2corner() might be phased out in a future version, unless it is found useful for regulargrid netcdf reading/plotting.'))
-    
-    if len(cen.shape) != 2:
-        raise ValueError('input array should have 2 dimensions')
-    
-    cen_nobnd = corner2center(cen)
-    cen_nobnd_diff_ax0 = np.diff(cen_nobnd, axis=0)
-    add_top = cen_nobnd[0,:] - cen_nobnd_diff_ax0[0,:]
-    add_bot = cen_nobnd[-1,:] + cen_nobnd_diff_ax0[-1,:]
-    cen_vertbnd = np.vstack([add_top, cen_nobnd, add_bot])
-    cen_nobnd_diff_ax1 = np.diff(cen_vertbnd, axis=1)
-    add_left = cen_vertbnd[:,0] - cen_nobnd_diff_ax1[:,0]
-    add_right = cen_vertbnd[:,-1] + cen_nobnd_diff_ax1[:,-1]
-    cen_withbnd = np.vstack([add_left.T, cen_vertbnd.T, add_right.T]).T
-    cor = cen_withbnd
-        
-    return cor
-
-
-def corner2center(cor):
-    """
-    from OET but edited, original author is Gerben de Boer
-
-    cen = corner2center(cor) calculates the value of the center
-    of the pixels by avareging the surrounding 4 corner values
-    for arrays, or the surrounding 2 corner for vectors or [1,n]
-    or [n,1 2D arrays. corner2center works both for coordinate meshes
-    as well as data values defined on those meshes.
-    
-    >>> corner2center([1,3,5])
-    array([ 2.,  4.])
-    
-    >>> corner2center([[1,3,5]])
-    array([[ 2.,  4.]])
-    
-    >>> corner2center([[1],[3],[5]])
-    array([[ 2.],
-           [ 4.]])
-    
-    >>> corner2center([[1,3,5],[2,6,10]])
-    array([[ 3.,  6.]])
-    """
-    
-    warnings.warn(DeprecationWarning('corner2center() might be phased out in a future version, unless it is found useful for regulargrid netcdf reading/plotting.'))
-    
-    cor = np.asarray(cor)
-    shp = cor.shape
-    
-    if len(shp)==1 and len(cor)<2:
-        raise ValueError('at least 2 elements required')
-    elif len(shp)==1:
-        cen = np.zeros(tuple([shp[0]-1,1]))
-        cen = (cor[ :-1] + cor[1:  ])/2
-    elif len(shp)==2 and shp[0]==1:
-        cen = np.zeros(tuple([1,shp[1]-1]))
-        cen[:,:] = (cor[:, :-1] + cor[:,1:  ])/2
-    elif len(shp)==2 and shp[1]==1:
-        cen = np.zeros(tuple([shp[0]-1,1]))
-        cen[:,:] = (cor[ :-1,:] + cor[1:  ,:])/2
-    elif len(shp)==2: 
-        cen = np.zeros(tuple(np.array(shp)-1))
-        cen[:,:] = (cor[ :-1, :-1] + 
-                    cor[ :-1,1:  ] + 
-                    cor[1:  ,1:  ] + 
-                    cor[1:  , :-1])/4
-    elif len(shp)>3:
-        raise NotImplementedError('only 1D and 2D arrays implemented, only intervals and pixels, no voxels')
-    return cen
-
-
-def uva2xymagdeg(U1, V1, ALFAS, KCU=None, KCV=None, inactivewhen4x0=True): #only used in workinprogress_delft3D_netcdf.py
-    """
-    this function converts velocities in m,n-direction (defined mathematically, so 0 on x-axis and increasing counter-clockwise)
-    alpha is a matrix with orientations of cells, with respect to the north (varname='ALFAS') in D3D output
-    output:
-        vec_x - velocity in x-direction (east)
-        vec_y - velocity in y-direction (east)
-        vec_x - velocity in x-direction (east)
-        vec_x - velocity in x-direction (east)
-
-    De snelheden U1 zijn gedefinieerd op de U-punten. Die moet je eerst middelen naar de celcentra. Laat Uc de celcentre snelheid zijn:
-    Uc(m,n) = (U1(m,n) + U1(m-1,n))/2
-    Vc(m,n) = (V1(m,n) + V1(m,n-1))/2
-    Vervolgens moeten die componenten gedraaid worden daarvoor is de hoek ALFAS nodig.
-    Ux (m,n) = Uc(m,n)*cos(ALFAS) - Vc(m,n)*sin(ALFAS)
-    Uy (m,n) = Uc(m,n)*sin(ALFAS) + Vc(m,n)*cos(ALFAS)
-    Alles zou goed moeten gaan als je bij de middeling ervoor zorgt dat Uc(m,n) weer op de positie (m,n) in de array komt.
-    Uc = (U1(1:end-1,:) + U1(2:end-1,:))/2 gaat dus net mis.
-    Uc(2:end-1,: ) = (U1(1:end-1,: )) + U1(2:end,: ))/2 klopt wel, maar werkt alleen als je eerst Uc op de juiste afmeting hebt geïnitialiseerd.
-
-    vel_magn = np.sqrt(U1**2 + V1**2)
-    direction_math_deg = np.rad2deg(np.arctan2(V1, U1))+ALFAS
-    direction_naut_deg = (90-direction_math_deg)%360
-    vel_x = vel_magn*np.cos(np.deg2rad(direction_math_deg))
-    vel_y = vel_magn*np.sin(np.deg2rad(direction_math_deg))
-    """
-    #replace -999. by 0
-    U1[(U1==-999.)] = np.nan
-    V1[(V1==-999.)] = np.nan
-
-    #calculate UV velocities on centers
-    Uc = np.empty(shape=U1.shape)
-    Uc[:] = np.nan
-    Vc = np.empty(shape=U1.shape)
-    Vc[:] = np.nan
-    Uc[1:,:] = np.nansum([U1[:-1,:], U1[1:,:]], axis=0)/2
-    Vc[:,1:] = np.nansum([V1[:,:-1], V1[:,1:]], axis=0)/2
-    
-    #remove cells when all four velocity points (U1 and V1) were -999.
-    mask_u999 = np.zeros(shape=U1.shape)
-    mask_v999 = np.zeros(shape=U1.shape)
-    mask_u999[1:,:] = ~(np.isnan(U1[:-1,:]) & np.isnan(U1[1:,:]))
-    mask_v999[:,1:] = ~(np.isnan(V1[:,:-1]) & np.isnan(V1[:,1:]))
-    mask_UV999 = mask_u999 + mask_v999
-    Uc[mask_UV999==0] = np.nan
-    Vc[mask_UV999==0] = np.nan
-    
-    if inactivewhen4x0:
-        #mask cells when all four velocity points (U1 and V1) are 0.
-        mask_u999 = np.zeros(shape=U1.shape)
-        mask_v999 = np.zeros(shape=U1.shape)
-        mask_u999[1:,:] = ~((U1[:-1,:]==0) & (U1[1:,:]==0))
-        mask_v999[:,1:] = ~((V1[:,:-1]==0) & (V1[:,1:]==0))
-        mask_UV999 = mask_u999 + mask_v999
-        Uc[mask_UV999==0] = np.nan
-        Vc[mask_UV999==0] = np.nan
-    
-    #remove cell with uv mask (inactive when all four velocity points are masked, so sum is zero)
-    if KCU is not None and KCV is not None:
-        mask_u = np.zeros(shape=U1.shape)
-        mask_v = np.zeros(shape=U1.shape)
-        mask_u[1:,:] = KCU[:-1,:]+KCU[1:,:]
-        mask_v[:,1:] = KCV[:,:-1]+KCV[:,1:]
-        mask_UV = mask_u + mask_v
-        Uc[mask_UV==0] = np.nan
-        Vc[mask_UV==0] = np.nan
-    
-    vel_x = Uc*np.cos(np.deg2rad(ALFAS)) - Vc*np.sin(np.deg2rad(ALFAS))
-    vel_y = Uc*np.sin(np.deg2rad(ALFAS)) + Vc*np.cos(np.deg2rad(ALFAS))
-    vel_magn = np.sqrt(vel_x**2 + vel_y**2)
-    direction_naut_deg = np.rad2deg(np.arctan2(vel_y, vel_x))%360
-   
-    return vel_x, vel_y, vel_magn, direction_naut_deg
-
-
-
-
-
-
-
+# -*- coding: utf-8 -*-
+"""
+dfm_tools are post-processing tools for Delft3D FM
+Copyright (C) 2020 Deltares. All rights reserved.
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  if not, see <http://www.gnu.org/licenses/>.
+
+All names, logos, and references to "Deltares" are registered trademarks of
+Stichting Deltares and remain full property of Stichting Deltares at all times.
+All rights reserved.
+
+
+INFORMATION
+This script is part of dfm_tools: https://github.com/openearth/dfm_tools
+Check the README.rst on github for other available functions
+Check the tests folder on github for example scripts (this is the dfm_tools pytest testbank)
+Check the pptx and example figures in (created by the testbank): N:/Deltabox/Bulletin/veenstra/info dfm_tools
+
+Created on Sun Mar 22 08:41:00 2020
+
+@author: veenstra
+"""
+
+import warnings
+import numpy as np
+
+
+def center2corner(cen):
+    
+    warnings.warn(DeprecationWarning('center2corner() might be phased out in a future version, unless it is found useful for regulargrid netcdf reading/plotting.'))
+    
+    if len(cen.shape) != 2:
+        raise ValueError('input array should have 2 dimensions')
+    
+    cen_nobnd = corner2center(cen)
+    cen_nobnd_diff_ax0 = np.diff(cen_nobnd, axis=0)
+    add_top = cen_nobnd[0,:] - cen_nobnd_diff_ax0[0,:]
+    add_bot = cen_nobnd[-1,:] + cen_nobnd_diff_ax0[-1,:]
+    cen_vertbnd = np.vstack([add_top, cen_nobnd, add_bot])
+    cen_nobnd_diff_ax1 = np.diff(cen_vertbnd, axis=1)
+    add_left = cen_vertbnd[:,0] - cen_nobnd_diff_ax1[:,0]
+    add_right = cen_vertbnd[:,-1] + cen_nobnd_diff_ax1[:,-1]
+    cen_withbnd = np.vstack([add_left.T, cen_vertbnd.T, add_right.T]).T
+    cor = cen_withbnd
+        
+    return cor
+
+
+def corner2center(cor):
+    """
+    from OET but edited, original author is Gerben de Boer
+
+    cen = corner2center(cor) calculates the value of the center
+    of the pixels by avareging the surrounding 4 corner values
+    for arrays, or the surrounding 2 corner for vectors or [1,n]
+    or [n,1 2D arrays. corner2center works both for coordinate meshes
+    as well as data values defined on those meshes.
+    
+    >>> corner2center([1,3,5])
+    array([ 2.,  4.])
+    
+    >>> corner2center([[1,3,5]])
+    array([[ 2.,  4.]])
+    
+    >>> corner2center([[1],[3],[5]])
+    array([[ 2.],
+           [ 4.]])
+    
+    >>> corner2center([[1,3,5],[2,6,10]])
+    array([[ 3.,  6.]])
+    """
+    
+    warnings.warn(DeprecationWarning('corner2center() might be phased out in a future version, unless it is found useful for regulargrid netcdf reading/plotting.'))
+    
+    cor = np.asarray(cor)
+    shp = cor.shape
+    
+    if len(shp)==1 and len(cor)<2:
+        raise ValueError('at least 2 elements required')
+    elif len(shp)==1:
+        cen = np.zeros(tuple([shp[0]-1,1]))
+        cen = (cor[ :-1] + cor[1:  ])/2
+    elif len(shp)==2 and shp[0]==1:
+        cen = np.zeros(tuple([1,shp[1]-1]))
+        cen[:,:] = (cor[:, :-1] + cor[:,1:  ])/2
+    elif len(shp)==2 and shp[1]==1:
+        cen = np.zeros(tuple([shp[0]-1,1]))
+        cen[:,:] = (cor[ :-1,:] + cor[1:  ,:])/2
+    elif len(shp)==2: 
+        cen = np.zeros(tuple(np.array(shp)-1))
+        cen[:,:] = (cor[ :-1, :-1] + 
+                    cor[ :-1,1:  ] + 
+                    cor[1:  ,1:  ] + 
+                    cor[1:  , :-1])/4
+    elif len(shp)>3:
+        raise NotImplementedError('only 1D and 2D arrays implemented, only intervals and pixels, no voxels')
+    return cen
+
+
+def uva2xymagdeg(U1, V1, ALFAS, KCU=None, KCV=None, inactivewhen4x0=True): #only used in workinprogress_delft3D_netcdf.py
+    """
+    this function converts velocities in m,n-direction (defined mathematically, so 0 on x-axis and increasing counter-clockwise)
+    alpha is a matrix with orientations of cells, with respect to the north (varname='ALFAS') in D3D output
+    output:
+        vec_x - velocity in x-direction (east)
+        vec_y - velocity in y-direction (east)
+        vec_x - velocity in x-direction (east)
+        vec_x - velocity in x-direction (east)
+
+    De snelheden U1 zijn gedefinieerd op de U-punten. Die moet je eerst middelen naar de celcentra. Laat Uc de celcentre snelheid zijn:
+    Uc(m,n) = (U1(m,n) + U1(m-1,n))/2
+    Vc(m,n) = (V1(m,n) + V1(m,n-1))/2
+    Vervolgens moeten die componenten gedraaid worden daarvoor is de hoek ALFAS nodig.
+    Ux (m,n) = Uc(m,n)*cos(ALFAS) - Vc(m,n)*sin(ALFAS)
+    Uy (m,n) = Uc(m,n)*sin(ALFAS) + Vc(m,n)*cos(ALFAS)
+    Alles zou goed moeten gaan als je bij de middeling ervoor zorgt dat Uc(m,n) weer op de positie (m,n) in de array komt.
+    Uc = (U1(1:end-1,:) + U1(2:end-1,:))/2 gaat dus net mis.
+    Uc(2:end-1,: ) = (U1(1:end-1,: )) + U1(2:end,: ))/2 klopt wel, maar werkt alleen als je eerst Uc op de juiste afmeting hebt geïnitialiseerd.
+
+    vel_magn = np.sqrt(U1**2 + V1**2)
+    direction_math_deg = np.rad2deg(np.arctan2(V1, U1))+ALFAS
+    direction_naut_deg = (90-direction_math_deg)%360
+    vel_x = vel_magn*np.cos(np.deg2rad(direction_math_deg))
+    vel_y = vel_magn*np.sin(np.deg2rad(direction_math_deg))
+    """
+    #replace -999. by 0
+    U1[(U1==-999.)] = np.nan
+    V1[(V1==-999.)] = np.nan
+
+    #calculate UV velocities on centers
+    Uc = np.empty(shape=U1.shape)
+    Uc[:] = np.nan
+    Vc = np.empty(shape=U1.shape)
+    Vc[:] = np.nan
+    Uc[1:,:] = np.nansum([U1[:-1,:], U1[1:,:]], axis=0)/2
+    Vc[:,1:] = np.nansum([V1[:,:-1], V1[:,1:]], axis=0)/2
+    
+    #remove cells when all four velocity points (U1 and V1) were -999.
+    mask_u999 = np.zeros(shape=U1.shape)
+    mask_v999 = np.zeros(shape=U1.shape)
+    mask_u999[1:,:] = ~(np.isnan(U1[:-1,:]) & np.isnan(U1[1:,:]))
+    mask_v999[:,1:] = ~(np.isnan(V1[:,:-1]) & np.isnan(V1[:,1:]))
+    mask_UV999 = mask_u999 + mask_v999
+    Uc[mask_UV999==0] = np.nan
+    Vc[mask_UV999==0] = np.nan
+    
+    if inactivewhen4x0:
+        #mask cells when all four velocity points (U1 and V1) are 0.
+        mask_u999 = np.zeros(shape=U1.shape)
+        mask_v999 = np.zeros(shape=U1.shape)
+        mask_u999[1:,:] = ~((U1[:-1,:]==0) & (U1[1:,:]==0))
+        mask_v999[:,1:] = ~((V1[:,:-1]==0) & (V1[:,1:]==0))
+        mask_UV999 = mask_u999 + mask_v999
+        Uc[mask_UV999==0] = np.nan
+        Vc[mask_UV999==0] = np.nan
+    
+    #remove cell with uv mask (inactive when all four velocity points are masked, so sum is zero)
+    if KCU is not None and KCV is not None:
+        mask_u = np.zeros(shape=U1.shape)
+        mask_v = np.zeros(shape=U1.shape)
+        mask_u[1:,:] = KCU[:-1,:]+KCU[1:,:]
+        mask_v[:,1:] = KCV[:,:-1]+KCV[:,1:]
+        mask_UV = mask_u + mask_v
+        Uc[mask_UV==0] = np.nan
+        Vc[mask_UV==0] = np.nan
+    
+    vel_x = Uc*np.cos(np.deg2rad(ALFAS)) - Vc*np.sin(np.deg2rad(ALFAS))
+    vel_y = Uc*np.sin(np.deg2rad(ALFAS)) + Vc*np.cos(np.deg2rad(ALFAS))
+    vel_magn = np.sqrt(vel_x**2 + vel_y**2)
+    direction_naut_deg = np.rad2deg(np.arctan2(vel_y, vel_x))%360
+   
+    return vel_x, vel_y, vel_magn, direction_naut_deg
+
+
+
+
+
+
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools/xarray_helpers.py` & `dfm_tools-0.11.0/dfm_tools/xarray_helpers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Oct 14 19:58:36 2022
-
-@author: veenstra
-"""
-
-import os
-import re
-from netCDF4 import Dataset
-import xarray as xr
-import xugrid as xu
-import datetime as dt
-import glob
-import pandas as pd
-import warnings
-import numpy as np
-from dfm_tools.errors import OutOfRangeError
-
-
-def file_to_list(file_nc):
-    if isinstance(file_nc,list):
-        file_nc_list = file_nc
-    else:
-        basename = os.path.basename(file_nc)
-        dirname = os.path.dirname(file_nc)
-        ext = os.path.splitext(file_nc)[-1]
-        if '.*' in basename:
-            def glob_re(pattern, strings):
-                return list(filter(re.compile(pattern).search, strings))
-            file_nc_list = glob_re(basename, glob.glob(os.path.join(dirname,f'*{ext}')))
-        else:
-            file_nc_list = glob.glob(file_nc)
-        file_nc_list.sort()
-    if len(file_nc_list)==0:
-        raise FileNotFoundError('file(s) not found, empty file_nc_list')
-    return file_nc_list
-
-
-def preprocess_hisnc(ds):
-    """
-    Look for dim/coord combination and use this for Dataset.set_index(), to enable station/gs/crs/laterals label based indexing. If duplicate labels are found (like duplicate stations), these are dropped to avoid indexing issues.
-    
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        DESCRIPTION.
-    drop_duplicate_stations : TYPE, optional
-        DESCRIPTION. The default is True.
-
-    Returns
-    -------
-    ds : TYPE
-        DESCRIPTION.
-
-    """
-    
-    #generate dim_coord_dict to set indexes, this will be something like {'stations':'station_name','cross_section':'cross_section_name'} after loop
-    dim_coord_dict = {}
-    for ds_coord in ds.coords.keys():
-        ds_coord_dtype = ds[ds_coord].dtype
-        ds_coord_dim = ds[ds_coord].dims[0] #these vars always have only one dim
-        if ds_coord_dtype.str.startswith('|S'): #these are station/crs/laterals/gs names/ids
-            dim_coord_dict[ds_coord_dim] = ds_coord
-    
-    #loop over dimensions and set corresponding coordinates/variables from dim_coord_dict as their index
-    for dim in dim_coord_dict.keys():
-        coord = dim_coord_dict[dim]
-        ds[coord] = ds[coord].load().str.decode('utf-8',errors='ignore').str.strip() #.load() is essential to convert not only first letter of string.
-        ds = ds.set_index({dim:coord})
-        
-        #drop duplicate indices (stations/crs/gs), this avoids "InvalidIndexError: Reindexing only valid with uniquely valued Index objects"
-        duplicated_keepfirst = ds[dim].to_series().duplicated(keep='first')
-        if duplicated_keepfirst.sum()>0:
-            print(f'dropping {duplicated_keepfirst.sum()} duplicate "{coord}" labels to avoid InvalidIndexError')
-            ds = ds[{dim:~duplicated_keepfirst}]
-
-    #check dflowfm version/date and potentially raise warning about incorrect layers
-    try:
-        source_attr = ds.attrs['source'] # fails if no source attr present in dataset
-        source_attr_version = source_attr.split(', ')[1]
-        source_attr_date = source_attr.split(', ')[2]
-        if pd.Timestamp(source_attr_date) < dt.datetime(2020,11,28):
-            warnings.warn(UserWarning(f'Your model was run with a D-FlowFM version from before 28-10-2020 ({source_attr_version} from {source_attr_date}), the layers in the hisfile are incorrect. Check UNST-2920 and UNST-3024 for more information, it was fixed from OSS 67858.'))
-    except KeyError: #no source attr present in hisfile, cannot check version
-        pass
-    except IndexError: #contains no ', '
-        pass
-
-    return ds
-
-
-def preprocess_hirlam(ds):
-    """
-    add xy variables as longitude/latitude to avoid duplicate var/dim names (we rename it anyway otherwise)
-    add xy as variables again with help of NetCDF4
-    this function is hopefully temporary, necessary since >1D-variables cannot have the same name as one of its dimensions in xarray. Background and future solution: https://github.com/pydata/xarray/issues/6293
-    "MissingDimensionsError: 'y' has more than 1-dimension and the same name as one of its dimensions ('y', 'x'). xarray disallows such variables because they conflict with the coordinates used to label dimensions."
-    might be solved in https://github.com/pydata/xarray/releases/tag/v2023.02.0 (xr.concat), but not certain
-    """
-    
-    print('hirlam workaround: adding dropped x/y variables again as longitude/latitude')
-    file_nc_one = ds.encoding['source']
-    with Dataset(file_nc_one) as data_nc:
-        data_nc_x = data_nc['x']
-        data_nc_y = data_nc['y']
-        ds['longitude'] = xr.DataArray(data_nc_x,dims=data_nc_x.dimensions,attrs=data_nc_x.__dict__) 
-        ds['latitude'] = xr.DataArray(data_nc_y,dims=data_nc_y.dimensions,attrs=data_nc_y.__dict__)
-    ds = ds.set_coords(['latitude','longitude'])
-    for varkey in ds.data_vars:
-        del ds[varkey].encoding['coordinates'] #remove {'coordinates':'y x'} from encoding (otherwise set twice)
-    return ds
-
-
-def preprocess_ERA5(ds):
-    """
-    Reduces the expver dimension in some of the ERA5 data (mtpr and other variables), which occurs in files with very recent data. The dimension contains the unvalidated data from the latest month in the second index in the expver dimension. The reduction is done with mean, but this is arbitrary, since there is only one valid value per timestep and the other one is nan.
-    """
-    if 'expver' in ds.dims:
-        ds = ds.mean(dim='expver')
-    return ds
-
-
-def preprocess_woa(ds):
-    """
-    WOA time units is 'months since 0000-01-01 00:00:00' and calendar is not set (360_day is the only calendar that supports that unit in xarray)
-    """
-    ds.time.attrs['calendar'] = '360_day'
-    ds = xr.decode_cf(ds) #decode_cf after adding 360_day calendar attribute
-    return ds
-
-
-def prevent_dtype_int(ds): #TODO: this is not used, maybe phase out?
-    """
-    Prevent writing to int, since it might mess up dataset (https://github.com/Deltares/dfm_tools/issues/239 and https://github.com/pydata/xarray/issues/7039)
-    Since floats are used instead of ints, the disksize of the dataset will be larger
-    TODO: alternatively remove scale_factor key from attrs, so it can be recomputed (seems to also work): ds[var].encoding.pop('scale_factor')
-    TODO: maybe add to preprocess_ERA5 (preferrably popping scale_factor attribute to keep file size small)
-    """
-    for var in ds.data_vars:
-        var_encoding = ds[var].encoding
-        if 'dtype' in var_encoding.keys():
-            if 'int' in str(var_encoding['dtype']):
-                ds[var].encoding.pop('dtype') #remove dtype key from attrs
-    return ds
-
-
-def recompute_scaling_and_offset(ds:xr.Dataset) -> xr.Dataset:
-    """
-    Recompute add_offset and scale_factor for variables of dtype int. As suggested by https://github.com/ArcticSnow/TopoPyScale/issues/60#issuecomment-1459747654
-    This is a proper fix for https://github.com/Deltares/dfm_tools/issues/239, https://github.com/pydata/xarray/issues/7039 and more
-    However, rescaling causes minor semi-accuracy loss, but it does keep the disksize small (which does not happen when converting it to dtype(float32)).
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds : xr.Dataset
-        DESCRIPTION.
-
-    """
-
-    for var in ds.data_vars:
-        da = ds[var]
-        
-        if 'dtype' not in da.encoding: #check if dype is available, sometime encoding={}
-            continue
-        dtype = da.encoding['dtype']
-        
-        if 'int' not in str(dtype): #skip non-int vars TODO: make proper int-check?
-            continue
-        if 'scale_factor' not in da.encoding.keys() or 'add_offset' not in da.encoding.keys(): #prevent rescaling of non-scaled vars (like crs) #TODO: convert to set().issubset(set())
-            continue
-        
-        n = dtype.itemsize * 8 #n=16 for int16
-        vmin = float(da.min().values)
-        vmax = float(da.max().values)
-        
-        # stretch/compress data to the available packed range
-        scale_factor = (vmax - vmin) / (2 ** n - 1)
-        
-        # translate the range to be symmetric about zero
-        add_offset =  vmin + 2 ** (n - 1) * scale_factor
-        #add_offset = (vmax+vmin)/2 #difference with above is scale_factor/2
-        
-        da.encoding['scale_factor'] = scale_factor
-        da.encoding['add_offset'] = add_offset
-    return ds
-
-
-def merge_meteofiles(file_nc:str, preprocess=None, 
-                     chunks:dict = {'time':1},
-                     time_slice:slice = slice(None,None),
-                     add_global_overlap:bool = False, zerostart:bool = False) -> xr.Dataset:
-    """
-    for merging for instance meteo files
-    x/y and lon/lat are renamed to longitude/latitude #TODO: is this desireable?
-
-    Parameters
-    ----------
-    file_nc : str
-        DESCRIPTION.
-    preprocess : TYPE, optional
-        DESCRIPTION. The default is None.
-    chunks : dict, optional
-        Prevents large chunks and memory issues. The default is {'time':1}.
-    time_slice : slice, optional
-        DESCRIPTION. The default is slice(None,None).
-    add_global_overlap : bool, optional
-        GTSM specific: extend data beyond -180 to 180 longitude. The default is False.
-    zerostart : bool, optional
-        GTSM specific: extend data with 0-value fields 1 and 2 days before time_slice.start. The default is False.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    TYPE
-        DESCRIPTION.
-
-    """
-    #TODO: add ERA5 conversions and features from hydro_tools\ERA5\ERA52DFM.py (except for varRhoair_alt, request FM support for varying airpressure: https://issuetracker.deltares.nl/browse/UNST-6593)
-    #TODO: request FM support for charnock (etc) separate meteo forcing (currently airpressure_windx_windy_charnock merged file is required): https://issuetracker.deltares.nl/browse/UNST-6453
-    #TODO: provide extfile example with fmquantity/ncvarname combinations and cleanup FM code: https://issuetracker.deltares.nl/browse/UNST-6453
-    #TODO: add coordinate conversion (only valid for models with multidimensional lat/lon variables like HARMONIE and HIRLAM). This should work: ds_reproj = ds.set_crs(4326).to_crs(28992)
-    #TODO: add CMCC etc from gtsmip repos (mainly calendar conversion)
-    #TODO: put conversions in separate function?
-    #TODO: maybe add renaming like {'salinity':'so', 'water_temp':'thetao'} for hycom
-    
-    #hirlam workaround
-    if preprocess == preprocess_hirlam:
-        drop_variables = ['x','y'] #will be added again as longitude/latitude, this is a workaround (see dfmt.preprocess_hirlam for details)
-    else:
-        drop_variables = None
-    #woa workaround
-    if preprocess == preprocess_woa:
-        decode_cf = False
-    else:
-        decode_cf = True        
-
-    file_nc_list = file_to_list(file_nc)
-
-    print(f'>> opening multifile dataset of {len(file_nc_list)} files (can take a while with lots of files): ',end='')
-    dtstart = dt.datetime.now()
-    data_xr = xr.open_mfdataset(file_nc_list,
-                                parallel=True, #speeds up the process
-                                preprocess=preprocess,
-                                chunks=chunks,
-                                drop_variables=drop_variables, #necessary since dims/vars with equal names are not allowed by xarray, add again later and requested matroos to adjust netcdf format.
-                                decode_cf=decode_cf)
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    #rename variables
-    if 'longitude' not in data_xr.variables: #TODO: make generic, comparable rename in rename_dims_dict in dfmt.open_dataset_extra()
-        if 'lon' in data_xr.variables:
-            data_xr = data_xr.rename({'lon':'longitude', 'lat':'latitude'})
-        elif 'x' in data_xr.variables:
-            data_xr = data_xr.rename({'x':'longitude', 'y':'latitude'})
-        else:
-            raise KeyError('no longitude/latitude, lon/lat or x/y variables found in dataset')
-
-    varkeys = data_xr.variables.mapping.keys()
-    #data_xr.attrs['comment'] = 'merged with dfm_tools from https://github.com/Deltares/dfm_tools' #TODO: add something like this or other attributes? (some might also be dropped now)
-    
-    #select time and do checks #TODO: check if calendar is standard/gregorian
-    data_xr_tsel = data_xr.sel(time=time_slice)
-    if data_xr_tsel.get_index('time').duplicated().any():
-        print('dropping duplicate timesteps')
-        data_xr_tsel = data_xr_tsel.sel(time=~data_xr_tsel.get_index('time').duplicated()) #drop duplicate timesteps
-    
-    #check if there are times selected
-    if len(data_xr_tsel.time)==0:
-        raise OutOfRangeError(f'ERROR: no times selected, ds_text={data_xr.time[[0,-1]].to_numpy()} and time_slice={time_slice}')
-    
-    #check if there are no gaps (more than one unique timestep)
-    times_pd = data_xr_tsel['time'].to_series()
-    timesteps_uniq = times_pd.diff().iloc[1:].unique()
-    if len(timesteps_uniq)>1:
-        raise Exception(f'ERROR: gaps found in selected dataset (are there sourcefiles missing?), unique timesteps (hour): {timesteps_uniq/1e9/3600}')
-    
-    #check if requested times are available in selected files (in times_pd)
-    if time_slice.start not in times_pd.index:
-        raise OutOfRangeError(f'ERROR: time_slice_start="{time_slice.start}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
-    if time_slice.stop not in times_pd.index:
-        raise OutOfRangeError(f'ERROR: time_slice_stop="{time_slice.stop}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
-    
-    #TODO: check conversion implementation with hydro_tools\ERA5\ERA52DFM.py. Also move to separate function?
-    def get_unit(data_xr_var):
-        if 'units' in data_xr_var.attrs.keys():
-            unit = data_xr_var.attrs["units"]
-        else:
-            unit = '-'
-        return unit
-    #convert Kelvin to Celcius
-    for varkey_sel in ['air_temperature','dew_point_temperature','d2m','t2m']: # 2 meter dewpoint temparature / 2 meter temperature
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'C'
-            print(f'converting {varkey_sel} unit from Kelvin to Celcius: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] - 273.15
-    #convert fraction to percentage
-    for varkey_sel in ['cloud_area_fraction','tcc']: #total cloud cover
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = '%' #unit is soms al %
-            print(f'converting {varkey_sel} unit from fraction to percentage: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 100
-    #convert kg/m2/s to mm/day
-    for varkey_sel in ['mer','mtpr']: #mean evaporation rate / mean total precipitation rate
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'mm/day'
-            print(f'converting {varkey_sel} unit from kg/m2/s to mm/day: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 86400 # kg/m2/s to mm/day (assuming rho_water=1000)
-    #convert J/m2 to W/m2
-    for varkey_sel in ['ssr','strd']: #solar influx (surface_net_solar_radiation) / surface_thermal_radiation_downwards
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'W m**-2'
-            print(f'converting {varkey_sel} unit from J/m2 to W/m2: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] / 3600 # 3600s/h #TODO: 1W = 1J/s, so does not make sense?
-    #solar influx increase for beta=6%
-    if 'ssr' in varkeys:
-        print('ssr (solar influx) increase for beta=6%')
-        data_xr_tsel['ssr'] = data_xr_tsel['ssr'] *.94
-    
-    #convert 0to360 sourcedata to -180to+180
-    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any()
-    if convert_360to180:
-        data_xr.coords['longitude'] = (data_xr.coords['longitude'] + 180) % 360 - 180
-        data_xr = data_xr.sortby(data_xr['longitude'])
-    
-    #GTSM specific addition for longitude overlap
-    if add_global_overlap: # assumes -180 to ~+179.75 (full global extent, but no overlap). Does not seem to mess up results for local models.
-        if len(data_xr_tsel.longitude.values) != len(np.unique(data_xr_tsel.longitude.values%360)):
-            raise Exception(f'add_global_overlap=True, but there are already overlapping longitude values: {data_xr_tsel.longitude}')
-        overlap_ltor = data_xr_tsel.sel(longitude=data_xr_tsel.longitude<=-179)
-        overlap_ltor['longitude'] = overlap_ltor['longitude'] + 360
-        overlap_rtol = data_xr_tsel.sel(longitude=data_xr_tsel.longitude>=179)
-        overlap_rtol['longitude'] = overlap_rtol['longitude'] - 360
-        data_xr_tsel = xr.concat([data_xr_tsel,overlap_ltor,overlap_rtol],dim='longitude').sortby('longitude')
-    
-    #GTSM specific addition for zerovalues during spinup
-    if zerostart:
-        field_zerostart = data_xr_tsel.isel(time=[0,0])*0 #two times first field, set values to 0
-        field_zerostart['time'] = [times_pd.index[0]-dt.timedelta(days=2),times_pd.index[0]-dt.timedelta(days=1)] #TODO: is one zero field not enough? (is replacing first field not also ok? (results in 1hr transition period)
-        data_xr_tsel = xr.concat([field_zerostart,data_xr_tsel],dim='time')#.sortby('time')
-    
-    # converting from int16 to float32 (by removing dtype from encoding) or recompute scale_factor/add_offset is necessary for ERA5 dataset
-    #data_xr_tsel = prevent_dtype_int(data_xr_tsel)
-    data_xr_tsel = recompute_scaling_and_offset(data_xr_tsel)
-    
-    #data_xr_tsel.time.encoding['units'] = 'hours since 1900-01-01 00:00:00' #TODO: maybe add different reftime?
-    
-    return data_xr_tsel
-
-
-def Dataset_varswithdim(ds,dimname): #TODO: dit zit ook in xugrid, wordt nu gebruikt in hisfile voorbeeldscript en kan handig zijn, maar misschien die uit xugrid gebruiken?
-    if dimname not in ds.dims:
-        raise KeyError(f'dimension {dimname} not in dataset, available are: {list(ds.dims)}')
-    
-    varlist_keep = []
-    for varname in ds.variables.keys():
-        if dimname in ds[varname].dims:
-            varlist_keep.append(varname)
-    ds = ds[varlist_keep]
-    
-    return ds
-
-
-def get_vertical_dimensions(uds): #TODO: maybe add layer_dimension and interface_dimension properties to xugrid?
-    """
-    get vertical_dimensions from grid_info of ugrid mapfile (this will fail for hisfiles). The info is stored in the layer_dimension and interface_dimension attribute of the mesh2d variable of the dataset (stored in uds.grid after reading with xugrid)
-    
-    processing cb_3d_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    processing Grevelingen-FM_0*_map.nc
-        >> found layer/interface dimensions in file: nmesh2d_layer nmesh2d_interface (these are updated in open_partitioned_dataset)
-    processing DCSM-FM_0_5nm_0*_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    processing MB_02_0*_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    """
-    
-    if not hasattr(uds,'grid'): #early return in case of e.g. hisfile
-        return None, None
-        
-    gridname = uds.grid.name
-    grid_info = uds.grid.to_dataset()[gridname]
-    if hasattr(grid_info,'layer_dimension'):
-        return grid_info.layer_dimension, grid_info.interface_dimension
-    else:
-        return None, None
-
-
-def remove_ghostcells(uds): #TODO: create JIRA issue: add domainno attribute to partitioned mapfiles or remove ghostcells from output (or make values in ghostcells the same as not-ghostcells)
-    """
-    Dropping ghostcells if there is a domainno variable present and there is a domainno in the filename.
-    Not using most-occurring domainno in var, since this is not a valid assumption for merged datasets and might be invalid for a very small partition.
-    
-    """
-    gridname = uds.grid.name
-    varn_domain = f'{gridname}_flowelem_domain'
-    
-    #check if dataset has domainno variable, return uds if not present
-    if varn_domain not in uds.data_vars:
-        print('[nodomainvar] ',end='')
-        return uds
-    
-    #derive domainno from filename, return uds if not present
-    fname = uds.encoding['source']
-    if '_' not in fname: #safety escape in case there is no _ in the filename
-        print('[nodomainfname] ',end='')
-        return uds
-    fname_splitted = fname.split('_')
-    part_domainno_fromfname = fname_splitted[-2] #this is not valid for rstfiles (date follows after partnumber), but they cannot be read with xugrid anyway since they are mapformat=1
-    if not part_domainno_fromfname.isnumeric() or len(part_domainno_fromfname)!=4:
-        print('[nodomainfname] ',end='')
-        return uds
-    
-    #drop ghostcells
-    part_domainno_fromfname = int(part_domainno_fromfname)
-    da_domainno = uds[varn_domain]
-    idx = np.flatnonzero(da_domainno == part_domainno_fromfname)
-    uds = uds.isel({uds.grid.face_dimension:idx})
-    return uds
-
-
-def remove_periodic_cells(uds): #TODO: implement proper fix: https://github.com/Deltares/xugrid/issues/63
-    """
-    For global models with grids that go "around the back". Temporary fix to drop all faces that are larger than grid_extent/2 (eg 360/2=180 degrees in case of GTSM)
-    
-    """
-    #print('>> remove_periodic_cells() on dataset: ',end='')
-    #dtstart = dt.datetime.now()
-    face_node_x = uds.grid.face_node_coordinates[:,:,0]
-    grid_extent = uds.grid.bounds[2] - uds.grid.bounds[0]
-    face_node_maxdx = np.nanmax(face_node_x,axis=1) - np.nanmin(face_node_x,axis=1)
-    bool_face = face_node_maxdx < grid_extent/2
-    if bool_face.all(): #early return for when no cells have to be removed (might increase performance)
-        return uds
-    uds = uds.sel({uds.grid.face_dimension:bool_face})
-    #print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    return uds
-
-
-def open_partitioned_dataset(file_nc, chunks={'time':1}, remove_ghost=True, remove_periodic=False, **kwargs): 
-    """
-    using xugrid to read and merge partitions, with some additional features (remaning old layerdim, timings, set zcc/zw as data_vars)
-
-    Parameters
-    ----------
-    file_nc : TYPE
-        DESCRIPTION.
-    chunks : TYPE, optional
-        chunks={'time':1} increases performance significantly upon reading, but causes memory overloads when performing sum/mean/etc actions over time dimension (in that case 100/200 is better). The default is {'time':1}.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds_merged_xu : TYPE
-        DESCRIPTION.
-    
-    file_nc = 'p:\\1204257-dcsmzuno\\2006-2012\\3D-DCSM-FM\\A18b_ntsu1\\DFM_OUTPUT_DCSM-FM_0_5nm\\DCSM-FM_0_5nm_0*_map.nc' #3D DCSM
-    file_nc = 'p:\\archivedprojects\\11206813-006-kpp2021_rmm-2d\\C_Work\\31_RMM_FMmodel\\computations\\model_setup\\run_207\\results\\RMM_dflowfm_0*_map.nc' #RMM 2D
-    file_nc = 'p:\\1230882-emodnet_hrsm\\GTSMv5.0\\runs\\reference_GTSMv4.1_wiCA_2.20.06_mapformat4\\output\\gtsm_model_0*_map.nc' #GTSM 2D
-    file_nc = 'p:\\11208053-005-kpp2022-rmm3d\\C_Work\\01_saltiMarlein\\RMM_2019_computations_02\\computations\\theo_03\\DFM_OUTPUT_RMM_dflowfm_2019\\RMM_dflowfm_2019_0*_map.nc' #RMM 3D
-    file_nc = 'p:\\archivedprojects\\11203379-005-mwra-updated-bem\\03_model\\02_final\\A72_ntsu0_kzlb2\\DFM_OUTPUT_MB_02\\MB_02_0*_map.nc'
-    Timings (xu.open_dataset/xu.merge_partitions):
-        - DCSM 3D 20 partitions  367 timesteps: 231.5/ 4.5 sec (decode_times=False: 229.0 sec)
-        - RMM  2D  8 partitions  421 timesteps:  55.4/ 4.4 sec (decode_times=False:  56.6 sec)
-        - GTSM 2D  8 partitions  746 timesteps:  71.8/30.0 sec (decode_times=False: 204.8 sec)
-        - RMM  3D 40 partitions  146 timesteps: 168.8/ 6.3 sec (decode_times=False: 158.4 sec)
-        - MWRA 3D 20 partitions 2551 timesteps:  74.4/ 3.4 sec (decode_times=False:  79.0 sec)
-    
-    """
-    #TODO: FM-mapfiles contain wgs84/projected_coordinate_system variables. xugrid has .crs property, projected_coordinate_system/wgs84 should be updated to be crs so it will be automatically handled? >> make dflowfm issue (and https://github.com/Deltares/xugrid/issues/42)
-    #TODO: add support for multiple grids via keyword? GTSM+riv grid also only contains only one grid, so no testcase available
-    #TODO: speed up open_dataset https://github.com/Deltares/dfm_tools/issues/225 (also remove_ghost and remove_periodic)
-    
-    dtstart_all = dt.datetime.now()
-    file_nc_list = file_to_list(file_nc)
-    
-    print(f'>> xu.open_dataset() with {len(file_nc_list)} partition(s): ',end='')
-    dtstart = dt.datetime.now()
-    partitions = []
-    for iF, file_nc_one in enumerate(file_nc_list):
-        print(iF+1,end=' ')
-        ds = xr.open_dataset(file_nc_one, chunks=chunks, **kwargs)
-        if 'nFlowElem' in ds.dims and 'nNetElem' in ds.dims: #for mapformat1 mapfiles: merge different face dimensions (rename nFlowElem to nNetElem) to make sure the dataset topology is correct
-            print('[mapformat1] ',end='')
-            ds = ds.rename({'nFlowElem':'nNetElem'})
-        uds = xu.core.wrap.UgridDataset(ds)
-        if remove_ghost: #TODO: this makes it way slower (at least for GTSM), but is necessary since values on overlapping cells are not always identical (eg in case of Venice ucmag)
-            uds = remove_ghostcells(uds)
-        if remove_periodic: #TODO: makes it also slower, check if bool/idx makes difference in performance?
-            uds = remove_periodic_cells(uds)
-        partitions.append(uds)
-    print(': ',end='')
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    if len(partitions) == 1: #do not merge in case of 1 partition
-        return partitions[0]
-    
-    print(f'>> xu.merge_partitions() with {len(file_nc_list)} partition(s): ',end='')
-    dtstart = dt.datetime.now()
-    ds_merged_xu = xu.merge_partitions(partitions)
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    #print variables that are dropped in merging procedure. Often only ['mesh2d_face_x_bnd', 'mesh2d_face_y_bnd'], which can be derived by combining node_coordinates (mesh2d_node_x mesh2d_node_y) and face_node_connectivity (mesh2d_face_nodes). >> can be removed from FM-mapfiles (email of 16-1-2023)
-    varlist_onepart = list(partitions[0].variables.keys())
-    varlist_merged = list(ds_merged_xu.variables.keys())
-    varlist_dropped_bool = ~pd.Series(varlist_onepart).isin(varlist_merged)
-    varlist_dropped = pd.Series(varlist_onepart).loc[varlist_dropped_bool]
-    if varlist_dropped_bool.any():
-        print(f'>> some variables dropped with merging of partitions: {varlist_dropped.tolist()}')
-    
-    print(f'>> dfmt.open_partitioned_dataset() total: {(dt.datetime.now()-dtstart_all).total_seconds():.2f} sec')
-    return ds_merged_xu
-
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Oct 14 19:58:36 2022
+
+@author: veenstra
+"""
+
+import os
+import re
+from netCDF4 import Dataset
+import xarray as xr
+import xugrid as xu
+import datetime as dt
+import glob
+import pandas as pd
+import warnings
+import numpy as np
+from dfm_tools.errors import OutOfRangeError
+
+
+def file_to_list(file_nc):
+    if isinstance(file_nc,list):
+        file_nc_list = file_nc
+    else:
+        basename = os.path.basename(file_nc)
+        dirname = os.path.dirname(file_nc)
+        ext = os.path.splitext(file_nc)[-1]
+        if '.*' in basename:
+            def glob_re(pattern, strings):
+                return list(filter(re.compile(pattern).search, strings))
+            file_nc_list = glob_re(basename, glob.glob(os.path.join(dirname,f'*{ext}')))
+        else:
+            file_nc_list = glob.glob(file_nc)
+        file_nc_list.sort()
+    if len(file_nc_list)==0:
+        raise FileNotFoundError('file(s) not found, empty file_nc_list')
+    return file_nc_list
+
+
+def preprocess_hisnc(ds):
+    """
+    Look for dim/coord combination and use this for Dataset.set_index(), to enable station/gs/crs/laterals label based indexing. If duplicate labels are found (like duplicate stations), these are dropped to avoid indexing issues.
+    
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        DESCRIPTION.
+    drop_duplicate_stations : TYPE, optional
+        DESCRIPTION. The default is True.
+
+    Returns
+    -------
+    ds : TYPE
+        DESCRIPTION.
+
+    """
+    
+    #generate dim_coord_dict to set indexes, this will be something like {'stations':'station_name','cross_section':'cross_section_name'} after loop
+    dim_coord_dict = {}
+    for ds_coord in ds.coords.keys():
+        ds_coord_dtype = ds[ds_coord].dtype
+        ds_coord_dim = ds[ds_coord].dims[0] #these vars always have only one dim
+        if ds_coord_dtype.str.startswith('|S'): #these are station/crs/laterals/gs names/ids
+            dim_coord_dict[ds_coord_dim] = ds_coord
+    
+    #loop over dimensions and set corresponding coordinates/variables from dim_coord_dict as their index
+    for dim in dim_coord_dict.keys():
+        coord = dim_coord_dict[dim]
+        ds[coord] = ds[coord].load().str.decode('utf-8',errors='ignore').str.strip() #.load() is essential to convert not only first letter of string.
+        ds = ds.set_index({dim:coord})
+        
+        #drop duplicate indices (stations/crs/gs), this avoids "InvalidIndexError: Reindexing only valid with uniquely valued Index objects"
+        duplicated_keepfirst = ds[dim].to_series().duplicated(keep='first')
+        if duplicated_keepfirst.sum()>0:
+            print(f'dropping {duplicated_keepfirst.sum()} duplicate "{coord}" labels to avoid InvalidIndexError')
+            ds = ds[{dim:~duplicated_keepfirst}]
+
+    #check dflowfm version/date and potentially raise warning about incorrect layers
+    try:
+        source_attr = ds.attrs['source'] # fails if no source attr present in dataset
+        source_attr_version = source_attr.split(', ')[1]
+        source_attr_date = source_attr.split(', ')[2]
+        if pd.Timestamp(source_attr_date) < dt.datetime(2020,11,28):
+            warnings.warn(UserWarning(f'Your model was run with a D-FlowFM version from before 28-10-2020 ({source_attr_version} from {source_attr_date}), the layers in the hisfile are incorrect. Check UNST-2920 and UNST-3024 for more information, it was fixed from OSS 67858.'))
+    except KeyError: #no source attr present in hisfile, cannot check version
+        pass
+    except IndexError: #contains no ', '
+        pass
+
+    return ds
+
+
+def preprocess_hirlam(ds):
+    """
+    add xy variables as longitude/latitude to avoid duplicate var/dim names (we rename it anyway otherwise)
+    add xy as variables again with help of NetCDF4
+    this function is hopefully temporary, necessary since >1D-variables cannot have the same name as one of its dimensions in xarray. Background and future solution: https://github.com/pydata/xarray/issues/6293
+    "MissingDimensionsError: 'y' has more than 1-dimension and the same name as one of its dimensions ('y', 'x'). xarray disallows such variables because they conflict with the coordinates used to label dimensions."
+    might be solved in https://github.com/pydata/xarray/releases/tag/v2023.02.0 (xr.concat), but not certain
+    """
+    
+    print('hirlam workaround: adding dropped x/y variables again as longitude/latitude')
+    file_nc_one = ds.encoding['source']
+    with Dataset(file_nc_one) as data_nc:
+        data_nc_x = data_nc['x']
+        data_nc_y = data_nc['y']
+        ds['longitude'] = xr.DataArray(data_nc_x,dims=data_nc_x.dimensions,attrs=data_nc_x.__dict__) 
+        ds['latitude'] = xr.DataArray(data_nc_y,dims=data_nc_y.dimensions,attrs=data_nc_y.__dict__)
+    ds = ds.set_coords(['latitude','longitude'])
+    for varkey in ds.data_vars:
+        del ds[varkey].encoding['coordinates'] #remove {'coordinates':'y x'} from encoding (otherwise set twice)
+    return ds
+
+
+def preprocess_ERA5(ds):
+    """
+    Reduces the expver dimension in some of the ERA5 data (mtpr and other variables), which occurs in files with very recent data. The dimension contains the unvalidated data from the latest month in the second index in the expver dimension. The reduction is done with mean, but this is arbitrary, since there is only one valid value per timestep and the other one is nan.
+    """
+    if 'expver' in ds.dims:
+        ds = ds.mean(dim='expver')
+    return ds
+
+
+def preprocess_woa(ds):
+    """
+    WOA time units is 'months since 0000-01-01 00:00:00' and calendar is not set (360_day is the only calendar that supports that unit in xarray)
+    """
+    ds.time.attrs['calendar'] = '360_day'
+    ds = xr.decode_cf(ds) #decode_cf after adding 360_day calendar attribute
+    return ds
+
+
+def prevent_dtype_int(ds): #TODO: this is not used, maybe phase out?
+    """
+    Prevent writing to int, since it might mess up dataset (https://github.com/Deltares/dfm_tools/issues/239 and https://github.com/pydata/xarray/issues/7039)
+    Since floats are used instead of ints, the disksize of the dataset will be larger
+    TODO: alternatively remove scale_factor key from attrs, so it can be recomputed (seems to also work): ds[var].encoding.pop('scale_factor')
+    TODO: maybe add to preprocess_ERA5 (preferrably popping scale_factor attribute to keep file size small)
+    """
+    for var in ds.data_vars:
+        var_encoding = ds[var].encoding
+        if 'dtype' in var_encoding.keys():
+            if 'int' in str(var_encoding['dtype']):
+                ds[var].encoding.pop('dtype') #remove dtype key from attrs
+    return ds
+
+
+def recompute_scaling_and_offset(ds:xr.Dataset) -> xr.Dataset:
+    """
+    Recompute add_offset and scale_factor for variables of dtype int. As suggested by https://github.com/ArcticSnow/TopoPyScale/issues/60#issuecomment-1459747654
+    This is a proper fix for https://github.com/Deltares/dfm_tools/issues/239, https://github.com/pydata/xarray/issues/7039 and more
+    However, rescaling causes minor semi-accuracy loss, but it does keep the disksize small (which does not happen when converting it to dtype(float32)).
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds : xr.Dataset
+        DESCRIPTION.
+
+    """
+
+    for var in ds.data_vars:
+        da = ds[var]
+        
+        if 'dtype' not in da.encoding: #check if dype is available, sometime encoding={}
+            continue
+        dtype = da.encoding['dtype']
+        
+        if 'int' not in str(dtype): #skip non-int vars TODO: make proper int-check?
+            continue
+        if 'scale_factor' not in da.encoding.keys() or 'add_offset' not in da.encoding.keys(): #prevent rescaling of non-scaled vars (like crs) #TODO: convert to set().issubset(set())
+            continue
+        
+        n = dtype.itemsize * 8 #n=16 for int16
+        vmin = float(da.min().values)
+        vmax = float(da.max().values)
+        
+        # stretch/compress data to the available packed range
+        scale_factor = (vmax - vmin) / (2 ** n - 1)
+        
+        # translate the range to be symmetric about zero
+        add_offset =  vmin + 2 ** (n - 1) * scale_factor
+        #add_offset = (vmax+vmin)/2 #difference with above is scale_factor/2
+        
+        da.encoding['scale_factor'] = scale_factor
+        da.encoding['add_offset'] = add_offset
+    return ds
+
+
+def merge_meteofiles(file_nc:str, preprocess=None, 
+                     chunks:dict = {'time':1},
+                     time_slice:slice = slice(None,None),
+                     add_global_overlap:bool = False, zerostart:bool = False) -> xr.Dataset:
+    """
+    for merging for instance meteo files
+    x/y and lon/lat are renamed to longitude/latitude #TODO: is this desireable?
+
+    Parameters
+    ----------
+    file_nc : str
+        DESCRIPTION.
+    preprocess : TYPE, optional
+        DESCRIPTION. The default is None.
+    chunks : dict, optional
+        Prevents large chunks and memory issues. The default is {'time':1}.
+    time_slice : slice, optional
+        DESCRIPTION. The default is slice(None,None).
+    add_global_overlap : bool, optional
+        GTSM specific: extend data beyond -180 to 180 longitude. The default is False.
+    zerostart : bool, optional
+        GTSM specific: extend data with 0-value fields 1 and 2 days before time_slice.start. The default is False.
+
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    TYPE
+        DESCRIPTION.
+
+    """
+    #TODO: add ERA5 conversions and features from hydro_tools\ERA5\ERA52DFM.py (except for varRhoair_alt, request FM support for varying airpressure: https://issuetracker.deltares.nl/browse/UNST-6593)
+    #TODO: request FM support for charnock (etc) separate meteo forcing (currently airpressure_windx_windy_charnock merged file is required): https://issuetracker.deltares.nl/browse/UNST-6453
+    #TODO: provide extfile example with fmquantity/ncvarname combinations and cleanup FM code: https://issuetracker.deltares.nl/browse/UNST-6453
+    #TODO: add coordinate conversion (only valid for models with multidimensional lat/lon variables like HARMONIE and HIRLAM). This should work: ds_reproj = ds.set_crs(4326).to_crs(28992)
+    #TODO: add CMCC etc from gtsmip repos (mainly calendar conversion)
+    #TODO: put conversions in separate function?
+    #TODO: maybe add renaming like {'salinity':'so', 'water_temp':'thetao'} for hycom
+    
+    #hirlam workaround
+    if preprocess == preprocess_hirlam:
+        drop_variables = ['x','y'] #will be added again as longitude/latitude, this is a workaround (see dfmt.preprocess_hirlam for details)
+    else:
+        drop_variables = None
+    #woa workaround
+    if preprocess == preprocess_woa:
+        decode_cf = False
+    else:
+        decode_cf = True        
+
+    file_nc_list = file_to_list(file_nc)
+
+    print(f'>> opening multifile dataset of {len(file_nc_list)} files (can take a while with lots of files): ',end='')
+    dtstart = dt.datetime.now()
+    data_xr = xr.open_mfdataset(file_nc_list,
+                                parallel=True, #speeds up the process
+                                preprocess=preprocess,
+                                chunks=chunks,
+                                drop_variables=drop_variables, #necessary since dims/vars with equal names are not allowed by xarray, add again later and requested matroos to adjust netcdf format.
+                                decode_cf=decode_cf)
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    #rename variables
+    if 'longitude' not in data_xr.variables: #TODO: make generic, comparable rename in rename_dims_dict in dfmt.open_dataset_extra()
+        if 'lon' in data_xr.variables:
+            data_xr = data_xr.rename({'lon':'longitude', 'lat':'latitude'})
+        elif 'x' in data_xr.variables:
+            data_xr = data_xr.rename({'x':'longitude', 'y':'latitude'})
+        else:
+            raise KeyError('no longitude/latitude, lon/lat or x/y variables found in dataset')
+
+    varkeys = data_xr.variables.mapping.keys()
+    #data_xr.attrs['comment'] = 'merged with dfm_tools from https://github.com/Deltares/dfm_tools' #TODO: add something like this or other attributes? (some might also be dropped now)
+    
+    #select time and do checks #TODO: check if calendar is standard/gregorian
+    data_xr_tsel = data_xr.sel(time=time_slice)
+    if data_xr_tsel.get_index('time').duplicated().any():
+        print('dropping duplicate timesteps')
+        data_xr_tsel = data_xr_tsel.sel(time=~data_xr_tsel.get_index('time').duplicated()) #drop duplicate timesteps
+    
+    #check if there are times selected
+    if len(data_xr_tsel.time)==0:
+        raise OutOfRangeError(f'ERROR: no times selected, ds_text={data_xr.time[[0,-1]].to_numpy()} and time_slice={time_slice}')
+    
+    #check if there are no gaps (more than one unique timestep)
+    times_pd = data_xr_tsel['time'].to_series()
+    timesteps_uniq = times_pd.diff().iloc[1:].unique()
+    if len(timesteps_uniq)>1:
+        raise Exception(f'ERROR: gaps found in selected dataset (are there sourcefiles missing?), unique timesteps (hour): {timesteps_uniq/1e9/3600}')
+    
+    #check if requested times are available in selected files (in times_pd)
+    if time_slice.start not in times_pd.index:
+        raise OutOfRangeError(f'ERROR: time_slice_start="{time_slice.start}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
+    if time_slice.stop not in times_pd.index:
+        raise OutOfRangeError(f'ERROR: time_slice_stop="{time_slice.stop}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
+    
+    #TODO: check conversion implementation with hydro_tools\ERA5\ERA52DFM.py. Also move to separate function?
+    def get_unit(data_xr_var):
+        if 'units' in data_xr_var.attrs.keys():
+            unit = data_xr_var.attrs["units"]
+        else:
+            unit = '-'
+        return unit
+    #convert Kelvin to Celcius
+    for varkey_sel in ['air_temperature','dew_point_temperature','d2m','t2m']: # 2 meter dewpoint temparature / 2 meter temperature
+        if varkey_sel in varkeys:
+            current_unit = get_unit(data_xr_tsel[varkey_sel])
+            new_unit = 'C'
+            print(f'converting {varkey_sel} unit from Kelvin to Celcius: [{current_unit}] to [{new_unit}]')
+            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
+            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] - 273.15
+    #convert fraction to percentage
+    for varkey_sel in ['cloud_area_fraction','tcc']: #total cloud cover
+        if varkey_sel in varkeys:
+            current_unit = get_unit(data_xr_tsel[varkey_sel])
+            new_unit = '%' #unit is soms al %
+            print(f'converting {varkey_sel} unit from fraction to percentage: [{current_unit}] to [{new_unit}]')
+            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
+            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 100
+    #convert kg/m2/s to mm/day
+    for varkey_sel in ['mer','mtpr']: #mean evaporation rate / mean total precipitation rate
+        if varkey_sel in varkeys:
+            current_unit = get_unit(data_xr_tsel[varkey_sel])
+            new_unit = 'mm/day'
+            print(f'converting {varkey_sel} unit from kg/m2/s to mm/day: [{current_unit}] to [{new_unit}]')
+            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
+            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 86400 # kg/m2/s to mm/day (assuming rho_water=1000)
+    #convert J/m2 to W/m2
+    for varkey_sel in ['ssr','strd']: #solar influx (surface_net_solar_radiation) / surface_thermal_radiation_downwards
+        if varkey_sel in varkeys:
+            current_unit = get_unit(data_xr_tsel[varkey_sel])
+            new_unit = 'W m**-2'
+            print(f'converting {varkey_sel} unit from J/m2 to W/m2: [{current_unit}] to [{new_unit}]')
+            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
+            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] / 3600 # 3600s/h #TODO: 1W = 1J/s, so does not make sense?
+    #solar influx increase for beta=6%
+    if 'ssr' in varkeys:
+        print('ssr (solar influx) increase for beta=6%')
+        data_xr_tsel['ssr'] = data_xr_tsel['ssr'] *.94
+    
+    #convert 0to360 sourcedata to -180to+180
+    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any()
+    if convert_360to180:
+        data_xr.coords['longitude'] = (data_xr.coords['longitude'] + 180) % 360 - 180
+        data_xr = data_xr.sortby(data_xr['longitude'])
+    
+    #GTSM specific addition for longitude overlap
+    if add_global_overlap: # assumes -180 to ~+179.75 (full global extent, but no overlap). Does not seem to mess up results for local models.
+        if len(data_xr_tsel.longitude.values) != len(np.unique(data_xr_tsel.longitude.values%360)):
+            raise Exception(f'add_global_overlap=True, but there are already overlapping longitude values: {data_xr_tsel.longitude}')
+        overlap_ltor = data_xr_tsel.sel(longitude=data_xr_tsel.longitude<=-179)
+        overlap_ltor['longitude'] = overlap_ltor['longitude'] + 360
+        overlap_rtol = data_xr_tsel.sel(longitude=data_xr_tsel.longitude>=179)
+        overlap_rtol['longitude'] = overlap_rtol['longitude'] - 360
+        data_xr_tsel = xr.concat([data_xr_tsel,overlap_ltor,overlap_rtol],dim='longitude').sortby('longitude')
+    
+    #GTSM specific addition for zerovalues during spinup
+    if zerostart:
+        field_zerostart = data_xr_tsel.isel(time=[0,0])*0 #two times first field, set values to 0
+        field_zerostart['time'] = [times_pd.index[0]-dt.timedelta(days=2),times_pd.index[0]-dt.timedelta(days=1)] #TODO: is one zero field not enough? (is replacing first field not also ok? (results in 1hr transition period)
+        data_xr_tsel = xr.concat([field_zerostart,data_xr_tsel],dim='time')#.sortby('time')
+    
+    # converting from int16 to float32 (by removing dtype from encoding) or recompute scale_factor/add_offset is necessary for ERA5 dataset
+    #data_xr_tsel = prevent_dtype_int(data_xr_tsel)
+    data_xr_tsel = recompute_scaling_and_offset(data_xr_tsel)
+    
+    #data_xr_tsel.time.encoding['units'] = 'hours since 1900-01-01 00:00:00' #TODO: maybe add different reftime?
+    
+    return data_xr_tsel
+
+
+def Dataset_varswithdim(ds,dimname): #TODO: dit zit ook in xugrid, wordt nu gebruikt in hisfile voorbeeldscript en kan handig zijn, maar misschien die uit xugrid gebruiken?
+    if dimname not in ds.dims:
+        raise KeyError(f'dimension {dimname} not in dataset, available are: {list(ds.dims)}')
+    
+    varlist_keep = []
+    for varname in ds.variables.keys():
+        if dimname in ds[varname].dims:
+            varlist_keep.append(varname)
+    ds = ds[varlist_keep]
+    
+    return ds
+
+
+def get_vertical_dimensions(uds): #TODO: maybe add layer_dimension and interface_dimension properties to xugrid?
+    """
+    get vertical_dimensions from grid_info of ugrid mapfile (this will fail for hisfiles). The info is stored in the layer_dimension and interface_dimension attribute of the mesh2d variable of the dataset (stored in uds.grid after reading with xugrid)
+    
+    processing cb_3d_map.nc
+        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
+    processing Grevelingen-FM_0*_map.nc
+        >> found layer/interface dimensions in file: nmesh2d_layer nmesh2d_interface (these are updated in open_partitioned_dataset)
+    processing DCSM-FM_0_5nm_0*_map.nc
+        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
+    processing MB_02_0*_map.nc
+        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
+    """
+    
+    if not hasattr(uds,'grid'): #early return in case of e.g. hisfile
+        return None, None
+        
+    gridname = uds.grid.name
+    grid_info = uds.grid.to_dataset()[gridname]
+    if hasattr(grid_info,'layer_dimension'):
+        return grid_info.layer_dimension, grid_info.interface_dimension
+    else:
+        return None, None
+
+
+def remove_ghostcells(uds): #TODO: create JIRA issue: add domainno attribute to partitioned mapfiles or remove ghostcells from output (or make values in ghostcells the same as not-ghostcells)
+    """
+    Dropping ghostcells if there is a domainno variable present and there is a domainno in the filename.
+    Not using most-occurring domainno in var, since this is not a valid assumption for merged datasets and might be invalid for a very small partition.
+    
+    """
+    gridname = uds.grid.name
+    varn_domain = f'{gridname}_flowelem_domain'
+    
+    #check if dataset has domainno variable, return uds if not present
+    if varn_domain not in uds.data_vars:
+        print('[nodomainvar] ',end='')
+        return uds
+    
+    #derive domainno from filename, return uds if not present
+    fname = uds.encoding['source']
+    if '_' not in fname: #safety escape in case there is no _ in the filename
+        print('[nodomainfname] ',end='')
+        return uds
+    fname_splitted = fname.split('_')
+    part_domainno_fromfname = fname_splitted[-2] #this is not valid for rstfiles (date follows after partnumber), but they cannot be read with xugrid anyway since they are mapformat=1
+    if not part_domainno_fromfname.isnumeric() or len(part_domainno_fromfname)!=4:
+        print('[nodomainfname] ',end='')
+        return uds
+    
+    #drop ghostcells
+    part_domainno_fromfname = int(part_domainno_fromfname)
+    da_domainno = uds[varn_domain]
+    idx = np.flatnonzero(da_domainno == part_domainno_fromfname)
+    uds = uds.isel({uds.grid.face_dimension:idx})
+    return uds
+
+
+def remove_periodic_cells(uds): #TODO: implement proper fix: https://github.com/Deltares/xugrid/issues/63
+    """
+    For global models with grids that go "around the back". Temporary fix to drop all faces that are larger than grid_extent/2 (eg 360/2=180 degrees in case of GTSM)
+    
+    """
+    #print('>> remove_periodic_cells() on dataset: ',end='')
+    #dtstart = dt.datetime.now()
+    face_node_x = uds.grid.face_node_coordinates[:,:,0]
+    grid_extent = uds.grid.bounds[2] - uds.grid.bounds[0]
+    face_node_maxdx = np.nanmax(face_node_x,axis=1) - np.nanmin(face_node_x,axis=1)
+    bool_face = face_node_maxdx < grid_extent/2
+    if bool_face.all(): #early return for when no cells have to be removed (might increase performance)
+        return uds
+    uds = uds.sel({uds.grid.face_dimension:bool_face})
+    #print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    return uds
+
+
+def open_partitioned_dataset(file_nc, chunks={'time':1}, remove_ghost=True, remove_periodic=False, **kwargs): 
+    """
+    using xugrid to read and merge partitions, with some additional features (remaning old layerdim, timings, set zcc/zw as data_vars)
+
+    Parameters
+    ----------
+    file_nc : TYPE
+        DESCRIPTION.
+    chunks : TYPE, optional
+        chunks={'time':1} increases performance significantly upon reading, but causes memory overloads when performing sum/mean/etc actions over time dimension (in that case 100/200 is better). The default is {'time':1}.
+
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds_merged_xu : TYPE
+        DESCRIPTION.
+    
+    file_nc = 'p:\\1204257-dcsmzuno\\2006-2012\\3D-DCSM-FM\\A18b_ntsu1\\DFM_OUTPUT_DCSM-FM_0_5nm\\DCSM-FM_0_5nm_0*_map.nc' #3D DCSM
+    file_nc = 'p:\\archivedprojects\\11206813-006-kpp2021_rmm-2d\\C_Work\\31_RMM_FMmodel\\computations\\model_setup\\run_207\\results\\RMM_dflowfm_0*_map.nc' #RMM 2D
+    file_nc = 'p:\\1230882-emodnet_hrsm\\GTSMv5.0\\runs\\reference_GTSMv4.1_wiCA_2.20.06_mapformat4\\output\\gtsm_model_0*_map.nc' #GTSM 2D
+    file_nc = 'p:\\11208053-005-kpp2022-rmm3d\\C_Work\\01_saltiMarlein\\RMM_2019_computations_02\\computations\\theo_03\\DFM_OUTPUT_RMM_dflowfm_2019\\RMM_dflowfm_2019_0*_map.nc' #RMM 3D
+    file_nc = 'p:\\archivedprojects\\11203379-005-mwra-updated-bem\\03_model\\02_final\\A72_ntsu0_kzlb2\\DFM_OUTPUT_MB_02\\MB_02_0*_map.nc'
+    Timings (xu.open_dataset/xu.merge_partitions):
+        - DCSM 3D 20 partitions  367 timesteps: 231.5/ 4.5 sec (decode_times=False: 229.0 sec)
+        - RMM  2D  8 partitions  421 timesteps:  55.4/ 4.4 sec (decode_times=False:  56.6 sec)
+        - GTSM 2D  8 partitions  746 timesteps:  71.8/30.0 sec (decode_times=False: 204.8 sec)
+        - RMM  3D 40 partitions  146 timesteps: 168.8/ 6.3 sec (decode_times=False: 158.4 sec)
+        - MWRA 3D 20 partitions 2551 timesteps:  74.4/ 3.4 sec (decode_times=False:  79.0 sec)
+    
+    """
+    #TODO: FM-mapfiles contain wgs84/projected_coordinate_system variables. xugrid has .crs property, projected_coordinate_system/wgs84 should be updated to be crs so it will be automatically handled? >> make dflowfm issue (and https://github.com/Deltares/xugrid/issues/42)
+    #TODO: add support for multiple grids via keyword? GTSM+riv grid also only contains only one grid, so no testcase available
+    #TODO: speed up open_dataset https://github.com/Deltares/dfm_tools/issues/225 (also remove_ghost and remove_periodic)
+    
+    dtstart_all = dt.datetime.now()
+    file_nc_list = file_to_list(file_nc)
+    
+    print(f'>> xu.open_dataset() with {len(file_nc_list)} partition(s): ',end='')
+    dtstart = dt.datetime.now()
+    partitions = []
+    for iF, file_nc_one in enumerate(file_nc_list):
+        print(iF+1,end=' ')
+        ds = xr.open_dataset(file_nc_one, chunks=chunks, **kwargs)
+        if 'nFlowElem' in ds.dims and 'nNetElem' in ds.dims: #for mapformat1 mapfiles: merge different face dimensions (rename nFlowElem to nNetElem) to make sure the dataset topology is correct
+            print('[mapformat1] ',end='')
+            ds = ds.rename({'nFlowElem':'nNetElem'})
+        uds = xu.core.wrap.UgridDataset(ds)
+        if remove_ghost: #TODO: this makes it way slower (at least for GTSM), but is necessary since values on overlapping cells are not always identical (eg in case of Venice ucmag)
+            uds = remove_ghostcells(uds)
+        if remove_periodic: #TODO: makes it also slower, check if bool/idx makes difference in performance?
+            uds = remove_periodic_cells(uds)
+        partitions.append(uds)
+    print(': ',end='')
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    if len(partitions) == 1: #do not merge in case of 1 partition
+        return partitions[0]
+    
+    print(f'>> xu.merge_partitions() with {len(file_nc_list)} partition(s): ',end='')
+    dtstart = dt.datetime.now()
+    ds_merged_xu = xu.merge_partitions(partitions)
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    #print variables that are dropped in merging procedure. Often only ['mesh2d_face_x_bnd', 'mesh2d_face_y_bnd'], which can be derived by combining node_coordinates (mesh2d_node_x mesh2d_node_y) and face_node_connectivity (mesh2d_face_nodes). >> can be removed from FM-mapfiles (email of 16-1-2023)
+    varlist_onepart = list(partitions[0].variables.keys())
+    varlist_merged = list(ds_merged_xu.variables.keys())
+    varlist_dropped_bool = ~pd.Series(varlist_onepart).isin(varlist_merged)
+    varlist_dropped = pd.Series(varlist_onepart).loc[varlist_dropped_bool]
+    if varlist_dropped_bool.any():
+        print(f'>> some variables dropped with merging of partitions: {varlist_dropped.tolist()}')
+    
+    print(f'>> dfmt.open_partitioned_dataset() total: {(dt.datetime.now()-dtstart_all).total_seconds():.2f} sec')
+    return ds_merged_xu
+
```

### Comparing `dfm_tools-0.10.55/dfm_tools.egg-info/PKG-INFO` & `dfm_tools-0.11.0/dfm_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-Metadata-Version: 2.1
-Name: dfm-tools
-Version: 0.10.55
-Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
-Home-page: https://github.com/Deltares/dfm_tools
-Author: Jelmer Veenstra
-Author-email: Jelmer.Veenstra@Deltares.nl
-License: GNU General Public License v3 (GPLv3)
-Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: complete
-
-[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
-[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
-[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
-[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
-[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
-
-dfm_tools
-=========
-
-A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
-
-Information and examples
---------
-- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
-- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
-
-
-Installation
---------
-- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
-- open Anaconda prompt
-- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
-- ``conda activate dfm_tools_env``
-- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
-- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
-- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
-- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
-- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
+Metadata-Version: 2.1
+Name: dfm-tools
+Version: 0.11.0
+Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
+Home-page: https://github.com/Deltares/dfm_tools
+Author: Jelmer Veenstra
+Author-email: Jelmer.Veenstra@Deltares.nl
+License: GNU General Public License v3 (GPLv3)
+Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: complete
+
+[![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
+[![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
+[![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
+[![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
+[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+
+dfm_tools
+=========
+
+A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
+
+Information and examples
+--------
+- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
+- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
+- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
+- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
+- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
+
+Installation basics
+--------
+- latest release: ``pip install dfm_tools`` (excludes ``cartopy`` since it is only installable via conda)
+
+Installation recommendation
+--------
+- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
+- open Anaconda prompt
+- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
+- ``conda activate dfm_tools_env``
+- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
+- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
+- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
+- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
+- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
```

### Comparing `dfm_tools-0.10.55/dfm_tools.egg-info/SOURCES.txt` & `dfm_tools-0.11.0/dfm_tools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 dfm_tools/__init__.py
 dfm_tools/bathymetry.py
 dfm_tools/deprecated.py
 dfm_tools/download.py
@@ -13,15 +12,14 @@
 dfm_tools/hydrolib_helpers.py
 dfm_tools/interpolate_grid2bnd.py
 dfm_tools/linebuilder.py
 dfm_tools/meshkernel_helpers.py
 dfm_tools/modelbuilder.py
 dfm_tools/modplot.py
 dfm_tools/regulargrid.py
-dfm_tools/streamplot_COPY.py
 dfm_tools/xarray_helpers.py
 dfm_tools.egg-info/PKG-INFO
 dfm_tools.egg-info/SOURCES.txt
 dfm_tools.egg-info/dependency_links.txt
 dfm_tools.egg-info/not-zip-safe
 dfm_tools.egg-info/requires.txt
 dfm_tools.egg-info/top_level.txt
```

### Comparing `dfm_tools-0.10.55/tests/test_dfm_tools.py` & `dfm_tools-0.11.0/tests/test_dfm_tools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-#!/usr/bin/env python
-
-"""Tests for dfm_tools package environment"""
-
-import pytest
-import os
-import glob
-import dfm_tools as dfmt
-import numpy as np
-import hydrolib.core.dflowfm as hcdfm
-import pandas as pd
-import requests
-import pathlib
-import xarray as xr
-
-
-def download_testdata():
-    #TODO: work with pooch instead, like: https://github.com/Deltares/xugrid/blob/main/xugrid/data/sample_data.py
-    #TODO: make opendap folder structure the same as local testdata folder
-    
-    fname_list = []
-    fname_list += ['DFM_curvedbend_3D/cb_3d_map.nc']
-    fname_list += ['DFM_curvedbend_3D/cb_3d_his.nc']
-    fname_list += [f'DFM_grevelingen_3D/Grevelingen-FM_{i:04d}_map.nc' for i in range(8)]
-    fname_list += ['DFM_grevelingen_3D/Grevelingen-FM_0000_his.nc']
-    fname_list += ['DFM_grevelingen_3D/Grevelingen_FM_grid_20190603_net.nc']
-    # fname_list += ['westernscheldt_sph_map.nc']
-
-    for fname in fname_list:
-        file_nc = os.path.join(dir_testinput,fname)
-        file_dirname = os.path.dirname(file_nc)
-        if os.path.exists(file_nc): #skip if file exists
-            continue
-        pathlib.Path(file_dirname).mkdir(parents=True, exist_ok=True) #make subdir if needed
-        
-        file_url = f'https://opendap.deltares.nl/thredds/fileServer/opendap/deltares/Delft3D/netcdf_example_files/{fname}'
-        print(f'downloading {file_url} to {file_nc}')
-        r = requests.get(file_url, allow_redirects=True)
-        r.raise_for_status() #raise HTTPError if url not exists
-        with open(file_nc, 'wb') as f:
-            f.write(r.content)
-
-dir_testinput = os.path.join(r'c:\DATA','dfm_tools_testdata') #on WCF
-if not os.path.exists(dir_testinput): #for instance when running on github or 
-    dir_testinput = './dfm_tools_testdata'
-    download_testdata()
-
-
-# ACCEPTANCE TESTS VIA EXAMPLE SCRIPTS, these are the ones who are only meant to generate output files
-
-dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
-list_configfiles = glob.glob(os.path.join(dir_tests,'examples','*.py')) + glob.glob(os.path.join(dir_tests,'examples_workinprogress','*.py'))
-list_configfiles = [x for x in list_configfiles if 'workinprogress_xarray_performance' not in x] #ignore this slow script
-dir_output_general = os.path.join(dir_tests,'examples_output')
-if not os.path.exists(dir_output_general):
-    os.mkdir(dir_output_general)
-
-@pytest.mark.requireslocaldata
-@pytest.mark.acceptance
-@pytest.mark.parametrize("file_config", [pytest.param(file_config, id=os.path.basename(file_config).replace('.py','')) for file_config in list_configfiles])
-def test_run_examples(file_config):
-    # 1. Set up test data
-    dir_output = os.path.join(dir_output_general,os.path.basename(file_config).replace('.py',''))
-    if not os.path.exists(dir_output):
-        os.mkdir(dir_output)
-    os.chdir(dir_output)
-    test = os.system(f'python {file_config}')#+ " & pause")
-    
-    if test:
-        raise OSError('execution did not finish properly')
-
-
-##### UNITTESTS AND SYSTEMTESTS
-
-@pytest.mark.unittest
-def test_import_shapely():
-    """
-    tests whether shapely can be imported successfully, this is a problem in some environments
-    in that case 'import shapely' works, but import 'shapely.geometry' fails
-    """
-    import shapely
-    import shapely.geometry
-    
-
-@pytest.mark.parametrize("file_nc, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0000_map.nc'), (5599,3,2), id='from 1 map partion Grevelingen'),
-                                                    pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen_FM_grid_20190603_net.nc'), (44804,4,2), id='fromnet Grevelingen')])
-@pytest.mark.systemtest
-def test_facenodecoordinates_shape(file_nc, expected_size):
-    
-    uds = dfmt.open_partitioned_dataset(file_nc)
-    facenodecoordinates = uds.grid.face_node_coordinates
-    
-    assert facenodecoordinates.shape == expected_size
-
-
-@pytest.mark.parametrize("file_nc, varname, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc'), 'mesh2d_sa1', (44796, 36), id='from partitioned map Grevelingen'),
-                                                             pytest.param(os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0*_map.nc'), 'mesh2d_Chlfa', (17385, 39), id='from partitioned waq map coastserv'),
-                                                             #pytest.param(r'p:\11205258-006-kpp2020_rmm-g6\C_Work\01_Rooster\final_totaalmodel\rooster_rmm_v1p5_net.nc', 'mesh2d_face_x', (44804,), id='fromnet RMM'), #no time dimension
-                                                             ])
-@pytest.mark.requireslocaldata
-@pytest.mark.unittest
-def test_getmapdata(file_nc, varname, expected_size):
-    """
-    Checks whether ghost cells are properly taken care of (by asserting shape). And also whether varname can be found from attributes in case of Chlfa.
-    
-    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc')
-    expected_size = (44796,)
-    """
-    
-    data_xr_map = dfmt.open_partitioned_dataset(file_nc)
-    data_xr_map = dfmt.rename_waqvars(data_xr_map)
-    data_varsel = data_xr_map[varname].isel(time=2)
-    
-    assert data_varsel.shape == expected_size
-
-
-@pytest.mark.requireslocaldata
-@pytest.mark.unittest
-def test_rename_waqvars():
-    file_nc = os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0000_map.nc')
-    uds = dfmt.open_partitioned_dataset(file_nc)
-    uds = dfmt.rename_waqvars(uds)
-    
-    assert 'mesh2d_Chlfa' in uds.data_vars
-
-
-@pytest.mark.requireslocaldata
-@pytest.mark.unittest
-def test_rename_fouvars_regular():
-    file_nc_fou = r'p:\archivedprojects\11203379-005-mwra-updated-bem\03_model\02_final\A72_ntsu0_kzlb2\DFM_OUTPUT_MB_02_fou\MB_02_0000_fou.nc'
-    uds = dfmt.open_partitioned_dataset(file_nc_fou)
-    uds_renamed = dfmt.rename_fouvars(uds)
-    
-    assert 'mesh2d_tem_mean_20160201000000_20160301000000' in uds_renamed.data_vars
-    assert 'mesh2d_uy_mean_20160101000000_20170101000000' in uds_renamed.data_vars
-    
-    
-@pytest.mark.requireslocaldata
-@pytest.mark.unittest
-def test_rename_fouvars_tidal():
-    file_nc_fou = r'p:\1230882-emodnet_hrsm\GTSMv3.0EMODnet\EMOD_MichaelTUM_yearcomponents\GTSMv4.1_yeartide_2014_2.20.06\output\gtsm_model_0000_fou.nc'
-    uds = dfmt.open_partitioned_dataset(file_nc_fou)
-    uds_renamed = dfmt.rename_fouvars(uds,drop_tidal_times=False)
-    uds_renamed_clean = dfmt.rename_fouvars(uds)
-    
-    assert 'mesh2d_s1_mean_20131231000000_20150101000000' in uds_renamed.data_vars
-    assert 'mesh2d_s1_min_20131231000000_20150101000000' in uds_renamed.data_vars
-    assert 'mesh2d_s1_mindepth_20131231000000_20150101000000' in uds_renamed.data_vars
-    assert 'mesh2d_s1_ampM2_20131231000000_20141227180000' in uds_renamed.data_vars
-    assert 'mesh2d_s1_mean_20131231000000_20150101000000' in uds_renamed_clean.data_vars
-    assert 'mesh2d_s1_min_20131231000000_20150101000000' in uds_renamed_clean.data_vars
-    assert 'mesh2d_s1_mindepth_20131231000000_20150101000000' in uds_renamed_clean.data_vars
-    assert 'mesh2d_s1_ampM2' in uds_renamed_clean.data_vars
-
-
-@pytest.mark.unittest
-def test_calc_dist_pythagoras():
-    """
-    all crossings for cb3 and testline (which has linebend in cell en with line crosses same cell twice)
-    """
-    edge_index = np.array([0,0,0,1,1,1,2,2])
-
-    edges = np.array([[[2084.67741935, 3353.02419355],
-                       [2255.79637097, 3307.15725806]],
-                      [[2255.79637097, 3307.15725806],
-                       [2222.27822581, 3206.60282258]],
-                      [[2222.27822581, 3206.60282258],
-                       [2128.78024194, 3266.58266129]]])
-
-    intersections = np.array([[[2084.67741935, 3353.02419355],
-                               [2144.15041424, 3337.08297842]],
-                              [[2144.15041424, 3337.08297842],
-                               [2202.53662217, 3321.43306702]],
-                              [[2202.53662217, 3321.43306702],
-                               [2255.79637097, 3307.15725806]],
-                              [[2255.79637097, 3307.15725806],
-                               [2246.9810802,  3280.71138574]],
-                              [[2246.9810802,  3280.71138574],
-                               [2239.02015401, 3256.82860719]],
-                              [[2239.02015401, 3256.82860719],
-                               [2222.27822581, 3206.60282258]],
-                              [[2222.27822581, 3206.60282258],
-                               [2173.05750857, 3238.17837704]],
-                              [[2173.05750857, 3238.17837704],
-                               [2128.78024194, 3266.58266129]]])
-    
-    edge_len = dfmt.calc_dist_pythagoras(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
-    edge_len_cum = np.cumsum(edge_len)
-    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
-    crs_dist_starts = dfmt.calc_dist_pythagoras(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
-    crs_dist_stops  = dfmt.calc_dist_pythagoras(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
-    
-    crs_dist_starts_check = np.array([  0.        ,  61.57239204, 122.01963352, 177.15945184,
-                                      205.03584892, 230.21050794, 283.15313349, 341.63128877])
-    crs_dist_stops_check = np.array([ 61.57239204, 122.01963352, 177.15945184, 205.03584892,
-                                     230.21050794, 283.15313349, 341.63128877, 394.23622869])
-    
-    assert np.allclose(crs_dist_starts, crs_dist_starts_check)
-    assert np.allclose(crs_dist_stops, crs_dist_stops_check)
-
-
-@pytest.mark.unittest
-def test_calc_dist_haversine():
-    """
-    first 15 crossings for DSCM
-    """
-    edge_index = np.array([0,0,0,0,0,0,0,0,0,0,0,0,0,0,0])
- 
-    edges = np.array([[[ 8.92659074, 56.91538014],
-                       [ 8.58447136, 58.66874192]]])
-  
-    intersections = np.array([[[ 8.8856893 , 57.125     ],
-                               [ 8.88406329, 57.13333333]],
-                              [[ 8.88406329, 57.13333333],
-                               [ 8.88243727, 57.14166667]],
-                              [[ 8.88243727, 57.14166667],
-                               [ 8.88081125, 57.15      ]],
-                              [[ 8.88081125, 57.15      ],
-                               [ 8.87918524, 57.15833333]],
-                              [[ 8.87918524, 57.15833333],
-                               [ 8.87755922, 57.16666667]],
-                              [[ 8.87755922, 57.16666667],
-                               [ 8.87593321, 57.175     ]],
-                              [[ 8.87593321, 57.175     ],
-                               [ 8.875     , 57.17978268]],
-                              [[ 8.875     , 57.17978268],
-                               [ 8.87430719, 57.18333333]],
-                              [[ 8.87430719, 57.18333333],
-                               [ 8.87268117, 57.19166667]],
-                              [[ 8.87268117, 57.19166667],
-                               [ 8.87105516, 57.2       ]],
-                              [[ 8.87105516, 57.2       ],
-                               [ 8.86942914, 57.20833333]],
-                              [[ 8.86942914, 57.20833333],
-                               [ 8.86780312, 57.21666667]],
-                              [[ 8.86780312, 57.21666667],
-                               [ 8.86617711, 57.225     ]],
-                              [[ 8.86617711, 57.225     ],
-                               [ 8.86455109, 57.23333333]],
-                              [[ 8.86455109, 57.23333333],
-                               [ 8.86292507, 57.24166667]]])
-    
-    edge_len = dfmt.calc_dist_haversine(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
-    edge_len_cum = np.cumsum(edge_len)
-    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
-    crs_dist_starts = dfmt.calc_dist_haversine(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
-    crs_dist_stops  = dfmt.calc_dist_haversine(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
-    
-    crs_dist_starts_check = np.array([23439.77082715, 24371.57628696, 25303.38057682, 26235.18142118,
-                                      27166.97986164, 28098.77713142, 29030.57089118, 29565.34666042,
-                                      29962.36237409, 30894.15262176, 31825.93935877, 32757.7238182 ,
-                                      33689.50704171, 34621.28675393, 35553.06418784])
-    crs_dist_stops_check = np.array([24371.57628696, 25303.38057682, 26235.18142118, 27166.97986164,
-                                     28098.77713142, 29030.57089118, 29565.34666042, 29962.36237409,
-                                     30894.15262176, 31825.93935877, 32757.7238182 , 33689.50704171,
-                                     34621.28675393, 35553.06418784, 36484.84038514])
-    
-    assert np.allclose(crs_dist_starts, crs_dist_starts_check)
-    assert np.allclose(crs_dist_stops, crs_dist_stops_check)
-
-
-@pytest.mark.unittest
-def test_intersect_edges():
-    """
-    ordering of xu.ugrid2d.intersect_edges return arrays is wrong, but we test it here since this test will fail once sorting is fixed in xugrid or numba.celltree. If so, depracate dfmt.intersect_edges_withsort()
-    """
-    
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
-                    
-    line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
-                           [2255.79637097, 3307.15725806],
-                           [2222.27822581, 3206.60282258],
-                           [2128.78024194, 3266.58266129]])
-    
-    uds = dfmt.open_partitioned_dataset(file_nc)
-    
-    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
-    edge_index, face_index, intersections = uds.grid.intersect_edges(edges)
-    
-    assert (edge_index == np.array([0, 0, 0, 1, 1, 1, 2, 2])).all()
-    assert (face_index == np.array([ 91, 146, 147, 202, 147, 201, 146, 201])).all()
-
-
-@pytest.mark.unittest
-def test_intersect_edges_withsort():
-    """
-    ordering of xu.ugrid2d.intersect_edges return arrays is wrong, so dfmt.intersect_edges_withsort() combines it with sorting. The line array clearly shows different ordering of the resulting face_index array
-    """
-    
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
-    
-    line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
-                           [2255.79637097, 3307.15725806],
-                           [2222.27822581, 3206.60282258],
-                           [2128.78024194, 3266.58266129]])
-    
-    uds = dfmt.open_partitioned_dataset(file_nc)
-    
-    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
-    edge_index, face_index, intersections = dfmt.intersect_edges_withsort(uds,edges)
-    
-    assert (edge_index == np.array([0, 0, 0, 1, 1, 1, 2, 2])).all()
-    assert (face_index == np.array([ 91, 146, 147, 147, 202, 201, 201, 146])).all()
-
-
-@pytest.mark.unittest
-def test_zlayermodel_correct_layers():
-    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc') #zlayer
-    data_frommap_merged = dfmt.open_partitioned_dataset(file_nc)
-    
-    timestep = 3
-    
-    data_frommap_timesel = data_frommap_merged.isel(time=timestep) #select data for all layers
-    data_frommap_merged_fullgrid = dfmt.reconstruct_zw_zcc_fromz(data_frommap_timesel)
-    
-    vals_zw_top = data_frommap_merged_fullgrid['mesh2d_flowelem_zw'].isel(nmesh2d_interface=-1).to_numpy()
-    vals_zw_bot = data_frommap_merged_fullgrid['mesh2d_flowelem_zw'].isel(nmesh2d_interface=0).to_numpy()
-    vals_wl = data_frommap_merged_fullgrid['mesh2d_s1'].to_numpy()
-    vals_bl = data_frommap_merged_fullgrid['mesh2d_flowelem_bl'].to_numpy()
-    assert (np.abs(vals_zw_top-vals_wl)<1e-6).all()
-    assert (np.abs(vals_zw_bot-vals_bl)<1e-6).all()
-
-    
-@pytest.mark.requireslocaldata
-def test_timmodel_to_dataframe():
-    
-    file_tim = os.path.join(dir_testinput,'Brouwerssluis_short.tim')
-    
-    data_tim = hcdfm.TimModel(file_tim)
-    
-    refdate = '2016-01-01'
-    tim_pd = dfmt.TimModel_to_DataFrame(data_tim, parse_column_labels=True, refdate=refdate)
-    
-    assert tim_pd.index[0] == pd.Timestamp('2016-01-01 00:00:00')
-    assert len(tim_pd) == 91
-    assert tim_pd.columns[-1] == 'Phaeocystis_P (g/m3)'
-
-
-@pytest.mark.systemtest
-def test_opendataset_ugridplot(): #this one fails with xarray>=2023.3.0: https://github.com/Deltares/xugrid/issues/78
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D/cb_3d_map.nc')
-    
-    uds = dfmt.open_partitioned_dataset(file_nc,chunks={'time':1})
-
-    uds['mesh2d_flowelem_bl'].ugrid.plot(edgecolors='face', cmap='jet')
-    
-    
-@pytest.mark.unittest
-def test_xr_interp_to_newdim(): #this one fails with scipy>=1.10.0: https://github.com/pydata/xarray/issues/7701
-    ds = xr.Dataset()
-    so_np = np.array([[[35.819576, 35.82568 , 35.82873 ],
-                       [35.819576, 35.824154, 35.831783],
-                       [35.822628, 35.824154, 35.82873 ]],
-                      
-                      [[35.802788, 35.80584 , 35.815   ],
-                       [35.815   , 35.810417, 35.821102],
-                       [35.824154, 35.813473, 35.81805 ]],
-                      
-                      [[35.786003, 35.789055,       np.nan],
-                       [35.807365, 35.796684,       np.nan],
-                       [35.824154, 35.80584 ,       np.nan]],
-                      
-                      [[35.776848,       np.nan,       np.nan],
-                       [35.792107,       np.nan,       np.nan],
-                       [35.822628,       np.nan,       np.nan]],
-                      
-                      [[35.781425,       np.nan,       np.nan],
-                       [35.792107,       np.nan,       np.nan],
-                       [35.789055,       np.nan,       np.nan]]])
-    ds['so'] = xr.DataArray(so_np,dims=('depth','latitude','longitude'))
-    ds['longitude'] = xr.DataArray([-9.6, -9.5, -9.4], dims=('longitude'))
-    ds['latitude'] = xr.DataArray([42.9, 43.0, 43.1], dims=('latitude'))
-    
-    x_xr = xr.DataArray([-9.5],dims=('plipoints'))
-    y_xr = xr.DataArray([43],dims=('plipoints'))
-    
-    
-    interp_with_floats = ds.interp(longitude=x_xr[0], latitude=y_xr[0], method='linear').so #selecting one value from the da drops the new plipoints dimension
-    interp_with_da_existing = ds.interp(longitude=x_xr.values, latitude=y_xr.values, method='linear').so.isel(longitude=0,latitude=0) #using the DataArray values keeps lat/lon dimenions, gives the same interp result
-    interp_with_da_newdim = ds.interp(longitude=x_xr, latitude=y_xr, method='linear').so.isel(plipoints=0) #using the DataArray introduces a plipoints dimension, which gives different interp result
-    print(interp_with_floats.to_numpy())
-    print(interp_with_da_existing.to_numpy())
-    print(interp_with_da_newdim.to_numpy())
-    print(xr.__version__)
-    
-    assert (interp_with_floats.isnull()==interp_with_da_existing.isnull()).all() #success
+#!/usr/bin/env python
+
+"""Tests for dfm_tools package environment"""
+
+import pytest
+import os
+import glob
+import dfm_tools as dfmt
+import numpy as np
+import hydrolib.core.dflowfm as hcdfm
+import pandas as pd
+import requests
+import pathlib
+import xarray as xr
+
+
+def download_testdata():
+    #TODO: work with pooch instead, like: https://github.com/Deltares/xugrid/blob/main/xugrid/data/sample_data.py
+    #TODO: make opendap folder structure the same as local testdata folder
+    
+    fname_list = []
+    fname_list += ['DFM_curvedbend_3D/cb_3d_map.nc']
+    fname_list += ['DFM_curvedbend_3D/cb_3d_his.nc']
+    fname_list += [f'DFM_grevelingen_3D/Grevelingen-FM_{i:04d}_map.nc' for i in range(8)]
+    fname_list += ['DFM_grevelingen_3D/Grevelingen-FM_0000_his.nc']
+    fname_list += ['DFM_grevelingen_3D/Grevelingen_FM_grid_20190603_net.nc']
+    # fname_list += ['westernscheldt_sph_map.nc']
+
+    for fname in fname_list:
+        file_nc = os.path.join(dir_testinput,fname)
+        file_dirname = os.path.dirname(file_nc)
+        if os.path.exists(file_nc): #skip if file exists
+            continue
+        pathlib.Path(file_dirname).mkdir(parents=True, exist_ok=True) #make subdir if needed
+        
+        file_url = f'https://opendap.deltares.nl/thredds/fileServer/opendap/deltares/Delft3D/netcdf_example_files/{fname}'
+        print(f'downloading {file_url} to {file_nc}')
+        r = requests.get(file_url, allow_redirects=True)
+        r.raise_for_status() #raise HTTPError if url not exists
+        with open(file_nc, 'wb') as f:
+            f.write(r.content)
+
+dir_testinput = os.path.join(r'c:\DATA','dfm_tools_testdata') #on WCF
+if not os.path.exists(dir_testinput): #for instance when running on github or 
+    dir_testinput = './dfm_tools_testdata'
+    download_testdata()
+
+
+# ACCEPTANCE TESTS VIA EXAMPLE SCRIPTS, these are the ones who are only meant to generate output files
+
+dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
+list_configfiles = glob.glob(os.path.join(dir_tests,'examples','*.py')) + glob.glob(os.path.join(dir_tests,'examples_workinprogress','*.py'))
+list_configfiles = [x for x in list_configfiles if 'workinprogress_xarray_performance' not in x] #ignore this slow script
+dir_output_general = os.path.join(dir_tests,'examples_output')
+if not os.path.exists(dir_output_general):
+    os.mkdir(dir_output_general)
+
+@pytest.mark.requireslocaldata
+@pytest.mark.acceptance
+@pytest.mark.parametrize("file_config", [pytest.param(file_config, id=os.path.basename(file_config).replace('.py','')) for file_config in list_configfiles])
+def test_run_examples(file_config):
+    # 1. Set up test data
+    dir_output = os.path.join(dir_output_general,os.path.basename(file_config).replace('.py',''))
+    if not os.path.exists(dir_output):
+        os.mkdir(dir_output)
+    os.chdir(dir_output)
+    test = os.system(f'python {file_config}')#+ " & pause")
+    
+    if test:
+        raise OSError('execution did not finish properly')
+
+
+##### UNITTESTS AND SYSTEMTESTS
+
+@pytest.mark.unittest
+def test_import_shapely():
+    """
+    tests whether shapely can be imported successfully, this is a problem in some environments
+    in that case 'import shapely' works, but import 'shapely.geometry' fails
+    """
+    import shapely
+    import shapely.geometry
+    
+
+@pytest.mark.parametrize("file_nc, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0000_map.nc'), (5599,3,2), id='from 1 map partion Grevelingen'),
+                                                    pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen_FM_grid_20190603_net.nc'), (44804,4,2), id='fromnet Grevelingen')])
+@pytest.mark.systemtest
+def test_facenodecoordinates_shape(file_nc, expected_size):
+    
+    uds = dfmt.open_partitioned_dataset(file_nc)
+    facenodecoordinates = uds.grid.face_node_coordinates
+    
+    assert facenodecoordinates.shape == expected_size
+
+
+@pytest.mark.parametrize("file_nc, varname, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc'), 'mesh2d_sa1', (44796, 36), id='from partitioned map Grevelingen'),
+                                                             pytest.param(os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0*_map.nc'), 'mesh2d_Chlfa', (17385, 39), id='from partitioned waq map coastserv'),
+                                                             #pytest.param(r'p:\11205258-006-kpp2020_rmm-g6\C_Work\01_Rooster\final_totaalmodel\rooster_rmm_v1p5_net.nc', 'mesh2d_face_x', (44804,), id='fromnet RMM'), #no time dimension
+                                                             ])
+@pytest.mark.requireslocaldata
+@pytest.mark.unittest
+def test_getmapdata(file_nc, varname, expected_size):
+    """
+    Checks whether ghost cells are properly taken care of (by asserting shape). And also whether varname can be found from attributes in case of Chlfa.
+    
+    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc')
+    expected_size = (44796,)
+    """
+    
+    data_xr_map = dfmt.open_partitioned_dataset(file_nc)
+    data_xr_map = dfmt.rename_waqvars(data_xr_map)
+    data_varsel = data_xr_map[varname].isel(time=2)
+    
+    assert data_varsel.shape == expected_size
+
+
+@pytest.mark.requireslocaldata
+@pytest.mark.unittest
+def test_rename_waqvars():
+    file_nc = os.path.join(r'p:\archivedprojects\11203850-coastserv\06-Model\waq_model\simulations\run0_20200319\DFM_OUTPUT_kzn_waq', 'kzn_waq_0000_map.nc')
+    uds = dfmt.open_partitioned_dataset(file_nc)
+    uds = dfmt.rename_waqvars(uds)
+    
+    assert 'mesh2d_Chlfa' in uds.data_vars
+
+
+@pytest.mark.requireslocaldata
+@pytest.mark.unittest
+def test_rename_fouvars_regular():
+    file_nc_fou = r'p:\archivedprojects\11203379-005-mwra-updated-bem\03_model\02_final\A72_ntsu0_kzlb2\DFM_OUTPUT_MB_02_fou\MB_02_0000_fou.nc'
+    uds = dfmt.open_partitioned_dataset(file_nc_fou)
+    uds_renamed = dfmt.rename_fouvars(uds)
+    
+    assert 'mesh2d_tem_mean_20160201000000_20160301000000' in uds_renamed.data_vars
+    assert 'mesh2d_uy_mean_20160101000000_20170101000000' in uds_renamed.data_vars
+    
+    
+@pytest.mark.requireslocaldata
+@pytest.mark.unittest
+def test_rename_fouvars_tidal():
+    file_nc_fou = r'p:\1230882-emodnet_hrsm\GTSMv3.0EMODnet\EMOD_MichaelTUM_yearcomponents\GTSMv4.1_yeartide_2014_2.20.06\output\gtsm_model_0000_fou.nc'
+    uds = dfmt.open_partitioned_dataset(file_nc_fou)
+    uds_renamed = dfmt.rename_fouvars(uds,drop_tidal_times=False)
+    uds_renamed_clean = dfmt.rename_fouvars(uds)
+    
+    assert 'mesh2d_s1_mean_20131231000000_20150101000000' in uds_renamed.data_vars
+    assert 'mesh2d_s1_min_20131231000000_20150101000000' in uds_renamed.data_vars
+    assert 'mesh2d_s1_mindepth_20131231000000_20150101000000' in uds_renamed.data_vars
+    assert 'mesh2d_s1_ampM2_20131231000000_20141227180000' in uds_renamed.data_vars
+    assert 'mesh2d_s1_mean_20131231000000_20150101000000' in uds_renamed_clean.data_vars
+    assert 'mesh2d_s1_min_20131231000000_20150101000000' in uds_renamed_clean.data_vars
+    assert 'mesh2d_s1_mindepth_20131231000000_20150101000000' in uds_renamed_clean.data_vars
+    assert 'mesh2d_s1_ampM2' in uds_renamed_clean.data_vars
+
+
+@pytest.mark.unittest
+def test_calc_dist_pythagoras():
+    """
+    all crossings for cb3 and testline (which has linebend in cell en with line crosses same cell twice)
+    """
+    edge_index = np.array([0,0,0,1,1,1,2,2])
+
+    edges = np.array([[[2084.67741935, 3353.02419355],
+                       [2255.79637097, 3307.15725806]],
+                      [[2255.79637097, 3307.15725806],
+                       [2222.27822581, 3206.60282258]],
+                      [[2222.27822581, 3206.60282258],
+                       [2128.78024194, 3266.58266129]]])
+
+    intersections = np.array([[[2084.67741935, 3353.02419355],
+                               [2144.15041424, 3337.08297842]],
+                              [[2144.15041424, 3337.08297842],
+                               [2202.53662217, 3321.43306702]],
+                              [[2202.53662217, 3321.43306702],
+                               [2255.79637097, 3307.15725806]],
+                              [[2255.79637097, 3307.15725806],
+                               [2246.9810802,  3280.71138574]],
+                              [[2246.9810802,  3280.71138574],
+                               [2239.02015401, 3256.82860719]],
+                              [[2239.02015401, 3256.82860719],
+                               [2222.27822581, 3206.60282258]],
+                              [[2222.27822581, 3206.60282258],
+                               [2173.05750857, 3238.17837704]],
+                              [[2173.05750857, 3238.17837704],
+                               [2128.78024194, 3266.58266129]]])
+    
+    edge_len = dfmt.calc_dist_pythagoras(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
+    edge_len_cum = np.cumsum(edge_len)
+    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
+    crs_dist_starts = dfmt.calc_dist_pythagoras(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
+    crs_dist_stops  = dfmt.calc_dist_pythagoras(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
+    
+    crs_dist_starts_check = np.array([  0.        ,  61.57239204, 122.01963352, 177.15945184,
+                                      205.03584892, 230.21050794, 283.15313349, 341.63128877])
+    crs_dist_stops_check = np.array([ 61.57239204, 122.01963352, 177.15945184, 205.03584892,
+                                     230.21050794, 283.15313349, 341.63128877, 394.23622869])
+    
+    assert np.allclose(crs_dist_starts, crs_dist_starts_check)
+    assert np.allclose(crs_dist_stops, crs_dist_stops_check)
+
+
+@pytest.mark.unittest
+def test_calc_dist_haversine():
+    """
+    first 15 crossings for DSCM
+    """
+    edge_index = np.array([0,0,0,0,0,0,0,0,0,0,0,0,0,0,0])
+ 
+    edges = np.array([[[ 8.92659074, 56.91538014],
+                       [ 8.58447136, 58.66874192]]])
+  
+    intersections = np.array([[[ 8.8856893 , 57.125     ],
+                               [ 8.88406329, 57.13333333]],
+                              [[ 8.88406329, 57.13333333],
+                               [ 8.88243727, 57.14166667]],
+                              [[ 8.88243727, 57.14166667],
+                               [ 8.88081125, 57.15      ]],
+                              [[ 8.88081125, 57.15      ],
+                               [ 8.87918524, 57.15833333]],
+                              [[ 8.87918524, 57.15833333],
+                               [ 8.87755922, 57.16666667]],
+                              [[ 8.87755922, 57.16666667],
+                               [ 8.87593321, 57.175     ]],
+                              [[ 8.87593321, 57.175     ],
+                               [ 8.875     , 57.17978268]],
+                              [[ 8.875     , 57.17978268],
+                               [ 8.87430719, 57.18333333]],
+                              [[ 8.87430719, 57.18333333],
+                               [ 8.87268117, 57.19166667]],
+                              [[ 8.87268117, 57.19166667],
+                               [ 8.87105516, 57.2       ]],
+                              [[ 8.87105516, 57.2       ],
+                               [ 8.86942914, 57.20833333]],
+                              [[ 8.86942914, 57.20833333],
+                               [ 8.86780312, 57.21666667]],
+                              [[ 8.86780312, 57.21666667],
+                               [ 8.86617711, 57.225     ]],
+                              [[ 8.86617711, 57.225     ],
+                               [ 8.86455109, 57.23333333]],
+                              [[ 8.86455109, 57.23333333],
+                               [ 8.86292507, 57.24166667]]])
+    
+    edge_len = dfmt.calc_dist_haversine(edges[:,0,0], edges[:,1,0], edges[:,0,1], edges[:,1,1])
+    edge_len_cum = np.cumsum(edge_len)
+    edge_len_cum0 = np.concatenate([[0],edge_len_cum[:-1]])
+    crs_dist_starts = dfmt.calc_dist_haversine(edges[edge_index,0,0], intersections[:,0,0], edges[edge_index,0,1], intersections[:,0,1]) + edge_len_cum0[edge_index]
+    crs_dist_stops  = dfmt.calc_dist_haversine(edges[edge_index,0,0], intersections[:,1,0], edges[edge_index,0,1], intersections[:,1,1]) + edge_len_cum0[edge_index]
+    
+    crs_dist_starts_check = np.array([23439.77082715, 24371.57628696, 25303.38057682, 26235.18142118,
+                                      27166.97986164, 28098.77713142, 29030.57089118, 29565.34666042,
+                                      29962.36237409, 30894.15262176, 31825.93935877, 32757.7238182 ,
+                                      33689.50704171, 34621.28675393, 35553.06418784])
+    crs_dist_stops_check = np.array([24371.57628696, 25303.38057682, 26235.18142118, 27166.97986164,
+                                     28098.77713142, 29030.57089118, 29565.34666042, 29962.36237409,
+                                     30894.15262176, 31825.93935877, 32757.7238182 , 33689.50704171,
+                                     34621.28675393, 35553.06418784, 36484.84038514])
+    
+    assert np.allclose(crs_dist_starts, crs_dist_starts_check)
+    assert np.allclose(crs_dist_stops, crs_dist_stops_check)
+
+
+@pytest.mark.unittest
+def test_intersect_edges():
+    """
+    ordering of xu.ugrid2d.intersect_edges return arrays is wrong, but we test it here since this test will fail once sorting is fixed in xugrid or numba.celltree. If so, depracate dfmt.intersect_edges_withsort()
+    """
+    
+    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
+                    
+    line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
+                           [2255.79637097, 3307.15725806],
+                           [2222.27822581, 3206.60282258],
+                           [2128.78024194, 3266.58266129]])
+    
+    uds = dfmt.open_partitioned_dataset(file_nc)
+    
+    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
+    edge_index, face_index, intersections = uds.grid.intersect_edges(edges)
+    
+    assert (edge_index == np.array([0, 0, 0, 1, 1, 1, 2, 2])).all()
+    assert (face_index == np.array([ 91, 146, 147, 202, 147, 201, 146, 201])).all()
+
+
+@pytest.mark.unittest
+def test_intersect_edges_withsort():
+    """
+    ordering of xu.ugrid2d.intersect_edges return arrays is wrong, so dfmt.intersect_edges_withsort() combines it with sorting. The line array clearly shows different ordering of the resulting face_index array
+    """
+    
+    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D','cb_3d_map.nc') #sigmalayer
+    
+    line_array = np.array([[2084.67741935, 3353.02419355], #with linebend in cell en with line crossing same cell twice
+                           [2255.79637097, 3307.15725806],
+                           [2222.27822581, 3206.60282258],
+                           [2128.78024194, 3266.58266129]])
+    
+    uds = dfmt.open_partitioned_dataset(file_nc)
+    
+    edges = np.stack([line_array[:-1],line_array[1:]],axis=1)
+    edge_index, face_index, intersections = dfmt.intersect_edges_withsort(uds,edges)
+    
+    assert (edge_index == np.array([0, 0, 0, 1, 1, 1, 2, 2])).all()
+    assert (face_index == np.array([ 91, 146, 147, 147, 202, 201, 201, 146])).all()
+
+
+@pytest.mark.unittest
+def test_zlayermodel_correct_layers():
+    file_nc = os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0*_map.nc') #zlayer
+    data_frommap_merged = dfmt.open_partitioned_dataset(file_nc)
+    
+    timestep = 3
+    
+    data_frommap_timesel = data_frommap_merged.isel(time=timestep) #select data for all layers
+    data_frommap_merged_fullgrid = dfmt.reconstruct_zw_zcc_fromz(data_frommap_timesel)
+    
+    vals_zw_top = data_frommap_merged_fullgrid['mesh2d_flowelem_zw'].isel(nmesh2d_interface=-1).to_numpy()
+    vals_zw_bot = data_frommap_merged_fullgrid['mesh2d_flowelem_zw'].isel(nmesh2d_interface=0).to_numpy()
+    vals_wl = data_frommap_merged_fullgrid['mesh2d_s1'].to_numpy()
+    vals_bl = data_frommap_merged_fullgrid['mesh2d_flowelem_bl'].to_numpy()
+    assert (np.abs(vals_zw_top-vals_wl)<1e-6).all()
+    assert (np.abs(vals_zw_bot-vals_bl)<1e-6).all()
+
+    
+@pytest.mark.requireslocaldata
+def test_timmodel_to_dataframe():
+    
+    file_tim = os.path.join(dir_testinput,'Brouwerssluis_short.tim')
+    
+    data_tim = hcdfm.TimModel(file_tim)
+    
+    refdate = '2016-01-01'
+    tim_pd = dfmt.TimModel_to_DataFrame(data_tim, parse_column_labels=True, refdate=refdate)
+    
+    assert tim_pd.index[0] == pd.Timestamp('2016-01-01 00:00:00')
+    assert len(tim_pd) == 91
+    assert tim_pd.columns[-1] == 'Phaeocystis_P (g/m3)'
+
+
+@pytest.mark.systemtest
+def test_opendataset_ugridplot(): #this one fails with xarray>=2023.3.0: https://github.com/Deltares/xugrid/issues/78
+    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D/cb_3d_map.nc')
+    
+    uds = dfmt.open_partitioned_dataset(file_nc,chunks={'time':1})
+
+    uds['mesh2d_flowelem_bl'].ugrid.plot(edgecolors='face', cmap='jet')
+    
+    
+@pytest.mark.unittest
+def test_xr_interp_to_newdim(): #this one fails with scipy>=1.10.0: https://github.com/pydata/xarray/issues/7701
+    ds = xr.Dataset()
+    so_np = np.array([[[35.819576, 35.82568 , 35.82873 ],
+                       [35.819576, 35.824154, 35.831783],
+                       [35.822628, 35.824154, 35.82873 ]],
+                      
+                      [[35.802788, 35.80584 , 35.815   ],
+                       [35.815   , 35.810417, 35.821102],
+                       [35.824154, 35.813473, 35.81805 ]],
+                      
+                      [[35.786003, 35.789055,       np.nan],
+                       [35.807365, 35.796684,       np.nan],
+                       [35.824154, 35.80584 ,       np.nan]],
+                      
+                      [[35.776848,       np.nan,       np.nan],
+                       [35.792107,       np.nan,       np.nan],
+                       [35.822628,       np.nan,       np.nan]],
+                      
+                      [[35.781425,       np.nan,       np.nan],
+                       [35.792107,       np.nan,       np.nan],
+                       [35.789055,       np.nan,       np.nan]]])
+    ds['so'] = xr.DataArray(so_np,dims=('depth','latitude','longitude'))
+    ds['longitude'] = xr.DataArray([-9.6, -9.5, -9.4], dims=('longitude'))
+    ds['latitude'] = xr.DataArray([42.9, 43.0, 43.1], dims=('latitude'))
+    
+    x_xr = xr.DataArray([-9.5],dims=('plipoints'))
+    y_xr = xr.DataArray([43],dims=('plipoints'))
+    
+    
+    interp_with_floats = ds.interp(longitude=x_xr[0], latitude=y_xr[0], method='linear').so #selecting one value from the da drops the new plipoints dimension
+    interp_with_da_existing = ds.interp(longitude=x_xr.values, latitude=y_xr.values, method='linear').so.isel(longitude=0,latitude=0) #using the DataArray values keeps lat/lon dimenions, gives the same interp result
+    interp_with_da_newdim = ds.interp(longitude=x_xr, latitude=y_xr, method='linear').so.isel(plipoints=0) #using the DataArray introduces a plipoints dimension, which gives different interp result
+    print(interp_with_floats.to_numpy())
+    print(interp_with_da_existing.to_numpy())
+    print(interp_with_da_newdim.to_numpy())
+    print(xr.__version__)
+    
+    assert (interp_with_floats.isnull()==interp_with_da_existing.isnull()).all() #success
     assert (interp_with_floats.isnull()==interp_with_da_newdim.isnull()).all() #fails with scipy>=1.10.0
```


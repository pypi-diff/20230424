# Comparing `tmp/quasardb-3.9.8.tar.gz` & `tmp/quasardb-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasardb-3.9.8.tar", last modified: Fri Mar 26 09:14:10 2021, max compression
+gzip compressed data, was "quasardb-3.9.9.tar", last modified: Tue Jul  6 07:27:48 2021, max compression
```

## Comparing `quasardb-3.9.8.tar` & `quasardb-3.9.9.tar`

### file list

```diff
@@ -1,185 +1,189 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.209954 quasardb-3.9.8/
--rw-rw-r--   0 root         (0) root         (0)     2092 2021-03-26 09:13:08.000000 quasardb-3.9.8/.clang-format
--rw-rw-r--   0 root         (0) root         (0)     1749 2021-03-26 09:13:08.000000 quasardb-3.9.8/.gitignore
--rw-rw-r--   0 root         (0) root         (0)      129 2021-03-26 09:13:08.000000 quasardb-3.9.8/.gitmodules
--rw-rw-r--   0 root         (0) root         (0)     1467 2021-03-26 09:13:08.000000 quasardb-3.9.8/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      927 2021-03-26 09:14:10.209954 quasardb-3.9.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2829 2021-03-26 09:13:08.000000 quasardb-3.9.8/README.md
--rw-rw-r--   0 root         (0) root         (0)      245 2021-03-26 09:13:08.000000 quasardb-3.9.8/dev-requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      574 2021-03-26 09:13:08.000000 quasardb-3.9.8/docgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.169957 quasardb-3.9.8/docker/
--rw-rw-r--   0 root         (0) root         (0)      135 2021-03-26 09:13:08.000000 quasardb-3.9.8/docker/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1563 2021-03-26 09:13:08.000000 quasardb-3.9.8/docker/Dockerfile.centos
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.173956 quasardb-3.9.8/examples/
--rw-rw-r--   0 root         (0) root         (0)     6355 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/batch_ts_insert.py
--rw-rw-r--   0 root         (0) root         (0)     3101 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/cluster_sync.py
--rw-rw-r--   0 root         (0) root         (0)     3318 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/csv_insert.py
--rw-rw-r--   0 root         (0) root         (0)     2772 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/expiry.py
--rw-rw-r--   0 root         (0) root         (0)   437175 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/fake_currency_minutes.csv
--rw-rw-r--   0 root         (0) root         (0)     6931 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/import_minutes.py
--rw-rw-r--   0 root         (0) root         (0)     3194 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/query_tags.py
--rw-rw-r--   0 root         (0) root         (0)     4484 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/temperature.py
--rw-rw-r--   0 root         (0) root         (0)     4609 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/time_series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.173956 quasardb-3.9.8/examples/tutorial/
--rw-rw-r--   0 root         (0) root         (0)     3132 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/tutorial/pandas_tutorial.py
--rw-rw-r--   0 root         (0) root         (0)     6103 2021-03-26 09:13:08.000000 quasardb-3.9.8/examples/tutorial/python.py
--rw-rw-r--   0 root         (0) root         (0)       72 2021-03-26 09:13:08.000000 quasardb-3.9.8/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.181956 quasardb-3.9.8/quasardb/
--rw-rw-r--   0 root         (0) root         (0)     4115 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1845 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3299 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/batch_column.hpp
--rw-rw-r--   0 root         (0) root         (0)     9903 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/batch_inserter.hpp
--rw-rw-r--   0 root         (0) root         (0)     6552 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/blob.hpp
--rw-rw-r--   0 root         (0) root         (0)    13226 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/cluster.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.181956 quasardb-3.9.8/quasardb/detail/
--rw-rw-r--   0 root         (0) root         (0)     4822 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/detail/ts_column.hpp
--rw-rw-r--   0 root         (0) root         (0)     2995 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/direct_blob.hpp
--rw-rw-r--   0 root         (0) root         (0)     2699 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/direct_handle.hpp
--rw-rw-r--   0 root         (0) root         (0)     2530 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/direct_integer.hpp
--rw-rw-r--   0 root         (0) root         (0)     8878 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/entry.hpp
--rw-rw-r--   0 root         (0) root         (0)     6397 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/error.hpp
--rw-rw-r--   0 root         (0) root         (0)     3492 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/firehose.py
--rw-rw-r--   0 root         (0) root         (0)     2417 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/handle.hpp
--rw-rw-r--   0 root         (0) root         (0)     3847 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/integer.hpp
--rw-rw-r--   0 root         (0) root         (0)     2927 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/logger.cpp
--rw-rw-r--   0 root         (0) root         (0)     7072 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/logger.hpp
--rw-rw-r--   0 root         (0) root         (0)     1822 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/memcpy_wrap.cpp
--rw-rw-r--   0 root         (0) root         (0)     3290 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/node.hpp
--rw-rw-r--   0 root         (0) root         (0)     6415 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/numpy.hpp
--rw-rw-r--   0 root         (0) root         (0)     6762 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/options.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.185955 quasardb-3.9.8/quasardb/pandas/
--rw-rw-r--   0 root         (0) root         (0)    22159 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pandas/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6521 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/perf.hpp
--rw-rw-r--   0 root         (0) root         (0)    27044 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pinned_writer.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.189955 quasardb-3.9.8/quasardb/pybind11/
--rw-rw-r--   0 root         (0) root         (0)     1304 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.appveyor.yml
--rw-rw-r--   0 root         (0) root         (0)      523 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.clang-format
--rw-rw-r--   0 root         (0) root         (0)      242 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.clang-tidy
--rw-rw-r--   0 root         (0) root         (0)     2196 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.cmake-format.yaml
--rw-rw-r--   0 root         (0) root         (0)      452 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     2460 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 root         (0) root         (0)       62 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/.readthedocs.yml
--rw-rw-r--   0 root         (0) root         (0)    10364 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1684 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      256 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     8064 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.165957 quasardb-3.9.8/quasardb/pybind11/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.193955 quasardb-3.9.8/quasardb/pybind11/include/pybind11/
--rw-rw-r--   0 root         (0) root         (0)    21412 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 root         (0) root         (0)     6118 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 root         (0) root         (0)    95557 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 root         (0) root         (0)     7812 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 root         (0) root         (0)      120 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/common.h
--rw-rw-r--   0 root         (0) root         (0)     2037 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.197955 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/
--rw-rw-r--   0 root         (0) root         (0)    27823 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 root         (0) root         (0)    40452 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 root         (0) root         (0)     3602 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 root         (0) root         (0)    16397 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 root         (0) root         (0)    16375 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 root         (0) root         (0)     1486 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 root         (0) root         (0)    29086 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 root         (0) root         (0)     7843 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 root         (0) root         (0)     5079 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 root         (0) root         (0)     3709 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 root         (0) root         (0)     6084 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 root         (0) root         (0)    70448 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 root         (0) root         (0)     9085 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 root         (0) root         (0)     2049 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/options.h
--rw-rw-r--   0 root         (0) root         (0)   111558 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 root         (0) root         (0)    66118 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/pytypes.h
--rw-rw-r--   0 root         (0) root         (0)    14136 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 root         (0) root         (0)    23912 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.197955 quasardb-3.9.8/quasardb/pybind11/pybind11/
--rw-rw-r--   0 root         (0) root         (0)      217 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1158 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/__main__.py
--rw-rw-r--   0 root         (0) root         (0)      202 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/_version.py
--rw-rw-r--   0 root         (0) root         (0)      137 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/_version.pyi
--rw-rw-r--   0 root         (0) root         (0)      663 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/commands.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/py.typed
--rw-rw-r--   0 root         (0) root         (0)    15110 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/setup_helpers.py
--rw-rw-r--   0 root         (0) root         (0)     1899 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pybind11/setup_helpers.pyi
--rw-rw-r--   0 root         (0) root         (0)      118 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     2185 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3499 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.201954 quasardb-3.9.8/quasardb/pybind11/tools/
--rw-rw-r--   0 root         (0) root         (0)     2295 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 root         (0) root         (0)     3105 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 root         (0) root         (0)     9977 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/FindPythonLibsNew.cmake
--rwxrwxr-x   0 root         (0) root         (0)     1427 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/check-style.sh
--rw-rw-r--   0 root         (0) root         (0)      952 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 root         (0) root         (0)     1121 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/libsize.py
--rw-rw-r--   0 root         (0) root         (0)     1202 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/make_changelog.py
--rw-rw-r--   0 root         (0) root         (0)    14003 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 root         (0) root         (0)     7010 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 root         (0) root         (0)     9172 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 root         (0) root         (0)     7276 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 root         (0) root         (0)       94 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1822 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 root         (0) root         (0)      915 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 root         (0) root         (0)     2625 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/qdb_client.cpp
--rw-rw-r--   0 root         (0) root         (0)     6404 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/query.cpp
--rw-rw-r--   0 root         (0) root         (0)     2942 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/query.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.201954 quasardb-3.9.8/quasardb/reader/
--rw-rw-r--   0 root         (0) root         (0)     9352 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/reader/ts_row.hpp
--rw-rw-r--   0 root         (0) root         (0)     6706 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/reader/ts_value.hpp
--rw-rw-r--   0 root         (0) root         (0)      580 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/remove_cvref.hpp
--rw-rw-r--   0 root         (0) root         (0)     1791 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/stats.py
--rw-rw-r--   0 root         (0) root         (0)    14771 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/table.hpp
--rw-rw-r--   0 root         (0) root         (0)     6552 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/table_reader.hpp
--rw-rw-r--   0 root         (0) root         (0)     2655 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/tag.hpp
--rw-rw-r--   0 root         (0) root         (0)    14349 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/ts_convert.hpp
--rw-rw-r--   0 root         (0) root         (0)     4161 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/ts_iterator.hpp
--rw-rw-r--   0 root         (0) root         (0)     3664 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/utils.hpp
--rw-rw-r--   0 root         (0) root         (0)     2759 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/version.cpp
--rw-rw-r--   0 root         (0) root         (0)     2106 2021-03-26 09:13:08.000000 quasardb-3.9.8/quasardb/version.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.181956 quasardb-3.9.8/quasardb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      927 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4891 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-03-26 09:14:10.000000 quasardb-3.9.8/quasardb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.169957 quasardb-3.9.8/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.201954 quasardb-3.9.8/scripts/release/
--rw-rw-r--   0 root         (0) root         (0)     1604 2021-03-26 09:13:08.000000 quasardb-3.9.8/scripts/release/set_version.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.201954 quasardb-3.9.8/scripts/test/
--rw-rw-r--   0 root         (0) root         (0)       42 2021-03-26 09:13:08.000000 quasardb-3.9.8/scripts/test/smoke-test.py
--rwxrwxr-x   0 root         (0) root         (0)      291 2021-03-26 09:13:08.000000 quasardb-3.9.8/scripts/test/smoke-test.sh
--rw-rw-r--   0 root         (0) root         (0)       63 2021-03-26 09:14:10.213954 quasardb-3.9.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     6106 2021-03-26 09:13:08.000000 quasardb-3.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-26 09:14:10.209954 quasardb-3.9.8/tests/
--rw-rw-r--   0 root         (0) root         (0)     4271 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/conftest.py
--rw-rw-r--   0 root         (0) root         (0)      361 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_basic.py
--rw-rw-r--   0 root         (0) root         (0)    10797 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_batch_inserter.py
--rw-rw-r--   0 root         (0) root         (0)     7368 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_bench_pinned_writer.py
--rw-rw-r--   0 root         (0) root         (0)     2865 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_blob.py
--rw-rw-r--   0 root         (0) root         (0)     1480 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_buf_size.py
--rw-rw-r--   0 root         (0) root         (0)      406 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_cluster.py
--rw-rw-r--   0 root         (0) root         (0)     2146 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_connection.py
--rw-rw-r--   0 root         (0) root         (0)      231 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_error.py
--rw-rw-r--   0 root         (0) root         (0)      319 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_examples.py
--rw-rw-r--   0 root         (0) root         (0)     2963 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_expiry.py
--rw-rw-r--   0 root         (0) root         (0)     3974 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_firehose.py
--rw-rw-r--   0 root         (0) root         (0)      290 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_getTimeout.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_info.py
--rw-rw-r--   0 root         (0) root         (0)      879 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_integer.py
--rw-rw-r--   0 root         (0) root         (0)     2082 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_logging.py
--rw-rw-r--   0 root         (0) root         (0)     1118 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_node.py
--rw-rw-r--   0 root         (0) root         (0)      910 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_option_client_max_parallelism.py
--rw-rw-r--   0 root         (0) root         (0)    10883 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_pandas.py
--rw-rw-r--   0 root         (0) root         (0)     2752 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_pandas_benchmark.py
--rw-rw-r--   0 root         (0) root         (0)    14326 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_pandas_pinned.py
--rw-rw-r--   0 root         (0) root         (0)     1144 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_perf.py
--rw-rw-r--   0 root         (0) root         (0)    26248 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_pinned_writer.py
--rw-rw-r--   0 root         (0) root         (0)      649 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_prefix.py
--rw-rw-r--   0 root         (0) root         (0)     9256 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_query.py
--rw-rw-r--   0 root         (0) root         (0)     1059 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_query_find.py
--rw-rw-r--   0 root         (0) root         (0)      485 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_setCompression.py
--rw-rw-r--   0 root         (0) root         (0)      517 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_setMaxCardinality.py
--rw-rw-r--   0 root         (0) root         (0)      529 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_setTimeout.py
--rw-rw-r--   0 root         (0) root         (0)     2726 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_stats.py
--rw-rw-r--   0 root         (0) root         (0)      649 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_suffix.py
--rw-rw-r--   0 root         (0) root         (0)    18494 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_table.py
--rw-rw-r--   0 root         (0) root         (0)     6954 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_table_reader.py
--rw-rw-r--   0 root         (0) root         (0)      971 2021-03-26 09:13:08.000000 quasardb-3.9.8/tests/test_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.368872 quasardb-3.9.9/
+-rw-rw-r--   0 root         (0) root         (0)     2092 2021-07-06 07:21:45.000000 quasardb-3.9.9/.clang-format
+-rw-rw-r--   0 root         (0) root         (0)     1749 2021-07-06 07:21:45.000000 quasardb-3.9.9/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)      129 2021-07-06 07:21:45.000000 quasardb-3.9.9/.gitmodules
+-rw-rw-r--   0 root         (0) root         (0)     1467 2021-07-06 07:21:45.000000 quasardb-3.9.9/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      941 2021-07-06 07:27:48.368872 quasardb-3.9.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2829 2021-07-06 07:21:45.000000 quasardb-3.9.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)      255 2021-07-06 07:21:45.000000 quasardb-3.9.9/dev-requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      574 2021-07-06 07:21:45.000000 quasardb-3.9.9/docgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.332873 quasardb-3.9.9/docker/
+-rw-rw-r--   0 root         (0) root         (0)     1476 2021-07-06 07:21:45.000000 quasardb-3.9.9/docker/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)     1563 2021-07-06 07:21:45.000000 quasardb-3.9.9/docker/Dockerfile.centos
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.332873 quasardb-3.9.9/examples/
+-rw-rw-r--   0 root         (0) root         (0)     6355 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/batch_ts_insert.py
+-rw-rw-r--   0 root         (0) root         (0)     3101 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/cluster_sync.py
+-rw-rw-r--   0 root         (0) root         (0)     3318 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/csv_insert.py
+-rw-rw-r--   0 root         (0) root         (0)     2772 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/expiry.py
+-rw-rw-r--   0 root         (0) root         (0)   437175 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/fake_currency_minutes.csv
+-rw-rw-r--   0 root         (0) root         (0)     6931 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/import_minutes.py
+-rw-rw-r--   0 root         (0) root         (0)     3194 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/query_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     4484 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/temperature.py
+-rw-rw-r--   0 root         (0) root         (0)     4609 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.336873 quasardb-3.9.9/examples/tutorial/
+-rw-rw-r--   0 root         (0) root         (0)     3132 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/tutorial/pandas_tutorial.py
+-rw-rw-r--   0 root         (0) root         (0)     6103 2021-07-06 07:21:45.000000 quasardb-3.9.9/examples/tutorial/python.py
+-rw-rw-r--   0 root         (0) root         (0)       72 2021-07-06 07:21:45.000000 quasardb-3.9.9/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.340873 quasardb-3.9.9/quasardb/
+-rw-rw-r--   0 root         (0) root         (0)     4427 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1845 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3299 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/batch_column.hpp
+-rw-rw-r--   0 root         (0) root         (0)     9903 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/batch_inserter.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6552 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/blob.hpp
+-rw-rw-r--   0 root         (0) root         (0)    13226 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/cluster.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.344873 quasardb-3.9.9/quasardb/detail/
+-rw-rw-r--   0 root         (0) root         (0)     5372 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/detail/ts_column.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2995 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/direct_blob.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2699 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/direct_handle.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2530 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/direct_integer.hpp
+-rw-rw-r--   0 root         (0) root         (0)     8878 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/entry.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6397 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/error.hpp
+-rw-rw-r--   0 root         (0) root         (0)     3492 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/firehose.py
+-rw-rw-r--   0 root         (0) root         (0)     2417 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/handle.hpp
+-rw-rw-r--   0 root         (0) root         (0)     3847 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/integer.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2927 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/logger.cpp
+-rw-rw-r--   0 root         (0) root         (0)     7072 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/logger.hpp
+-rw-rw-r--   0 root         (0) root         (0)     1822 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/memcpy_wrap.cpp
+-rw-rw-r--   0 root         (0) root         (0)     3290 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/node.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6415 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/numpy.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6762 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/options.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.344873 quasardb-3.9.9/quasardb/pandas/
+-rw-rw-r--   0 root         (0) root         (0)    22159 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pandas/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6521 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/perf.hpp
+-rw-rw-r--   0 root         (0) root         (0)    27044 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pinned_writer.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.348873 quasardb-3.9.9/quasardb/pybind11/
+-rw-rw-r--   0 root         (0) root         (0)     1304 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.appveyor.yml
+-rw-rw-r--   0 root         (0) root         (0)      523 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.clang-format
+-rw-rw-r--   0 root         (0) root         (0)      242 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.clang-tidy
+-rw-rw-r--   0 root         (0) root         (0)     2196 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 root         (0) root         (0)      452 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     2460 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 root         (0) root         (0)       62 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/.readthedocs.yml
+-rw-rw-r--   0 root         (0) root         (0)    10364 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1684 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      256 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     8064 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.328873 quasardb-3.9.9/quasardb/pybind11/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.352873 quasardb-3.9.9/quasardb/pybind11/include/pybind11/
+-rw-rw-r--   0 root         (0) root         (0)    21412 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 root         (0) root         (0)     6118 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 root         (0) root         (0)    95557 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 root         (0) root         (0)     7812 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 root         (0) root         (0)      120 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 root         (0) root         (0)     2037 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.352873 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 root         (0) root         (0)    27823 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 root         (0) root         (0)    40452 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 root         (0) root         (0)     3602 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 root         (0) root         (0)    16397 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 root         (0) root         (0)    16375 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 root         (0) root         (0)     1486 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-r--   0 root         (0) root         (0)    29086 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 root         (0) root         (0)     7843 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 root         (0) root         (0)     5079 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 root         (0) root         (0)     3709 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 root         (0) root         (0)     6084 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 root         (0) root         (0)    70448 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 root         (0) root         (0)     9085 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 root         (0) root         (0)     2049 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 root         (0) root         (0)   111558 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 root         (0) root         (0)    66118 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/pytypes.h
+-rw-rw-r--   0 root         (0) root         (0)    14136 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 root         (0) root         (0)    23912 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.356872 quasardb-3.9.9/quasardb/pybind11/pybind11/
+-rw-rw-r--   0 root         (0) root         (0)      217 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1158 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)      202 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/_version.py
+-rw-rw-r--   0 root         (0) root         (0)      137 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/_version.pyi
+-rw-rw-r--   0 root         (0) root         (0)      663 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/commands.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/py.typed
+-rw-rw-r--   0 root         (0) root         (0)    15110 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/setup_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)     1899 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pybind11/setup_helpers.pyi
+-rw-rw-r--   0 root         (0) root         (0)      118 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     2185 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3499 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.356872 quasardb-3.9.9/quasardb/pybind11/tools/
+-rw-rw-r--   0 root         (0) root         (0)     2295 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 root         (0) root         (0)     3105 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 root         (0) root         (0)     9977 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/FindPythonLibsNew.cmake
+-rwxrwxr-x   0 root         (0) root         (0)     1427 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/check-style.sh
+-rw-rw-r--   0 root         (0) root         (0)      952 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 root         (0) root         (0)     1121 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/libsize.py
+-rw-rw-r--   0 root         (0) root         (0)     1202 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 root         (0) root         (0)    14003 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 root         (0) root         (0)     7010 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 root         (0) root         (0)     9172 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 root         (0) root         (0)     7276 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 root         (0) root         (0)       94 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1822 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 root         (0) root         (0)      915 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 root         (0) root         (0)     2625 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/qdb_client.cpp
+-rw-rw-r--   0 root         (0) root         (0)     6483 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/query.cpp
+-rw-rw-r--   0 root         (0) root         (0)     2942 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/query.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.356872 quasardb-3.9.9/quasardb/reader/
+-rw-rw-r--   0 root         (0) root         (0)     9352 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/reader/ts_row.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6706 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/reader/ts_value.hpp
+-rw-rw-r--   0 root         (0) root         (0)      580 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/remove_cvref.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2607 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/stats.py
+-rw-rw-r--   0 root         (0) root         (0)    14771 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/table.hpp
+-rw-rw-r--   0 root         (0) root         (0)     6552 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/table_reader.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2655 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/tag.hpp
+-rw-rw-r--   0 root         (0) root         (0)    14349 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/ts_convert.hpp
+-rw-rw-r--   0 root         (0) root         (0)     4161 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/ts_iterator.hpp
+-rw-rw-r--   0 root         (0) root         (0)     3664 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/utils.hpp
+-rw-rw-r--   0 root         (0) root         (0)     2759 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/version.cpp
+-rw-rw-r--   0 root         (0) root         (0)     2106 2021-07-06 07:21:45.000000 quasardb-3.9.9/quasardb/version.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.344873 quasardb-3.9.9/quasardb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      941 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4975 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-07-06 07:27:48.000000 quasardb-3.9.9/quasardb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.328873 quasardb-3.9.9/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.360872 quasardb-3.9.9/scripts/release/
+-rw-rw-r--   0 root         (0) root         (0)     1604 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/release/set_version.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.360872 quasardb-3.9.9/scripts/teamcity/
+-rw-rw-r--   0 root         (0) root         (0)      239 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/teamcity/10.build.sh
+-rw-rw-r--   0 root         (0) root         (0)      883 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/teamcity/20.test.sh
+-rw-rw-r--   0 root         (0) root         (0)      157 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/teamcity/30.doc.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.360872 quasardb-3.9.9/scripts/test/
+-rw-rw-r--   0 root         (0) root         (0)       42 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/test/smoke-test.py
+-rwxrwxr-x   0 root         (0) root         (0)      291 2021-07-06 07:21:45.000000 quasardb-3.9.9/scripts/test/smoke-test.sh
+-rw-rw-r--   0 root         (0) root         (0)       63 2021-07-06 07:27:48.368872 quasardb-3.9.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     6124 2021-07-06 07:21:45.000000 quasardb-3.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 07:27:48.368872 quasardb-3.9.9/tests/
+-rw-rw-r--   0 root         (0) root         (0)     4271 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)      361 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_basic.py
+-rw-rw-r--   0 root         (0) root         (0)    10797 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_batch_inserter.py
+-rw-rw-r--   0 root         (0) root         (0)     7368 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_bench_pinned_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     2865 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_blob.py
+-rw-rw-r--   0 root         (0) root         (0)     1480 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_buf_size.py
+-rw-rw-r--   0 root         (0) root         (0)      406 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_cluster.py
+-rw-rw-r--   0 root         (0) root         (0)     2146 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_connection.py
+-rw-rw-r--   0 root         (0) root         (0)      231 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_error.py
+-rw-rw-r--   0 root         (0) root         (0)      319 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_examples.py
+-rw-rw-r--   0 root         (0) root         (0)     2963 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_expiry.py
+-rw-rw-r--   0 root         (0) root         (0)     3974 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_firehose.py
+-rw-rw-r--   0 root         (0) root         (0)      290 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_getTimeout.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_info.py
+-rw-rw-r--   0 root         (0) root         (0)      879 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_integer.py
+-rw-rw-r--   0 root         (0) root         (0)     2082 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_logging.py
+-rw-rw-r--   0 root         (0) root         (0)     1118 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_node.py
+-rw-rw-r--   0 root         (0) root         (0)      910 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_option_client_max_parallelism.py
+-rw-rw-r--   0 root         (0) root         (0)    10883 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_pandas.py
+-rw-rw-r--   0 root         (0) root         (0)     2752 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_pandas_benchmark.py
+-rw-rw-r--   0 root         (0) root         (0)    14326 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_pandas_pinned.py
+-rw-rw-r--   0 root         (0) root         (0)     1144 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_perf.py
+-rw-rw-r--   0 root         (0) root         (0)    26248 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_pinned_writer.py
+-rw-rw-r--   0 root         (0) root         (0)      649 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_prefix.py
+-rw-rw-r--   0 root         (0) root         (0)     9256 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_query.py
+-rw-rw-r--   0 root         (0) root         (0)     1059 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_query_find.py
+-rw-rw-r--   0 root         (0) root         (0)      485 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_setCompression.py
+-rw-rw-r--   0 root         (0) root         (0)      517 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_setMaxCardinality.py
+-rw-rw-r--   0 root         (0) root         (0)      529 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_setTimeout.py
+-rw-rw-r--   0 root         (0) root         (0)     3538 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_stats.py
+-rw-rw-r--   0 root         (0) root         (0)      649 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_suffix.py
+-rw-rw-r--   0 root         (0) root         (0)    19287 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_table.py
+-rw-rw-r--   0 root         (0) root         (0)     6954 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_table_reader.py
+-rw-rw-r--   0 root         (0) root         (0)      971 2021-07-06 07:21:45.000000 quasardb-3.9.9/tests/test_tag.py
```

### Comparing `quasardb-3.9.8/.clang-format` & `quasardb-3.9.9/.clang-format`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/.gitignore` & `quasardb-3.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/LICENSE.md` & `quasardb-3.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/PKG-INFO` & `quasardb-3.9.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: quasardb
-Version: 3.9.8
+Version: 3.9.9
 Summary: Python API for quasardb
 Home-page: https://www.quasardb.net/
 Author: quasardb SAS
 Author-email: contact@quasardb.net
 License: BSD
-Description: UNKNOWN
 Keywords: quasardb timeseries database API driver
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `quasardb-3.9.8/README.md` & `quasardb-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/docgen.py` & `quasardb-3.9.9/docgen.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/docker/Dockerfile.centos` & `quasardb-3.9.9/docker/Dockerfile.centos`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/batch_ts_insert.py` & `quasardb-3.9.9/examples/batch_ts_insert.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/cluster_sync.py` & `quasardb-3.9.9/examples/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/csv_insert.py` & `quasardb-3.9.9/examples/csv_insert.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/expiry.py` & `quasardb-3.9.9/examples/expiry.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/fake_currency_minutes.csv` & `quasardb-3.9.9/examples/fake_currency_minutes.csv`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/import_minutes.py` & `quasardb-3.9.9/examples/import_minutes.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/query_tags.py` & `quasardb-3.9.9/examples/query_tags.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/temperature.py` & `quasardb-3.9.9/examples/temperature.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/time_series.py` & `quasardb-3.9.9/examples/time_series.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/tutorial/pandas_tutorial.py` & `quasardb-3.9.9/examples/tutorial/pandas_tutorial.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/examples/tutorial/python.py` & `quasardb-3.9.9/examples/tutorial/python.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/CMakeLists.txt` & `quasardb-3.9.9/quasardb/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 project(quasardb)
 set(CMAKE_EXPORT_COMPILE_COMMANDS TRUE)
 set(CMAKE_BUILD_WITH_INSTALL_RPATH TRUE)
 
 set(PACKAGE_NAME quasardb)
 
 # step 1: discover libraries
-set(QDB_API_DIR "${CMAKE_SOURCE_DIR}/../qdb")
+if(DEFINED ENV{QDB_API_PATH})
+  message(STATUS "Getting qdb API from environment variable QDB_API_PATH: $ENV{QDB_API_PATH}")
+  set(QDB_API_DIR $ENV{QDB_API_PATH})
+else()
+  set(QDB_API_DIR "${CMAKE_SOURCE_DIR}/../qdb")
+endif()
+
 find_library(
   QDB_API_LIB
   NAMES qdb_api
   PATHS ${QDB_API_DIR}/lib
   NO_DEFAULT_PATH)
 
 if(QDB_API_LIB)
@@ -103,14 +109,15 @@
 # for Apple we need to change the id otherwise we won't be able to load the
 # extension
 if(APPLE)
   execute_process(COMMAND install_name_tool -id "@loader_path/libqdb_api.dylib"
                           ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/libqdb_api.dylib)
 endif()
 
+
 # step 3: build
 pybind11_add_module(
   quasardb
   cluster.hpp
   error.hpp
   entry.hpp
   blob.hpp
@@ -133,12 +140,21 @@
   detail/ts_column.hpp
   reader/ts_row.hpp
   reader/ts_value.hpp)
 
 target_compile_definitions(quasardb PUBLIC QDB_PY_VERSION="${QDB_PY_VERSION}")
 target_link_libraries(quasardb PUBLIC ${QDB_API_LIB})
 
+if(CMAKE_COMPILER_IS_GNUCXX)
+  target_link_options(
+    quasardb
+    PUBLIC
+    -static-libgcc
+    -static-libstdc++
+  )
+endif()
+
 if(APPLE)
   set_target_properties(quasardb PROPERTIES INSTALL_RPATH "@loader_path")
 else()
   set_target_properties(quasardb PROPERTIES INSTALL_RPATH "$ORIGIN/")
 endif()
```

### Comparing `quasardb-3.9.8/quasardb/__init__.py` & `quasardb-3.9.9/quasardb/__init__.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/batch_column.hpp` & `quasardb-3.9.9/quasardb/batch_column.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/batch_inserter.hpp` & `quasardb-3.9.9/quasardb/batch_inserter.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/blob.hpp` & `quasardb-3.9.9/quasardb/blob.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/cluster.hpp` & `quasardb-3.9.9/quasardb/cluster.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/detail/ts_column.hpp` & `quasardb-3.9.9/quasardb/detail/ts_column.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -34,27 +34,50 @@
 
 namespace qdb
 {
 
 namespace detail
 {
 
+std::string type_to_string (qdb_ts_column_type_t t) {
+  switch (t) {
+  case qdb_ts_column_double:
+    return "double";
+  case qdb_ts_column_blob:
+    return "blob";
+  case qdb_ts_column_int64:
+    return "int64";
+  case qdb_ts_column_timestamp:
+    return "timestamp";
+  case qdb_ts_column_string:
+    return "string";
+  default:
+    return "uninitialized";
+  }
+}
+
 struct column_info
 {
     column_info() = default;
 
     column_info(qdb_ts_column_type_t t, const std::string & n)
         : type{t}
         , name{n}
     {}
 
     column_info(const qdb_ts_column_info_t & ci)
         : column_info{ci.type, ci.name}
     {}
 
+    std::string repr() const
+    {
+        return "<quasardb.ColumnInfo name='" + name + "' type='" + type_to_string(type) + "'>";
+    }
+
+
     operator qdb_ts_column_info_t() const noexcept
     {
         qdb_ts_column_info_t res;
 
         // WARNING(leon): we assume that the lifetime of `this` is longer
         // than `res`, and that the string does not need to be deep-copied.
         //
@@ -130,19 +153,21 @@
 template <typename Module>
 static inline void register_ts_column(Module & m)
 {
     namespace py = pybind11;
 
     py::class_<column_info>{m, "ColumnInfo"}                        //
         .def(py::init<qdb_ts_column_type_t, const std::string &>()) //
+        .def("__repr__", &column_info::repr)
         .def_readwrite("type", &column_info::type)                  //
         .def_readwrite("name", &column_info::name);                 //
 
     py::class_<indexed_column_info>{m, "IndexedColumnInfo"}  //
         .def(py::init<qdb_ts_column_type_t, qdb_size_t &>()) //
         .def_readonly("type", &indexed_column_info::type)    //
         .def_readonly("index", &indexed_column_info::index); //
+
 }
 
 } // namespace detail
 
 } // namespace qdb
```

### Comparing `quasardb-3.9.8/quasardb/direct_blob.hpp` & `quasardb-3.9.9/quasardb/direct_blob.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/direct_handle.hpp` & `quasardb-3.9.9/quasardb/direct_handle.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/direct_integer.hpp` & `quasardb-3.9.9/quasardb/direct_integer.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/entry.hpp` & `quasardb-3.9.9/quasardb/entry.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/error.hpp` & `quasardb-3.9.9/quasardb/error.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/firehose.py` & `quasardb-3.9.9/quasardb/firehose.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/handle.hpp` & `quasardb-3.9.9/quasardb/handle.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/integer.hpp` & `quasardb-3.9.9/quasardb/integer.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/logger.cpp` & `quasardb-3.9.9/quasardb/logger.cpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/logger.hpp` & `quasardb-3.9.9/quasardb/logger.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/memcpy_wrap.cpp` & `quasardb-3.9.9/quasardb/memcpy_wrap.cpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/node.hpp` & `quasardb-3.9.9/quasardb/node.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/numpy.hpp` & `quasardb-3.9.9/quasardb/numpy.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/options.hpp` & `quasardb-3.9.9/quasardb/options.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pandas/__init__.py` & `quasardb-3.9.9/quasardb/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/perf.hpp` & `quasardb-3.9.9/quasardb/perf.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pinned_writer.hpp` & `quasardb-3.9.9/quasardb/pinned_writer.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/.appveyor.yml` & `quasardb-3.9.9/quasardb/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/.clang-format` & `quasardb-3.9.9/quasardb/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/.cmake-format.yaml` & `quasardb-3.9.9/quasardb/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/.pre-commit-config.yaml` & `quasardb-3.9.9/quasardb/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/CMakeLists.txt` & `quasardb-3.9.9/quasardb/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/LICENSE` & `quasardb-3.9.9/quasardb/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/README.rst` & `quasardb-3.9.9/quasardb/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/attr.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/buffer_info.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/cast.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/chrono.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/complex.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/class.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/common.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/descr.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/init.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/internals.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/detail/typeid.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/eigen.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/embed.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/eval.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/functional.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/iostream.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/numpy.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/operators.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/options.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/pybind11.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/pytypes.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/stl.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/include/pybind11/stl_bind.h` & `quasardb-3.9.9/quasardb/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/pybind11/__main__.py` & `quasardb-3.9.9/quasardb/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/pybind11/commands.py` & `quasardb-3.9.9/quasardb/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/pybind11/setup_helpers.py` & `quasardb-3.9.9/quasardb/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/pybind11/setup_helpers.pyi` & `quasardb-3.9.9/quasardb/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/setup.cfg` & `quasardb-3.9.9/quasardb/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/setup.py` & `quasardb-3.9.9/quasardb/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/FindCatch.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/FindEigen3.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/FindPythonLibsNew.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/check-style.sh` & `quasardb-3.9.9/quasardb/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/cmake_uninstall.cmake.in` & `quasardb-3.9.9/quasardb/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/libsize.py` & `quasardb-3.9.9/quasardb/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/make_changelog.py` & `quasardb-3.9.9/quasardb/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/pybind11Common.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/pybind11Config.cmake.in` & `quasardb-3.9.9/quasardb/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/pybind11NewTools.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/pybind11Tools.cmake` & `quasardb-3.9.9/quasardb/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/setup_global.py.in` & `quasardb-3.9.9/quasardb/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/pybind11/tools/setup_main.py.in` & `quasardb-3.9.9/quasardb/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/qdb_client.cpp` & `quasardb-3.9.9/quasardb/qdb_client.cpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/query.cpp` & `quasardb-3.9.9/quasardb/query.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,18 @@
             auto value                      = coerce_point(r->rows[i][j], parse_blobs[j]);
 
             row[column_name] = value;
         }
 
         ret.push_back(row);
     }
+    
+
+    // all values are copied, it's ok to release
+    qdb_release(*h, r);
 
     return ret;
 }
 
 /**
  * Useful for pre-allocating entire numpy arrays: probe the data type for the first
  * non-null column.
```

### Comparing `quasardb-3.9.8/quasardb/query.hpp` & `quasardb-3.9.9/quasardb/query.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/reader/ts_row.hpp` & `quasardb-3.9.9/quasardb/reader/ts_row.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/reader/ts_value.hpp` & `quasardb-3.9.9/quasardb/reader/ts_value.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/remove_cvref.hpp` & `quasardb-3.9.9/quasardb/remove_cvref.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/table.hpp` & `quasardb-3.9.9/quasardb/table.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/table_reader.hpp` & `quasardb-3.9.9/quasardb/table_reader.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/tag.hpp` & `quasardb-3.9.9/quasardb/tag.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/ts_convert.hpp` & `quasardb-3.9.9/quasardb/ts_convert.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/ts_iterator.hpp` & `quasardb-3.9.9/quasardb/ts_iterator.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/utils.hpp` & `quasardb-3.9.9/quasardb/utils.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/version.cpp` & `quasardb-3.9.9/quasardb/version.cpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb/version.hpp` & `quasardb-3.9.9/quasardb/version.hpp`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/quasardb.egg-info/PKG-INFO` & `quasardb-3.9.9/quasardb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: quasardb
-Version: 3.9.8
+Version: 3.9.9
 Summary: Python API for quasardb
 Home-page: https://www.quasardb.net/
 Author: quasardb SAS
 Author-email: contact@quasardb.net
 License: BSD
-Description: UNKNOWN
 Keywords: quasardb timeseries database API driver
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `quasardb-3.9.8/quasardb.egg-info/SOURCES.txt` & `quasardb-3.9.9/quasardb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,17 @@
 quasardb/pybind11/tools/pybind11Tools.cmake
 quasardb/pybind11/tools/pyproject.toml
 quasardb/pybind11/tools/setup_global.py.in
 quasardb/pybind11/tools/setup_main.py.in
 quasardb/reader/ts_row.hpp
 quasardb/reader/ts_value.hpp
 scripts/release/set_version.sh
+scripts/teamcity/10.build.sh
+scripts/teamcity/20.test.sh
+scripts/teamcity/30.doc.sh
 scripts/test/smoke-test.py
 scripts/test/smoke-test.sh
 tests/conftest.py
 tests/test_basic.py
 tests/test_batch_inserter.py
 tests/test_bench_pinned_writer.py
 tests/test_blob.py
```

### Comparing `quasardb-3.9.8/scripts/release/set_version.sh` & `quasardb-3.9.9/scripts/release/set_version.sh`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/setup.py` & `quasardb-3.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools.command.build_ext import build_ext
 
 from setuptools import setup, Extension
 from setuptools.command.bdist_egg import bdist_egg as old_bdist_egg  # pylint: disable=C0412
 from pkg_resources import get_build_platform
 from wheel.bdist_wheel import bdist_wheel as old_bdist_wheel
 
-qdb_version = "3.9.8"
+qdb_version = "3.9.9"
 
 # package_modules are our 'extra' files. Our cmake configuration copies our QDB_API_LIB
 # into our source directory, and by adding this to `package_modules` we tell setuptools to
 # package this.
 package_modules = glob.glob(os.path.join('quasardb', 'lib*'))
 package_name = 'quasardb'
 
@@ -155,15 +155,15 @@
           "xmlrunner >= 1.7.7",
           "future >= 0.17.1",
           "numpy >= 1.16.1",
           "pytest == 5.3.1",
           "pytest-runner == 5.2",
           "pytest-benchmark == 3.2.2",
           "pytz >= 2018.9",
-          "pandas"],
+          "pandas >= 1.0.0, < 1.3.0"],
       install_requires=[
           "xmlrunner >= 1.7.7",
           "future >= 0.17.1",
           "numpy >= 1.16.1"],
       packages=[package_name],
       package_data={package_name: package_modules},
       ext_modules=[CMakeExtension('quasardb', 'quasardb/')],
```

### Comparing `quasardb-3.9.8/tests/conftest.py` & `quasardb-3.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_batch_inserter.py` & `quasardb-3.9.9/tests/test_batch_inserter.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_bench_pinned_writer.py` & `quasardb-3.9.9/tests/test_bench_pinned_writer.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_blob.py` & `quasardb-3.9.9/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_buf_size.py` & `quasardb-3.9.9/tests/test_buf_size.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_connection.py` & `quasardb-3.9.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_expiry.py` & `quasardb-3.9.9/tests/test_expiry.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_firehose.py` & `quasardb-3.9.9/tests/test_firehose.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_info.py` & `quasardb-3.9.9/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_integer.py` & `quasardb-3.9.9/tests/test_integer.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_logging.py` & `quasardb-3.9.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_node.py` & `quasardb-3.9.9/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_option_client_max_parallelism.py` & `quasardb-3.9.9/tests/test_option_client_max_parallelism.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_pandas.py` & `quasardb-3.9.9/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_pandas_benchmark.py` & `quasardb-3.9.9/tests/test_pandas_benchmark.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_pandas_pinned.py` & `quasardb-3.9.9/tests/test_pandas_pinned.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_perf.py` & `quasardb-3.9.9/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_pinned_writer.py` & `quasardb-3.9.9/tests/test_pinned_writer.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_prefix.py` & `quasardb-3.9.9/tests/test_prefix.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_query.py` & `quasardb-3.9.9/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_query_find.py` & `quasardb-3.9.9/tests/test_query_find.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_setMaxCardinality.py` & `quasardb-3.9.9/tests/test_setMaxCardinality.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_setTimeout.py` & `quasardb-3.9.9/tests/test_setTimeout.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_suffix.py` & `quasardb-3.9.9/tests/test_suffix.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_table.py` & `quasardb-3.9.9/tests/test_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,33 @@
 
 def _check_ts_results(results, generated, count):
     assert len(results) == 2
 
     np.testing.assert_array_equal(results[0][:count], generated[0][:count])
     np.testing.assert_array_equal(results[1][:count], generated[1][:count])
 
+def test_column_info_repr(column_name):
+    double = quasardb.ColumnInfo(quasardb.ColumnType.Double, column_name)
+    blob = quasardb.ColumnInfo(quasardb.ColumnType.Blob, column_name)
+    int64 = quasardb.ColumnInfo(quasardb.ColumnType.Int64, column_name)
+    timestamp = quasardb.ColumnInfo(quasardb.ColumnType.Timestamp, column_name)
+    string = quasardb.ColumnInfo(quasardb.ColumnType.String, column_name)
+
+    assert column_name in str(double)
+    assert column_name in str(blob)
+    assert column_name in str(int64)
+    assert column_name in str(timestamp)
+    assert column_name in str(string)
+
+    assert 'double'    in str(double)
+    assert 'blob'      in str(blob)
+    assert 'int64'     in str(int64)
+    assert 'timestamp' in str(timestamp)
+    assert 'string'    in str(string)
+
 
 def test_list_columns_throws_when_timeseries_does_not_exist(
         qdbd_connection, entry_name):
     table = qdbd_connection.table(entry_name)
     with pytest.raises(quasardb.Error):
         table.list_columns()
```

### Comparing `quasardb-3.9.8/tests/test_table_reader.py` & `quasardb-3.9.9/tests/test_table_reader.py`

 * *Files identical despite different names*

### Comparing `quasardb-3.9.8/tests/test_tag.py` & `quasardb-3.9.9/tests/test_tag.py`

 * *Files identical despite different names*


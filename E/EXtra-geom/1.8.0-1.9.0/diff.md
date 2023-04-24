# Comparing `tmp/EXtra-geom-1.8.0.tar.gz` & `tmp/EXtra-geom-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EXtra-geom-1.8.0.tar", last modified: Tue Oct 18 11:53:18 2022, max compression
+gzip compressed data, was "EXtra-geom-1.9.0.tar", last modified: Fri Oct 28 10:38:55 2022, max compression
```

## Comparing `EXtra-geom-1.8.0.tar` & `EXtra-geom-1.9.0.tar`

### file list

```diff
@@ -1,82 +1,37 @@
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.702456 EXtra-geom-1.8.0/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       23 2019-11-14 13:16:04.000000 EXtra-geom-1.8.0/.coveragerc
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.623455 EXtra-geom-1.8.0/.github/
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.623455 EXtra-geom-1.8.0/.github/dependabot/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      297 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/.github/dependabot/constraints.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      125 2020-12-02 10:56:21.000000 EXtra-geom-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.623455 EXtra-geom-1.8.0/.github/workflows/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1078 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/.github/workflows/tests.yml
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      162 2020-03-24 10:23:54.000000 EXtra-geom-1.8.0/.gitignore
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2019-11-14 13:16:04.000000 EXtra-geom-1.8.0/Dockerfile
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.624456 EXtra-geom-1.8.0/EXtra_geom.egg-info/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2057 2022-10-18 11:53:18.000000 EXtra-geom-1.8.0/EXtra_geom.egg-info/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1778 2022-10-18 11:53:18.000000 EXtra-geom-1.8.0/EXtra_geom.egg-info/SOURCES.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2022-10-18 11:53:18.000000 EXtra-geom-1.8.0/EXtra_geom.egg-info/dependency_links.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      233 2022-10-18 11:53:18.000000 EXtra-geom-1.8.0/EXtra_geom.egg-info/requires.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       11 2022-10-18 11:53:18.000000 EXtra-geom-1.8.0/EXtra_geom.egg-info/top_level.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2019-11-14 13:16:05.000000 EXtra-geom-1.8.0/LICENSE
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       73 2019-11-14 13:16:04.000000 EXtra-geom-1.8.0/MANIFEST.in
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      666 2019-12-16 13:40:28.000000 EXtra-geom-1.8.0/Makefile
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2057 2022-10-18 11:53:18.702456 EXtra-geom-1.8.0/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1128 2021-09-22 08:21:30.000000 EXtra-geom-1.8.0/README.md
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       13 2019-11-14 13:16:04.000000 EXtra-geom-1.8.0/codecov.yml
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.687456 EXtra-geom-1.8.0/docs/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7740 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/Makefile
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.694456 EXtra-geom-1.8.0/docs/_static/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/_static/.keep
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    21142 2020-11-20 16:57:27.000000 EXtra-geom-1.8.0/docs/_static/agipd_500k2g_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57574 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/_static/agipd_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   108114 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/_static/agipd_layout.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46830 2022-08-11 13:53:29.000000 EXtra-geom-1.8.0/docs/_static/dssc_hexes.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    30875 2022-08-11 13:53:29.000000 EXtra-geom-1.8.0/docs/_static/dssc_hexes.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46070 2019-12-16 13:40:28.000000 EXtra-geom-1.8.0/docs/_static/dssc_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    75907 2019-12-16 13:40:28.000000 EXtra-geom-1.8.0/docs/_static/dssc_layout.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    54105 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/_static/lpd_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    82299 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/_static/lpd_layout.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    98764 2021-04-12 11:40:26.000000 EXtra-geom-1.8.0/docs/agipd_geometry.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)  2536104 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/docs/apply_geometry.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   112386 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/docs/azimuthal-int-diagram.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6125 2022-10-18 11:51:21.000000 EXtra-geom-1.8.0/docs/changelog.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     9810 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/docs/conf.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    98510 2020-12-02 11:01:51.000000 EXtra-geom-1.8.0/docs/convert_coords.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    63752 2019-12-16 13:40:28.000000 EXtra-geom-1.8.0/docs/dssc_geo_june19.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   162523 2022-08-11 13:53:29.000000 EXtra-geom-1.8.0/docs/dssc_geometry.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   177932 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/docs/epix_geometry.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1465 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/docs/faq.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   116553 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/docs/generic_geometry.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8259 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/docs/geometry.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1443 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/docs/index.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    91555 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/docs/jungfrau_geometry.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    95847 2021-04-12 11:40:40.000000 EXtra-geom-1.8.0/docs/lpd_geometry.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   425808 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/lpd_mar_18.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   387944 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/lpd_mar_18_axesfixed.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7291 2019-11-14 13:17:29.000000 EXtra-geom-1.8.0/docs/make.bat
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   131048 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/docs/masks.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      547 2019-12-16 13:40:28.000000 EXtra-geom-1.8.0/docs/performance.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   284832 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/docs/pyfai.ipynb
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.697456 EXtra-geom-1.8.0/extra_geom/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2216 2022-10-18 11:52:48.000000 EXtra-geom-1.8.0/extra_geom/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    42268 2022-03-22 13:08:27.000000 EXtra-geom-1.8.0/extra_geom/base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7091 2022-08-11 13:53:29.000000 EXtra-geom-1.8.0/extra_geom/crystfel_fmt.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    87506 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/extra_geom/detectors.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8696 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/extra_geom/lpd_old.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1095 2022-03-02 10:26:33.000000 EXtra-geom-1.8.0/extra_geom/pyfai.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9291 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/extra_geom/snapped.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-18 11:53:18.702456 EXtra-geom-1.8.0/extra_geom/tests/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-12-02 11:01:51.000000 EXtra-geom-1.8.0/extra_geom/tests/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    63752 2020-12-02 11:01:51.000000 EXtra-geom-1.8.0/extra_geom/tests/dssc_geo_june19.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   425808 2020-12-02 11:01:51.000000 EXtra-geom-1.8.0/extra_geom/tests/lpd_mar_18.h5
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6715 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/extra_geom/tests/test_agipd500k2g_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8798 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/extra_geom/tests/test_agipd_geometry.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3881 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/extra_geom/tests/test_dssc_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6628 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/extra_geom/tests/test_epix_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2930 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/extra_geom/tests/test_generic_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1171 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/extra_geom/tests/test_geometry_old.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2671 2022-10-18 10:51:35.000000 EXtra-geom-1.8.0/extra_geom/tests/test_jungfrau_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    12460 2022-03-02 13:10:50.000000 EXtra-geom-1.8.0/extra_geom/tests/test_lpd_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2321 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/extra_geom/tests/test_pnccd_geometry.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      568 2021-07-15 14:56:21.000000 EXtra-geom-1.8.0/extra_geom/tests/utils.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       54 2020-12-02 11:01:51.000000 EXtra-geom-1.8.0/pytest.ini
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       82 2019-11-14 13:16:04.000000 EXtra-geom-1.8.0/readthedocs.yml
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       38 2022-10-18 11:53:18.702456 EXtra-geom-1.8.0/setup.cfg
--rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)     2467 2022-10-18 10:51:31.000000 EXtra-geom-1.8.0/setup.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-28 10:38:55.417019 EXtra-geom-1.9.0/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       23 2019-11-14 13:16:04.000000 EXtra-geom-1.9.0/.coveragerc
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-28 10:38:55.409018 EXtra-geom-1.9.0/EXtra_geom.egg-info/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2077 2022-10-28 10:38:55.000000 EXtra-geom-1.9.0/EXtra_geom.egg-info/PKG-INFO
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      874 2022-10-28 10:38:55.000000 EXtra-geom-1.9.0/EXtra_geom.egg-info/SOURCES.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        1 2022-10-28 10:38:55.000000 EXtra-geom-1.9.0/EXtra_geom.egg-info/dependency_links.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      249 2022-10-28 10:38:55.000000 EXtra-geom-1.9.0/EXtra_geom.egg-info/requires.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       11 2022-10-28 10:38:55.000000 EXtra-geom-1.9.0/EXtra_geom.egg-info/top_level.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2019-11-14 13:16:05.000000 EXtra-geom-1.9.0/LICENSE
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       73 2019-11-14 13:16:04.000000 EXtra-geom-1.9.0/MANIFEST.in
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2077 2022-10-28 10:38:55.417019 EXtra-geom-1.9.0/PKG-INFO
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1128 2021-09-22 08:21:30.000000 EXtra-geom-1.9.0/README.md
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-28 10:38:55.411018 EXtra-geom-1.9.0/extra_geom/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2240 2022-10-28 10:37:55.000000 EXtra-geom-1.9.0/extra_geom/__init__.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    42268 2022-03-22 13:08:27.000000 EXtra-geom-1.9.0/extra_geom/base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7091 2022-08-11 13:53:29.000000 EXtra-geom-1.9.0/extra_geom/crystfel_fmt.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    91179 2022-10-28 10:30:25.000000 EXtra-geom-1.9.0/extra_geom/detectors.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8696 2021-07-15 14:56:21.000000 EXtra-geom-1.9.0/extra_geom/lpd_old.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1095 2022-03-02 10:26:33.000000 EXtra-geom-1.9.0/extra_geom/pyfai.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9291 2022-10-18 10:51:35.000000 EXtra-geom-1.9.0/extra_geom/snapped.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-10-28 10:38:55.417019 EXtra-geom-1.9.0/extra_geom/tests/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-12-02 11:01:51.000000 EXtra-geom-1.9.0/extra_geom/tests/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    63752 2020-12-02 11:01:51.000000 EXtra-geom-1.9.0/extra_geom/tests/dssc_geo_june19.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)   425808 2020-12-02 11:01:51.000000 EXtra-geom-1.9.0/extra_geom/tests/lpd_mar_18.h5
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6715 2022-03-02 13:10:50.000000 EXtra-geom-1.9.0/extra_geom/tests/test_agipd500k2g_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8798 2022-03-02 13:10:50.000000 EXtra-geom-1.9.0/extra_geom/tests/test_agipd_geometry.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4522 2022-10-28 10:30:25.000000 EXtra-geom-1.9.0/extra_geom/tests/test_dssc_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6628 2022-03-02 13:10:50.000000 EXtra-geom-1.9.0/extra_geom/tests/test_epix_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2930 2021-07-15 14:56:21.000000 EXtra-geom-1.9.0/extra_geom/tests/test_generic_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1171 2021-07-15 14:56:21.000000 EXtra-geom-1.9.0/extra_geom/tests/test_geometry_old.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2671 2022-10-18 10:51:35.000000 EXtra-geom-1.9.0/extra_geom/tests/test_jungfrau_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    12460 2022-03-02 13:10:50.000000 EXtra-geom-1.9.0/extra_geom/tests/test_lpd_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2321 2021-07-15 14:56:21.000000 EXtra-geom-1.9.0/extra_geom/tests/test_pnccd_geometry.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      568 2021-07-15 14:56:21.000000 EXtra-geom-1.9.0/extra_geom/tests/utils.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       54 2020-12-02 11:01:51.000000 EXtra-geom-1.9.0/pytest.ini
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       38 2022-10-28 10:38:55.417019 EXtra-geom-1.9.0/setup.cfg
+-rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)     2500 2022-10-28 10:30:25.000000 EXtra-geom-1.9.0/setup.py
```

### Comparing `EXtra-geom-1.8.0/EXtra_geom.egg-info/PKG-INFO` & `EXtra-geom-1.9.0/EXtra_geom.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: EXtra-geom
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tools to work with EuXFEL detector geometry and assemble detector images
 Home-page: https://github.com/European-XFEL/EXtra-geom
 Author: European XFEL GmbH
 Author-email: da-support@xfel.eu
 Maintainer: Thomas Michelat
 License: BSD-3-Clause
 Project-URL: Documentation, https://extra-geom.readthedocs.io/en/latest/
 Project-URL: Changelog, https://extra-geom.readthedocs.io/en/latest/changelog.html
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
@@ -55,7 +56,9 @@
 -----
 
 Tests can be run as follows:
 
     python3 -m pytest -v --pyargs extra_geom
 
 In the source directory, you can also omit `--pyargs extra_geom`.
+
+
```

### Comparing `EXtra-geom-1.8.0/LICENSE` & `EXtra-geom-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/PKG-INFO` & `EXtra-geom-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: EXtra-geom
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tools to work with EuXFEL detector geometry and assemble detector images
 Home-page: https://github.com/European-XFEL/EXtra-geom
 Author: European XFEL GmbH
 Author-email: da-support@xfel.eu
 Maintainer: Thomas Michelat
 License: BSD-3-Clause
 Project-URL: Documentation, https://extra-geom.readthedocs.io/en/latest/
 Project-URL: Changelog, https://extra-geom.readthedocs.io/en/latest/changelog.html
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
@@ -55,7 +56,9 @@
 -----
 
 Tests can be run as follows:
 
     python3 -m pytest -v --pyargs extra_geom
 
 In the source directory, you can also omit `--pyargs extra_geom`.
+
+
```

### Comparing `EXtra-geom-1.8.0/README.md` & `EXtra-geom-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/docs/dssc_geo_june19.h5` & `EXtra-geom-1.9.0/extra_geom/tests/dssc_geo_june19.h5`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/docs/lpd_mar_18.h5` & `EXtra-geom-1.9.0/extra_geom/tests/lpd_mar_18.h5`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/__init__.py` & `EXtra-geom-1.9.0/extra_geom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 You should have received a copy of the 3-Clause BSD License along with this
 program. If not, see <https://opensource.org/licenses/BSD-3-Clause>
 """
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
-from .detectors import (AGIPD_1MGeometry, AGIPD_500K2GGeometry, DSSC_1MGeometry, Epix10KGeometry, Epix100Geometry,
-                        GenericGeometry, JUNGFRAUGeometry, LPD_1MGeometry, PNCCDGeometry, agipd_asic_seams)
+from .detectors import (AGIPD_1MGeometry, AGIPD_500K2GGeometry, DSSC_1MGeometry,
+                        Epix10KGeometry, Epix100Geometry, GenericGeometry, JUNGFRAUGeometry, LPD_1MGeometry,
+                        PNCCDGeometry, agipd_asic_seams)
 
 __all__ = [
     'AGIPD_1MGeometry',
     'AGIPD_500K2GGeometry',
     'agipd_asic_seams',
     'GenericGeometry',
     'DSSC_1MGeometry',
```

### Comparing `EXtra-geom-1.8.0/extra_geom/base.py` & `EXtra-geom-1.9.0/extra_geom/base.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/crystfel_fmt.py` & `EXtra-geom-1.9.0/extra_geom/crystfel_fmt.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/detectors.py` & `EXtra-geom-1.9.0/extra_geom/detectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,14 +1045,16 @@
     # The unit is the width of a pixel, 236 μm.
     # The 4/3 extends the hexagons into the next row to correctly tessellate.
     _pixel_corners = np.stack([
         (np.array([0, 0.25, 0.75, 1, 0.75, 0.25]) * 4 / 3),
         [0.5, 1, 1, 0.5, 0, 0]
     ])
 
+    _cartesian_geom_cached = None
+
     @classmethod
     def from_quad_positions(cls, quad_pos, *, unit=1e-3, asic_gap=None,
                             panel_gap=None):
         """Generate a DSSC-1M geometry from quadrant positions.
 
         This produces an idealised geometry, assuming all modules are perfectly
         flat, aligned and equally spaced within their quadrant.
@@ -1364,14 +1366,45 @@
 
     @staticmethod
     def split_tiles(module_data):
         # Split into 2 tiles along the fast-scan axis
         # This simple slicing is faster than np.split().
         return [module_data[..., :256], module_data[..., 256:]]
 
+    @property
+    def _cartesian_geom(self):
+        if self._cartesian_geom_cached is None:
+            conversion_const = 2 ** 0.5 / 3 ** 0.25
+            new_modules = []
+            for module in self.modules:
+                new_modules.append([
+                    GeometryFragment(
+                        corner_pos=tile.corner_pos,
+                        ss_vec=tile.ss_vec / conversion_const,
+                        fs_vec=tile.fs_vec * conversion_const,
+                        ss_pixels=DSSC_1MGeometryCartesian.frag_ss_pixels,
+                        fs_pixels=DSSC_1MGeometryCartesian.frag_fs_pixels,
+                    ) for tile in module
+                ])
+            self._cartesian_geom_cached = DSSC_1MGeometryCartesian(new_modules)
+
+        return self._cartesian_geom_cached
+
+    def position_modules_cartesian(self, data, out=None, threadpool=None):
+        """Assemble DSSC data on a square pixel grid
+
+        This converts the data from DSSC's hexagonal pixels to a similar number
+        of pixels on a square grid, and displays the image.
+        The arguments are the same as for :meth:`position_modules`.
+        """
+        cart_data = self._cartesian_geom.transform_data(data)
+        return self._cartesian_geom.position_modules(
+            cart_data, out=out, threadpool=threadpool
+        )
+
     def plot_data(self,
                   data, *,
                   axis_units='px',
                   frontview=True,
                   ax=None,
                   figsize=None,
                   colorbar=False,
@@ -1478,14 +1511,24 @@
             ax.invert_xaxis()
 
         # Draw a cross at the centre
         ax.hlines(0, -cross_size, +cross_size, colors='w', linewidths=1)
         ax.vlines(0, -cross_size, +cross_size, colors='w', linewidths=1)
         return ax
 
+    def plot_data_cartesian(self, data, **kwargs):
+        """Plot the given data converted to square pixels
+
+        This converts the data from DSSC's hexagonal pixels to a similar number
+        of pixels on a square grid, and displays the image.
+        It accepts all the same keyword arguments as :meth:`plot_data`.
+        """
+        cart_data = self._cartesian_geom.transform_data(data)
+        return self._cartesian_geom.plot_data(cart_data, **kwargs)
+
     @classmethod
     def _tile_slice(cls, tileno):
         tile_offset = tileno * cls.frag_fs_pixels
         fs_slice = slice(tile_offset, tile_offset + cls.frag_fs_pixels)
         ss_slice = slice(0, cls.frag_ss_pixels)  # Every tile covers the full pixel range
         return ss_slice, fs_slice
 
@@ -1520,14 +1563,65 @@
         if centre:
             # Vertical (slow scan) centre is 2/3 of the way to the start of the
             # next row of hexagons, because the tessellating pixels extend
             # beyond the start of the next row.
             ss_coords += 2/3
             fs_coords += 0.5
 
+class DSSC_1MGeometryCartesian(DetectorGeometryBase):
+    """Detector layout for DSSC-1M, for square-pixel support
+
+    The coordinates used in this class are 3D (x, y, z), and represent metres.
+
+    You won't normally use this class directly: use the
+    position_modules_cartesian or plot_data_cartesian methods on the main
+    DSSC_1MGeometry class instead.
+    """
+    detector_type_name = 'DSSC-1M'
+    pixel_size = 236e-6 * (3 ** 0.25) / (2 ** 0.5)  # ~220 um
+    frag_ss_pixels = 119
+    frag_fs_pixels = 275
+    n_quads = 4
+    n_modules = 16
+    n_tiles_per_module = 2
+    expected_data_shape = (16, 119, 550)
+
+    @staticmethod
+    def split_tiles(module_data):
+        return [module_data[..., :275], module_data[..., 275:]]
+
+    @classmethod
+    def _tile_slice(cls, tileno):
+        tile_offset = tileno * cls.frag_fs_pixels
+        fs_slice = slice(tile_offset, tile_offset + cls.frag_fs_pixels)
+        ss_slice = slice(0, cls.frag_ss_pixels)  # Every tile covers the full pixel range
+        return ss_slice, fs_slice
+
+    @classmethod
+    def _module_coords_to_tile(cls, slow_scan, fast_scan):
+        tileno, tile_fs = np.divmod(fast_scan, cls.frag_fs_pixels)
+        return tileno.astype(np.int16), slow_scan, tile_fs
+
+    @staticmethod
+    def transform_data(data):
+        """Convert data taken by DSSC onto a cartesian grid
+
+        This requires the separate condat_gridconv package.
+        """
+        from condat_gridconv import hex2cart
+
+        assert data.shape[-2:] == (128, 512)
+        modules = data.reshape(-1, 128, 512)
+        cart_modules = []
+        for module in modules:
+            cart_modules.append(np.concatenate([
+                hex2cart(tile) for tile in DSSC_1MGeometry.split_tiles(module)
+            ], axis=-1))
+        return np.stack(cart_modules).reshape(data.shape[:-2] + (119, 550))
+
 
 class DSSC_Geometry(DSSC_1MGeometry):
     """DEPRECATED: Use DSSC_1MGeometry instead"""
     def __init__(self, modules, filename='No file', metadata=None):
         super().__init__(modules, filename, metadata)
         warnings.warn(
             "DSSC_Geometry has been renamed to DSSC_1MGeometry.", stacklevel=2
```

### Comparing `EXtra-geom-1.8.0/extra_geom/lpd_old.py` & `EXtra-geom-1.9.0/extra_geom/lpd_old.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/pyfai.py` & `EXtra-geom-1.9.0/extra_geom/pyfai.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/snapped.py` & `EXtra-geom-1.9.0/extra_geom/snapped.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_agipd500k2g_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_agipd500k2g_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_agipd_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_agipd_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_dssc_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_dssc_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,27 +38,49 @@
     # Smoketest
     ax = geom.plot_data_hexes(np.zeros((16, 128, 512)), colorbar=True)
     assert isinstance(ax, Axes)
 
     ax = geom.plot_data_hexes(np.zeros((128, 512)), module=4, colorbar=True)
     assert isinstance(ax, Axes)
 
+def test_plot_data_cartesian():
+    geom = DSSC_1MGeometry.from_h5_file_and_quad_positions(
+        sample_xfel_geom, QUAD_POS
+    )
+    # Smoketest
+    ax = geom.plot_data_cartesian(np.zeros((16, 128, 512)), colorbar=True)
+    assert isinstance(ax, Axes)
+
 
 def test_snap_assemble_data():
     geom = DSSC_1MGeometry.from_h5_file_and_quad_positions(
         sample_xfel_geom, QUAD_POS
     )
 
     stacked_data = np.zeros((16, 128, 512))
     img, centre = geom.position_modules_fast(stacked_data)
     assert img.shape == (1281, 1099)
     assert tuple(centre) == (656, 552)
     assert np.isnan(img[0, 0])
     assert img[50, 50] == 0
 
+
+def test_assemble_data_cartesian():
+    geom = DSSC_1MGeometry.from_h5_file_and_quad_positions(
+        sample_xfel_geom, QUAD_POS
+    )
+
+    stacked_data = np.zeros((16, 128, 512))
+    img, centre = geom.position_modules_cartesian(stacked_data)
+    assert img.shape == (1192, 1180)
+    assert tuple(centre) == (610, 593)
+    assert np.isnan(img[0, 0])
+    assert img[50, 50] == 0
+
+
 def test_to_distortion_array():
     geom = DSSC_1MGeometry.from_h5_file_and_quad_positions(
         sample_xfel_geom, QUAD_POS
     )
     # Smoketest
     distortion = geom.to_distortion_array()
     assert isinstance(distortion, np.ndarray)
```

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_epix_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_epix_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_generic_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_generic_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_geometry_old.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_geometry_old.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_jungfrau_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_jungfrau_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_lpd_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_lpd_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/test_pnccd_geometry.py` & `EXtra-geom-1.9.0/extra_geom/tests/test_pnccd_geometry.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/extra_geom/tests/utils.py` & `EXtra-geom-1.9.0/extra_geom/tests/utils.py`

 * *Files identical despite different names*

### Comparing `EXtra-geom-1.8.0/setup.py` & `EXtra-geom-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,15 @@
               'pytest-cov',
               'coverage',
               'nbval',
               'testpath',
               'xarray',
               'EXtra-data',
               'pyFAI',
+              'condat_gridconv',
           ]
       },
       python_requires='>=3.6',
       classifiers=[
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
```


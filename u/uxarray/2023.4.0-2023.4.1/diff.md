# Comparing `tmp/uxarray-2023.4.0.tar.gz` & `tmp/uxarray-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxarray-2023.4.0.tar", last modified: Tue Apr 11 21:51:59 2023, max compression
+gzip compressed data, was "uxarray-2023.4.1.tar", last modified: Mon Apr 24 21:49:06 2023, max compression
```

## Comparing `uxarray-2023.4.0.tar` & `uxarray-2023.4.1.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.996580 uxarray-2023.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.996580 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/upstream-dev-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 21:51:48.000000 uxarray-2023.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 21:51:48.000000 uxarray-2023.4.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-11 21:51:48.000000 uxarray-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-11 21:51:59.036582 uxarray-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-11 21:51:48.000000 uxarray-2023.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-11 21:51:48.000000 uxarray-2023.4.0/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/science.svg
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/tips.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/DOE_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/EarthCube_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/NSF_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/PANGEO_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/uxarray_temp_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/thumbnails/default.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/000-template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    65555 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/001-read-grid-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/002-access-grid-info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/gallery.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/user_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/user_api/uxarray_api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 21:51:48.000000 uxarray-2023.4.0/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:51:48.000000 uxarray-2023.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:51:59.036582 uxarray-2023.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 21:51:48.000000 uxarray-2023.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/exodus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/exodus/mixed/
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/exodus/mixed/mixed.exo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/exodus/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/exodus/outCSne8/outCSne8.g
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/mpas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/mpas/QU/
--rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/scrip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/scrip/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/scrip/outCSne8/outCSne8.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/shp/
--rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/shp/grid_fire.shp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/ugrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.024581 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.028581 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/
--rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/grid.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v1.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v2.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v3.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.028581 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/
--rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30.ug
--rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
--rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.032581 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/
--rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
--rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.032581 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
--rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_ugrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/uxarray/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_ugrid.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/get_quadratureDG.py
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/upstream-dev-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-24 21:48:56.000000 uxarray-2023.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 21:48:56.000000 uxarray-2023.4.1/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-24 21:48:56.000000 uxarray-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-24 21:49:06.904318 uxarray-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-24 21:48:56.000000 uxarray-2023.4.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-24 21:48:56.000000 uxarray-2023.4.1/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/science.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/tips.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/DOE_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/EarthCube_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/NSF_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/PANGEO_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/uxarray_temp_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/thumbnails/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/000-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    65555 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/001-read-grid-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/002-access-grid-info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/003-area-calc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/gallery.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/user_api/uxarray_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 21:48:56.000000 uxarray-2023.4.1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 21:48:56.000000 uxarray-2023.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:49:06.904318 uxarray-2023.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-24 21:48:56.000000 uxarray-2023.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/exodus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/exodus/mixed/
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/exodus/mixed/mixed.exo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/outCSne8.g
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/mpas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/mpas/QU/
+-rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/scrip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/outCSne8.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/shp/
+-rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/shp/grid_fire.shp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/test/meshfiles/ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.896318 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.900318 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/grid.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v3.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.900318 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/
+-rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30.ug
+-rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/
+-rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
+-rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
+-rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/uxarray/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/get_quadratureDG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21464 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/top_level.txt
```

### Comparing `uxarray-2023.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `uxarray-2023.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `uxarray-2023.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/.github/workflows/ci.yml` & `uxarray-2023.4.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,14 @@
           python -m pytest test
 
       - name: Run Coverage Tests
         run: |
           python -m pytest test -v --cov=./uxarray --cov-report=xml
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `uxarray-2023.4.0/.github/workflows/pypi.yaml` & `uxarray-2023.4.1/.github/workflows/pypi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   test-build:
     if: github.repository == 'UXARRAY/uxarray'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
@@ -28,15 +28,15 @@
   publish:
     needs: test-build
     if: startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v4.6.0
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm wheel twine check-manifest
       - name: Build tarball and wheels
```

### Comparing `uxarray-2023.4.0/.github/workflows/upstream-dev-ci.yml` & `uxarray-2023.4.1/.github/workflows/upstream-dev-ci.yml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/.gitignore` & `uxarray-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/.pre-commit-config.yaml` & `uxarray-2023.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/LICENSE` & `uxarray-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/PKG-INFO` & `uxarray-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
```

### Comparing `uxarray-2023.4.0/README.md` & `uxarray-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/Makefile` & `uxarray-2023.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/icons/code.svg` & `uxarray-2023.4.1/docs/_static/images/icons/code.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/icons/tips.svg` & `uxarray-2023.4.1/docs/_static/images/icons/tips.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/logos/DOE_vertical.png` & `uxarray-2023.4.1/docs/_static/images/logos/DOE_vertical.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/logos/EarthCube_logo.png` & `uxarray-2023.4.1/docs/_static/images/logos/EarthCube_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/logos/NSF_logo.png` & `uxarray-2023.4.1/docs/_static/images/logos/NSF_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/logos/PANGEO_logo.png` & `uxarray-2023.4.1/docs/_static/images/logos/PANGEO_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/logos/uxarray_temp_logo.png` & `uxarray-2023.4.1/docs/_static/images/logos/uxarray_temp_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/images/nsf.png` & `uxarray-2023.4.1/docs/_static/images/nsf.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/_static/thumbnails/default.svg` & `uxarray-2023.4.1/docs/_static/thumbnails/default.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/conf.py` & `uxarray-2023.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/contributing.rst` & `uxarray-2023.4.1/docs/contributing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 
 .. caution::
     Please also ensure that you are changing the `UXarray draft API
     <https://github.com/UXARRAY/uxarray/blob/main/docs/user_api/uxarray_api.md>`_
     accordingly if you are proposing changes to the API (e.g. new functions/attributes,
     modification(s) to existing functions, etc.)
 
-3.7.3.5. Usage examples
+3.7.3.4. Usage examples
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 .. note::
     This may not be required for every PR and can be handled as separate PRs when
     needed. However, it would be a great practice to provide usage examples in the
     same PR, especially for demonstrating the use of complex UXarray functions.
```

### Comparing `uxarray-2023.4.0/docs/examples/000-template.ipynb` & `uxarray-2023.4.1/docs/examples/000-template.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/examples/001-read-grid-data.ipynb` & `uxarray-2023.4.1/docs/examples/001-read-grid-data.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/examples/002-access-grid-info.ipynb` & `uxarray-2023.4.1/docs/examples/002-access-grid-info.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/index.rst` & `uxarray-2023.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/installation.rst` & `uxarray-2023.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/make.bat` & `uxarray-2023.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/docs/user_api/index.rst` & `uxarray-2023.4.1/docs/user_api/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -36,7 +36,11 @@
    helpers.calculate_spherical_triangle_jacobian
    helpers.calculate_spherical_triangle_jacobian_barycentric
    helpers.get_all_face_area_from_coords
    helpers.get_gauss_quadratureDG
    helpers.get_tri_quadratureDG
    helpers.grid_center_lat_lon
    helpers.parse_grid_type
+   helpers.node_xyz_to_lonlat_rad
+   helpers.node_lonlat_rad_to_xyz
+   helpers.normalize_in_place
+   helpers.close_face_nodes
```

### Comparing `uxarray-2023.4.0/docs/user_api/uxarray_api.md` & `uxarray-2023.4.1/docs/user_api/uxarray_api.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/meta.yaml` & `uxarray-2023.4.1/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% set version = "2023.04.0" %}
+{% set version = "2023.04.1" %}
 
 package:
   name: 'uxarray'
   version: {{ version }}
 
 build:
   noarch: python
```

### Comparing `uxarray-2023.4.0/setup.py` & `uxarray-2023.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/exodus/mixed/mixed.exo` & `uxarray-2023.4.1/test/meshfiles/exodus/mixed/mixed.exo`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/exodus/outCSne8/outCSne8.g` & `uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/outCSne8.g`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc` & `uxarray-2023.4.1/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/scrip/outCSne8/outCSne8.nc` & `uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/outCSne8.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/shp/grid_fire.shp` & `uxarray-2023.4.1/test/meshfiles/shp/grid_fire.shp`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/README.md` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/u.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/v.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/grid.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/grid.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v1.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v1.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v2.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v3.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v3.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30.ug` & `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug` & `uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug` & `uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc` & `uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/test_exodus.py` & `uxarray-2023.4.1/test/test_exodus.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/test_grid.py` & `uxarray-2023.4.1/test/test_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -107,18 +107,14 @@
         # Now consturct the grid using the faces_coords
         verts_cart = np.array(faces_coords)
         vgrid = ux.Grid(verts_cart,
                         vertices=True,
                         islatlon=False,
                         concave=False)
 
-        # Since the read-in data are cartesian coordinates, we should change the unit to m
-        vgrid.ds.Mesh2_node_x.attrs["units"] = "m"
-        vgrid.ds.Mesh2_node_y.attrs["units"] = "m"
-        vgrid.ds.Mesh2_node_z.attrs["units"] = "m"
         assert (vgrid.source_grid == "From vertices")
         assert (vgrid.nMesh2_face == 6)
         assert (vgrid.nMesh2_node == 8)
         vgrid.encode_as("ugrid")
 
         # Test the case when user created a nested one-face grid
         faces_verts_one = np.array([
@@ -267,20 +263,14 @@
         n_nodes = grid.Mesh2_node_x.shape[0]
         n_faces, n_face_nodes = grid.Mesh2_face_nodes.shape
 
         self.assertEqual(n_nodes, grid.nMesh2_node)
         self.assertEqual(n_faces, grid.nMesh2_face)
         self.assertEqual(n_face_nodes, grid.nMaxMesh2_face_nodes)
 
-    # def test_init_dimension_attrs(self):
-
-    # TODO: Move to test_shpfile/scrip when implemented
-    # use external package to read?
-    # https://gis.stackexchange.com/questions/113799/how-to-read-a-shapefile-in-python
-
     def test_read_shpfile(self):
         """Reads a shape file and write ugrid file."""
         with self.assertRaises(RuntimeError):
             shp_filename = current_path / "meshfiles" / "shp" / "grid_fire.shp"
             tgrid = ux.Grid(str(shp_filename))
 
     def test_read_scrip(self):
@@ -292,36 +282,44 @@
         # Test read from scrip and from ugrid for grid class
         xr_grid_s8 = xr.open_dataset(scrip_8)
         ux_grid_s8 = ux.Grid(xr_grid_s8)  # tests from scrip
 
         xr_grid_u30 = xr.open_dataset(ug_30)
         ux_grid_u30 = ux.Grid(xr_grid_u30)  # tests from ugrid
 
+    def test_build_face_dimension(self):
+        """Tests the construction of the ``Mesh2_face_dimension`` variable."""
+        grids = [self.tgrid1, self.tgrid2, self.tgrid3]
+
+        for grid in grids:
+            # highest possible dimension dimension for a face
+            max_dimension = grid.nMaxMesh2_face_nodes
+
+            # face must be at least a triangle
+            min_dimension = 3
+
+            assert grid.Mesh2_face_dimension.min() >= min_dimension
+            assert grid.Mesh2_face_dimension.max() <= max_dimension
+
 
 class TestIntegrate(TestCase):
     mesh_file30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
     data_file30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30_vortex.nc"
     data_file30_v2 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30_var2.nc"
 
     def test_calculate_total_face_area_triangle(self):
         """Create a uxarray grid from vertices and saves an exodus file."""
         verts = [[[0.57735027, -5.77350269e-01, -0.57735027],
                   [0.57735027, 5.77350269e-01, -0.57735027],
                   [-0.57735027, 5.77350269e-01, -0.57735027]]]
-        vgrid = ux.Grid(verts)
 
-        # get node names for each grid object
-        x_var = vgrid.ds_var_names["Mesh2_node_x"]
-        y_var = vgrid.ds_var_names["Mesh2_node_y"]
-        z_var = vgrid.ds_var_names["Mesh2_node_z"]
-
-        vgrid.ds[x_var].attrs["units"] = "m"
-        vgrid.ds[y_var].attrs["units"] = "m"
-        vgrid.ds[z_var].attrs["units"] = "m"
+        # load grid
+        vgrid = ux.Grid(verts, vertices=True, islatlon=False, concave=False)
 
+        #calculate area
         area_gaussian = vgrid.calculate_total_face_area(
             quadrature_rule="gaussian", order=5)
         nt.assert_almost_equal(area_gaussian, constants.TRI_AREA, decimal=3)
 
         area_triangular = vgrid.calculate_total_face_area(
             quadrature_rule="triangular", order=4)
         nt.assert_almost_equal(area_triangular, constants.TRI_AREA, decimal=1)
@@ -332,14 +330,34 @@
         xr_grid = xr.open_dataset(str(self.mesh_file30))
         grid = ux.Grid(xr_grid)
 
         area = grid.calculate_total_face_area()
 
         nt.assert_almost_equal(area, constants.MESH30_AREA, decimal=3)
 
+    def test_calculate_total_face_area_sphere(self):
+        """Computes the total face area of an MPAS mesh that lies on a unit
+        sphere, with an expected total face area of 4pi."""
+        mpas_grid_path = current_path / 'meshfiles' / "mpas" / "QU" / 'mesh.QU.1920km.151026.nc'
+
+        ds = xr.open_dataset(mpas_grid_path)
+        primal_grid = ux.Grid(ds, use_dual=False)
+        dual_grid = ux.Grid(ds, use_dual=True)
+
+        primal_face_area = primal_grid.calculate_total_face_area()
+        dual_face_area = dual_grid.calculate_total_face_area()
+
+        nt.assert_almost_equal(primal_face_area,
+                               constants.UNIT_SPHERE_AREA,
+                               decimal=3)
+
+        nt.assert_almost_equal(dual_face_area,
+                               constants.UNIT_SPHERE_AREA,
+                               decimal=3)
+
     def test_integrate(self):
         xr_grid = xr.open_dataset(self.mesh_file30)
         xr_psi = xr.open_dataset(self.data_file30)
         xr_v2 = xr.open_dataset(self.data_file30_v2)
 
         u_grid = ux.Grid(xr_grid)
 
@@ -355,22 +373,44 @@
     def test_compute_face_areas_geoflow_small(self):
         """Checks if the GeoFlow Small can generate a face areas output."""
         geoflow_small_grid = current_path / "meshfiles" / "ugrid" / "geoflow-small" / "grid.nc"
         grid_1_ds = xr.open_dataset(geoflow_small_grid)
         grid_1 = ux.Grid(grid_1_ds)
         grid_1.compute_face_areas()
 
-    def test_compute_face_areas_fesom(self):
-        """Checks if the FESOM PI-Grid Output can generate a face areas
-        output."""
-
-        fesom_grid_small = current_path / "meshfiles" / "ugrid" / "fesom" / "fesom.mesh.diag.nc"
-        grid_2_ds = xr.open_dataset(fesom_grid_small)
-        grid_2 = ux.Grid(grid_2_ds)
-        grid_2.compute_face_areas()
+    # removed test until fix to tranposed face nodes
+    # def test_compute_face_areas_fesom(self):
+    #     """Checks if the FESOM PI-Grid Output can generate a face areas
+    #     output."""
+    #
+    #     fesom_grid_small = current_path / "meshfiles" / "ugrid" / "fesom" / "fesom.mesh.diag.nc"
+    #     grid_2_ds = xr.open_dataset(fesom_grid_small)
+    #     grid_2 = ux.Grid(grid_2_ds)
+    #     grid_2.compute_face_areas()
+
+    def test_verts_calc_area(self):
+        faces_verts_ndarray = np.array([
+            np.array([[150, 10, 0], [160, 20, 0], [150, 30, 0], [135, 30, 0],
+                      [125, 20, 0], [135, 10, 0]]),
+            np.array([[125, 20, 0], [135, 30, 0], [125, 60, 0], [110, 60, 0],
+                      [100, 30, 0], [105, 20, 0]]),
+            np.array([[95, 10, 0], [105, 20, 0], [100, 30, 0], [85, 30, 0],
+                      [75, 20, 0], [85, 10, 0]]),
+        ])
+        # load our vertices into a UXarray Grid object
+        verts_grid = ux.Grid(faces_verts_ndarray,
+                             vertices=True,
+                             islatlon=True,
+                             concave=False)
+
+        face_verts_areas = verts_grid.face_areas
+
+        nt.assert_almost_equal(face_verts_areas.sum(),
+                               constants.FACE_VERTS_AREA,
+                               decimal=3)
 
 
 class TestPopulateCoordinates(TestCase):
 
     def test_populate_cartesian_xyz_coord(self):
         # The following testcases are generated through the matlab cart2sph/sph2cart functions
         # These points correspond to the eight vertices of a cube.
@@ -394,15 +434,15 @@
 
         cart_z = [
             -0.577366836872017, 0.577366836872017, -0.577366836872017,
             0.577366836872017
         ]
 
         verts_degree = np.stack((lon_deg, lat_deg), axis=1)
-        vgrid = ux.Grid([verts_degree])
+        vgrid = ux.Grid([verts_degree], islatlon=False)
         vgrid._populate_cartesian_xyz_coord()
         for i in range(0, vgrid.nMesh2_node):
             nt.assert_almost_equal(vgrid.ds["Mesh2_node_cart_x"].values[i],
                                    cart_x[i],
                                    decimal=12)
             nt.assert_almost_equal(vgrid.ds["Mesh2_node_cart_y"].values[i],
                                    cart_y[i],
@@ -433,21 +473,70 @@
         ]
         cart_z = [
             0.577366836872017, -0.577366836872017, 0.577366836872017,
             -0.577366836872017
         ]
 
         verts_cart = np.stack((cart_x, cart_y, cart_z), axis=1)
-        vgrid = ux.Grid([verts_cart])
-        vgrid.ds.Mesh2_node_x.attrs["units"] = "m"
-        vgrid.ds.Mesh2_node_y.attrs["units"] = "m"
-        vgrid.ds.Mesh2_node_z.attrs["units"] = "m"
+        vgrid = ux.Grid([verts_cart], islatlon=False)
         vgrid._populate_lonlat_coord()
         # The connectivity in `__from_vert__()` will be formed in a reverse order
         lon_deg, lat_deg = zip(*reversed(list(zip(lon_deg, lat_deg))))
         for i in range(0, vgrid.nMesh2_node):
             nt.assert_almost_equal(vgrid.ds["Mesh2_node_x"].values[i],
                                    lon_deg[i],
                                    decimal=12)
             nt.assert_almost_equal(vgrid.ds["Mesh2_node_y"].values[i],
                                    lat_deg[i],
                                    decimal=12)
+
+
+class TestConnectivity(TestCase):
+    mpas_filepath = current_path / "meshfiles" / "mpas" / "QU" / "mesh.QU.1920km.151026.nc"
+    exodus_filepath = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
+    ugrid_filepath_01 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
+    ugrid_filepath_02 = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
+    ugrid_filepath_03 = current_path / "meshfiles" / "ugrid" / "ov_RLL10deg_CSne4" / "ov_RLL10deg_CSne4.ug"
+
+    def test_build_edge_nodes(self):
+        """Tests the construction of (``Mesh2_edge_nodes``) on an MPAS grid
+        with known edge nodes."""
+
+        # grid with known edge node connectivity
+        mpas_grid_xr = xr.open_dataset(self.mpas_filepath)
+        mpas_grid_ux = ux.Grid(mpas_grid_xr)
+        edge_nodes_expected = mpas_grid_ux.ds['Mesh2_edge_nodes'].values
+
+        # arrange edge nodes in the same manner as Grid._build_edge_node_connectivity
+        edge_nodes_expected.sort(axis=1)
+        edge_nodes_expected = np.unique(edge_nodes_expected, axis=0)
+
+        # construct edge nodes
+        mpas_grid_ux._build_edge_node_connectivity()
+        edge_nodes_output = mpas_grid_ux.ds['Mesh2_edge_nodes'].values
+
+        assert np.array_equal(edge_nodes_expected, edge_nodes_output)
+
+        # euler's formula (n_face = n_edges - n_nodes + 2)
+        n_face = mpas_grid_ux.nMesh2_node
+        n_node = mpas_grid_ux.nMesh2_face
+        n_edge = edge_nodes_output.shape[0]
+
+        assert (n_face == n_edge - n_node + 2)
+
+    def test_edge_nodes_euler(self):
+        """Verifies that (``nMesh2_edge``) follows euler's formula."""
+        grid_paths = [
+            self.exodus_filepath, self.ugrid_filepath_01,
+            self.ugrid_filepath_02, self.ugrid_filepath_03
+        ]
+
+        for grid_path in grid_paths:
+            grid_xr = xr.open_dataset(grid_path)
+            grid_ux = ux.Grid(grid_xr)
+
+            n_face = grid_ux.nMesh2_node
+            n_node = grid_ux.nMesh2_face
+            n_edge = grid_ux.nMesh2_edge
+
+            # euler's formula (n_face = n_edges - n_nodes + 2)
+            assert (n_face == n_edge - n_node + 2)
```

### Comparing `uxarray-2023.4.0/test/test_helpers.py` & `uxarray-2023.4.1/test/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,20 @@
     def test_face_area_coords(self):
         """Test function for helper function get_all_face_area_from_coords."""
         # Note: currently only testing one face, but this can be used to get area of multiple faces
         x = np.array([0.57735027, 0.57735027, -0.57735027])
         y = np.array([-5.77350269e-01, 5.77350269e-01, 5.77350269e-01])
         z = np.array([-0.57735027, -0.57735027, -0.57735027])
         face_nodes = np.array([[0, 1, 2]]).astype(INT_DTYPE)
+        face_dimension = np.array([3], dtype=INT_DTYPE)
         area = ux.get_all_face_area_from_coords(x,
                                                 y,
                                                 z,
                                                 face_nodes,
+                                                face_dimension,
                                                 3,
                                                 coords_type="cartesian")
         nt.assert_almost_equal(area, constants.TRI_AREA, decimal=1)
 
     def test_calculate_face_area(self):
         """Test function for helper function calculate_face_area - only one face."""
         # Note: currently only testing one face, but this can be used to get area of multiple faces
@@ -89,52 +91,63 @@
         np.testing.assert_array_almost_equal(scrip_center_lat, calc_lat)
         np.testing.assert_array_almost_equal(scrip_center_lon, calc_lon)
 
 
 class TestCoordinatesConversion(TestCase):
 
     def test_normalize_in_place(self):
-        [x, y, z] = ux.helpers._normalize_in_place(
+        [x, y, z] = ux.helpers.normalize_in_place(
             [random.random(), random.random(),
              random.random()])
         self.assertLessEqual(np.absolute(np.sqrt(x * x + y * y + z * z) - 1),
                              err_tolerance)
 
-    def test_convert_node_xyz_to_lonlat_rad(self):
-        [x, y, z] = ux.helpers._normalize_in_place([
+    def test_node_xyz_to_lonlat_rad(self):
+        [x, y, z] = ux.helpers.normalize_in_place([
             random.uniform(-1, 1),
             random.uniform(-1, 1),
             random.uniform(-1, 1)
         ])
-        [lon, lat] = ux.helpers._convert_node_xyz_to_lonlat_rad([x, y, z])
-        [new_x, new_y,
-         new_z] = ux.helpers._convert_node_lonlat_rad_to_xyz([lon, lat])
+        [lon, lat] = ux.helpers.node_xyz_to_lonlat_rad([x, y, z])
+        [new_x, new_y, new_z] = ux.helpers.node_lonlat_rad_to_xyz([lon, lat])
         self.assertLessEqual(np.absolute(new_x - x), err_tolerance)
         self.assertLessEqual(np.absolute(new_y - y), err_tolerance)
         self.assertLessEqual(np.absolute(new_z - z), err_tolerance)
 
-    def test_convert_node_latlon_rad_to_xyz(self):
+    def test_node_latlon_rad_to_xyz(self):
         [lon, lat] = [
             random.uniform(0, 2 * np.pi),
             random.uniform(-0.5 * np.pi, 0.5 * np.pi)
         ]
-        [x, y, z] = ux.helpers._convert_node_lonlat_rad_to_xyz([lon, lat])
-        [new_lon,
-         new_lat] = ux.helpers._convert_node_xyz_to_lonlat_rad([x, y, z])
+        [x, y, z] = ux.helpers.node_lonlat_rad_to_xyz([lon, lat])
+        [new_lon, new_lat] = ux.helpers.node_xyz_to_lonlat_rad([x, y, z])
         self.assertLessEqual(np.absolute(new_lon - lon), err_tolerance)
         self.assertLessEqual(np.absolute(new_lat - lat), err_tolerance)
 
 
 class TestConstants(TestCase):
     # DTYPE as set in constants.py
     expected_int_dtype = INT_DTYPE
 
     # INT_FILL_VALUE as set in constants.py
     fv = INT_FILL_VALUE
 
+    def test_invalid_indexing(self):
+        """Tests if the current INT_DTYPE and INT_FILL_VALUE throw the correct
+        errors when indexing."""
+        dummy_data = np.array([1, 2, 3, 4])
+
+        invalid_indices = np.array([self.fv, self.fv], dtype=INT_DTYPE)
+        invalid_index = self.fv
+
+        # invalid index/indices should throw an Index Error
+        with self.assertRaises(IndexError):
+            dummy_data[invalid_indices]
+            dummy_data[invalid_index]
+
     def test_replace_fill_values(self):
         """Tests _replace_fill_values() helper function across multiple
         different dtype arrays used as face_nodes."""
 
         # expected output from _replace_fill_values()
         face_nodes_gold = np.array(
             [[1, 2, self.fv], [self.fv, self.fv, self.fv]], dtype=INT_DTYPE)
```

### Comparing `uxarray-2023.4.0/test/test_mpas.py` & `uxarray-2023.4.1/test/test_mpas.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,7 +92,33 @@
 
         # test data output
         verticesOnCell = _replace_padding(verticesOnCell, nEdgesOnCell)
         verticesOnCell = _replace_zeros(verticesOnCell)
         verticesOnCell = _to_zero_index(verticesOnCell)
 
         assert np.array_equal(verticesOnCell, gold_output)
+
+    def test_set_attrs(self):
+        """Tests the execution of "_set_global_attrs", checking for attributes
+        being correctly stored in "Grid.ds"."""
+
+        # full set of expected mpas attributes
+        expected_attrs = [
+            'sphere_radius', 'mesh_spec', 'on_a_sphere', 'mesh_id',
+            'is_periodic', 'x_period', 'y_period'
+        ]
+
+        # included attrs: 'sphere_radius', 'mesh_spec' 'on_a_sphere'
+        ds = _read_mpas(self.mpas_xr_ds)
+
+        # set dummy attrs to test execution
+        ds.attrs['mesh_id'] = "12345678"
+        ds.attrs['is_periodic'] = "YES"
+        ds.attrs['x_period'] = 1.0
+        ds.attrs['y_period'] = 1.0
+
+        # create a grid
+        uxgrid = ux.Grid(ds)
+
+        # check if all expected attributes are set
+        for mpas_attr in expected_attrs:
+            assert mpas_attr in uxgrid.ds.attrs
```

### Comparing `uxarray-2023.4.0/test/test_scrip.py` & `uxarray-2023.4.1/test/test_scrip.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/test/test_ugrid.py` & `uxarray-2023.4.1/test/test_ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/uxarray/_exodus.py` & `uxarray-2023.4.1/uxarray/_exodus.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/uxarray/_mpas.py` & `uxarray-2023.4.1/uxarray/_mpas.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,49 +232,50 @@
         Input MPAS dataset
     out_ds : xarray.Dataset
         Output dataset where the MPAS Primal-Mesh is encoded in the UGRID
         conventions with global attributes included
     """
 
     # defines if the mesh describes points that lie on the surface of a sphere or not
-    if 'sphere_radius' in in_ds:
-        out_ds['sphere_radius'] = in_ds.sphere_radius
+    if 'sphere_radius' in in_ds.attrs:
+        out_ds.attrs['sphere_radius'] = in_ds.sphere_radius
     else:
         warnings.warn("Missing Required Attribute: 'sphere_radius'")
 
     # typically a random string used for tracking mesh provenance
-    if 'mesh_id' in in_ds:
-        out_ds['mesh_id'] = in_ds.mesh_id
+    if 'mesh_id' in in_ds.attrs:
+        out_ds.attrs['mesh_id'] = in_ds.mesh_id
     else:
         warnings.warn("Missing Required Attribute: 'mesh_id'")
 
     # defines the version of the MPAS Mesh specification the mesh conforms to
-    if 'mesh_spec' in in_ds:
-        out_ds['mesh_spec'] = in_ds.mesh_spec
+    if 'mesh_spec' in in_ds.attrs:
+        out_ds.attrs['mesh_spec'] = in_ds.mesh_spec
     else:
         warnings.warn("Missing Required Attribute: 'mesh_spec'")
 
     # defines if the mesh describes points that lie on the surface of a sphere or not
-    if "on_a_sphere" in in_ds:
-        out_ds['on_a_sphere'] = in_ds.on_a_sphere
+    if "on_a_sphere" in in_ds.attrs:
+        out_ds.attrs['on_a_sphere'] = in_ds.on_a_sphere
         # required attributes if mesh does not lie on a sphere
         if in_ds.on_a_sphere == "NO":
             # defines if the mesh has any periodic boundaries
-            out_ds['is_periodic'] = in_ds.is_periodic
-            if in_ds.is_periodic == "YES":
-                # period of the mesh in the x direction
-                if "x_period" in in_ds:
-                    out_ds['x_period'] = in_ds.x_period
-                else:
-                    warnings.warn("Missing Required Attribute: 'x_period'")
-                # period of the mesh in the y direction
-                if "y_period" in in_ds:
-                    out_ds['y_period'] = in_ds.y_period
-                else:
-                    warnings.warn("Missing Required Attribute: 'y_period'")
+            if "is_periodic" in in_ds.attrs:
+                out_ds.attrs['is_periodic'] = in_ds.is_periodic
+                if in_ds.is_periodic == "YES":
+                    # period of the mesh in the x direction
+                    if "x_period" in in_ds.attrs:
+                        out_ds.attrs['x_period'] = in_ds.x_period
+                    else:
+                        warnings.warn("Missing Required Attribute: 'x_period'")
+                    # period of the mesh in the y direction
+                    if "y_period" in in_ds.attrs:
+                        out_ds.attrs['y_period'] = in_ds.y_period
+                    else:
+                        warnings.warn("Missing Required Attribute: 'y_period'")
     else:
         warnings.warn("Missing Required Attribute: 'on_a_sphere'")
 
 
 def _replace_padding(verticesOnCell, nEdgesOnCell):
     """Replaces the padded values in verticesOnCell defined by nEdgesOnCell
     with a fill-value.
```

### Comparing `uxarray-2023.4.0/uxarray/_scrip.py` & `uxarray-2023.4.1/uxarray/_scrip.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/uxarray/_ugrid.py` & `uxarray-2023.4.1/uxarray/_ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/uxarray/get_quadratureDG.py` & `uxarray-2023.4.1/uxarray/get_quadratureDG.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.0/uxarray/grid.py` & `uxarray-2023.4.1/uxarray/grid.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # reader and writer imports
 from ._exodus import _read_exodus, _encode_exodus
 from ._ugrid import _read_ugrid, _encode_ugrid
 from ._shapefile import _read_shpfile
 from ._scrip import _read_scrip, _encode_scrip
 from ._mpas import _read_mpas
-from .helpers import get_all_face_area_from_coords, parse_grid_type, _convert_node_xyz_to_lonlat_rad, _convert_node_lonlat_rad_to_xyz
+from .helpers import get_all_face_area_from_coords, parse_grid_type, node_xyz_to_lonlat_rad, node_lonlat_rad_to_xyz, close_face_nodes
 from .constants import INT_DTYPE, INT_FILL_VALUE
 
 
 class Grid:
     """
     Examples
     ----------
@@ -95,14 +95,22 @@
             self.__from_ds__(dataset=dataset)
         else:
             raise RuntimeError("Dataset is not a valid input type.")
 
         # initialize convenience attributes
         self.__init_grid_var_attrs__()
 
+        # construct connectivity
+        if self.source_grid != "From vertices":
+            if "Mesh2_edge_nodes" not in self.ds:
+                self._build_edge_node_connectivity()
+
+        # build face dimension, possibly safeguard for large datasets
+        self._build_face_dimension()
+
     def __init_ds_var_names__(self):
         """Populates a dictionary for storing uxarray's internal representation
         of xarray object.
 
         Note ugrid conventions are flexible with names of variables, see:
         http://ugrid-conventions.github.io/ugrid-conventions/
         """
@@ -171,24 +179,30 @@
                 "node_coordinates": "Mesh2_node_x Mesh2_node_y Mesh2_node_z",
                 "node_dimension": "nMesh2_node",
                 "face_node_connectivity": "Mesh2_face_nodes",
                 "face_dimension": "nMesh2_face"
             })
         self.ds.Mesh2.attrs['topology_dimension'] = dataset.ndim
 
-        # set default coordinate units to spherical coordinates
-        # users can change to cartesian if using cartesian for initialization
-        x_units = "degrees_east"
-        y_units = "degrees_north"
-        if dataset[0][0].size > 2:
+        if self.islatlon is not None and self.islatlon is False:
+            x_units = 'm'
+            y_units = 'm'
+            z_units = 'm'
+        else:
+            x_units = "degrees_east"
+            y_units = "degrees_north"
             z_units = "elevation"
+
         x_coord = dataset[:, :, 0].flatten()
         y_coord = dataset[:, :, 1].flatten()
+
         if dataset[0][0].size > 2:
             z_coord = dataset[:, :, 2].flatten()
+        else:
+            z_coord = x_coord * 0.0
 
         # Identify unique vertices and their indices
         unique_verts, indices = np.unique(dataset.reshape(
             -1, dataset.shape[-1]),
                                           axis=0,
                                           return_inverse=True)
 
@@ -210,27 +224,32 @@
 
             # Remove the rows corresponding to False values in unique_verts
             unique_verts = np.delete(unique_verts, false_indices, axis=0)
 
             # Update indices accordingly
             for i, idx in enumerate(false_indices):
                 indices[indices == idx] = INT_FILL_VALUE
-                indices[indices > idx] -= 1
+                indices[(indices > idx) & (indices != INT_FILL_VALUE)] -= 1
 
         # Create coordinate DataArrays
         self.ds["Mesh2_node_x"] = xr.DataArray(data=unique_verts[:, 0],
                                                dims=["nMesh2_node"],
                                                attrs={"units": x_units})
         self.ds["Mesh2_node_y"] = xr.DataArray(data=unique_verts[:, 1],
                                                dims=["nMesh2_node"],
                                                attrs={"units": y_units})
         if dataset.shape[-1] > 2:
             self.ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 2],
                                                    dims=["nMesh2_node"],
                                                    attrs={"units": z_units})
+        else:
+            self.ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 1] *
+                                                   0.0,
+                                                   dims=["nMesh2_node"],
+                                                   attrs={"units": z_units})
 
         # Create connectivity array using indices of unique vertices
         connectivity = indices.reshape(dataset.shape[:-1])
         self.ds["Mesh2_face_nodes"] = xr.DataArray(
             data=xr.DataArray(connectivity).astype(INT_DTYPE),
             dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
             attrs={
@@ -337,48 +356,59 @@
         --------
         Open a uxarray grid file
 
         >>> grid = ux.open_dataset("/home/jain/uxarray/test/meshfiles/ugrid/outCSne30/outCSne30.ug")
 
         Get area of all faces in the same order as listed in grid.ds.Mesh2_face_nodes
 
-        >>> grid.get_face_areas
+        >>> grid.face_areas
         array([0.00211174, 0.00211221, 0.00210723, ..., 0.00210723, 0.00211221,
             0.00211174])
         """
-        if self._face_areas is None:
-            # area of a face call needs the units for coordinate conversion if spherical grid is used
-            coords_type = "spherical"
-            if not "degree" in self.Mesh2_node_x.units:
-                coords_type = "cartesian"
-
-            face_nodes = self.Mesh2_face_nodes.data
-            dim = self.Mesh2.attrs['topology_dimension']
-
-            # initialize z
-            z = np.zeros((self.nMesh2_node))
-
-            # call func to cal face area of all nodes
-            x = self.Mesh2_node_x.data
-            y = self.Mesh2_node_y.data
-            # check if z dimension
-            if self.Mesh2.topology_dimension > 2:
-                z = self.Mesh2_node_z.data
-
-            # call function to get area of all the faces as a np array
-            self._face_areas = get_all_face_area_from_coords(
-                x, y, z, face_nodes, dim, quadrature_rule, order, coords_type)
+        # if self._face_areas is None: # this allows for using the cached result,
+        # but is not the expected behavior behavior as we are in need to recompute if this function is called with different quadrature_rule or order
+
+        # area of a face call needs the units for coordinate conversion if spherical grid is used
+        coords_type = "spherical"
+        if not "degree" in self.Mesh2_node_x.units:
+            coords_type = "cartesian"
+
+        face_nodes = self.Mesh2_face_nodes.data
+        face_dimension = self.Mesh2_face_dimension.data
+        dim = self.Mesh2.attrs['topology_dimension']
+
+        # initialize z
+        z = np.zeros((self.nMesh2_node))
+
+        # call func to cal face area of all nodes
+        x = self.Mesh2_node_x.data
+        y = self.Mesh2_node_y.data
+        # check if z dimension
+        if self.Mesh2.topology_dimension > 2:
+            z = self.Mesh2_node_z.data
+
+        # Note: x, y, z are np arrays of type float
+        # Using np.issubdtype to check if the type is float
+        # if not (int etc.), convert to float, this is to avoid numba errors
+        x, y, z = (arr.astype(float)
+                   if not np.issubdtype(arr[0], np.floating) else arr
+                   for arr in (x, y, z))
+
+        # call function to get area of all the faces as a np array
+        self._face_areas = get_all_face_area_from_coords(
+            x, y, z, face_nodes, face_dimension, dim, quadrature_rule, order,
+            coords_type)
 
         return self._face_areas
 
     # use the property keyword for declaration on face_areas property
     @property
     def face_areas(self):
         """Declare face_areas as a property."""
-
+        # if self._face_areas is not None: it allows for using the cached result
         if self._face_areas is None:
             self.compute_face_areas()
         return self._face_areas
 
     def integrate(self, var_ds, quadrature_rule="triangular", order=4):
         """Integrates over all the faces of the given mesh.
 
@@ -419,14 +449,89 @@
             )
         var_key = var_key[0]
         face_vals = var_ds[var_key].to_numpy()
         integral = np.dot(face_areas, face_vals)
 
         return integral
 
+    def _build_edge_node_connectivity(self):
+        """Constructs the UGRID connectivity variable (``Mesh2_edge_nodes``)
+        and stores it within the internal (``Grid.ds``) and through the
+        attribute (``Grid.Mesh2_edge_nodes``).
+
+        Additionally, the attributes (``inverse_indices``) and
+        (``fill_value_mask``) are stored for constructing other
+        connectivity variables.
+        """
+        padded_face_nodes = close_face_nodes(self.Mesh2_face_nodes.values,
+                                             self.nMesh2_face,
+                                             self.nMaxMesh2_face_nodes)
+
+        # array of empty edge nodes where each entry is a pair of indices
+        edge_nodes = np.empty((self.nMesh2_face * self.nMaxMesh2_face_nodes, 2),
+                              dtype=INT_DTYPE)
+
+        # first index includes starting node up to non-padded value
+        edge_nodes[:, 0] = padded_face_nodes[:, :-1].ravel()
+
+        # second index includes second node up to padded value
+        edge_nodes[:, 1] = padded_face_nodes[:, 1:].ravel()
+
+        # sorted edge nodes
+        edge_nodes.sort(axis=1)
+
+        # unique edge nodes
+        edge_nodes_unique, inverse_indices = np.unique(edge_nodes,
+                                                       return_inverse=True,
+                                                       axis=0)
+        # find all edge nodes that contain a fill value
+        fill_value_mask = np.logical_or(
+            edge_nodes_unique[:, 0] == INT_FILL_VALUE,
+            edge_nodes_unique[:, 1] == INT_FILL_VALUE)
+
+        # all edge nodes that do not contain a fill value
+        non_fill_value_mask = np.logical_not(fill_value_mask)
+        edge_nodes_unique = edge_nodes_unique[non_fill_value_mask]
+
+        # Update inverse_indices accordingly
+        indices_to_update = np.where(fill_value_mask)[0]
+
+        remove_mask = np.isin(inverse_indices, indices_to_update)
+        inverse_indices[remove_mask] = INT_FILL_VALUE
+
+        # Compute the indices where inverse_indices exceeds the values in indices_to_update
+        indexes = np.searchsorted(indices_to_update,
+                                  inverse_indices,
+                                  side='right')
+        # subtract the corresponding indexes from `inverse_indices`
+        for i in range(len(inverse_indices)):
+            if inverse_indices[i] != INT_FILL_VALUE:
+                inverse_indices[i] -= indexes[i]
+
+        # add Mesh2_edge_nodes to internal dataset
+        self.ds['Mesh2_edge_nodes'] = xr.DataArray(
+            edge_nodes_unique,
+            dims=["nMesh2_edge", "Two"],
+            attrs={
+                "cf_role":
+                    "edge_node_connectivity",
+                "long_name":
+                    "Maps every edge to the two nodes that it connects",
+                "start_index":
+                    INT_DTYPE(0),
+                "inverse_indices":
+                    inverse_indices,
+                "fill_value_mask":
+                    fill_value_mask
+            })
+
+        # set standardized attributes
+        setattr(self, "Mesh2_edge_nodes", self.ds['Mesh2_edge_nodes'])
+        setattr(self, "nMesh2_edge", edge_nodes_unique.shape[0])
+
     def _populate_cartesian_xyz_coord(self):
         """A helper function that populates the xyz attribute in UXarray.ds.
         This function is called when we need to use the cartesian coordinates
         for each node to do the calculation but the input data only has the
         "Mesh2_node_x" and "Mesh2_node_y" in degree.
 
         Note
@@ -453,15 +558,15 @@
             return
 
         # check for units and create Mesh2_node_cart_x/y/z set to self.ds
         nodes_lon_rad = np.deg2rad(self.Mesh2_node_x.values)
         nodes_lat_rad = np.deg2rad(self.Mesh2_node_y.values)
         nodes_rad = np.stack((nodes_lon_rad, nodes_lat_rad), axis=1)
         nodes_cart = np.asarray(
-            list(map(_convert_node_lonlat_rad_to_xyz, list(nodes_rad))))
+            list(map(node_lonlat_rad_to_xyz, list(nodes_rad))))
 
         self.ds["Mesh2_node_cart_x"] = xr.DataArray(
             data=nodes_cart[:, 0],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "cartesian x",
                 "units": "m",
@@ -532,15 +637,15 @@
             data=self.ds["Mesh2_node_z"].values)
 
         # convert the input cartesian values into the longitude latitude degree
         nodes_cart = np.stack(
             (self.ds["Mesh2_node_x"].values, self.ds["Mesh2_node_y"].values,
              self.ds["Mesh2_node_z"].values),
             axis=1).tolist()
-        nodes_rad = list(map(_convert_node_xyz_to_lonlat_rad, nodes_cart))
+        nodes_rad = list(map(node_xyz_to_lonlat_rad, nodes_cart))
         nodes_degree = np.rad2deg(nodes_rad)
         self.ds["Mesh2_node_x"] = xr.DataArray(
             data=nodes_degree[:, 0],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "longitude",
                 "long_name": "longitude of mesh nodes",
@@ -550,7 +655,33 @@
             data=nodes_degree[:, 1],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "lattitude",
                 "long_name": "latitude of mesh nodes",
                 "units": "degrees_north",
             })
+
+    def _build_face_dimension(self):
+        """Constructs ``Mesh2_face_dimension``, which calculates the dimension
+        of each face in ``Mesh2_face_nodes``"""
+
+        # Triangular Mesh
+        if not hasattr(self, "nMaxMesh2_face_nodes"):
+            nMaxMesh2_face_nodes = self.Mesh2_face_nodes.shape[1]
+            setattr(self, "nMaxMesh2_face_nodes", nMaxMesh2_face_nodes)
+
+        # padding to shape [nMesh2_face, nMaxMesh2_face_nodes + 1]
+        closed = np.ones((self.nMesh2_face, self.nMaxMesh2_face_nodes + 1),
+                         dtype=INT_DTYPE) * INT_FILL_VALUE
+
+        closed[:, :-1] = self.Mesh2_face_nodes.copy()
+
+        face_dimension = np.argmax(closed == INT_FILL_VALUE, axis=1)
+
+        # add to internal dataset
+        self.ds["Mesh2_face_dimension"] = xr.DataArray(
+            data=face_dimension,
+            dims=["nMesh2_face"],
+            attrs={"long_name": "number of non-fill value nodes for each face"})
+
+        # standardized attribute
+        setattr(self, "Mesh2_face_dimension", self.ds["Mesh2_face_dimension"])
```

### Comparing `uxarray-2023.4.0/uxarray/helpers.py` & `uxarray-2023.4.1/uxarray/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import xarray as xr
 from pathlib import PurePath
 from .get_quadratureDG import get_gauss_quadratureDG, get_tri_quadratureDG
 from numba import njit, config
 import math
 
-from .constants import INT_DTYPE
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 
 config.DISABLE_JIT = False
 
 
 def parse_grid_type(dataset):
     """Checks input and contents to determine grid type. Supports detection of
     UGrid, SCRIP, Exodus and shape file.
@@ -150,22 +150,22 @@
     for j in range(0, num_triangles):
         node1 = np.array([x[0], y[0], z[0]], dtype=np.float64)
         node2 = np.array([x[j + 1], y[j + 1], z[j + 1]], dtype=np.float64)
         node3 = np.array([x[j + 2], y[j + 2], z[j + 2]], dtype=np.float64)
 
         if (coords_type == "spherical"):
             node1 = np.array(
-                _convert_node_lonlat_rad_to_xyz(
-                    [np.deg2rad(x[0]), np.deg2rad(y[0])]))
+                node_lonlat_rad_to_xyz([np.deg2rad(x[0]),
+                                        np.deg2rad(y[0])]))
             node2 = np.array(
-                _convert_node_lonlat_rad_to_xyz(
+                node_lonlat_rad_to_xyz(
                     [np.deg2rad(x[j + 1]),
                      np.deg2rad(y[j + 1])]))
             node3 = np.array(
-                _convert_node_lonlat_rad_to_xyz(
+                node_lonlat_rad_to_xyz(
                     [np.deg2rad(x[j + 2]),
                      np.deg2rad(y[j + 2])]))
 
         for p in range(len(dW)):
             if quadrature_rule == "gaussian":
                 for q in range(len(dW)):
                     dA = dG[0][p]
@@ -184,14 +184,15 @@
 
 
 @njit
 def get_all_face_area_from_coords(x,
                                   y,
                                   z,
                                   face_nodes,
+                                  face_geometry,
                                   dim,
                                   quadrature_rule="triangular",
                                   order=4,
                                   coords_type="spherical"):
     """Given coords, connectivity and other area calculation params, this
     routine loop over all faces and return an numpy array with areas of each
     face.
@@ -222,33 +223,36 @@
     coords_type : str, optional
         coordinate type, default is spherical, can be cartesian also.
 
     Returns
     -------
     area of all faces : ndarray
     """
-    num_faces = face_nodes.shape[0]
-    area = np.zeros(num_faces)  # set area of each face to 0
 
-    face_nodes = face_nodes[:].astype(INT_DTYPE)
+    n_face, n_max_face_nodes = face_nodes.shape
 
-    for i in range(num_faces):
-        face_z = np.zeros(len(face_nodes[i]))
+    # set initial area of each face to 0
+    area = np.zeros(n_face)
+
+    for face_idx, max_nodes in enumerate(face_geometry):
+        face_x = x[face_nodes[face_idx, 0:max_nodes]]
+        face_y = y[face_nodes[face_idx, 0:max_nodes]]
 
-        face_x = x[face_nodes[i]]
-        face_y = y[face_nodes[i]]
         # check if z dimension
+
         if dim > 2:
-            face_z = z[face_nodes[i]]
+            face_z = z[face_nodes[face_idx, 0:max_nodes]]
+        else:
+            face_z = face_x * 0.0
 
         # After getting all the nodes of a face assembled call the  cal. face area routine
         face_area = calculate_face_area(face_x, face_y, face_z, quadrature_rule,
                                         order, coords_type)
-
-        area[i] = face_area
+        # store current face area
+        area[face_idx] = face_area
 
     return area
 
 
 @njit
 def calculate_spherical_triangle_jacobian(node1, node2, node3, dA, dB):
     """Calculate Jacobian of a spherical triangle. This is a helper function
@@ -459,15 +463,15 @@
     # Make negative lons positive
     center_lon[center_lon < 0] += 360
 
     return center_lat, center_lon
 
 
 @njit
-def _convert_node_lonlat_rad_to_xyz(node_coord):
+def node_lonlat_rad_to_xyz(node_coord):
     """Helper function to Convert the node coordinate from 2D
     longitude/latitude to normalized 3D xyz.
 
     Parameters
     ----------
     node: float list
         2D coordinates[longitude, latitude] in radiance
@@ -487,15 +491,15 @@
             "Input array should have a length of 2: [longitude, latitude]")
     lon = node_coord[0]
     lat = node_coord[1]
     return [np.cos(lon) * np.cos(lat), np.sin(lon) * np.cos(lat), np.sin(lat)]
 
 
 @njit
-def _convert_node_xyz_to_lonlat_rad(node_coord):
+def node_xyz_to_lonlat_rad(node_coord):
     """Calculate the latitude and longitude in radiance for a node represented
     in the [x, y, z] 3D Cartesian coordinates.
 
     Parameters
     ----------
     node_coord: float list
         3D Cartesian Coordinates [x, y, z] of the node
@@ -509,15 +513,15 @@
     ----------
     RuntimeError
         The input array doesn't have the size of 3.
     """
     if len(node_coord) != 3:
         raise RuntimeError("Input array should have a length of 3: [x, y, z]")
     reference_tolerance = 1.0e-12
-    [dx, dy, dz] = _normalize_in_place(node_coord)
+    [dx, dy, dz] = normalize_in_place(node_coord)
     dx /= np.absolute(dx * dx + dy * dy + dz * dz)
     dy /= np.absolute(dx * dx + dy * dy + dz * dz)
     dz /= np.absolute(dx * dx + dy * dy + dz * dz)
 
     if np.absolute(dz) < (1.0 - reference_tolerance):
         d_lon_rad = math.atan2(dy, dx)
         d_lat_rad = np.arcsin(dz)
@@ -531,15 +535,15 @@
         d_lon_rad = 0.0
         d_lat_rad = -0.5 * np.pi
 
     return [d_lon_rad, d_lat_rad]
 
 
 @njit
-def _normalize_in_place(node):
+def normalize_in_place(node):
     """Helper function to project an arbitrary node in 3D coordinates [x, y, z]
     on the unit sphere. It uses the `np.linalg.norm` internally to calculate
     the magnitude.
 
     Parameters
     ----------
     node: float list
@@ -554,15 +558,15 @@
     ----------
     RuntimeError
         The input array doesn't have the size of 3.
     """
     if len(node) != 3:
         raise RuntimeError("Input array should have a length of 3: [x, y, z]")
 
-    return list(np.array(node) / np.linalg.norm(np.array(node), ord=2))
+    return np.array(node) / np.linalg.norm(np.array(node), ord=2)
 
 
 def _replace_fill_values(grid_var, original_fill, new_fill, new_dtype=None):
     """Replaces all instances of the the current fill value (``original_fill``)
     in (``grid_var``) with (``new_fill``) and converts to the dtype defined by
     (``new_dtype``)
 
@@ -614,7 +618,58 @@
         raise ValueError(f'Data type {grid_var.dtype} not supported'
                          f'for grid variables')
 
     # replace all zeros with a fill value
     grid_var[fill_val_idx] = new_fill
 
     return grid_var
+
+
+def close_face_nodes(Mesh2_face_nodes, nMesh2_face, nMaxMesh2_face_nodes):
+    """Closes (``Mesh2_face_nodes``) by inserting the first node index after
+    the last non-fill-value node.
+
+    Parameters
+    ----------
+    Mesh2_face_nodes : np.ndarray
+        Connectivity array for constructing a face from its nodes
+    nMesh2_face : constant
+        Number of faces
+    nMaxMesh2_face_nodes : constant
+        Max number of nodes that compose a face
+
+    Returns
+    ----------
+    closed : ndarray
+        Closed (padded) Mesh2_face_nodes
+
+    Example
+    ----------
+    Given face nodes with shape [2 x 5]
+        [0, 1, 2, 3, FILL_VALUE]
+        [4, 5, 6, 7, 8]
+    Pads them to the following with shape [2 x 6]
+        [0, 1, 2, 3, 0, FILL_VALUE]
+        [4, 5, 6, 7, 8, 4]
+    """
+
+    # padding to shape [nMesh2_face, nMaxMesh2_face_nodes + 1]
+    closed = np.ones((nMesh2_face, nMaxMesh2_face_nodes + 1),
+                     dtype=INT_DTYPE) * INT_FILL_VALUE
+
+    # set all non-paded values to original face nodee values
+    closed[:, :-1] = Mesh2_face_nodes.copy()
+
+    # instance of first fill value
+    first_fv_idx_2d = np.argmax(closed == INT_FILL_VALUE, axis=1)
+
+    # 2d to 1d index for np.put()
+    first_fv_idx_1d = first_fv_idx_2d + (
+        (nMaxMesh2_face_nodes + 1) * np.arange(0, nMesh2_face))
+
+    # column of first node values
+    first_node_value = Mesh2_face_nodes[:, 0].copy()
+
+    # insert first node column at occurrence of first fill value
+    np.put(closed.ravel(), first_fv_idx_1d, first_node_value)
+
+    return closed
```

### Comparing `uxarray-2023.4.0/uxarray.egg-info/PKG-INFO` & `uxarray-2023.4.1/uxarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
```

### Comparing `uxarray-2023.4.0/uxarray.egg-info/SOURCES.txt` & `uxarray-2023.4.1/uxarray.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 docs/_static/images/logos/PANGEO_logo.png
 docs/_static/images/logos/uxarray_temp_logo.png
 docs/_static/thumbnails/default.svg
 docs/_templates/breadcrumbs.html
 docs/examples/000-template.ipynb
 docs/examples/001-read-grid-data.ipynb
 docs/examples/002-access-grid-info.ipynb
+docs/examples/003-area-calc.ipynb
 docs/internal_api/index.rst
 docs/user_api/index.rst
 docs/user_api/uxarray_api.md
 test/__init__.py
 test/constants.py
 test/test_exodus.py
 test/test_grid.py
```


# Comparing `tmp/impsparc-2.0.4.tar.gz` & `tmp/impsparc-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-2.0.4.tar", last modified: Fri Apr 21 13:34:59 2023, max compression
+gzip compressed data, was "impsparc-2.0.5.tar", last modified: Mon Apr 24 07:42:42 2023, max compression
```

## Comparing `impsparc-2.0.4.tar` & `impsparc-2.0.5.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.823481 impsparc-2.0.4/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.4/LICENSE.md
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.4/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-21 13:34:59.822923 impsparc-2.0.4/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.4/README.md
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.629014 impsparc-2.0.4/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.641939 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.644281 impsparc-2.0.4/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.4/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.676888 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60112 2023-04-21 10:43:22.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.715713 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.726664 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/json_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.744526 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.745782 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.622204 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.797361 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.802528 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.815589 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.747992 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.620233 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.755218 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.761145 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.770852 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.789831 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    17455 2023-04-21 10:44:55.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.4/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-21 13:34:59.821898 impsparc-2.0.4/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      217 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-21 13:34:59.000000 impsparc-2.0.4/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-21 13:34:59.823638 impsparc-2.0.4/setup.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1250 2023-04-21 13:34:49.000000 impsparc-2.0.4/setup.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.110858 impsparc-2.0.5/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.5/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.5/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-24 07:42:42.110521 impsparc-2.0.5/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.5/README.md
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.011076 impsparc-2.0.5/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.033131 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.034118 impsparc-2.0.5/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.5/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.039812 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60112 2023-04-21 10:43:22.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.047472 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.051673 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/json_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.057919 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.058462 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.008214 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.097241 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.099831 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.106437 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.059116 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.006385 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.078209 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.080747 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.085425 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.093779 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    17513 2023-04-24 07:41:23.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.5/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-24 07:42:42.109941 impsparc-2.0.5/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      217 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-24 07:42:41.000000 impsparc-2.0.5/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-24 07:42:42.110962 impsparc-2.0.5/setup.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1250 2023-04-24 07:42:03.000000 impsparc-2.0.5/setup.py
```

### Comparing `impsparc-2.0.4/LICENSE.md` & `impsparc-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/PKG-INFO` & `impsparc-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.4
+Version: 2.0.5
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-2.0.4/README.md` & `impsparc-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-2.0.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/base.py` & `impsparc-2.0.5/cvsvc_apirisk/score/base.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python
 
 import sys
+import os
 from argparse import ArgumentParser
 from configparser import ConfigParser
 
 import networkit as nk
 from sqlitedict import SqliteDict
 
 
@@ -46,14 +47,15 @@
 
         self.create_node_id_key_mapping()
         # this variable to passed in get node index while querying node-id-mapping variable
         self.total_node_plus_ten = self.G.numberOfNodes() + 10
 
 
     def create_node_id_key_mapping(self):
+        os.unlink("node_id_key_mapping.sqlite")
         self.node_id_mapping = SqliteDict("node_id_key_mapping.sqlite",
                                           tablename='node_id_key_mapping',
                                           outer_stack=False)
         for node in self.G.iterNodes():
             self.node_id_mapping[self.node_attributes['node_name_sp'][node]] = node
         self.node_id_mapping.commit()
     #     self.node_id_mapping.close()
```

### Comparing `impsparc-2.0.4/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-2.0.5/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/impsparc.egg-info/PKG-INFO` & `impsparc-2.0.5/impsparc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.4
+Version: 2.0.5
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-2.0.4/impsparc.egg-info/SOURCES.txt` & `impsparc-2.0.5/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.4/setup.py` & `impsparc-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "2.0.4"),
+    version=os.environ.get("VER", "2.0.5"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```


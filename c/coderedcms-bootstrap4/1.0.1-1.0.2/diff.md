# Comparing `tmp/coderedcms-bootstrap4-1.0.1.tar.gz` & `tmp/coderedcms-bootstrap4-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderedcms-bootstrap4-1.0.1.tar", last modified: Thu Aug 25 14:46:04 2022, max compression
+gzip compressed data, was "coderedcms-bootstrap4-1.0.2.tar", last modified: Mon Apr 24 15:23:02 2023, max compression
```

## Comparing `coderedcms-bootstrap4-1.0.1.tar` & `coderedcms-bootstrap4-1.0.2.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.510232 coderedcms-bootstrap4-1.0.1/
--rw-rw-rw-   0        0        0     1548 2022-08-08 18:10:37.000000 coderedcms-bootstrap4-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      105 2022-08-08 18:10:37.000000 coderedcms-bootstrap4-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1979 2022-08-25 14:46:04.510232 coderedcms-bootstrap4-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2022-08-08 18:32:41.000000 coderedcms-bootstrap4-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.330134 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.318098 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.327888 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.351948 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/
--rw-rw-rw-   0        0        0     5972 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css
--rw-rw-rw-   0        0        0     5962 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css.map
--rw-rw-rw-   0        0        0     4900 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.min.css
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.358548 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/
--rw-rw-rw-   0        0        0      738 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-article.scss
--rw-rw-rw-   0        0        0      381 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-bs-overrides.scss
--rw-rw-rw-   0        0        0      168 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-gallery.scss
--rw-rw-rw-   0        0        0      480 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-hero.scss
--rw-rw-rw-   0        0        0     1897 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-location.scss
--rw-rw-rw-   0        0        0     2202 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-navbar.scss
--rw-rw-rw-   0        0        0      908 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-pricelist.scss
--rw-rw-rw-   0        0        0      256 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-richtext.scss
--rw-rw-rw-   0        0        0      650 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/codered-front.scss
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.330134 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.358548 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/
--rw-rw-rw-   0        0        0     1131 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/LICENSE
--rw-rw-rw-   0        0        0      130 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/README.txt
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.327888 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.365792 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/
--rw-rw-rw-   0        0        0    67472 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   163856 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    50636 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   115091 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0     4784 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0    78154 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     3922 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    33156 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0   200387 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
--rw-rw-rw-   0        0        0   515619 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   162264 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   654593 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.373078 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/
--rw-rw-rw-   0        0        0   230599 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   426918 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    83376 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   308871 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   137714 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
--rw-rw-rw-   0        0        0   271784 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    62563 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   185257 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.328691 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.378207 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/
--rw-rw-rw-   0        0        0     3189 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/alert.js
--rw-rw-rw-   0        0        0     5730 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/button.js
--rw-rw-rw-   0        0        0    15927 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/carousel.js
--rw-rw-rw-   0        0        0     9721 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/collapse.js
--rw-rw-rw-   0        0        0    14056 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
--rw-rw-rw-   0        0        0    16934 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/modal.js
--rw-rw-rw-   0        0        0     3815 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/popover.js
--rw-rw-rw-   0        0        0     8160 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
--rw-rw-rw-   0        0        0     6171 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tab.js
--rw-rw-rw-   0        0        0     4718 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/toast.js
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.378207 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/
--rw-rw-rw-   0        0        0     3420 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js
--rw-rw-rw-   0        0        0    18232 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
--rw-rw-rw-   0        0        0     5071 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/util.js
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.394555 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/
--rw-rw-rw-   0        0        0     1164 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_alert.scss
--rw-rw-rw-   0        0        0     1121 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_badge.scss
--rw-rw-rw-   0        0        0     1326 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3626 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
--rw-rw-rw-   0        0        0     2685 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
--rw-rw-rw-   0        0        0     5940 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_card.scss
--rw-rw-rw-   0        0        0     4843 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
--rw-rw-rw-   0        0        0      940 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_close.scss
--rw-rw-rw-   0        0        0     1012 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_code.scss
--rw-rw-rw-   0        0        0    15700 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_custom-forms.scss
--rw-rw-rw-   0        0        0     4436 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
--rw-rw-rw-   0        0        0     9246 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_forms.scss
--rw-rw-rw-   0        0        0     5391 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_functions.scss
--rw-rw-rw-   0        0        0     1745 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_grid.scss
--rw-rw-rw-   0        0        0     1158 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_images.scss
--rw-rw-rw-   0        0        0     6521 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_input-group.scss
--rw-rw-rw-   0        0        0      406 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_jumbotron.scss
--rw-rw-rw-   0        0        0     3870 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
--rw-rw-rw-   0        0        0       83 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_media.scss
--rw-rw-rw-   0        0        0     1050 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
--rw-rw-rw-   0        0        0     6310 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_modal.scss
--rw-rw-rw-   0        0        0     2344 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_nav.scss
--rw-rw-rw-   0        0        0     7529 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
--rw-rw-rw-   0        0        0     1823 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
--rw-rw-rw-   0        0        0     4720 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_popover.scss
--rw-rw-rw-   0        0        0     2838 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_print.scss
--rw-rw-rw-   0        0        0     1171 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_progress.scss
--rw-rw-rw-   0        0        0    11539 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
--rw-rw-rw-   0        0        0      572 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_root.scss
--rw-rw-rw-   0        0        0     1287 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
--rw-rw-rw-   0        0        0     3544 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tables.scss
--rw-rw-rw-   0        0        0     1132 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
--rw-rw-rw-   0        0        0     2518 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
--rw-rw-rw-   0        0        0      363 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
--rw-rw-rw-   0        0        0     2222 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_type.scss
--rw-rw-rw-   0        0        0      536 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
--rw-rw-rw-   0        0        0    48615 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_variables.scss
--rw-rw-rw-   0        0        0      598 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
--rw-rw-rw-   0        0        0      409 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0      918 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.425966 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/
--rw-rw-rw-   0        0        0      242 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
--rw-rw-rw-   0        0        0      695 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_background-variant.scss
--rw-rw-rw-   0        0        0      320 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_badge.scss
--rw-rw-rw-   0        0        0     1828 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      532 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4482 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3525 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1422 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
--rw-rw-rw-   0        0        0       93 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      613 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0      392 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_float.scss
--rw-rw-rw-   0        0        0     5815 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
--rw-rw-rw-   0        0        0     2050 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     2089 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid-framework.scss
--rw-rw-rw-   0        0        0     2086 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
--rw-rw-rw-   0        0        0      757 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_hover.scss
--rw-rw-rw-   0        0        0     1155 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
--rw-rw-rw-   0        0        0      433 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      170 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
--rw-rw-rw-   0        0        0      369 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_nav-divider.scss
--rw-rw-rw-   0        0        0      462 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      481 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      202 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
--rw-rw-rw-   0        0        0      827 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_screen-reader.scss
--rw-rw-rw-   0        0        0      148 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_size.scss
--rw-rw-rw-   0        0        0      794 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_table-row.scss
--rw-rw-rw-   0        0        0      474 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-emphasis.scss
--rw-rw-rw-   0        0        0      326 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-hide.scss
--rw-rw-rw-   0        0        0      168 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      681 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
--rw-rw-rw-   0        0        0      189 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_visibility.scss
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.425966 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/
--rw-rw-rw-   0        0        0      420 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_align.scss
--rw-rw-rw-   0        0        0      409 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_background.scss
--rw-rw-rw-   0        0        0     1771 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_borders.scss
--rw-rw-rw-   0        0        0       37 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_clearfix.scss
--rw-rw-rw-   0        0        0      519 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_display.scss
--rw-rw-rw-   0        0        0      853 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_embed.scss
--rw-rw-rw-   0        0        0     2769 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_flex.scss
--rw-rw-rw-   0        0        0      376 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_float.scss
--rw-rw-rw-   0        0        0      142 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_interactions.scss
--rw-rw-rw-   0        0        0      133 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_overflow.scss
--rw-rw-rw-   0        0        0      484 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_position.scss
--rw-rw-rw-   0        0        0      115 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_screenreaders.scss
--rw-rw-rw-   0        0        0      249 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_shadows.scss
--rw-rw-rw-   0        0        0      498 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_sizing.scss
--rw-rw-rw-   0        0        0     2108 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_spacing.scss
--rw-rw-rw-   0        0        0      431 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_stretched-link.scss
--rw-rw-rw-   0        0        0     2106 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_text.scss
--rw-rw-rw-   0        0        0      174 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_visibility.scss
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.425966 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/
--rw-rw-rw-   0        0        0     7067 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.441860 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/
--rw-rw-rw-   0        0        0   287630 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.js
--rw-rw-rw-   0        0        0   137986 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.map
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.331029 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.331029 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.457848 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/
--rw-rw-rw-   0        0        0     1023 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/accordion_block.html
--rw-rw-rw-   0        0        0      805 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/article_block_card.html
--rw-rw-rw-   0        0        0      188 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/base_block.html
--rw-rw-rw-   0        0        0     2129 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/base_link_block.html
--rw-rw-rw-   0        0        0      651 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/button_block.html
--rw-rw-rw-   0        0        0      746 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_block.html
--rw-rw-rw-   0        0        0      856 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_blurb.html
--rw-rw-rw-   0        0        0      787 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_foot.html
--rw-rw-rw-   0        0        0      730 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head.html
--rw-rw-rw-   0        0        0      771 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head_foot.html
--rw-rw-rw-   0        0        0      786 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_img.html
--rw-rw-rw-   0        0        0      283 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_columns.html
--rw-rw-rw-   0        0        0      280 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_deck.html
--rw-rw-rw-   0        0        0      281 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_group.html
--rw-rw-rw-   0        0        0     2025 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/carousel_block.html
--rw-rw-rw-   0        0        0      401 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/column_block.html
--rw-rw-rw-   0        0        0      955 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/content_wall_block.html
--rw-rw-rw-   0        0        0      141 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/document_link_block.html
--rw-rw-rw-   0        0        0      925 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/download_block.html
--rw-rw-rw-   0        0        0      106 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/embed_video_block.html
--rw-rw-rw-   0        0        0       99 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/external_link_block.html
--rw-rw-rw-   0        0        0      723 2022-08-25 14:39:42.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/google_map.html
--rw-rw-rw-   0        0        0      383 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/grid_block.html
--rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/h1_block.html
--rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/h2_block.html
--rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/h3_block.html
--rw-rw-rw-   0        0        0      790 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/hero_block.html
--rw-rw-rw-   0        0        0      278 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/image_block.html
--rw-rw-rw-   0        0        0     1189 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/image_gallery_block.html
--rw-rw-rw-   0        0        0      632 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/image_link_block.html
--rw-rw-rw-   0        0        0     1028 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/modal_block.html
--rw-rw-rw-   0        0        0      168 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/page_link_block.html
--rw-rw-rw-   0        0        0      371 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_columns.html
--rw-rw-rw-   0        0        0      368 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_deck.html
--rw-rw-rw-   0        0        0      369 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_group.html
--rw-rw-rw-   0        0        0      960 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_media.html
--rw-rw-rw-   0        0        0      401 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_block.html
--rw-rw-rw-   0        0        0      614 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_list_group.html
--rw-rw-rw-   0        0        0      304 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_block.html
--rw-rw-rw-   0        0        0      793 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_card.html
--rw-rw-rw-   0        0        0     1171 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_form.html
--rw-rw-rw-   0        0        0      248 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pricelist_block.html
--rw-rw-rw-   0        0        0      509 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pricelistitem_block.html
--rw-rw-rw-   0        0        0      348 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/quote_block.html
--rw-rw-rw-   0        0        0      216 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/reusable_content_block.html
--rw-rw-rw-   0        0        0       89 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/rich_text_block.html
--rw-rw-rw-   0        0        0     1095 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/table_block.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.473479 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/
--rw-rw-rw-   0        0        0      267 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/date.html
--rw-rw-rw-   0        0        0      416 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/datetime.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.473479 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/
--rw-rw-rw-   0        0        0     6685 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
--rw-rw-rw-   0        0        0      793 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-rw-rw-   0        0        0      264 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/time.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.473479 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/
--rw-rw-rw-   0        0        0      465 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-align-left.svg
--rw-rw-rw-   0        0        0      573 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-check-square-o.svg
--rw-rw-rw-   0        0        0      277 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-columns.svg
--rw-rw-rw-   0        0        0      359 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-desktop.svg
--rw-rw-rw-   0        0        0      571 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-font.svg
--rw-rw-rw-   0        0        0      292 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-google.svg
--rw-rw-rw-   0        0        0      813 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hand-pointer-o.svg
--rw-rw-rw-   0        0        0      666 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hashtag.svg
--rw-rw-rw-   0        0        0      840 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-header.svg
--rw-rw-rw-   0        0        0      835 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-list-alt.svg
--rw-rw-rw-   0        0        0      459 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-map.svg
--rw-rw-rw-   0        0        0      448 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-newspaper-o.svg
--rw-rw-rw-   0        0        0      721 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-puzzle-piece.svg
--rw-rw-rw-   0        0        0      635 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-recycle.svg
--rw-rw-rw-   0        0        0      174 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-stop.svg
--rw-rw-rw-   0        0        0      505 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-th-large.svg
--rw-rw-rw-   0        0        0      762 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-universal-access.svg
--rw-rw-rw-   0        0        0      548 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-usd.svg
--rw-rw-rw-   0        0        0      225 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-window-maximize.svg
--rw-rw-rw-   0        0        0      199 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-window-minimize.svg
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.489128 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/
--rw-rw-rw-   0        0        0      689 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_dropdowns.html
--rw-rw-rw-   0        0        0      579 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_nav.html
--rw-rw-rw-   0        0        0      265 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/form_honeypot.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.489128 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/
--rw-rw-rw-   0        0        0      485 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/calendar.html
--rw-rw-rw-   0        0        0      379 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/calendar_ical_button.html
--rw-rw-rw-   0        0        0      414 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/recurring_ical_button.html
--rw-rw-rw-   0        0        0      588 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/single_ical_button.html
--rw-rw-rw-   0        0        0      353 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/iframe_gmap.html
--rw-rw-rw-   0        0        0      340 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/map_list_description.html
--rw-rw-rw-   0        0        0      107 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/map_pin_description.html
--rw-rw-rw-   0        0        0     1065 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/pagination.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.489128 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/
--rw-rw-rw-   0        0        0      525 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/render_field.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.505075 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0     2018 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_index_page.html
--rw-rw-rw-   0        0        0     1547 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.html
--rw-rw-rw-   0        0        0     1019 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.search.html
--rw-rw-rw-   0        0        0     9340 2022-08-25 14:40:47.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/base.html
--rw-rw-rw-   0        0        0     1769 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/event_index_page.html
--rw-rw-rw-   0        0        0     2307 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/event_page.html
--rw-rw-rw-   0        0        0     1111 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/form_page.html
--rw-rw-rw-   0        0        0      252 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/form_page_landing.html
--rw-rw-rw-   0        0        0       55 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/home_page.html
--rw-rw-rw-   0        0        0     1563 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/location_index_page.html
--rw-rw-rw-   0        0        0     1058 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/location_page.html
--rw-rw-rw-   0        0        0     2614 2022-08-25 14:41:03.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/search.html
--rw-rw-rw-   0        0        0      424 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/search_result.html
--rw-rw-rw-   0        0        0     2462 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/stream_form_page.html
--rw-rw-rw-   0        0        0      532 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/web_page.html
--rw-rw-rw-   0        0        0      639 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/web_page_notitle.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.505075 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/snippets/
--rw-rw-rw-   0        0        0      490 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/snippets/footer.html
--rw-rw-rw-   0        0        0     2318 2022-08-25 14:41:09.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/snippets/navbar.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.505075 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/widgets/
--rw-rw-rw-   0        0        0     1316 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/widgets/checkbox_classifiers.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.505075 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailcore/
--rw-rw-rw-   0        0        0      852 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailcore/password_required.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.505075 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailembeds/
--rw-rw-rw-   0        0        0      681 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailembeds/embed_frontend.html
-drwxrwxrwx   0        0        0        0 2022-08-25 14:46:04.346159 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/
--rw-rw-rw-   0        0        0     1979 2022-08-25 14:46:04.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18818 2022-08-25 14:46:04.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-25 14:46:04.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-08-25 14:46:04.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-08-25 14:46:04.000000 coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-25 14:46:04.510232 coderedcms-bootstrap4-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      991 2022-08-25 14:43:27.000000 coderedcms-bootstrap4-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.819223 coderedcms-bootstrap4-1.0.2/
+-rw-rw-rw-   0        0        0     1548 2022-08-08 18:10:37.000000 coderedcms-bootstrap4-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      105 2022-08-08 18:10:37.000000 coderedcms-bootstrap4-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-04-24 15:23:02.819223 coderedcms-bootstrap4-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2022-08-08 18:32:41.000000 coderedcms-bootstrap4-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.628015 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.624027 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.625025 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.641296 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/
+-rw-rw-rw-   0        0        0     5972 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css
+-rw-rw-rw-   0        0        0     5962 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css.map
+-rw-rw-rw-   0        0        0     4900 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.min.css
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.645892 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/
+-rw-rw-rw-   0        0        0      738 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-article.scss
+-rw-rw-rw-   0        0        0      381 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-bs-overrides.scss
+-rw-rw-rw-   0        0        0      168 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-gallery.scss
+-rw-rw-rw-   0        0        0      480 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-hero.scss
+-rw-rw-rw-   0        0        0     1897 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-location.scss
+-rw-rw-rw-   0        0        0     2202 2022-08-08 18:10:38.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-navbar.scss
+-rw-rw-rw-   0        0        0      908 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-pricelist.scss
+-rw-rw-rw-   0        0        0      256 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-richtext.scss
+-rw-rw-rw-   0        0        0      650 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/codered-front.scss
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.628015 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.647926 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/
+-rw-rw-rw-   0        0        0     1131 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0      130 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.626017 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.661129 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/
+-rw-rw-rw-   0        0        0    67472 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   163856 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    50636 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   115091 2022-08-08 18:10:39.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0     4784 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0    78154 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     3922 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    33156 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0   200387 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
+-rw-rw-rw-   0        0        0   515619 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   162264 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   654593 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.672529 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/
+-rw-rw-rw-   0        0        0   230599 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   426918 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    83376 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   308871 2022-08-08 18:10:40.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   137714 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
+-rw-rw-rw-   0        0        0   271784 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    62563 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   185257 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.627016 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.683648 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/
+-rw-rw-rw-   0        0        0     3189 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/alert.js
+-rw-rw-rw-   0        0        0     5730 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/button.js
+-rw-rw-rw-   0        0        0    15927 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/carousel.js
+-rw-rw-rw-   0        0        0     9721 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/collapse.js
+-rw-rw-rw-   0        0        0    14056 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
+-rw-rw-rw-   0        0        0    16934 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/modal.js
+-rw-rw-rw-   0        0        0     3815 2022-08-08 18:10:41.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/popover.js
+-rw-rw-rw-   0        0        0     8160 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
+-rw-rw-rw-   0        0        0     6171 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tab.js
+-rw-rw-rw-   0        0        0     4718 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/toast.js
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.684652 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/
+-rw-rw-rw-   0        0        0     3420 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js
+-rw-rw-rw-   0        0        0    18232 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
+-rw-rw-rw-   0        0        0     5071 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/util.js
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.719116 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/
+-rw-rw-rw-   0        0        0     1164 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_alert.scss
+-rw-rw-rw-   0        0        0     1121 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_badge.scss
+-rw-rw-rw-   0        0        0     1326 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3626 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
+-rw-rw-rw-   0        0        0     2685 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
+-rw-rw-rw-   0        0        0     5940 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_card.scss
+-rw-rw-rw-   0        0        0     4843 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
+-rw-rw-rw-   0        0        0      940 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_close.scss
+-rw-rw-rw-   0        0        0     1012 2022-08-08 18:10:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_code.scss
+-rw-rw-rw-   0        0        0    15700 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_custom-forms.scss
+-rw-rw-rw-   0        0        0     4436 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
+-rw-rw-rw-   0        0        0     9246 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_forms.scss
+-rw-rw-rw-   0        0        0     5391 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_functions.scss
+-rw-rw-rw-   0        0        0     1745 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_grid.scss
+-rw-rw-rw-   0        0        0     1158 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_images.scss
+-rw-rw-rw-   0        0        0     6521 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_input-group.scss
+-rw-rw-rw-   0        0        0      406 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_jumbotron.scss
+-rw-rw-rw-   0        0        0     3870 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
+-rw-rw-rw-   0        0        0       83 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_media.scss
+-rw-rw-rw-   0        0        0     1050 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
+-rw-rw-rw-   0        0        0     6310 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_modal.scss
+-rw-rw-rw-   0        0        0     2344 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_nav.scss
+-rw-rw-rw-   0        0        0     7529 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
+-rw-rw-rw-   0        0        0     1823 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
+-rw-rw-rw-   0        0        0     4720 2022-08-08 18:10:43.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_popover.scss
+-rw-rw-rw-   0        0        0     2838 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_print.scss
+-rw-rw-rw-   0        0        0     1171 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_progress.scss
+-rw-rw-rw-   0        0        0    11539 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
+-rw-rw-rw-   0        0        0      572 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_root.scss
+-rw-rw-rw-   0        0        0     1287 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
+-rw-rw-rw-   0        0        0     3544 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tables.scss
+-rw-rw-rw-   0        0        0     1132 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
+-rw-rw-rw-   0        0        0     2518 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
+-rw-rw-rw-   0        0        0      363 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
+-rw-rw-rw-   0        0        0     2222 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_type.scss
+-rw-rw-rw-   0        0        0      536 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
+-rw-rw-rw-   0        0        0    48615 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_variables.scss
+-rw-rw-rw-   0        0        0      598 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0      409 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0      918 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.742651 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/
+-rw-rw-rw-   0        0        0      242 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      695 2022-08-08 18:10:44.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_background-variant.scss
+-rw-rw-rw-   0        0        0      320 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_badge.scss
+-rw-rw-rw-   0        0        0     1828 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      532 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4482 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3525 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1422 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
+-rw-rw-rw-   0        0        0       93 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      613 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0      392 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_float.scss
+-rw-rw-rw-   0        0        0     5815 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     2050 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     2089 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid-framework.scss
+-rw-rw-rw-   0        0        0     2086 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      757 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_hover.scss
+-rw-rw-rw-   0        0        0     1155 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
+-rw-rw-rw-   0        0        0      433 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      170 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      369 2022-08-08 18:10:45.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_nav-divider.scss
+-rw-rw-rw-   0        0        0      462 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      481 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      202 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
+-rw-rw-rw-   0        0        0      827 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_screen-reader.scss
+-rw-rw-rw-   0        0        0      148 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_size.scss
+-rw-rw-rw-   0        0        0      794 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_table-row.scss
+-rw-rw-rw-   0        0        0      474 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-emphasis.scss
+-rw-rw-rw-   0        0        0      326 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-hide.scss
+-rw-rw-rw-   0        0        0      168 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      681 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
+-rw-rw-rw-   0        0        0      189 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_visibility.scss
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.755662 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/
+-rw-rw-rw-   0        0        0      420 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_align.scss
+-rw-rw-rw-   0        0        0      409 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_background.scss
+-rw-rw-rw-   0        0        0     1771 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_borders.scss
+-rw-rw-rw-   0        0        0       37 2022-08-08 18:10:46.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_clearfix.scss
+-rw-rw-rw-   0        0        0      519 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_display.scss
+-rw-rw-rw-   0        0        0      853 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_embed.scss
+-rw-rw-rw-   0        0        0     2769 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_flex.scss
+-rw-rw-rw-   0        0        0      376 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_float.scss
+-rw-rw-rw-   0        0        0      142 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_interactions.scss
+-rw-rw-rw-   0        0        0      133 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_overflow.scss
+-rw-rw-rw-   0        0        0      484 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_position.scss
+-rw-rw-rw-   0        0        0      115 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_screenreaders.scss
+-rw-rw-rw-   0        0        0      249 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_shadows.scss
+-rw-rw-rw-   0        0        0      498 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_sizing.scss
+-rw-rw-rw-   0        0        0     2108 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_spacing.scss
+-rw-rw-rw-   0        0        0      431 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_stretched-link.scss
+-rw-rw-rw-   0        0        0     2106 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_text.scss
+-rw-rw-rw-   0        0        0      174 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_visibility.scss
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.756660 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/
+-rw-rw-rw-   0        0        0     7067 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.759912 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/
+-rw-rw-rw-   0        0        0   287630 2022-08-08 18:10:47.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.js
+-rw-rw-rw-   0        0        0   137986 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.map
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.632272 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.631785 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.786493 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/
+-rw-rw-rw-   0        0        0     1023 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/accordion_block.html
+-rw-rw-rw-   0        0        0      805 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/article_block_card.html
+-rw-rw-rw-   0        0        0      188 2022-08-08 18:10:48.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/base_block.html
+-rw-rw-rw-   0        0        0     2129 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/base_link_block.html
+-rw-rw-rw-   0        0        0      651 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/button_block.html
+-rw-rw-rw-   0        0        0      746 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_block.html
+-rw-rw-rw-   0        0        0      856 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_blurb.html
+-rw-rw-rw-   0        0        0      787 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_foot.html
+-rw-rw-rw-   0        0        0      730 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head.html
+-rw-rw-rw-   0        0        0      771 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head_foot.html
+-rw-rw-rw-   0        0        0      786 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_img.html
+-rw-rw-rw-   0        0        0      283 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_columns.html
+-rw-rw-rw-   0        0        0      280 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_deck.html
+-rw-rw-rw-   0        0        0      281 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/cardgrid_group.html
+-rw-rw-rw-   0        0        0     2025 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/carousel_block.html
+-rw-rw-rw-   0        0        0      401 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/column_block.html
+-rw-rw-rw-   0        0        0      955 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/content_wall_block.html
+-rw-rw-rw-   0        0        0      141 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/document_link_block.html
+-rw-rw-rw-   0        0        0      925 2022-08-08 18:10:49.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/download_block.html
+-rw-rw-rw-   0        0        0      106 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/embed_video_block.html
+-rw-rw-rw-   0        0        0       99 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/external_link_block.html
+-rw-rw-rw-   0        0        0      723 2022-08-25 14:39:42.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/google_map.html
+-rw-rw-rw-   0        0        0      383 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/grid_block.html
+-rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/h1_block.html
+-rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/h2_block.html
+-rw-rw-rw-   0        0        0      200 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/h3_block.html
+-rw-rw-rw-   0        0        0      790 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/hero_block.html
+-rw-rw-rw-   0        0        0      278 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/image_block.html
+-rw-rw-rw-   0        0        0     1189 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/image_gallery_block.html
+-rw-rw-rw-   0        0        0      632 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/image_link_block.html
+-rw-rw-rw-   0        0        0     1028 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/modal_block.html
+-rw-rw-rw-   0        0        0      168 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/page_link_block.html
+-rw-rw-rw-   0        0        0      371 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_columns.html
+-rw-rw-rw-   0        0        0      368 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_deck.html
+-rw-rw-rw-   0        0        0      369 2022-08-08 18:10:50.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_card_group.html
+-rw-rw-rw-   0        0        0      960 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_media.html
+-rw-rw-rw-   0        0        0      401 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_block.html
+-rw-rw-rw-   0        0        0      614 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_list_group.html
+-rw-rw-rw-   0        0        0      304 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_block.html
+-rw-rw-rw-   0        0        0      793 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_card.html
+-rw-rw-rw-   0        0        0     1171 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_form.html
+-rw-rw-rw-   0        0        0      248 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pricelist_block.html
+-rw-rw-rw-   0        0        0      509 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pricelistitem_block.html
+-rw-rw-rw-   0        0        0      348 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/quote_block.html
+-rw-rw-rw-   0        0        0      216 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/reusable_content_block.html
+-rw-rw-rw-   0        0        0       89 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/rich_text_block.html
+-rw-rw-rw-   0        0        0     1095 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/table_block.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.788561 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/
+-rw-rw-rw-   0        0        0      267 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/date.html
+-rw-rw-rw-   0        0        0      416 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/datetime.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.789565 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/
+-rw-rw-rw-   0        0        0     6685 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-rw-rw-   0        0        0      793 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-rw-rw-   0        0        0      264 2022-08-08 18:10:51.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/time.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.800165 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/
+-rw-rw-rw-   0        0        0      465 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-align-left.svg
+-rw-rw-rw-   0        0        0      573 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-check-square-o.svg
+-rw-rw-rw-   0        0        0      277 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-columns.svg
+-rw-rw-rw-   0        0        0      359 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-desktop.svg
+-rw-rw-rw-   0        0        0      571 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-font.svg
+-rw-rw-rw-   0        0        0      292 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-google.svg
+-rw-rw-rw-   0        0        0      813 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hand-pointer-o.svg
+-rw-rw-rw-   0        0        0      666 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hashtag.svg
+-rw-rw-rw-   0        0        0      840 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-header.svg
+-rw-rw-rw-   0        0        0      835 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-list-alt.svg
+-rw-rw-rw-   0        0        0      459 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-map.svg
+-rw-rw-rw-   0        0        0      448 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-newspaper-o.svg
+-rw-rw-rw-   0        0        0      721 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-puzzle-piece.svg
+-rw-rw-rw-   0        0        0      635 2022-08-08 18:10:52.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-recycle.svg
+-rw-rw-rw-   0        0        0      174 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-stop.svg
+-rw-rw-rw-   0        0        0      505 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-th-large.svg
+-rw-rw-rw-   0        0        0      762 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-universal-access.svg
+-rw-rw-rw-   0        0        0      548 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-usd.svg
+-rw-rw-rw-   0        0        0      225 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-window-maximize.svg
+-rw-rw-rw-   0        0        0      199 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-window-minimize.svg
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.804335 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/
+-rw-rw-rw-   0        0        0      689 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_dropdowns.html
+-rw-rw-rw-   0        0        0      579 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_nav.html
+-rw-rw-rw-   0        0        0      265 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/form_honeypot.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.807061 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/
+-rw-rw-rw-   0        0        0      485 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/calendar.html
+-rw-rw-rw-   0        0        0      379 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/calendar_ical_button.html
+-rw-rw-rw-   0        0        0      414 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/recurring_ical_button.html
+-rw-rw-rw-   0        0        0      588 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/single_ical_button.html
+-rw-rw-rw-   0        0        0      353 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/iframe_gmap.html
+-rw-rw-rw-   0        0        0      340 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/map_list_description.html
+-rw-rw-rw-   0        0        0      107 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/map_pin_description.html
+-rw-rw-rw-   0        0        0     1065 2022-08-08 18:10:53.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/pagination.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.808065 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/
+-rw-rw-rw-   0        0        0      525 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/render_field.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.816015 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0     2018 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_index_page.html
+-rw-rw-rw-   0        0        0     1547 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.html
+-rw-rw-rw-   0        0        0     1019 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.search.html
+-rw-rw-rw-   0        0        0     9168 2023-04-24 15:19:18.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/base.html
+-rw-rw-rw-   0        0        0     1769 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/event_index_page.html
+-rw-rw-rw-   0        0        0     2307 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/event_page.html
+-rw-rw-rw-   0        0        0     1111 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/form_page.html
+-rw-rw-rw-   0        0        0      252 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/form_page_landing.html
+-rw-rw-rw-   0        0        0       55 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/home_page.html
+-rw-rw-rw-   0        0        0     1563 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/location_index_page.html
+-rw-rw-rw-   0        0        0     1058 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/location_page.html
+-rw-rw-rw-   0        0        0     2614 2022-08-25 14:41:03.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/search.html
+-rw-rw-rw-   0        0        0      424 2022-08-08 18:10:54.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/search_result.html
+-rw-rw-rw-   0        0        0     2462 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/stream_form_page.html
+-rw-rw-rw-   0        0        0      532 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/web_page.html
+-rw-rw-rw-   0        0        0      639 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/web_page_notitle.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.817015 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/snippets/
+-rw-rw-rw-   0        0        0      490 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/snippets/footer.html
+-rw-rw-rw-   0        0        0     2318 2022-08-25 14:41:09.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/snippets/navbar.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.817015 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/widgets/
+-rw-rw-rw-   0        0        0     1316 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/widgets/checkbox_classifiers.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.818210 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailcore/
+-rw-rw-rw-   0        0        0      852 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailcore/password_required.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.818210 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailembeds/
+-rw-rw-rw-   0        0        0      681 2022-08-08 18:10:55.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailembeds/embed_frontend.html
+drwxrwxrwx   0        0        0        0 2023-04-24 15:23:02.638085 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-04-24 15:23:02.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18818 2023-04-24 15:23:02.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:23:02.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-24 15:23:02.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-24 15:23:02.000000 coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:23:02.819223 coderedcms-bootstrap4-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-04-24 15:21:06.000000 coderedcms-bootstrap4-1.0.2/setup.py
```

### Comparing `coderedcms-bootstrap4-1.0.1/LICENSE` & `coderedcms-bootstrap4-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/PKG-INFO` & `coderedcms-bootstrap4-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coderedcms-bootstrap4
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bootstrap 4 compatibility theme for Wagtail CRX.
 Home-page: https://github.com/coderedcorp/coderedcms-bootstrap4
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD license
-Platform: UNKNOWN
 Classifier: Framework :: Wagtail
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -53,9 +52,7 @@
 That's it! Continue to extend templates or import static files as usual from
 `coderedcms` and you will instead be getting the Bootstrap 4 versions from this
 theme.
 
 NOTE: This theme will be maintained with necessary bug fixes, but will not
 receive any new designs or new features. It is recommended to eventually upgrade
 your sites to Bootstrap 5.
-
-
```

### Comparing `coderedcms-bootstrap4-1.0.1/README.md` & `coderedcms-bootstrap4-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/css/codered-front.min.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/css/codered-front.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-article.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-article.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-location.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-location.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-navbar.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/_codered-pricelist.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/_codered-pricelist.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/scss/codered-front.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/scss/codered-front.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/LICENSE` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/alert.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/button.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/carousel.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/collapse.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/dropdown.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/modal.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/popover.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tab.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/toast.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tools/sanitizer.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tooltip.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/util.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/js/src/util.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_alert.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_badge.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_button-group.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_buttons.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_card.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_carousel.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_close.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_code.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_code.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_custom-forms.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_forms.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_forms.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_functions.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_grid.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_images.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_input-group.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_input-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_list-group.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_mixins.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_modal.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_nav.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_navbar.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_pagination.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_popover.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_print.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_print.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_progress.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_reboot.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_root.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_spinners.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tables.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_toasts.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_type.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_utilities.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_variables.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_background-variant.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_background-variant.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid-framework.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_hover.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_screen-reader.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_table-row.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_borders.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_display.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_embed.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_flex.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_spacing.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_text.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.js` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.map` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/static/coderedcms/vendor/jquery/jquery-3.5.1.min.map`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/accordion_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/article_block_card.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/base_link_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/button_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_blurb.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_foot.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head_foot.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/card_img.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/carousel_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/content_wall_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/content_wall_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/download_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/google_map.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/google_map.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/hero_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/image_gallery_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/image_link_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/modal_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_media.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_list_group.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_card.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_form.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/blocks/table_block.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-check-square-o.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-check-square-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-font.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-font.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hand-pointer-o.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hashtag.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-hashtag.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-header.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-header.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-list-alt.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-list-alt.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-puzzle-piece.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-recycle.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-recycle.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-universal-access.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-universal-access.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/icons/cr-usd.svg` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/icons/cr-usd.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_dropdowns.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_nav.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/ical/single_ical_button.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/ical/single_ical_button.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/pagination.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/render_field.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_index_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.search.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/base.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,14 @@
     <body class="coderedcms-{{page.content_type.model}} {% if page.get_parent %}parent-page-{{page.get_parent.id}}{% endif %} {% block body_class %}{% endblock %}" id="page-{{page.id}}">
 
         {% include "coderedcms/includes/crx_banner.html" %}
 
         {% wagtailuserbar %}
 
         {% block ada_skip %}
-            {% if settings.coderedcms.ADASettings.skip_navigation %}
-                <a href='#content' title='Skip Navigation'>Skip Navigation</a>
-            {% endif %}
         {% endblock %}
 
         {% block navbar %}{% endblock %}
 
         <div id="content">
             {% block content %}
                 {% block messages %}
```

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/event_index_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/event_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/event_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/event_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/form_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/location_index_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/location_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/location_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/location_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/search.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/stream_form_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/web_page.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/pages/web_page_notitle.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/pages/web_page_notitle.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/snippets/navbar.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/coderedcms/widgets/checkbox_classifiers.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/coderedcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailcore/password_required.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailcore/password_required.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4/templates/wagtailembeds/embed_frontend.html` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4/templates/wagtailembeds/embed_frontend.html`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/PKG-INFO` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coderedcms-bootstrap4
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bootstrap 4 compatibility theme for Wagtail CRX.
 Home-page: https://github.com/coderedcorp/coderedcms-bootstrap4
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD license
-Platform: UNKNOWN
 Classifier: Framework :: Wagtail
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -53,9 +52,7 @@
 That's it! Continue to extend templates or import static files as usual from
 `coderedcms` and you will instead be getting the Bootstrap 4 versions from this
 theme.
 
 NOTE: This theme will be maintained with necessary bug fixes, but will not
 receive any new designs or new features. It is recommended to eventually upgrade
 your sites to Bootstrap 5.
-
-
```

### Comparing `coderedcms-bootstrap4-1.0.1/coderedcms_bootstrap4.egg-info/SOURCES.txt` & `coderedcms-bootstrap4-1.0.2/coderedcms_bootstrap4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderedcms-bootstrap4-1.0.1/setup.py` & `coderedcms-bootstrap4-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="coderedcms-bootstrap4",
-    version="1.0.1",
+    version="1.0.2",
     author="CodeRed LLC",
     author_email="info@coderedcorp.com",
     url="https://github.com/coderedcorp/coderedcms-bootstrap4",
     description="Bootstrap 4 compatibility theme for Wagtail CRX.",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="BSD license",
```


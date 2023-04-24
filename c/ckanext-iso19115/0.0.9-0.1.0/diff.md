# Comparing `tmp/ckanext-iso19115-0.0.9.tar.gz` & `tmp/ckanext-iso19115-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-iso19115-0.0.9.tar", last modified: Thu Jan 27 15:08:08 2022, max compression
+gzip compressed data, was "ckanext-iso19115-0.1.0.tar", last modified: Mon Apr 24 12:37:36 2023, max compression
```

## Comparing `ckanext-iso19115-0.0.9.tar` & `ckanext-iso19115-0.1.0.tar`

### file list

```diff
@@ -1,518 +1,520 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.205281 ckanext-iso19115-0.0.9/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-01-10 12:30:17.000000 ckanext-iso19115-0.0.9/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      213 2022-01-14 14:57:34.000000 ckanext-iso19115-0.0.9/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4020 2022-01-27 15:08:08.205281 ckanext-iso19115-0.0.9/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3336 2022-01-10 12:30:17.000000 ckanext-iso19115-0.0.9/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.961948 ckanext-iso19115-0.0.9/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-01-13 16:18:52.000000 ckanext-iso19115-0.0.9/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.965281 ckanext-iso19115-0.0.9/ckanext/iso19115/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-01-10 12:30:17.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.978614 ckanext-iso19115-0.0.9/ckanext/iso19115/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1558 2022-01-25 11:52:48.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2022-01-24 16:31:30.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      295 2022-01-24 16:30:08.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17712 2022-01-25 14:19:08.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/builder.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2712 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/cli.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.981948 ckanext-iso19115-0.0.9/ckanext/iso19115/converter/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8470 2022-01-27 14:57:12.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/converter/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/converter/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      473 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/formatter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1470 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      240 2022-01-21 14:55:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.981948 ckanext-iso19115-0.0.9/ckanext/iso19115/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-01-19 17:34:43.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1291 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/logic/action.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/fcc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.985281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/fcc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2125 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      386 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/fcc/1.0/fcc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.995281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22662 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    36680 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1105 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.011948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    23194 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11876 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1673 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7268 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.021948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1094 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3176 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2504 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7990 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1908 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.031948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      568 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2628 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3120 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24147 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.051948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      536 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      985 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24458 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2018-03-06 00:32:36.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.061948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    28570 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.065281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5292 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2676 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.068614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11689 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1515 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6015 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gml/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.068614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-01-10 17:45:18.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.071948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7647 2022-01-11 09:43:54.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1647 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.071948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      830 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.075281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    27705 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      529 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.078614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    31317 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6197 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8729 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      565 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.078614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3484 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.945281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.085281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15388 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    47074 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10279 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      773 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.088614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    27250 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9857 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      772 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5163 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.091948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1208 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/metadataWExtendedType.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.095281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3697 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/metadataWExtendedType.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.095281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7315 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2089 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/metadataWithExtensions.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.098614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7719 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2115 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/metadataWithExtensions.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.098614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    16887 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8053 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.101948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18555 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      818 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8063 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.101948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6129 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1657 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3984 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3130 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6840 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.105281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2588 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1932 2022-01-20 11:26:28.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6851 2022-01-11 10:36:06.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.105281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    35846 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5968 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/metadataDataServices.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.108614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7331 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/metadataDataServices.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.111948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4362 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1215 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5481 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.111948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2018-03-06 00:32:36.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4662 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5495 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.115281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19498 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7911 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5078 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5550 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.115281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15443 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4323 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      785 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2053 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.118614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1888 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.118614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21458 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8503 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2672 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.121948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2018-03-06 00:32:36.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21654 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8883 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13672 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.121948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8415 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13524 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      804 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1144 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3690 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.125281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    63662 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    28519 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      966 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3542 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8115 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.128614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10412 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      816 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.128614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15790 2018-03-14 16:33:57.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11514 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      822 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.131948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34660 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      815 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2530 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.131948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18947 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5793 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.131948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3816 2018-03-06 19:14:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1085 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19216 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5797 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.135281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17869 2018-03-14 16:16:02.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14304 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      766 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3106 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3080 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.135281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/
--rw-r--r--   0 sergey    (1000) sergey    (1000)   343012 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.151948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1298 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5491 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3666 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7611 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1356 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9309 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1275 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4780 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1759 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3482 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5198 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2609 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2613 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3892 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5085 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4764 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2458 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2110 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5518 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13239 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6065 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8025 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2341 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9218 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3764 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1457 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1734 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1490 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1234 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2235 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1443 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1454 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1448 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1258 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1497 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1750 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2277 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1752 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1489 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.151948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    53123 2018-03-05 22:27:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/pre/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.151948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/pre/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1786 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/pre/1.0/pre.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.151948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1126 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    26600 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.155281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    44106 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    16835 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    97327 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3766 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.155281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      746 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3870 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      477 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/point.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2131 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4186 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.158614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1947 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.948614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.158614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6136 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8465 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      946 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3569 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14230 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.165281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4638 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24482 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8411 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3723 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6522 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6231 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1218 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2961 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3718 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.165281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12203 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.165281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2618 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1669 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.165281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.165281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    78922 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    78916 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17207 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      520 2018-03-05 22:27:11.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.178614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14905 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    33323 2022-01-11 09:41:58.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18420 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18701 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    20827 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15923 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34674 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7137 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4161 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6807 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5584 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11523 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18929 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6625 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5824 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    42649 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12756 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4132 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5530 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4680 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15598 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12679 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7795 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22790 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12283 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11438 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.181948 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22050 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1159 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4087 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.185281 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3188 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15521 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6555 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11423 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    30936 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11736 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11329 2022-01-11 09:43:05.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7160 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19751 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5983 2022-01-11 09:42:19.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9289 2022-01-11 09:42:32.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5877 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6429 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2664 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5723 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13883 2022-01-11 09:42:48.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.188614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1180 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2166 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.188614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2700 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.188614 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1173 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-01-10 17:47:45.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1499 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.191948 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2192 2022-01-13 12:48:44.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/cit.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3229 2022-01-13 12:44:12.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/dqm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3369 2022-01-13 11:55:16.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/gex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3915 2022-01-13 11:34:41.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mco.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5156 2022-01-18 17:12:00.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1464 2022-01-13 11:58:17.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mdq.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5063 2022-01-13 13:09:55.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1465 2022-01-13 11:41:05.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mmi.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2269 2022-01-13 13:12:26.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mrc.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1000 2022-01-13 11:56:19.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mrd.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9064 2022-01-24 15:55:04.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mri.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5740 2022-01-13 12:47:36.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/srv.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.191948 ckanext-iso19115-0.0.9/ckanext/iso19115/templates/iso19115/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      784 2022-01-24 16:30:40.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/templates/iso19115/validate.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.195281 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-01-10 12:30:17.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1012 2022-01-18 17:31:48.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.195281 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/converter/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-01-19 09:58:13.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/converter/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:07.951948 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.198614 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7062 2022-01-14 14:37:13.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/basic.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7740 2022-01-14 10:52:46.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/complex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3099 2022-01-13 10:25:26.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4689 2022-01-13 11:13:23.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3445 2022-01-13 11:08:08.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2059 2022-01-17 08:31:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/minimal.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2117 2022-01-12 15:20:13.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2445 2022-01-12 15:11:15.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2022-01-12 15:13:09.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_no_root.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2421 2022-01-12 15:19:36.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1751 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/test_converter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2022-01-12 14:27:12.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.201948 ckanext-iso19115-0.0.9/ckanext/iso19115/types/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      473 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2023 2022-01-24 14:27:37.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3833 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/cit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1169 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/gco.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      245 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/gcx.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1260 2022-01-24 09:03:44.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/gex.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10400 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/gml.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      546 2022-01-24 09:11:55.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/lan.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7528 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mac.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      566 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mas.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3748 2022-01-27 13:37:32.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mcc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      930 2022-01-24 09:11:25.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mco.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3102 2022-01-24 13:58:19.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mdb.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4763 2022-01-26 07:33:47.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mdq.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mex.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mmi.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      298 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mpc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1659 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2696 2022-01-24 13:08:42.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrd.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2050 2022-01-24 09:05:07.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mri.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1528 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrl.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      452 2022-01-24 09:41:51.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1614 2022-01-26 14:35:21.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/msr.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1304 2022-01-24 09:04:10.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/types/srv.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7874 2022-01-24 15:51:25.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1134 2022-01-18 17:31:48.000000 ckanext-iso19115-0.0.9/ckanext/iso19115/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-01-27 15:08:08.205281 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4020 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    23074 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       66 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       48 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-01-27 15:08:07.000000 ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       69 2022-01-13 16:18:47.000000 ckanext-iso19115-0.0.9/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-01-10 12:30:17.000000 ckanext-iso19115-0.0.9/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1643 2022-01-27 15:08:08.205281 ckanext-iso19115-0.0.9/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-01-10 12:35:41.000000 ckanext-iso19115-0.0.9/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      220 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3983 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3336 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1982 2023-04-20 14:35:28.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2022-10-20 16:05:53.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      313 2022-10-20 16:02:32.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17689 2023-04-20 15:10:15.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/builder.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2712 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      324 2023-04-24 12:36:18.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/config_declaration.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9306 2022-10-20 20:12:54.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      684 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/formatter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3844 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      240 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1387 2022-10-20 19:05:20.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/action.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2125 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      386 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/fcc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    36680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1105 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    23194 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11876 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1673 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7268 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1094 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3176 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2504 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7990 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1908 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      568 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2628 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3120 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24147 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      536 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      985 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    28570 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5292 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2676 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1515 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6015 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      830 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    27705 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      529 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    31317 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6197 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8729 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      565 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3484 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15388 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    47074 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10279 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      773 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    27250 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9857 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      772 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5163 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1208 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/metadataWExtendedType.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3697 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/metadataWExtendedType.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7315 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2089 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/metadataWithExtensions.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7719 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/metadataWithExtensions.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    16887 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      818 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1657 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3984 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2588 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1932 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6851 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    35846 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5968 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/metadataDataServices.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7331 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/metadataDataServices.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4362 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1215 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5481 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5495 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19498 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5078 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5550 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      785 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1888 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8503 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21654 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8415 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13524 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      804 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1144 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3690 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    63662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    28519 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      966 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3542 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10412 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11514 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      822 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34660 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      815 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5793 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19216 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5797 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17869 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14304 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3080 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)   343012 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1298 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5491 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3666 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7611 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1356 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9309 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1275 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4780 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1759 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5198 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2609 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2613 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3892 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2110 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5518 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13239 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6065 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8025 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2341 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1457 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1734 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1490 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1234 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2235 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1454 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1448 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1258 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1497 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1750 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2277 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1752 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1489 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    53123 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1786 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/pre.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1126 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    26600 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    44106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    16835 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    97327 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      746 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3870 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      477 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/point.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2131 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4186 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6136 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      946 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3569 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14230 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4638 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8411 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6522 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6231 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2961 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3718 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12203 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2618 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1669 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    78922 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    78916 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17207 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      520 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14905 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    33323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18420 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18701 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    20827 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15923 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34674 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7137 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4161 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6807 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5584 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11523 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18929 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6625 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5824 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    42649 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12756 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4132 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15598 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12679 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7795 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12283 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11438 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22050 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1159 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4087 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15521 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11423 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    30936 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11736 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11329 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7160 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5983 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9289 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5877 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6429 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2664 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1180 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2700 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1173 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1773 2023-03-01 20:48:28.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/presets.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2192 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/cit.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3229 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/dqm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3369 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/gex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3915 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mco.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5156 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1464 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdq.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mmi.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2269 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrc.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1000 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrd.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9064 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mri.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/srv.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      784 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/validate.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1012 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/converter/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/converter/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7062 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/basic.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/complex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3099 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2059 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/minimal.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2117 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_root.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2421 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_converter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/types/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      473 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2023 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3833 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/cit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gco.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      245 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gcx.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1367 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gex.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10400 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gml.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      546 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/lan.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7528 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mac.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      566 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mas.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3721 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mcc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      930 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mco.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3016 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdb.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4763 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdq.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mex.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mmi.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      298 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mpc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1763 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2696 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrd.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2236 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mri.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1528 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrl.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      452 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1532 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/msr.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1304 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/srv.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8286 2023-04-20 15:09:16.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1134 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3983 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    23163 2023-04-24 12:37:36.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       65 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       58 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 21:32:30.000000 ckanext-iso19115-0.1.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1654 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/setup.py
```

### Comparing `ckanext-iso19115-0.0.9/LICENSE` & `ckanext-iso19115-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/PKG-INFO` & `ckanext-iso19115-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ckanext-iso19115
-Version: 0.0.9
-Summary: UNKNOWN
+Version: 0.1.0
 Home-page: https://github.com/DataShades/ckanext-iso19115
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
@@ -137,9 +135,7 @@
 
        git tag 0.0.1
        git push --tags
 
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
-
-
```

### Comparing `ckanext-iso19115-0.0.9/README.md` & `ckanext-iso19115-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/assets/script.js` & `ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-script.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -9,50 +9,74 @@
 
         initialize: function() {
             $.proxyAll(this, /_on/);
             this.el.on("click", this._onClick);
         },
 
         _onClick: function() {
-            this.sandbox.client.call("GET", "iso19115_package_check", "?id=" + this.options.id, this._onSuccess, this._onError);
+            this.sandbox.client.call(
+                "GET",
+                "iso19115_package_check",
+                "?id=" + this.options.id,
+                this._onSuccess,
+                this._onError
+            );
         },
 
         _onSuccess: function() {
-            const target = this.options.target ? $(this.options.target) : this.sandbox.notify.el;
-            const msg = this.create("", "Dataset can be converted into valid ISO 19115 XML", "info");
+            const target = this.options.target ?
+                $(this.options.target) :
+                this.sandbox.notify.el;
+            const msg = this.create(
+                "",
+                "Dataset can be converted into valid ISO 19115 XML",
+                "info"
+            );
             this.report(msg, target);
-
         },
 
         _onError: function(err) {
-            const target = this.options.target ? $(this.options.target) : this.sandbox.notify.el;
+            const target = this.options.target ?
+                $(this.options.target) :
+                this.sandbox.notify.el;
             const errors = err.responseJSON.error;
             for (let type of Object.keys(errors)) {
                 if (type.slice(0, 2) === "__") {
                     continue;
                 }
-                const content = $.map(errors[type], function(text) {
-                    return $('<pre class="iso-validation-report">').append($("<code>", {
-                        text
-                    }));
+
+                let messages = errors[type];
+                if (type === "message") {
+                    messages = [messages];
+                }
+
+                const content = $.map(messages, function(text) {
+                    return $('<pre class="iso-validation-report">').append(
+                        $("<code>", {
+                            text
+                        })
+                    );
                 });
                 const msg = this.create(type, content, "error");
                 this.report(msg, target);
             }
         },
 
         report: function(msg, target) {
             target.append(msg.alert());
         },
 
         create: function(title, message, type) {
-            var alert = $('<div class="alert fade in"><strong></strong><a class="close" data-dismiss="alert">x</a></div>');
-            alert.addClass('alert-' + (type || 'error'));
-            alert.find('strong').text(title);
-
+            var alert = $(
+                '<div class="alert fade show alert-dismissible"><strong></strong></div>'
+            );
+            alert.addClass("alert-" + (type || "error"));
+            alert.find("strong").text(title);
 
             alert.append(message);
+            alert.append(
+                '<button type="button" class="btn-close" data-bs-dismiss="alert"></button>'
+            );
             return alert;
-
-        }
+        },
     };
 });
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/assets/style.css` & `ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-style.css`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/builder.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
         self.root = el
 
     def build(self, data):
         ns = {f"xmlns:{k}": v for k, v in utils.ns.items()}
         if len(data) < 2 or not isinstance(data[1], dict):
             data[1:1] = [{}]
-        # breakpoint()
         data[1].update(ns)
 
         el = self.root.encode(data, converter=xmlschema.JsonMLConverter)
         return el
 
     def example(
         self,
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/cli.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/converter/__init__.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/converter/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import dataclasses
 import contextlib
-from typing import Any
+from typing import Any, Iterable
 from typing_extensions import TypeAlias
 import ckan.plugins.toolkit as tk
 
 from ..types.base import JmlRecord
 from . import helpers as h
 
 from ..types import *
@@ -59,154 +59,178 @@
         ...
 
     def build(self):
         result = jml(self.data)
         return result
 
     def _add_identifier(self):
+        mcc.MD_Identifier
         identifier: mcc.MD_Identifier = h.id(
             self.pkg["id"], codeSpace="urn:uuid"
         )
         self.data.metadataIdentifier = identifier
 
     def _add_default_locale(self):
+        lan.PT_Locale
         locale = h.locale(
             self.pkg.get("language") or tk.config.get("ckan.locale_default")
         )
-        self.data.set_locale(locale)
+        self.data.defaultLocale = locale
 
     def _add_parent(self):
-        parent: cit.CI_Citation
+        cit.CI_Citation
         pass
 
     def _add_scope(self):
+        mdb.MD_MetadataScope
         scope: mdb.MD_MetadataScope = mdb.MD_MetadataScope(
             mcc.MD_ScopeCode("dataset"), h.cs("Dataset")
         )
 
         self.data.metadataScope.append(scope)
 
     def _add_contacts(self):
+        cit.CI_Responsibility
         for contact in self.pkg.get("contact", []):
 
             ind = cit.CI_Individual(
                 name=h.cs(contact.get("inidvidual")),
                 positionName=h.cs(contact.get("position")),
             )
             org = h.org(
                 contact.get("name"),
                 contactInfo=[
                     cit.CI_Contact(
                         phone=[h.phone(contact.get("phone"))],
-                        address=[
-                            h.address(email=h.cs(contact.get("email")))
-                        ],
+                        address=[h.address(email=h.cs(contact.get("email")))],
                     )
                 ],
                 individual=[ind],
             )
             resp = cit.CI_Responsibility(contact["role"], [org])
             self.data.add_contact(resp)
 
+        for contact in self._extra_contacts():
+            self.data.add_contact(contact)
+
+    def _extra_contacts(self) -> Iterable[cit.CI_Responsibility]:
+        return []
+
     def _add_dates(self):
-        has_creation = True
+        cit.CI_Date
+        has_creation = False
 
         for date in self.pkg.get("date_info", []):
             self.data.add_dateInfo(
                 cit.CI_Date(
                     h.date(date["date"]), cit.CI_DateTypeCode(date["type"])
                 )
             )
             if date["type"] == "creation":
                 has_creation = True
+
         if not has_creation:
             creation = self.pkg["metadata_created"]
+
             self.data.add_dateInfo(
-                cit.CI_Date(h.date(creation), cit.CI_DateTypeCode(creation))
+                cit.CI_Date(h.date(creation), cit.CI_DateTypeCode("creation"))
             )
 
     def _add_standard(self):
+        cit.CI_Citation
         standard: cit.CI_Citation = h.citation("ISO 19115", edition="2016")
         self.data.metadataStandard.append(standard)
 
     def _add_profile(self):
-        profile: cit.CI_Citation
+        cit.CI_Citation
         pass
 
     def _add_alternative_reference(self):
-        ref: cit.CI_Citation
+        cit.CI_Citation
         pass
 
     def _add_other_locale(self):
-        locale: lan.PT_Locale
+        lan.PT_Locale
         pass
 
     def _add_linkage(self):
-        link: cit.CI_OnlineResource
+        cit.CI_OnlineResource
         pass
 
     def _add_spatial_representation(self):
-        spatial: mcc.Abstract_SpatialRepresentation
-        pass
+        # mcc.Abstract_SpatialRepresentation
+        msr.MD_GridSpatialRepresentation
+        msr.MD_VectorSpatialRepresentation
+        for rep in self.pkg.get("vector_spatial_representation", []):
+            self.data.spatialRepresentationInfo.append(
+                msr.MD_VectorSpatialRepresentation(
+                    geometricObjects=msr.MD_GeometricObjects(
+                        msr.MD_GeometricObjectTypeCode(rep["type"]),
+                        gco.Integer(rep.get("count") or 0),
+                    )
+                )
+            )
 
     def _add_reference_system(self):
-        ref: mrs.MD_ReferenceSystem
+        mrs.MD_ReferenceSystem
         pass
 
     def _add_metadata_extension(self):
-        ext: mex.MD_MetadataExtensionInformation
+        mex.MD_MetadataExtensionInformation
         pass
 
     def _add_identification(self):
-        cit: cit.CI_Citation = h.citation(
+        mcc.Abstract_ResourceDescription
+        mri.MD_DataIdentification
+        srv.SV_ServiceIdentification
+
+        citation: cit.CI_Citation = h.citation(
             self.pkg["title"], identifier=h.id(self.pkg["id"])
         )
-        poc = self._make_user_contact("author", self.pkg["creator_user_id"])
-        kw = [h.keyword(t) for t in self.pkg["tags"]]
-
-        resources = []
-        for res in self.pkg["resources"]:
-            r_name = (
-                h.citation(res["name"], presentationForm="documentDigital")
-                if res["name"]
-                else None
-            )
-            resources.append(
-                mri.MD_AssociatedResource(
-                    r_name,
-                    mri.DS_AssociationTypeCode("isComposedOf"),
-                )
-            )
+        kw = [h.keyword(t if isinstance(t, str) else t['name']) for t in self.pkg["tags"]]
 
         ident: mri.MD_DataIdentification = mri.MD_DataIdentification(
-            cit,
+            citation,
             self.pkg["notes"],
-            pointOfContact=[poc] if poc else [],
             descriptiveKeywords=kw,
-            associatedResource=resources,
         )
-
         self.data.add_identificationInfo(ident)
 
-    def _add_content(self):
-        content: mcc.Abstract_ContentInformation
-        content: mrc.MD_FeatureCatalogueDescription
-        content: mrc.MD_CoverageDescription
-        content: mrc.MD_FeatureCatalogue
+        # for res in self.pkg["resources"]:
+        #     self.data.add_identificationInfo(
+        #         mri.MD_DataIdentification(
+        #             h.citation(
+        #                 res["name"], presentationForm="documentDigital"
+        #             ),
+        #             h.cs(res["description"]),
+        #             resourceFormat=[
+        #                 mrd.MD_Format(
+        #                     cit.CI_Citation(res["format"]),
+        #                     res.get("version"),
+        #                 )
+        #             ],
+        #         )
+        #     )
 
+    def _add_content(self):
+        # mcc.Abstract_ContentInformation
+        mrc.MD_FeatureCatalogueDescription
+        mrc.MD_CoverageDescription
+        mrc.MD_FeatureCatalogue
         pass
 
     def _add_distribution(self):
-        dist: mrd.MD_Distribution
+        mrd.MD_Distribution
         pass
 
     def _add_dq(self):
+        mdq.DQ_DataQuality
         for dq in self.pkg.get("data_quality", []):
             result = mdq.DQ_DescriptiveResult(
-                statement=h.cs(dq["details"] or "xx")
+                statement=h.cs(dq.get("details") or "...")
             )
             if "date" in dq:
                 result.dateTime = h.date(dq["date"], True)
 
             report: mdq.AbstractDQ_Element = h.make(
                 dq["type"], result=[result]
             )
@@ -215,35 +239,35 @@
                 mdq.DQ_DataQuality(
                     scope=mcc.MD_Scope(mcc.MD_ScopeCode("dataset")),
                     report=[report],
                 )
             )
 
     def _add_lineage(self):
-        ln: mrl.LI_Lineage
+        mrl.LI_Lineage
         pass
 
     def _add_catalogue(self):
-        catalogue: mpc.MD_PortrayalCatalogueReference
+        mpc.MD_PortrayalCatalogueReference
         pass
 
     def _add_constraints(self):
-        ctr: mco.MD_Constraints
+        mco.MD_Constraints
         pass
 
     def _add_schema(self):
-        schema: mas.MD_ApplicationSchemaInformation
+        mas.MD_ApplicationSchemaInformation
         pass
 
     def _add_maintenance(self):
-        maintenance: mmi.MD_MaintenanceInformation
+        mmi.MD_MaintenanceInformation
         pass
 
     def _add_acquisition(self):
-        acq: mac.MI_AcquisitionInformation
+        mac.MI_AcquisitionInformation
         pass
 
     def _make_user_contact(self, role: str, user_id: str):
         with contextlib.suppress(tk.NotAuthorized):
             author = tk.get_action("user_show")({}, {"id": user_id})
             return h.responsibility(
                 role, h.individual(author["fullname"] or author["name"])
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/converter/helpers.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/converter/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/logic/action.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/logic/action.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,10 +43,13 @@
     )
 
     pkg = tk.get_action("package_show")(context, data_dict)
     conv.initialize(pkg)
     conv.process()
     conv.finalize()
 
-    result = conv.build()
+    try:
+        result = conv.build()
+    except ValueError as e:
+        raise tk.ValidationError({"schema": [str(e)]})
 
     return result
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd` & `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/plugin.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,20 @@
     from ckanext.metaexport.interfaces import IMetaexport
 except ImportError:
     IMetaexport = None
 
 from . import cli, interfaces, views, helpers
 from .logic import action
 
+try:
+    config_declarations = tk.blanket.config_declarations
+except AttributeError:
+    config_declarations = lambda cls: cls
 
+@config_declarations
 class Iso19115Plugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IActions)
     plugins.implements(plugins.IClick)
     plugins.implements(plugins.IBlueprint)
     plugins.implements(plugins.IConfigurer)
     plugins.implements(plugins.ITemplateHelpers)
     plugins.implements(interfaces.IIso19115, inherit=True)
@@ -38,15 +43,20 @@
         tk.add_template_directory(config, "templates")
         tk.add_resource("assets", "iso19115")
 
     # IMetaexport
     def register_metaexport_format(self):
         from . import formatter
 
-        return dict(iso19115=formatter.Iso19115())
+        return dict(
+            iso19115=formatter.Iso19115(),
+            iso19115_html=formatter.Iso19115Html(),
+            iso19115_pdf=formatter.Iso19115Pdf(),
+
+        )
 
     def register_data_extractors(self, formatters):
         formatters.get("iso19115").set_data_extractor(_data_extractor)
 
     # ITemplateHelpers
     def get_helpers(self):
         return helpers.get_helpers()
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/cit.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/cit.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/dqm.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/dqm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/gex.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/gex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mco.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mco.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mdb.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mdq.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdq.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mex.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mmi.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mmi.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mrc.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrc.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mrd.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrd.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/mri.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mri.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/schematron/srv.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/srv.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/templates/iso19115/validate.html` & `ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/validate.html`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/conftest.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/basic.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/basic.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/complex.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/complex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/minimal.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/minimal.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/test_converter.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/tests/test_plugin.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/base.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/cit.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/cit.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/gco.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gco.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     value: str
 
 
 @dataclass
 class Real(Atomic):
     value: float
 
+@dataclass
+class Decimal(Atomic):
+    value: str
+
 
 @dataclass
 class Measure(Atomic):
     value: float
 
 
 @dataclass
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/gex.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gex.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if TYPE_CHECKING:
     from . import *
 
 
 @dataclass
 class EX_Extent:
-    description: Optional[str] = None
+    description: Optional[gco.CharacterString] = None
     geographicElement: list[AbstractEX_GeographicExtent] = field(
         default_factory=list
     )
     temporalElement: list[EX_TemporalExtent] = field(default_factory=list)
     verticalElement: list[EX_VerticalExtent] = field(default_factory=list)
 
 
@@ -28,26 +28,26 @@
 @dataclass
 class EX_TemporalExtent:
     extent: gml.AbstractTimePrimitive
 
 
 @dataclass
 class AbstractEX_GeographicExtent:
-    extentTypeCode: bool
+    extentTypeCode: Optional[gco.Boolean] = None
 
 
 @dataclass
 class EX_GeographicDescription(AbstractEX_GeographicExtent):
-    geographicIdentifier: mcc.MD_Identifier
+    geographicIdentifier: mcc.MD_Identifier = None
 
 
 @dataclass
 class EX_BoundingPolygon(AbstractEX_GeographicExtent):
     polygon: list[gml.AbstractGeometry] = field(default_factory=list)
 
 
 @dataclass
 class EX_GeographicBoundingBox(AbstractEX_GeographicExtent):
-    westBoundLongitude: str
-    eastBoundLongitude: str
-    southBoundLatitude: str
-    northBoundLatitude: str
+    westBoundLongitude: gco.Decimal = None
+    eastBoundLongitude: gco.Decimal = None
+    southBoundLatitude: gco.Decimal = None
+    northBoundLatitude: gco.Decimal = None
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/gml.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gml.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/lan.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/lan.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mac.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mac.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mas.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mas.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mcc.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mcc.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,14 @@
 
 @dataclass
 class MD_SpatialRepresentationTypeCode(Codelist):
     pass
 
 
 @dataclass
-class MD_TopicCategoryCode(Codelist):
-    pass
-
-
-@dataclass
 class Abstract_ResourceDescription:
     citation: cit.CI_Citation
     abstract: gco.CharacterString
     purpose: Optional[gco.CharacterString] = None
     credit: Optional[list[gco.CharacterString]] = field(default_factory=list)
     status: Optional[list[Codelist[mcc.MD_ProgressCode]]] = field(
         default_factory=list
@@ -90,15 +85,15 @@
     ] = field(default_factory=list)
     spatialResolution: Optional[list[mri.MD_Resolution]] = field(
         default_factory=list
     )
     temporalResolution: Optional[list[gco.TM_PeriodDuration]] = field(
         default_factory=list
     )
-    topicCategory: Optional[list[Codelist[mcc.MD_TopicCategoryCode]]] = field(
+    topicCategory: Optional[list[Codelist[mri.MD_TopicCategoryCode]]] = field(
         default_factory=list
     )
     extent: Optional[list[gex.EX_Extent]] = field(default_factory=list)
     additionalDocumentation: list[cit.CI_Citation] = field(
         default_factory=list
     )
     processingLevel: Optional[mcc.MD_Identifier] = None
@@ -121,15 +116,15 @@
     associatedResource: Optional[list[mri.MD_AssociatedResource]] = field(
         default_factory=list
     )
 
 
 @dataclass
 class Abstract_SpatialRepresentation:
-    ...
+    scope: Optional[mcc.MD_Scope] = None
     # |msr:MD_GridSpatialRepresentation [id, uuid] (too deep...)
     # |msr:MD_VectorSpatialRepresentation [id, uuid] (too deep...)
 
 
 @dataclass
 class Abstract_ContentInformation:
     ...
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mco.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mco.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mdb.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,10 +88,7 @@
         self.contact.append(contact)
 
     def add_identificationInfo(
         self,
         ident: Union[mri.MD_DataIdentification, srv.SV_ServiceIdentification],
     ):
         self.identificationInfo.append(ident)
-
-    def set_locale(self, locale: lan.PT_Locale):
-        self.defaultLocale = locale
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mdq.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdq.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mmi.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mmi.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrc.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Optional
 
 from .base import Codelist
 
-from . import gco
+from . import gco, mcc
 
 if TYPE_CHECKING:
     from . import *
 
 
 @dataclass
 class MD_CoverageContentTypeCode(Codelist):
@@ -35,31 +35,31 @@
     )
     attribute: Optional[list[mrc.MD_RangeDimension]] = field(
         default_factory=list
     )
 
 
 @dataclass
-class MD_FeatureCatalogueDescription:
+class MD_FeatureCatalogueDescription(mcc.Abstract_ContentInformation):
     complianceCode: Optional[gco.Boolean] = None
     locale: Optional[list[lan.PT_Locale]] = field(default_factory=list)
     includedWithDataset: Optional[gco.Boolean] = None
     featureTypes: Optional[list[mrc.MD_FeatureTypeInfo]] = field(
         default_factory=list
     )
     featureCatalogueCitation: Optional[list[cit.CI_Citation]] = field(
         default_factory=list
     )
 
 
 @dataclass
-class MD_CoverageDescription:
+class MD_CoverageDescription(mcc.Abstract_ContentInformation):
     attributeDescription: gco.RecordType = None
     processingLevelCode: Optional[mcc.MD_Identifier] = None
     attributeGroup: Optional[list[mrc.MD_AttributeGroup]] = field(
         default_factory=list
     )
 
 
 @dataclass
-class MD_FeatureCatalogue:
+class MD_FeatureCatalogue(mcc.Abstract_ContentInformation):
     featureCatalogue: list[Any] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrd.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrd.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mri.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mri.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Optional
 
-from .base import Codelist
+from .base import Codelist, Atomic
 
 if TYPE_CHECKING:
     from . import *
 
 
 @dataclass
+class MD_TopicCategoryCode(Atomic):
+    value: str
+
+
+@dataclass
+class MD_RepresentativeFraction:
+    denominator: gco.Integer
+
+
+@dataclass
 class MD_Resolution:
-    ...
+    equivalentScale: MD_RepresentativeFraction
 
 
 @dataclass
 class MD_KeywordTypeCode(Codelist):
     pass
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/mrl.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrl.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/msr.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/msr.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,23 +43,21 @@
 class MD_GeometricObjects:
     geometricObjectType: Codelist[MD_GeometricObjectTypeCode]
     geometricObjectCount: Optional[gco.Integer] = None
 
 
 @dataclass
 class MD_GridSpatialRepresentation(mcc.Abstract_SpatialRepresentation):
-    scope: Optional[mcc.MD_Scope] = None
     numberOfDimensions: gco.Integer = gco.Integer(0)
     axisDimensionProperties: Optional[list[msr.MD_Dimension]] = field(
         default_factory=list
     )
     cellGeometry: Codelist[msr.MD_CellGeometryCode] = None
     transformationParameterAvailability: gco.Boolean = gco.Boolean(False)
 
 
 @dataclass
 class MD_VectorSpatialRepresentation(mcc.Abstract_SpatialRepresentation):
-    scope: Optional[mcc.MD_Scope] = None
     topologyLevel: Optional[Codelist[MD_TopologyLevelCode]] = None
     geometricObjects: Optional[list[MD_GeometricObjects]] = field(
         default_factory=list
     )
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/types/srv.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/types/srv.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/utils.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from __future__ import annotations
 
+import logging
 import functools
 import pickle
+import tempfile
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Container, Iterable, Optional, cast
 from xml.etree import ElementTree as xtree
 
 import ckan.plugins.toolkit as tk
 import xmlschema
 from lxml import etree as ltree
 from lxml import isoschematron
 
 from . import builder
 from .types.base import CodeListValue
 
+log = logging.getLogger(__name__)
+
+CONFIG_CACHE_DIR = "ckanext.iso19115.misc.cache_dir"
+
 DEFAULT_XSD = "mdb2"
 _root = Path(__file__).parent
+_tempdir = tempfile.mkdtemp(prefix="iso19115")
 
 _codelists = _root / "namespaces/19115/resources/Codelists/cat/codelists.xml"
 
 ns = {
     "srv": "http://standards.iso.org/iso/19115/-3/srv/2.0",
     "cat": "http://standards.iso.org/iso/19115/-3/cat/1.0",
     "cit": "http://standards.iso.org/iso/19115/-3/cit/2.0",
@@ -74,14 +81,21 @@
 
 for f in _schematron_mapping.values():
     assert (
         f.is_file()
     ), f"Schema {f} does not exists. Have you extracted namespaces.zip?"
 
 
+def _get_cache_path(name):
+    cache_dir = Path(tk.config.get(CONFIG_CACHE_DIR) or _tempdir)
+    cache_dir.mkdir(parents=True, exist_ok=True)
+    return cache_dir / f"{name}.pickle"
+
+
+
 def lookup(root: str, schema: xmlschema.XMLSchema):
     qualified_root = root
 
     try:
         _ns, tag = root.split(":")
         qualified_root = "{%s}%s" % (ns[_ns], tag)
     except (ValueError, KeyError):
@@ -100,16 +114,17 @@
                 break
 
     # el = schema.find(f".//{root}", namespaces=utils.ns)
     return el
 
 
 def _get_schema(name: str, rebuild: bool = False) -> xmlschema.XMLSchema:
-    cache = _root / f"{name}.pickle"
+    cache = _get_cache_path(name)
     if not cache.is_file() or rebuild:
+        log.info("Building the cache at %s...", cache)
         schema = xmlschema.XMLSchema(
             str(_schema_mapping[name]), validation="lax"
         )
         with cache.open("wb") as dest:
             pickle.dump(schema, dest)
     with cache.open("rb") as src:
         return pickle.load(src)
@@ -204,15 +219,15 @@
     namespaces = {"cat": xml.nsmap["cat"], "gco": xml.nsmap["gco"]}
     codes = xml.xpath(xpath, namespaces=namespaces)
 
     return [
         CodeListValue(
             code.find(
                 "cat:identifier/gco:ScopedName", namespaces=namespaces
-            ).text,
+            ).text.strip(),
             code.find(
                 "cat:definition/gco:CharacterString", namespaces=namespaces
             ).text,
         )
         for code in codes
     ]
```

### Comparing `ckanext-iso19115-0.0.9/ckanext/iso19115/views.py` & `ckanext-iso19115-0.1.0/ckanext/iso19115/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/PKG-INFO` & `ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ckanext-iso19115
-Version: 0.0.9
-Summary: UNKNOWN
+Version: 0.1.0
 Home-page: https://github.com/DataShades/ckanext-iso19115
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
@@ -137,9 +135,7 @@
 
        git tag 0.0.1
        git push --tags
 
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
-
-
```

### Comparing `ckanext-iso19115-0.0.9/ckanext_iso19115.egg-info/SOURCES.txt` & `ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 requirements.txt
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/iso19115/__init__.py
 ckanext/iso19115/builder.py
 ckanext/iso19115/cli.py
+ckanext/iso19115/config_declaration.yaml
 ckanext/iso19115/formatter.py
 ckanext/iso19115/helpers.py
 ckanext/iso19115/interfaces.py
 ckanext/iso19115/plugin.py
+ckanext/iso19115/presets.yaml
 ckanext/iso19115/utils.py
 ckanext/iso19115/views.py
-ckanext/iso19115/assets/script.js
-ckanext/iso19115/assets/style.css
+ckanext/iso19115/assets/iso19115-script.js
+ckanext/iso19115/assets/iso19115-style.css
 ckanext/iso19115/assets/webassets.yml
 ckanext/iso19115/converter/__init__.py
 ckanext/iso19115/converter/helpers.py
 ckanext/iso19115/logic/__init__.py
 ckanext/iso19115/logic/action.py
 ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd
 ckanext/iso19115/namespaces/19110/fcc/1.0/fcc.xsd
```

### Comparing `ckanext-iso19115-0.0.9/setup.cfg` & `ckanext-iso19115-0.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-iso19115
-version = 0.0.9
+version = 0.1.0
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-iso19115
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
@@ -22,14 +22,15 @@
 python_requires = >= 3.7
 install_requires = 
 	xmlschema
 	faker
 	exrex
 	ckanapi
 	typing_extensions
+	pycountry
 packages = find:
 namespace_packages = ckanext
 include_package_data = True
 
 [options.entry_points]
 ckan.plugins = 
 	iso19115 = ckanext.iso19115.plugin:Iso19115Plugin
```


# Comparing `tmp/STEAM_materials-2023.4.0.tar.gz` & `tmp/STEAM_materials-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEAM_materials-2023.4.0.tar", last modified: Thu Apr 20 13:05:27 2023, max compression
+gzip compressed data, was "STEAM_materials-2023.4.1.tar", last modified: Mon Apr 24 09:10:37 2023, max compression
```

## Comparing `STEAM_materials-2023.4.0.tar` & `STEAM_materials-2023.4.1.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 13:05:27.789842 STEAM_materials-2023.4.0/
--rw-rw-rw-   0        0        0       37 2022-04-11 08:27:26.000000 STEAM_materials-2023.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      465 2023-04-20 13:05:27.789842 STEAM_materials-2023.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       68 2022-04-05 13:59:57.000000 STEAM_materials-2023.4.0/README.md
--rw-rw-rw-   0        0        0       86 2022-04-05 14:02:07.000000 STEAM_materials-2023.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 13:05:27.789842 STEAM_materials-2023.4.0/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-04-20 13:04:52.000000 STEAM_materials-2023.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:05:25.936964 STEAM_materials-2023.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 13:05:25.957913 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/
--rw-rw-rw-   0        0        0      465 2023-04-20 13:05:25.000000 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2023-04-20 13:05:25.000000 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 13:05:25.000000 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 13:05:25.000000 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 13:05:25.000000 STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 13:05:25.966754 STEAM_materials-2023.4.0/src/steammaterials/
-drwxrwxrwx   0        0        0        0 2023-04-20 13:05:27.788845 STEAM_materials-2023.4.0/src/steammaterials/CFUN/
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:53.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/BHAir_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-20 13:03:53.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/BHIron2_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:53.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:53.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-20 13:03:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
--rw-rw-rw-   0        0        0   124928 2023-04-20 13:03:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:55.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:03:55.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:55.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:56.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:56.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-20 13:03:56.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:56.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:56.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-20 13:03:57.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:57.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
--rw-rw-rw-   0        0        0   129536 2023-04-20 13:03:57.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:03:58.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:03:58.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:03:58.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:03:58.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-20 13:03:58.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-20 13:04:02.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-20 13:04:05.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:59.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAg_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:03:59.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:03:59.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-20 13:04:00.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:04:00.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
--rw-rw-rw-   0        0        0   105472 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-20 13:04:00.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kG10_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kHast_v1.dll
--rw-rw-rw-   0        0        0   124416 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kHe_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-20 13:04:01.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
--rw-rw-rw-   0        0        0   124416 2023-04-20 13:04:02.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
--rw-rw-rw-   0        0        0   105984 2023-04-20 13:04:02.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-20 13:04:03.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-20 13:04:04.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-20 13:04:04.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-20 13:04:04.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2023.4.0/src/steammaterials/CFUN/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-04-19 07:04:52.000000 STEAM_materials-2023.4.0/src/steammaterials/STEAM_materials.py
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2023.4.0/src/steammaterials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:10:37.318934 STEAM_materials-2023.4.1/
+-rw-rw-rw-   0        0        0       37 2022-04-11 08:27:26.000000 STEAM_materials-2023.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      465 2023-04-24 09:10:37.317798 STEAM_materials-2023.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2022-04-05 13:59:57.000000 STEAM_materials-2023.4.1/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-05 14:02:07.000000 STEAM_materials-2023.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:10:37.318934 STEAM_materials-2023.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-04-24 09:09:26.000000 STEAM_materials-2023.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:10:34.878630 STEAM_materials-2023.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:10:34.969378 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/
+-rw-rw-rw-   0        0        0      465 2023-04-24 09:10:34.000000 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2023-04-24 09:10:34.000000 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:10:34.000000 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 09:10:34.000000 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 09:10:34.000000 STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 09:10:34.975360 STEAM_materials-2023.4.1/src/steammaterials/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:10:37.314800 STEAM_materials-2023.4.1/src/steammaterials/CFUN/
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:07.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/BHAir_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-24 09:07:07.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/BHIron2_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:08.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:08.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:08.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:10.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-24 09:07:09.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:09.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
+-rw-rw-rw-   0        0        0   124928 2023-04-24 09:07:10.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:11.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:11.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:12.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:12.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:12.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-24 09:07:12.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:12.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:13.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-24 09:07:13.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:14.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
+-rw-rw-rw-   0        0        0   127488 2023-04-24 09:07:15.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1.dll
+-rw-rw-rw-   0        0        0   127488 2023-04-24 09:07:14.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1.dll
+-rw-rw-rw-   0        0        0   127488 2023-04-24 09:07:15.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1.dll
+-rw-rw-rw-   0        0        0   129536 2023-04-24 09:07:30.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:16.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:16.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:16.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:17.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-24 09:07:17.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-24 09:07:24.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-24 09:07:30.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:18.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAg_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:18.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:19.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-24 09:07:19.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:20.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
+-rw-rw-rw-   0        0        0   105472 2023-04-24 09:07:21.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-24 09:07:20.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:21.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kG10_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:22.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kHast_v1.dll
+-rw-rw-rw-   0        0        0   124416 2023-04-24 09:07:22.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kHe_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:23.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-24 09:07:23.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
+-rw-rw-rw-   0        0        0   124416 2023-04-24 09:07:24.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
+-rw-rw-rw-   0        0        0   105984 2023-04-24 09:07:25.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-24 09:07:25.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-24 09:07:26.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-24 09:07:26.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:27.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:27.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-24 09:07:28.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-24 09:07:28.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-24 09:07:29.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-24 09:07:29.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
+-rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2023.4.1/src/steammaterials/CFUN/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-04-19 07:04:52.000000 STEAM_materials-2023.4.1/src/steammaterials/STEAM_materials.py
+-rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-2023.4.1/src/steammaterials/__init__.py
```

### Comparing `STEAM_materials-2023.4.0/setup.py` & `STEAM_materials-2023.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="STEAM_materials",
-    version="2023.4.0",
+    version="2023.4.1",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Python wrapper for the steam materials package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam-material-library",
     keywords={'STEAM', 'API', 'MATERIALS', 'CERN'},
```

### Comparing `STEAM_materials-2023.4.0/src/STEAM_materials.egg-info/SOURCES.txt` & `STEAM_materials-2023.4.1/src/STEAM_materials.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,31 @@
 src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
 src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
 src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
 src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
 src/steammaterials/CFUN/CFUN_CvTi_v1.dll
 src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
 src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
+src/steammaterials/CFUN/CFUN_HTS_JcFit_SUPERPOWER_v1.dll
+src/steammaterials/CFUN/CFUN_HTS_JcFit_THEVA_v1.dll
+src/steammaterials/CFUN/CFUN_HTS_JcFit_sunam_v1.dll
 src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
 src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
 src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
 src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
 src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
 src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
 src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
 src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
 src/steammaterials/CFUN/CFUN_kAg_v1.dll
 src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
 src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
 src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
 src/steammaterials/CFUN/CFUN_kBrass_v1.dll
-src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll
+src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1.dll
 src/steammaterials/CFUN/CFUN_kCu_v1.dll
 src/steammaterials/CFUN/CFUN_kG10_v1.dll
 src/steammaterials/CFUN/CFUN_kHast_v1.dll
 src/steammaterials/CFUN/CFUN_kHe_v1.dll
 src/steammaterials/CFUN/CFUN_kKapton_v1.dll
 src/steammaterials/CFUN/CFUN_kSteel_v1.dll
 src/steammaterials/CFUN/CFUN_kStycast_v1.dll
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/BHAir_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/BHAir_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800016f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:53 2023
+Time/Date		Mon Apr 24 09:07:07 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000016f8
@@ -36569,19 +36569,17 @@
    18001b0dd:	add    %al,(%rax)
    18001b0df:	add    %dh,0x12(%rax)
    18001b0e2:	add    %eax,0x1(%rax)
    18001b0e8:	js     0x18001b0fc
    18001b0ea:	add    %eax,0x1(%rax)
    18001b0f0:	add    %al,(%rax)
    18001b0f2:	add    %al,(%rax)
-   18001b0f4:	cmp    %edi,(%rax)
-   18001b0f6:	rex.B
-   18001b0f7:	add    %al,%fs:(%rax)
-   18001b0fa:	add    %al,(%rax)
-   18001b0fc:	or     $0xc8000000,%eax
+   18001b0f4:	mov    $0x644646,%ebx
+   18001b0f9:	add    %al,(%rax)
+   18001b0fb:	add    %cl,-0x38000000(%rip)        # 0x14801b101
    18001b101:	add    (%rax),%al
    18001b103:	add    %ah,%ah
    18001b105:	mov    $0x1,%bl
    18001b107:	add    %ah,%ah
    18001b109:	popf
    18001b10a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/BHIron2_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/BHIron2_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001e30
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:53 2023
+Time/Date		Mon Apr 24 09:07:07 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000fa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001e30
@@ -37040,19 +37040,17 @@
    18001b2dd:	add    %al,(%rax)
    18001b2df:	add    %dh,0x12(%rax)
    18001b2e2:	add    %eax,0x1(%rax)
    18001b2e8:	js     0x18001b2fc
    18001b2ea:	add    %eax,0x1(%rax)
    18001b2f0:	add    %al,(%rax)
    18001b2f2:	add    %al,(%rax)
-   18001b2f4:	cmp    %edi,(%rax)
-   18001b2f6:	rex.B
-   18001b2f7:	add    %al,%fs:(%rax)
-   18001b2fa:	add    %al,(%rax)
-   18001b2fc:	or     $0xc8000000,%eax
+   18001b2f4:	mov    $0x644646,%ebx
+   18001b2f9:	add    %al,(%rax)
+   18001b2fb:	add    %cl,-0x38000000(%rip)        # 0x14801b301
    18001b301:	add    (%rax),%al
    18001b303:	add    %ch,%ah
    18001b305:	mov    $0x1,%ch
    18001b307:	add    %ch,%ah
    18001b309:	cmpsl  %es:(%rdi),%ds:(%rsi)
    18001b30a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAg_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAg_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800018d0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:53 2023
+Time/Date		Mon Apr 24 09:07:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000018d0
@@ -36505,19 +36505,17 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	cmp    %edi,(%rax)
-   18001b186:	rex.B
-   18001b187:	add    %al,%fs:(%rax)
-   18001b18a:	add    %al,(%rax)
-   18001b18c:	or     $0xc8000000,%eax
+   18001b184:	mov    $0x644646,%esp
+   18001b189:	add    %al,(%rax)
+   18001b18b:	add    %cl,-0x38000000(%rip)        # 0x14801b191
    18001b191:	add    (%rax),%al
    18001b193:	add    %ch,0x1(%rsp,%rsi,4)
    18001b197:	add    %ch,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001930
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:53 2023
+Time/Date		Mon Apr 24 09:07:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001930
@@ -36513,19 +36513,17 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	cmp    %edi,(%rax)
-   18001b186:	rex.B
-   18001b187:	add    %al,%fs:(%rax)
-   18001b18a:	add    %al,(%rax)
-   18001b18c:	or     $0xc8000000,%eax
+   18001b184:	mov    $0x644646,%esp
+   18001b189:	add    %al,(%rax)
+   18001b18b:	add    %cl,-0x38000000(%rip)        # 0x14801b191
    18001b191:	add    (%rax),%al
    18001b193:	add    %ch,0x1(%rsp,%rsi,4)
    18001b197:	add    %ch,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvAl_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvAl_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001860
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:54 2023
+Time/Date		Mon Apr 24 09:07:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001860
@@ -36582,19 +36582,17 @@
    18001b18d:	add    %al,(%rax)
    18001b18f:	add    %dh,0x12(%rax)
    18001b192:	add    %eax,0x1(%rax)
    18001b198:	js     0x18001b1ac
    18001b19a:	add    %eax,0x1(%rax)
    18001b1a0:	add    %al,(%rax)
    18001b1a2:	add    %al,(%rax)
-   18001b1a4:	cmp    (%rax),%bh
-   18001b1a6:	rex.B
-   18001b1a7:	add    %al,%fs:(%rax)
-   18001b1aa:	add    %al,(%rax)
-   18001b1ac:	or     $0xc8000000,%eax
+   18001b1a4:	mov    $0x644646,%esp
+   18001b1a9:	add    %al,(%rax)
+   18001b1ab:	add    %cl,-0x38000000(%rip)        # 0x14801b1b1
    18001b1b1:	add    (%rax),%al
    18001b1b3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1b7:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001970
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:54 2023
+Time/Date		Mon Apr 24 09:07:10 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001970
@@ -36526,19 +36526,17 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	cmp    (%rax),%bh
-   18001b196:	rex.B
-   18001b197:	add    %al,%fs:(%rax)
-   18001b19a:	add    %al,(%rax)
-   18001b19c:	or     $0xc8000000,%eax
+   18001b194:	mov    $0x644646,%esi
+   18001b199:	add    %al,(%rax)
+   18001b19b:	add    %cl,-0x38000000(%rip)        # 0x14801b1a1
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ch,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ch,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:54 2023
+Time/Date		Mon Apr 24 09:07:09 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017e0
@@ -36584,19 +36584,17 @@
    18001b13d:	add    %al,(%rax)
    18001b13f:	add    %dh,0x12(%rax)
    18001b142:	add    %eax,0x1(%rax)
    18001b148:	js     0x18001b15c
    18001b14a:	add    %eax,0x1(%rax)
    18001b150:	add    %al,(%rax)
    18001b152:	add    %al,(%rax)
-   18001b154:	cmp    (%rax),%bh
-   18001b156:	rex.B
-   18001b157:	add    %al,%fs:(%rax)
-   18001b15a:	add    %al,(%rax)
-   18001b15c:	or     $0xc8000000,%eax
+   18001b154:	mov    $0x644646,%ebp
+   18001b159:	add    %al,(%rax)
+   18001b15b:	add    %cl,-0x38000000(%rip)        # 0x14801b161
    18001b161:	add    (%rax),%al
    18001b163:	add    %ch,%ah
    18001b165:	mov    $0x1,%bl
    18001b167:	add    %ch,%ah
    18001b169:	popf
    18001b16a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017b0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:54 2023
+Time/Date		Mon Apr 24 09:07:09 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017b0
@@ -36495,19 +36495,17 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	cmp    (%rax),%bh
-   18001b196:	rex.B
-   18001b197:	add    %al,%fs:(%rax)
-   18001b19a:	add    %al,(%rax)
-   18001b19c:	or     $0xc8000000,%eax
+   18001b194:	mov    $0x644646,%ebp
+   18001b199:	add    %al,(%rax)
+   18001b19b:	add    %cl,-0x38000000(%rip)        # 0x14801b1a1
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvCu_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvCu_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001e10
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:54 2023
+Time/Date		Mon Apr 24 09:07:10 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001e10
@@ -36891,19 +36891,17 @@
    18001b1dd:	add    %al,(%rax)
    18001b1df:	add    %dh,0x12(%rax)
    18001b1e2:	add    %eax,0x1(%rax)
    18001b1e8:	js     0x18001b1fc
    18001b1ea:	add    %eax,0x1(%rax)
    18001b1f0:	add    %al,(%rax)
    18001b1f2:	add    %al,(%rax)
-   18001b1f4:	cmp    (%rax),%bh
-   18001b1f6:	rex.B
-   18001b1f7:	add    %al,%fs:(%rax)
-   18001b1fa:	add    %al,(%rax)
-   18001b1fc:	or     $0xc8000000,%eax
+   18001b1f4:	mov    $0x644646,%esi
+   18001b1f9:	add    %al,(%rax)
+   18001b1fb:	add    %cl,-0x38000000(%rip)        # 0x14801b201
    18001b201:	add    (%rax),%al
    18001b203:	add    %ch,%ah
    18001b205:	mov    $0x1,%ah
    18001b207:	add    %ch,%ah
    18001b209:	cmpsb  %es:(%rdi),%ds:(%rsi)
    18001b20a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvG10_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvG10_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001758
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:55 2023
+Time/Date		Mon Apr 24 09:07:11 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001758
@@ -36498,19 +36498,17 @@
    18001b15d:	add    %al,(%rax)
    18001b15f:	add    %dh,0x12(%rax)
    18001b162:	add    %eax,0x1(%rax)
    18001b168:	js     0x18001b17c
    18001b16a:	add    %eax,0x1(%rax)
    18001b170:	add    %al,(%rax)
    18001b172:	add    %al,(%rax)
-   18001b174:	cmp    (%rax),%edi
-   18001b176:	rex.B
-   18001b177:	add    %al,%fs:(%rax)
-   18001b17a:	add    %al,(%rax)
-   18001b17c:	or     $0xc8000000,%eax
+   18001b174:	mov    $0x644646,%edi
+   18001b179:	add    %al,(%rax)
+   18001b17b:	add    %cl,-0x38000000(%rip)        # 0x14801b181
    18001b181:	add    (%rax),%al
    18001b183:	add    %ah,0x1(%rsp,%rsi,4)
    18001b187:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvHast_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvHast_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800019a4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:55 2023
+Time/Date		Mon Apr 24 09:07:11 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000019a4
@@ -36754,19 +36754,17 @@
    18001b1cd:	add    %al,(%rax)
    18001b1cf:	add    %dh,0x12(%rax)
    18001b1d2:	add    %eax,0x1(%rax)
    18001b1d8:	js     0x18001b1ec
    18001b1da:	add    %eax,0x1(%rax)
    18001b1e0:	add    %al,(%rax)
    18001b1e2:	add    %al,(%rax)
-   18001b1e4:	cmp    (%rax),%edi
-   18001b1e6:	rex.B
-   18001b1e7:	add    %al,%fs:(%rax)
-   18001b1ea:	add    %al,(%rax)
-   18001b1ec:	or     $0xc8000000,%eax
+   18001b1e4:	mov    $0x644646,%edi
+   18001b1e9:	add    %al,(%rax)
+   18001b1eb:	add    %cl,-0x38000000(%rip)        # 0x14801b1f1
    18001b1f1:	add    (%rax),%al
    18001b1f3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1f7:	add    %ah,0x1(%rdx,%riz,4)
    18001b1fb:	add    %al,(%rax)
    18001b1fd:	add    %al,(%rax)
    18001b1ff:	add    %al,(%rcx)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvHe_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvHe_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800018d0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:55 2023
+Time/Date		Mon Apr 24 09:07:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000018d0
@@ -36766,17 +36766,16 @@
    18001b1cd:	add    %al,(%rax)
    18001b1cf:	add    %dh,0x12(%rax)
    18001b1d2:	add    %eax,0x1(%rax)
    18001b1d8:	js     0x18001b1ec
    18001b1da:	add    %eax,0x1(%rax)
    18001b1e0:	add    %al,(%rax)
    18001b1e2:	add    %al,(%rax)
-   18001b1e4:	cmp    (%rax),%edi
-   18001b1e6:	rex.B
-   18001b1e7:	add    %al,%fs:(%rax)
+   18001b1e4:	rolb   $0x64,0x46(%rsi)
+   18001b1e8:	add    %al,(%rax)
    18001b1ea:	add    %al,(%rax)
    18001b1ec:	or     $0xc8000000,%eax
    18001b1f1:	add    (%rax),%al
    18001b1f3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1f7:	add    %ah,0x1(%rax,%riz,4)
    18001b1fb:	add    %al,(%rax)
    18001b1fd:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001944
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:56 2023
+Time/Date		Mon Apr 24 09:07:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001944
@@ -36564,17 +36564,16 @@
    18001b15d:	add    %al,(%rax)
    18001b15f:	add    %dh,0x12(%rax)
    18001b162:	add    %eax,0x1(%rax)
    18001b168:	js     0x18001b17c
    18001b16a:	add    %eax,0x1(%rax)
    18001b170:	add    %al,(%rax)
    18001b172:	add    %al,(%rax)
-   18001b174:	cmp    $0x38,%al
-   18001b176:	rex.B
-   18001b177:	add    %al,%fs:(%rax)
+   18001b174:	rolb   $0x64,0x46(%rsi)
+   18001b178:	add    %al,(%rax)
    18001b17a:	add    %al,(%rax)
    18001b17c:	or     $0xc8000000,%eax
    18001b181:	add    (%rax),%al
    18001b183:	add    %ah,0x1(%rsp,%rsi,4)
    18001b187:	add    %ah,0x1(%rdx,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001994
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:56 2023
+Time/Date		Mon Apr 24 09:07:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001994
@@ -36618,17 +36618,16 @@
    18001b18d:	add    %al,(%rax)
    18001b18f:	add    %dh,0x12(%rax)
    18001b192:	add    %eax,0x1(%rax)
    18001b198:	js     0x18001b1ac
    18001b19a:	add    %eax,0x1(%rax)
    18001b1a0:	add    %al,(%rax)
    18001b1a2:	add    %al,(%rax)
-   18001b1a4:	cmp    $0x38,%al
-   18001b1a6:	rex.B
-   18001b1a7:	add    %al,%fs:(%rax)
+   18001b1a4:	rolb   $0x64,0x46(%rsi)
+   18001b1a8:	add    %al,(%rax)
    18001b1aa:	add    %al,(%rax)
    18001b1ac:	or     $0xc8000000,%eax
    18001b1b1:	add    (%rax),%al
    18001b1b3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1b7:	add    %ah,0x1(%rdx,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002070
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:56 2023
+Time/Date		Mon Apr 24 09:07:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000010000
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002070
@@ -36961,17 +36961,16 @@
    18001b1ed:	add    %al,(%rax)
    18001b1ef:	add    %dh,0x12(%rax)
    18001b1f2:	add    %eax,0x1(%rax)
    18001b1f8:	js     0x18001b20c
    18001b1fa:	add    %eax,0x1(%rax)
    18001b200:	add    %al,(%rax)
    18001b202:	add    %al,(%rax)
-   18001b204:	cmp    $0x38,%al
-   18001b206:	rex.B
-   18001b207:	add    %al,%fs:(%rax)
+   18001b204:	rolb   $0x64,0x46(%rsi)
+   18001b208:	add    %al,(%rax)
    18001b20a:	add    %al,(%rax)
    18001b20c:	or     $0xc8000000,%eax
    18001b211:	add    (%rax),%al
    18001b213:	add    %ch,%ah
    18001b215:	mov    $0x1,%ah
    18001b217:	add    %ch,%ah
    18001b219:	test   $0x1,%al
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001754
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:56 2023
+Time/Date		Mon Apr 24 09:07:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001754
@@ -36580,17 +36580,16 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	cmp    $0x38,%al
-   18001b186:	rex.B
-   18001b187:	add    %al,%fs:(%rax)
+   18001b184:	rolb   $0x64,0x46(%rsi)
+   18001b188:	add    %al,(%rax)
    18001b18a:	add    %al,(%rax)
    18001b18c:	or     $0xc8000000,%eax
    18001b191:	add    (%rax),%al
    18001b193:	add    %ah,0x1(%rsp,%rsi,4)
    18001b197:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_CvTi_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_CvTi_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001900
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:56 2023
+Time/Date		Mon Apr 24 09:07:13 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001900
@@ -36513,17 +36513,16 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	cmp    $0x38,%al
-   18001b186:	rex.B
-   18001b187:	add    %al,%fs:(%rax)
+   18001b184:	roll   $0x64,0x46(%rsi)
+   18001b188:	add    %al,(%rax)
    18001b18a:	add    %al,(%rax)
    18001b18c:	or     $0xc8000000,%eax
    18001b191:	add    (%rax),%al
    18001b193:	add    %ch,0x1(%rsp,%rsi,4)
    18001b197:	add    %ch,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800016ec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:57 2023
+Time/Date		Mon Apr 24 09:07:13 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000016ec
@@ -36539,17 +36539,18 @@
    18001b0dd:	add    %al,(%rax)
    18001b0df:	add    %dh,0x12(%rax)
    18001b0e2:	add    %eax,0x1(%rax)
    18001b0e8:	js     0x18001b0fc
    18001b0ea:	add    %eax,0x1(%rax)
    18001b0f0:	add    %al,(%rax)
    18001b0f2:	add    %al,(%rax)
-   18001b0f4:	cmp    $0x644138,%eax
-   18001b0f9:	add    %al,(%rax)
-   18001b0fb:	add    %cl,-0x38000000(%rip)        # 0x14801b101
+   18001b0f4:	roll   $0x64,0x46(%rsi)
+   18001b0f8:	add    %al,(%rax)
+   18001b0fa:	add    %al,(%rax)
+   18001b0fc:	or     $0xc8000000,%eax
    18001b101:	add    (%rax),%al
    18001b103:	add    %ah,%ah
    18001b105:	mov    $0x1,%bl
    18001b107:	add    %ah,%ah
    18001b109:	popf
    18001b10a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001820
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:57 2023
+Time/Date		Mon Apr 24 09:07:14 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001820
@@ -36594,17 +36594,18 @@
    18001b0dd:	add    %al,(%rax)
    18001b0df:	add    %dh,0x12(%rax)
    18001b0e2:	add    %eax,0x1(%rax)
    18001b0e8:	js     0x18001b0fc
    18001b0ea:	add    %eax,0x1(%rax)
    18001b0f0:	add    %al,(%rax)
    18001b0f2:	add    %al,(%rax)
-   18001b0f4:	cmp    $0x644138,%eax
-   18001b0f9:	add    %al,(%rax)
-   18001b0fb:	add    %cl,-0x38000000(%rip)        # 0x14801b101
+   18001b0f4:	ret    $0x4646
+   18001b0f7:	add    %al,%fs:(%rax)
+   18001b0fa:	add    %al,(%rax)
+   18001b0fc:	or     $0xc8000000,%eax
    18001b101:	add    (%rax),%al
    18001b103:	add    %ah,%ah
    18001b105:	mov    $0x1,%bl
    18001b107:	add    %ah,%ah
    18001b109:	lahf
    18001b10a:	add    %eax,(%rax)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002280
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:57 2023
+Time/Date		Mon Apr 24 09:07:30 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	000000000000fe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002280
@@ -37749,17 +37749,18 @@
    18001c6cd:	add    %al,(%rax)
    18001c6cf:	add    %dh,0x22(%rax)
    18001c6d2:	add    %eax,0x1(%rax)
    18001c6d8:	js     0x18001c6fc
    18001c6da:	add    %eax,0x1(%rax)
    18001c6e0:	add    %al,(%rax)
    18001c6e2:	add    %al,(%rax)
-   18001c6e4:	cmp    $0x644138,%eax
-   18001c6e9:	add    %al,(%rax)
-   18001c6eb:	add    %cl,-0x38000000(%rip)        # 0x14801c6f1
+   18001c6e4:	rolb   %cl,0x46(%rsi)
+   18001c6e7:	add    %al,%fs:(%rax)
+   18001c6ea:	add    %al,(%rax)
+   18001c6ec:	or     $0xc8000000,%eax
    18001c6f1:	add    (%rax),%al
    18001c6f3:	add    %ah,0x1(%rcx,%rcx,8)
    18001c6f7:	add    %ah,0x1(%rdi,%rsi,4)
    18001c6fb:	add    %al,(%rax)
    18001c6fd:	add    %al,(%rax)
    18001c6ff:	add    %al,(%rcx)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000187c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:58 2023
+Time/Date		Mon Apr 24 09:07:16 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000187c
@@ -36640,16 +36640,18 @@
    18001b12d:	add    %al,(%rax)
    18001b12f:	add    %dh,0x12(%rax)
    18001b132:	add    %eax,0x1(%rax)
    18001b138:	js     0x18001b14c
    18001b13a:	add    %eax,0x1(%rax)
    18001b140:	add    %al,(%rax)
    18001b142:	add    %al,(%rax)
-   18001b144:	ds cmp %al,0x64(%rcx)
-   18001b148:	add    %al,(%rax)
+   18001b144:	(bad)
+   18001b145:	rex.RX
+   18001b146:	rex.RX
+   18001b147:	add    %al,%fs:(%rax)
    18001b14a:	add    %al,(%rax)
    18001b14c:	or     $0xc8000000,%eax
    18001b151:	add    (%rax),%al
    18001b153:	add    %ah,%ah
    18001b155:	mov    $0x1,%bl
    18001b157:	add    %ah,%ah
    18001b159:	movabs 0x1,%eax
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800019b4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:58 2023
+Time/Date		Mon Apr 24 09:07:16 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000019b4
@@ -36688,16 +36688,18 @@
    18001b12d:	add    %al,(%rax)
    18001b12f:	add    %dh,0x12(%rax)
    18001b132:	add    %eax,0x1(%rax)
    18001b138:	js     0x18001b14c
    18001b13a:	add    %eax,0x1(%rax)
    18001b140:	add    %al,(%rax)
    18001b142:	add    %al,(%rax)
-   18001b144:	ds cmp %al,0x64(%rcx)
-   18001b148:	add    %al,(%rax)
+   18001b144:	(bad)
+   18001b145:	rex.RX
+   18001b146:	rex.RX
+   18001b147:	add    %al,%fs:(%rax)
    18001b14a:	add    %al,(%rax)
    18001b14c:	or     $0xc8000000,%eax
    18001b151:	add    (%rax),%al
    18001b153:	add    %ah,%ah
    18001b155:	mov    $0x1,%bl
    18001b157:	add    %ah,%ah
    18001b159:	movabs 0x1,%eax
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000187c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:58 2023
+Time/Date		Mon Apr 24 09:07:16 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000187c
@@ -36638,16 +36638,18 @@
    18001b12d:	add    %al,(%rax)
    18001b12f:	add    %dh,0x12(%rax)
    18001b132:	add    %eax,0x1(%rax)
    18001b138:	js     0x18001b14c
    18001b13a:	add    %eax,0x1(%rax)
    18001b140:	add    %al,(%rax)
    18001b142:	add    %al,(%rax)
-   18001b144:	ds cmp %al,0x64(%rcx)
-   18001b148:	add    %al,(%rax)
+   18001b144:	(bad)
+   18001b145:	rex.RX
+   18001b146:	rex.RX
+   18001b147:	add    %al,%fs:(%rax)
    18001b14a:	add    %al,(%rax)
    18001b14c:	or     $0xc8000000,%eax
    18001b151:	add    (%rax),%al
    18001b153:	add    %ah,%ah
    18001b155:	mov    $0x1,%bl
    18001b157:	add    %ah,%ah
    18001b159:	movabs 0x1,%eax
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001888
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:58 2023
+Time/Date		Mon Apr 24 09:07:17 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001888
@@ -36575,16 +36575,16 @@
    18001b12d:	add    %al,(%rax)
    18001b12f:	add    %dh,0x12(%rax)
    18001b132:	add    %eax,0x1(%rax)
    18001b138:	js     0x18001b14c
    18001b13a:	add    %eax,0x1(%rax)
    18001b140:	add    %al,(%rax)
    18001b142:	add    %al,(%rax)
-   18001b144:	ds cmp %al,0x64(%rcx)
-   18001b148:	add    %al,(%rax)
+   18001b144:	(bad)
+   18001b147:	add    %al,%fs:(%rax)
    18001b14a:	add    %al,(%rax)
    18001b14c:	or     $0xc8000000,%eax
    18001b151:	add    (%rax),%al
    18001b153:	add    %ah,%ah
    18001b155:	mov    $0x1,%bl
    18001b157:	add    %ah,%ah
    18001b159:	lahf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017ac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:58 2023
+Time/Date		Mon Apr 24 09:07:17 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fc00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017ac
@@ -37158,16 +37158,16 @@
    18001b44d:	add    %al,(%rax)
    18001b44f:	add    %dh,0x12(%rax)
    18001b452:	add    %eax,0x1(%rax)
    18001b458:	js     0x18001b46c
    18001b45a:	add    %eax,0x1(%rax)
    18001b460:	add    %al,(%rax)
    18001b462:	add    %al,(%rax)
-   18001b464:	ds cmp %al,0x64(%rcx)
-   18001b468:	add    %al,(%rax)
+   18001b464:	(bad)
+   18001b467:	add    %al,%fs:(%rax)
    18001b46a:	add    %al,(%rax)
    18001b46c:	or     $0xc8000000,%eax
    18001b471:	add    (%rax),%al
    18001b473:	add    %ah,%ah
    18001b475:	mov    $0x1,%dh
    18001b477:	add    %ah,%ah
    18001b479:	cmpsb  %es:(%rdi),%ds:(%rsi)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000195c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:02 2023
+Time/Date		Mon Apr 24 09:07:24 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000195c
@@ -37249,16 +37249,18 @@
    18001b42d:	add    %al,(%rax)
    18001b42f:	add    %dh,0x12(%rax)
    18001b432:	add    %eax,0x1(%rax)
    18001b438:	js     0x18001b44c
    18001b43a:	add    %eax,0x1(%rax)
    18001b440:	add    %al,(%rax)
    18001b442:	add    %al,(%rax)
-   18001b444:	rex.X cmp %al,0x64(%rcx)
-   18001b448:	add    %al,(%rax)
+   18001b444:	int3
+   18001b445:	rex.RX
+   18001b446:	rex.RX
+   18001b447:	add    %al,%fs:(%rax)
    18001b44a:	add    %al,(%rax)
    18001b44c:	or     $0xc8000000,%eax
    18001b451:	add    (%rax),%al
    18001b453:	add    %ah,%ah
    18001b455:	mov    $0x1,%dh
    18001b457:	add    %ah,%ah
    18001b459:	test   $0x1,%al
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001658
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:05 2023
+Time/Date		Mon Apr 24 09:07:30 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001658
@@ -36526,16 +36526,16 @@
    18001b0ed:	add    %al,(%rax)
    18001b0ef:	add    %dh,0x12(%rax)
    18001b0f2:	add    %eax,0x1(%rax)
    18001b0f8:	js     0x18001b10c
    18001b0fa:	add    %eax,0x1(%rax)
    18001b100:	add    %al,(%rax)
    18001b102:	add    %al,(%rax)
-   18001b104:	cmp    %r8b,0x64(%r9)
-   18001b108:	add    %al,(%rax)
+   18001b104:	rolb   %cl,0x46(%rsi)
+   18001b107:	add    %al,%fs:(%rax)
    18001b10a:	add    %al,(%rax)
    18001b10c:	or     $0xc8000000,%eax
    18001b111:	add    (%rax),%al
    18001b113:	add    %ah,%ah
    18001b115:	mov    $0x1,%bl
    18001b117:	add    %ah,%ah
    18001b119:	popf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAg_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAg_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001b70
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:59 2023
+Time/Date		Mon Apr 24 09:07:18 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001b70
@@ -36765,16 +36765,15 @@
    18001b19d:	add    %al,(%rax)
    18001b19f:	add    %dh,0x12(%rax)
    18001b1a2:	add    %eax,0x1(%rax)
    18001b1a8:	js     0x18001b1bc
    18001b1aa:	add    %eax,0x1(%rax)
    18001b1b0:	add    %al,(%rax)
    18001b1b2:	add    %al,(%rax)
-   18001b1b4:	(bad)
-   18001b1b5:	cmp    %al,0x64(%rcx)
+   18001b1b4:	movb   $0x64,0x46(%rsi)
    18001b1b8:	add    %al,(%rax)
    18001b1ba:	add    %al,(%rax)
    18001b1bc:	or     $0xc8000000,%eax
    18001b1c1:	add    (%rax),%al
    18001b1c3:	add    %ch,0x1(%rsp,%rsi,4)
    18001b1c7:	add    %ch,0x1(%rdx,%riz,4)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001a04
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:59 2023
+Time/Date		Mon Apr 24 09:07:18 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001a04
@@ -36599,16 +36599,15 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	(bad)
-   18001b185:	cmp    %al,0x64(%rcx)
+   18001b184:	movb   $0x64,0x46(%rsi)
    18001b188:	add    %al,(%rax)
    18001b18a:	add    %al,(%rax)
    18001b18c:	or     $0xc8000000,%eax
    18001b191:	add    (%rax),%al
    18001b193:	add    %ah,0x1(%rsp,%rsi,4)
    18001b197:	add    %ah,0x1(%rdx,%riz,4)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001b74
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:03:59 2023
+Time/Date		Mon Apr 24 09:07:19 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fc00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001b74
@@ -36640,19 +36640,16 @@
    18001b16d:	add    %al,(%rax)
    18001b16f:	add    %dh,0x12(%rax)
    18001b172:	add    %eax,0x1(%rax)
    18001b178:	js     0x18001b18c
    18001b17a:	add    %eax,0x1(%rax)
    18001b180:	add    %al,(%rax)
    18001b182:	add    %al,(%rax)
-   18001b184:	(bad)
-   18001b185:	cmp    %al,0x64(%rcx)
-   18001b188:	add    %al,(%rax)
-   18001b18a:	add    %al,(%rax)
-   18001b18c:	or     $0xc8000000,%eax
+   18001b184:	movl   $0x64,0x46(%rsi)
+   18001b18b:	add    %cl,-0x38000000(%rip)        # 0x14801b191
    18001b191:	add    (%rax),%al
    18001b193:	add    %ah,0x1(%rsp,%rsi,4)
    18001b197:	add    %ah,0x1(%rsp,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001bf8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:00 2023
+Time/Date		Mon Apr 24 09:07:19 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fc00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001bf8
@@ -36670,18 +36670,16 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	rex cmp %al,0x64(%rcx)
-   18001b198:	add    %al,(%rax)
-   18001b19a:	add    %al,(%rax)
-   18001b19c:	or     $0xc8000000,%eax
+   18001b194:	movl   $0x64,0x46(%rsi)
+   18001b19b:	add    %cl,-0x38000000(%rip)        # 0x14801b1a1
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rsp,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
 	...
    18001b209:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kBrass_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kBrass_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001aa8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:00 2023
+Time/Date		Mon Apr 24 09:07:20 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001aa8
@@ -36742,15 +36742,15 @@
    18001b18d:	add    %al,(%rax)
    18001b18f:	add    %dh,0x12(%rax)
    18001b192:	add    %eax,0x1(%rax)
    18001b198:	js     0x18001b1ac
    18001b19a:	add    %eax,0x1(%rax)
    18001b1a0:	add    %al,(%rax)
    18001b1a2:	add    %al,(%rax)
-   18001b1a4:	rex cmp %al,0x64(%rcx)
+   18001b1a4:	enter  $0x4646,$0x64
    18001b1a8:	add    %al,(%rax)
    18001b1aa:	add    %al,(%rax)
    18001b1ac:	or     $0xc8000000,%eax
    18001b1b1:	add    (%rax),%al
    18001b1b3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1b7:	add    %ah,0x1(%rdx,%riz,4)
 	...
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kCu_Wiedemann_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800014f0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:21 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000dc00
 SizeOfInitializedData	000000000000ce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000014f0
@@ -147,15 +147,15 @@
 There is an export table in .rdata at 0x180017d10
 
 The Export Tables (interpreted .rdata section contents)
 
 Export Flags 			0
 Time/Date stamp 		ffffffff
 Major/Minor 			0/0
-Name 				0000000000017d56 CFUN_kCu_Wiedermann_v1.dll
+Name 				0000000000017d56 CFUN_kCu_Wiedemann_v1.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000003
 	[Name Pointer/Ordinal] Table	00000003
 Table Addresses
 	Export Address Table 		0000000000017d38
 	Name Pointer Table 		0000000000017d44
@@ -2476,19 +2476,19 @@
 	  050: 18 00 00 00 dc 45 00 00 00 00 00 00 00 00 00 00
 	  060: 00 00 00 00 00 00 00 00 98 9a 01 00 00 00 00 00
 	  070: ff ff ff ff 00 00 00 00 18 00 00 00 38 46 00 00
 	  080: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  090: 00 00 00 00 00 00 00 00 ff ff ff ff 00 00 00 00
 	  0a0: 56 7d 01 00 01 00 00 00 03 00 00 00 03 00 00 00
 	  0b0: 38 7d 01 00 44 7d 01 00 50 7d 01 00 30 10 00 00
-	  0c0: 20 10 00 00 00 10 00 00 71 7d 01 00 76 7d 01 00
-	  0d0: 83 7d 01 00 00 00 01 00 02 00 43 46 55 4e 5f 6b
-	  0e0: 43 75 5f 57 69 65 64 65 72 6d 61 6e 6e 5f 76 31
-	  0f0: 2e 64 6c 6c 00 65 76 61 6c 00 67 65 74 4c 61 73
-	  100: 74 45 72 72 6f 72 00 69 6e 69 74 00 b0 7d 01 00
+	  0c0: 20 10 00 00 00 10 00 00 70 7d 01 00 75 7d 01 00
+	  0d0: 82 7d 01 00 00 00 01 00 02 00 43 46 55 4e 5f 6b
+	  0e0: 43 75 5f 57 69 65 64 65 6d 61 6e 6e 5f 76 31 2e
+	  0f0: 64 6c 6c 00 65 76 61 6c 00 67 65 74 4c 61 73 74
+	  100: 45 72 72 6f 72 00 69 6e 69 74 00 00 b0 7d 01 00
 	  110: 00 00 00 00 00 00 00 00 40 81 01 00 00 f0 00 00
 	  120: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  130: 00 00 00 00 f8 7f 01 00 00 00 00 00 12 80 01 00
 	  140: 00 00 00 00 28 80 01 00 00 00 00 00 3e 80 01 00
 	  150: 00 00 00 00 58 80 01 00 00 00 00 00 6e 80 01 00
 	  160: 00 00 00 00 82 80 01 00 00 00 00 00 9c 80 01 00
 	  170: 00 00 00 00 b0 80 01 00 00 00 00 00 c4 80 01 00
@@ -30877,16 +30877,18 @@
    1800168ed:	add    %al,(%rax)
    1800168ef:	add    %dh,-0xe(%rax)
    1800168f2:	add    %al,0x1(%rax)
    1800168f8:	js     0x1800168ec
    1800168fa:	add    %al,0x1(%rax)
    180016900:	add    %al,(%rax)
    180016902:	add    %al,(%rax)
-   180016904:	cmp    %al,0x64(%r9)
-   180016908:	add    %al,(%rax)
+   180016904:	leave
+   180016905:	rex.RX
+   180016906:	rex.RX
+   180016907:	add    %al,%fs:(%rax)
    18001690a:	add    %al,(%rax)
    18001690c:	or     $0xc8000000,%eax
    180016911:	add    (%rax),%al
    180016913:	add    %ah,%ah
    180016915:	imul   $0x0,(%rcx),%eax
    180016918:	in     $0x5b,%al
    18001691a:	add    %eax,(%rax)
@@ -32980,50 +32982,53 @@
    180017d36:	add    %eax,(%rax)
    180017d38:	xor    %dl,(%rax)
    180017d3a:	add    %al,(%rax)
    180017d3c:	and    %dl,(%rax)
    180017d3e:	add    %al,(%rax)
    180017d40:	add    %dl,(%rax)
    180017d42:	add    %al,(%rax)
-   180017d44:	jno    0x180017dc3
+   180017d44:	jo     0x180017dc3
    180017d46:	add    %eax,(%rax)
-   180017d48:	jbe    0x180017dc7
+   180017d48:	jne    0x180017dc7
    180017d4a:	add    %eax,(%rax)
-   180017d4c:	cmpl   $0x0,0x1(%rbp)
-   180017d50:	add    %al,(%rax)
-   180017d52:	add    %eax,(%rax)
-   180017d54:	add    (%rax),%al
-   180017d56:	rex.XB
-   180017d57:	rex.RX push %rbp
+   180017d4c:	(bad)
+   180017d4d:	jge    0x180017d50
+   180017d4f:	add    %al,(%rax)
+   180017d51:	add    %al,(%rcx)
+   180017d53:	add    %al,(%rdx)
+   180017d55:	add    %al,0x46(%rbx)
+   180017d58:	push   %rbp
    180017d59:	rex.WRX pop %rdi
    180017d5b:	imul   $0x5f,0x75(%rbx),%eax
    180017d5f:	push   %rdi
-   180017d60:	imul   $0x616d7265,0x64(%rbp),%esp
+   180017d60:	imul   $0x6e616d65,0x64(%rbp),%esp
    180017d67:	outsb  %ds:(%rsi),(%dx)
-   180017d68:	outsb  %ds:(%rsi),(%dx)
-   180017d69:	pop    %rdi
-   180017d6a:	jbe    0x180017d9d
-   180017d6c:	cs fs insb (%dx),%es:(%rdi)
-   180017d6f:	insb   (%dx),%es:(%rdi)
-   180017d70:	add    %ah,0x76(%rbp)
-   180017d73:	(bad)
-   180017d74:	insb   (%dx),%es:(%rdi)
-   180017d75:	add    %ah,0x65(%rdi)
-   180017d78:	je     0x180017dc6
-   180017d7a:	(bad)
-   180017d7b:	jae    0x180017df1
-   180017d7d:	rex.RB jb 0x180017df2
-   180017d80:	outsl  %ds:(%rsi),(%dx)
-   180017d81:	jb     0x180017d83
-   180017d83:	imul   $0x7db00074,0x69(%rsi),%ebp
-   180017d8a:	add    %eax,(%rax)
+   180017d68:	pop    %rdi
+   180017d69:	jbe    0x180017d9c
+   180017d6b:	cs fs insb (%dx),%es:(%rdi)
+   180017d6e:	insb   (%dx),%es:(%rdi)
+   180017d6f:	add    %ah,0x76(%rbp)
+   180017d72:	(bad)
+   180017d73:	insb   (%dx),%es:(%rdi)
+   180017d74:	add    %ah,0x65(%rdi)
+   180017d77:	je     0x180017dc5
+   180017d79:	(bad)
+   180017d7a:	jae    0x180017df0
+   180017d7c:	rex.RB jb 0x180017df1
+   180017d7f:	outsl  %ds:(%rsi),(%dx)
+   180017d80:	jb     0x180017d82
+   180017d82:	imul   $0xb0000074,0x69(%rsi),%ebp
+   180017d89:	jge    0x180017d8c
+	...
+   180017d93:	add    %al,-0x7f(%rax)
+   180017d96:	add    %eax,(%rax)
+   180017d98:	add    %dh,%al
 	...
-   180017d94:	rex addl $0xf00000,(%rcx)
-	...
-   180017daf:	add    %bh,%al
+   180017dae:	add    %al,(%rax)
+   180017db0:	clc
    180017db1:	jg     0x180017db4
    180017db3:	add    %al,(%rax)
    180017db5:	add    %al,(%rax)
    180017db7:	add    %dl,(%rdx)
    180017db9:	addb   $0x0,(%rcx)
    180017dbc:	add    %al,(%rax)
    180017dbe:	add    %al,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kCu_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kCu_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017ac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:00 2023
+Time/Date		Mon Apr 24 09:07:20 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fc00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017ac
@@ -37132,15 +37132,15 @@
    18001b43d:	add    %al,(%rax)
    18001b43f:	add    %dh,0x12(%rax)
    18001b442:	add    %eax,0x1(%rax)
    18001b448:	js     0x18001b45c
    18001b44a:	add    %eax,0x1(%rax)
    18001b450:	add    %al,(%rax)
    18001b452:	add    %al,(%rax)
-   18001b454:	rex cmp %al,0x64(%rcx)
+   18001b454:	enter  $0x4646,$0x64
    18001b458:	add    %al,(%rax)
    18001b45a:	add    %al,(%rax)
    18001b45c:	or     $0xc8000000,%eax
    18001b461:	add    (%rax),%al
    18001b463:	add    %ah,%ah
    18001b465:	mov    $0x1,%dh
    18001b467:	add    %ah,%ah
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kG10_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kG10_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001744
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:21 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001744
@@ -36490,16 +36490,18 @@
    18001b15d:	add    %al,(%rax)
    18001b15f:	add    %dh,0x12(%rax)
    18001b162:	add    %eax,0x1(%rax)
    18001b168:	js     0x18001b17c
    18001b16a:	add    %eax,0x1(%rax)
    18001b170:	add    %al,(%rax)
    18001b172:	add    %al,(%rax)
-   18001b174:	cmp    %al,0x64(%r9)
-   18001b178:	add    %al,(%rax)
+   18001b174:	leave
+   18001b175:	rex.RX
+   18001b176:	rex.RX
+   18001b177:	add    %al,%fs:(%rax)
    18001b17a:	add    %al,(%rax)
    18001b17c:	or     $0xc8000000,%eax
    18001b181:	add    (%rax),%al
    18001b183:	add    %ah,0x1(%rsp,%rsi,4)
    18001b187:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kHast_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kHast_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017c0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:22 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017c0
@@ -36546,16 +36546,16 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	cmp    %al,0x64(%r9)
-   18001b198:	add    %al,(%rax)
+   18001b194:	lret   $0x4646
+   18001b197:	add    %al,%fs:(%rax)
    18001b19a:	add    %al,(%rax)
    18001b19c:	or     $0xc8000000,%eax
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kHe_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kHe_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001f70
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:22 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001f70
@@ -36924,16 +36924,16 @@
    18001b1ad:	add    %al,(%rax)
    18001b1af:	add    %dh,0x12(%rax)
    18001b1b2:	add    %eax,0x1(%rax)
    18001b1b8:	js     0x18001b1cc
    18001b1ba:	add    %eax,0x1(%rax)
    18001b1c0:	add    %al,(%rax)
    18001b1c2:	add    %al,(%rax)
-   18001b1c4:	cmp    %al,0x64(%r9)
-   18001b1c8:	add    %al,(%rax)
+   18001b1c4:	lret   $0x4646
+   18001b1c7:	add    %al,%fs:(%rax)
    18001b1ca:	add    %al,(%rax)
    18001b1cc:	or     $0xc8000000,%eax
    18001b1d1:	add    (%rax),%al
    18001b1d3:	add    %ch,0x1(%rsp,%rsi,4)
    18001b1d7:	add    %ch,0x1(%rsi,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kKapton_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kKapton_v1.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017d4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:23 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017d4
@@ -36522,16 +36522,18 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	cmp    %al,0x64(%r9)
-   18001b198:	add    %al,(%rax)
+   18001b194:	lret
+   18001b195:	rex.RX
+   18001b196:	rex.RX
+   18001b197:	add    %al,%fs:(%rax)
    18001b19a:	add    %al,(%rax)
    18001b19c:	or     $0xc8000000,%eax
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rax,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kSteel_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kSteel_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017c0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:01 2023
+Time/Date		Mon Apr 24 09:07:23 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017c0
@@ -36485,16 +36485,18 @@
    18001b13d:	add    %al,(%rax)
    18001b13f:	add    %dh,0x12(%rax)
    18001b142:	add    %eax,0x1(%rax)
    18001b148:	js     0x18001b15c
    18001b14a:	add    %eax,0x1(%rax)
    18001b150:	add    %al,(%rax)
    18001b152:	add    %al,(%rax)
-   18001b154:	cmp    %al,0x64(%r9)
-   18001b158:	add    %al,(%rax)
+   18001b154:	lret
+   18001b155:	rex.RX
+   18001b156:	rex.RX
+   18001b157:	add    %al,%fs:(%rax)
    18001b15a:	add    %al,(%rax)
    18001b15c:	or     $0xc8000000,%eax
    18001b161:	add    (%rax),%al
    18001b163:	add    %ch,%ah
    18001b165:	mov    $0x1,%bl
    18001b167:	add    %ch,%ah
    18001b169:	popf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_kStycast_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_kStycast_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001dfc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:02 2023
+Time/Date		Mon Apr 24 09:07:24 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001dfc
@@ -36783,16 +36783,18 @@
    18001b1ad:	add    %al,(%rax)
    18001b1af:	add    %dh,0x12(%rax)
    18001b1b2:	add    %eax,0x1(%rax)
    18001b1b8:	js     0x18001b1cc
    18001b1ba:	add    %eax,0x1(%rax)
    18001b1c0:	add    %al,(%rax)
    18001b1c2:	add    %al,(%rax)
-   18001b1c4:	rex.X cmp %al,0x64(%rcx)
-   18001b1c8:	add    %al,(%rax)
+   18001b1c4:	int3
+   18001b1c5:	rex.RX
+   18001b1c6:	rex.RX
+   18001b1c7:	add    %al,%fs:(%rax)
    18001b1ca:	add    %al,(%rax)
    18001b1cc:	or     $0xc8000000,%eax
    18001b1d1:	add    (%rax),%al
    18001b1d3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1d7:	add    %ah,0x1(%rsi,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_quenchState_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_quenchState_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800015ec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:02 2023
+Time/Date		Mon Apr 24 09:07:25 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000de00
 SizeOfInitializedData	000000000000ce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000015ec
@@ -30941,16 +30941,17 @@
    1800168fd:	add    %al,(%rax)
    1800168ff:	add    %dh,-0xe(%rax)
    180016902:	add    %al,0x1(%rax)
    180016908:	js     0x1800168fc
    18001690a:	add    %al,0x1(%rax)
    180016910:	add    %al,(%rax)
    180016912:	add    %al,(%rax)
-   180016914:	rex.X cmp %al,0x64(%rcx)
-   180016918:	add    %al,(%rax)
+   180016914:	int    $0x46
+   180016916:	rex.RX
+   180016917:	add    %al,%fs:(%rax)
    18001691a:	add    %al,(%rax)
    18001691c:	or     $0xc8000000,%eax
    180016921:	add    (%rax),%al
    180016923:	add    %ah,%ah
    180016925:	imul   $0x0,(%rcx),%eax
    180016928:	in     $0x5d,%al
    18001692a:	add    %eax,(%rax)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001960
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:25 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001960
@@ -37144,16 +37144,17 @@
    18001b48d:	add    %al,(%rax)
    18001b48f:	add    %dh,0x12(%rax)
    18001b492:	add    %eax,0x1(%rax)
    18001b498:	js     0x18001b4ac
    18001b49a:	add    %eax,0x1(%rax)
    18001b4a0:	add    %al,(%rax)
    18001b4a2:	add    %al,(%rax)
-   18001b4a4:	rex.XB cmp %al,0x64(%r9)
-   18001b4a8:	add    %al,(%rax)
+   18001b4a4:	int    $0x46
+   18001b4a6:	rex.RX
+   18001b4a7:	add    %al,%fs:(%rax)
    18001b4aa:	add    %al,(%rax)
    18001b4ac:	or     $0xc8000000,%eax
    18001b4b1:	add    (%rax),%al
    18001b4b3:	add    %ah,0x1(%rdi,%rsi,4)
    18001b4b7:	add    %ah,0x1(%rcx,%rbp,4)
 	...
    18001b4ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001938
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001938
@@ -37151,16 +37151,18 @@
    18001b48d:	add    %al,(%rax)
    18001b48f:	add    %dh,0x12(%rax)
    18001b492:	add    %eax,0x1(%rax)
    18001b498:	js     0x18001b4ac
    18001b49a:	add    %eax,0x1(%rax)
    18001b4a0:	add    %al,(%rax)
    18001b4a2:	add    %al,(%rax)
-   18001b4a4:	rex.XB cmp %al,0x64(%r9)
-   18001b4a8:	add    %al,(%rax)
+   18001b4a4:	(bad)
+   18001b4a5:	rex.RX
+   18001b4a6:	rex.RX
+   18001b4a7:	add    %al,%fs:(%rax)
    18001b4aa:	add    %al,(%rax)
    18001b4ac:	or     $0xc8000000,%eax
    18001b4b1:	add    (%rax),%al
    18001b4b3:	add    %ah,0x1(%rdi,%rsi,4)
    18001b4b7:	add    %ah,0x1(%rcx,%rbp,4)
 	...
    18001b4ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002094
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		0000000000010000
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002094
@@ -36934,16 +36934,18 @@
    18001b1dd:	add    %al,(%rax)
    18001b1df:	add    %dh,0x12(%rax)
    18001b1e2:	add    %eax,0x1(%rax)
    18001b1e8:	js     0x18001b1fc
    18001b1ea:	add    %eax,0x1(%rax)
    18001b1f0:	add    %al,(%rax)
    18001b1f2:	add    %al,(%rax)
-   18001b1f4:	rex.XB cmp %al,0x64(%r9)
-   18001b1f8:	add    %al,(%rax)
+   18001b1f4:	(bad)
+   18001b1f5:	rex.RX
+   18001b1f6:	rex.RX
+   18001b1f7:	add    %al,%fs:(%rax)
    18001b1fa:	add    %al,(%rax)
    18001b1fc:	or     $0xc8000000,%eax
    18001b201:	add    (%rax),%al
    18001b203:	add    %ah,%ah
    18001b205:	mov    $0x1,%ah
    18001b207:	add    %ah,%ah
    18001b209:	test   $0x1,%al
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001aec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:27 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001aec
@@ -36632,16 +36632,18 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	rex.XB cmp %al,0x64(%r9)
-   18001b198:	add    %al,(%rax)
+   18001b194:	iret
+   18001b195:	rex.RX
+   18001b196:	rex.RX
+   18001b197:	add    %al,%fs:(%rax)
    18001b19a:	add    %al,(%rax)
    18001b19c:	or     $0xc8000000,%eax
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rdx,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001aec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:27 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fa00
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001aec
@@ -36635,16 +36635,18 @@
    18001b17d:	add    %al,(%rax)
    18001b17f:	add    %dh,0x12(%rax)
    18001b182:	add    %eax,0x1(%rax)
    18001b188:	js     0x18001b19c
    18001b18a:	add    %eax,0x1(%rax)
    18001b190:	add    %al,(%rax)
    18001b192:	add    %al,(%rax)
-   18001b194:	rex.XB cmp %al,0x64(%r9)
-   18001b198:	add    %al,(%rax)
+   18001b194:	iret
+   18001b195:	rex.RX
+   18001b196:	rex.RX
+   18001b197:	add    %al,%fs:(%rax)
    18001b19a:	add    %al,(%rax)
    18001b19c:	or     $0xc8000000,%eax
    18001b1a1:	add    (%rax),%al
    18001b1a3:	add    %ah,0x1(%rsp,%rsi,4)
    18001b1a7:	add    %ah,0x1(%rdx,%riz,4)
 	...
    18001b1ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800017c0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:03 2023
+Time/Date		Mon Apr 24 09:07:28 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000017c0
@@ -36481,16 +36481,16 @@
    18001b13d:	add    %al,(%rax)
    18001b13f:	add    %dh,0x12(%rax)
    18001b142:	add    %eax,0x1(%rax)
    18001b148:	js     0x18001b15c
    18001b14a:	add    %eax,0x1(%rax)
    18001b150:	add    %al,(%rax)
    18001b152:	add    %al,(%rax)
-   18001b154:	rex.XB cmp %al,0x64(%r9)
-   18001b158:	add    %al,(%rax)
+   18001b154:	rolb   0x46(%rsi)
+   18001b157:	add    %al,%fs:(%rax)
    18001b15a:	add    %al,(%rax)
    18001b15c:	or     $0xc8000000,%eax
    18001b161:	add    (%rax),%al
    18001b163:	add    %ch,%ah
    18001b165:	mov    $0x1,%bl
    18001b167:	add    %ch,%ah
    18001b169:	popf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001954
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:04 2023
+Time/Date		Mon Apr 24 09:07:28 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000fe00
 SizeOfInitializedData	000000000000fc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001954
@@ -37162,16 +37162,16 @@
    18001b48d:	add    %al,(%rax)
    18001b48f:	add    %dh,0x12(%rax)
    18001b492:	add    %eax,0x1(%rax)
    18001b498:	js     0x18001b4ac
    18001b49a:	add    %eax,0x1(%rax)
    18001b4a0:	add    %al,(%rax)
    18001b4a2:	add    %al,(%rax)
-   18001b4a4:	cmp    %r8b,0x64(%rcx)
-   18001b4a8:	add    %al,(%rax)
+   18001b4a4:	rolb   0x46(%rsi)
+   18001b4a7:	add    %al,%fs:(%rax)
    18001b4aa:	add    %al,(%rax)
    18001b4ac:	or     $0xc8000000,%eax
    18001b4b1:	add    (%rax),%al
    18001b4b3:	add    %ah,0x1(%rdi,%rsi,4)
    18001b4b7:	add    %ah,0x1(%rcx,%rbp,4)
 	...
    18001b4ff:	add    %al,(%rcx)
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001834
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:04 2023
+Time/Date		Mon Apr 24 09:07:29 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f800
 SizeOfInitializedData	000000000000f800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001834
@@ -36606,16 +36606,16 @@
    18001b14d:	add    %al,(%rax)
    18001b14f:	add    %dh,0x12(%rax)
    18001b152:	add    %eax,0x1(%rax)
    18001b158:	js     0x18001b16c
    18001b15a:	add    %eax,0x1(%rax)
    18001b160:	add    %al,(%rax)
    18001b162:	add    %al,(%rax)
-   18001b164:	cmp    %r8b,0x64(%rcx)
-   18001b168:	add    %al,(%rax)
+   18001b164:	roll   0x46(%rsi)
+   18001b167:	add    %al,%fs:(%rax)
    18001b16a:	add    %al,(%rax)
    18001b16c:	or     $0xc8000000,%eax
    18001b171:	add    (%rax),%al
    18001b173:	add    %ah,%ah
    18001b175:	mov    $0x1,%bl
    18001b177:	add    %ah,%ah
    18001b179:	lahf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll` & `STEAM_materials-2023.4.1/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001740
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 20 13:04:04 2023
+Time/Date		Mon Apr 24 09:07:29 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000f600
 SizeOfInitializedData	000000000000f600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001740
@@ -36521,16 +36521,16 @@
    18001b10d:	add    %al,(%rax)
    18001b10f:	add    %dh,0x12(%rax)
    18001b112:	add    %eax,0x1(%rax)
    18001b118:	js     0x18001b12c
    18001b11a:	add    %eax,0x1(%rax)
    18001b120:	add    %al,(%rax)
    18001b122:	add    %al,(%rax)
-   18001b124:	cmp    %r8b,0x64(%rcx)
-   18001b128:	add    %al,(%rax)
+   18001b124:	roll   0x46(%rsi)
+   18001b127:	add    %al,%fs:(%rax)
    18001b12a:	add    %al,(%rax)
    18001b12c:	or     $0xc8000000,%eax
    18001b131:	add    (%rax),%al
    18001b133:	add    %ch,%ah
    18001b135:	mov    $0x1,%bl
    18001b137:	add    %ch,%ah
    18001b139:	popf
```

### Comparing `STEAM_materials-2023.4.0/src/steammaterials/STEAM_materials.py` & `STEAM_materials-2023.4.1/src/steammaterials/STEAM_materials.py`

 * *Files identical despite different names*


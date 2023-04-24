# Comparing `tmp/lowatt-enedis-2.0.0.tar.gz` & `tmp/lowatt-enedis-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lowatt-enedis-2.0.0.tar", last modified: Thu Feb  3 09:04:17 2022, max compression
+gzip compressed data, was "lowatt-enedis-2.1.0.tar", last modified: Mon Apr 24 09:14:40 2023, max compression
```

## Comparing `lowatt-enedis-2.0.0.tar` & `lowatt-enedis-2.1.0.tar`

### file list

```diff
@@ -1,142 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)    34619 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/test/test_lowatt_enedis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/test/data/consulterMesuresDetailleesResponse.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/test/data/consulterMesuresResponse.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    37212 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    38245 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    37212 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    38245 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    37450 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    38452 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    36631 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    37127 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    40590 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    36163 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    36631 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    37127 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (121)    11723 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    37450 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    38416 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    37450 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    38224 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    23914 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/certauth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11404 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/lowatt_enedis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 09:04:17.000000 lowatt-enedis-2.0.0/lowatt_enedis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-02-03 09:04:06.000000 lowatt-enedis-2.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.589472 lowatt-enedis-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    34619 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/certauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28507 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.589472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38416 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40590 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-24 09:14:40.613472 lowatt-enedis-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/consulterMesuresDetailleesResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/consulterMesuresResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    74247 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/test_lowatt_enedis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lowatt-enedis-2.0.0/.github/workflows/tox.yml` & `lowatt-enedis-2.1.0/.github/workflows/tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
           - tox_env: check-manifest
           - tox_env: lint
-          - tox_env: py37
-          - tox_env: py38
           - tox_env: py39
+          - tox_env: py310
+          - tox_env: py311
 
     steps:
       - uses: actions/checkout@v2
       - name: Find python version
         id: py_ver
         shell: python
         if: ${{ contains(matrix.tox_env, 'py') }}
@@ -60,18 +60,18 @@
     runs-on: ubuntu-latest
 
     env:
       PY_COLORS: 1
       TOXENV: packaging
 
     steps:
-      - name: Switch to using Python 3.6 by default
+      - name: Switch to using Python 3.9 by default
         uses: actions/setup-python@v2
         with:
-          python-version: 3.6
+          python-version: 3.9
       - name: Install tox
         run: python -m pip install --user tox
       - name: Check out src from Git
         uses: actions/checkout@v2
         with:
           # Get shallow Git history (default) for release events
           # but have a complete clone for any other workflows.
```

### Comparing `lowatt-enedis-2.0.0/COPYING` & `lowatt-enedis-2.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/setup.py` & `lowatt-enedis-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/setup.cfg` & `lowatt-enedis-2.1.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -4,38 +4,44 @@
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Lowatt
 author_email = info@lowatt.fr
 url = https://github.com/lowatt/lowatt-enedis
 license = GPL3
 classifiers = 
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Topic :: System :: Archiving :: Mirroring
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 setup_requires = 
 	setuptools_scm
-python_requires = >=3.7
+python_requires = >=3.9
 packages = find:
 install_requires = 
 	python-dateutil
 	suds-py3
-	typing-extensions
 include_package_data = True
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
+	lxml
+	freezegun
+	pyyaml
 typing = 
 	mypy
 	types-python-dateutil
 	types-setuptools
+	types-freezegun
+	types-PyYAML
 
 [options.entry_points]
 console_scripts = 
 	lowatt-enedis = lowatt_enedis.__main__:run
 
 [egg_info]
 tag_build =
```

### Comparing `lowatt-enedis-2.0.0/test/test_lowatt_enedis.py` & `lowatt-enedis-2.1.0/test/test_lowatt_enedis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,40 @@
+import argparse
 import contextlib
 import datetime
 import io
 import os
 import sys
-from dataclasses import dataclass
+from typing import Iterator
 
 import pkg_resources
 import pytest
+import suds.sudsobject
 from suds.client import Client, SoapClient
 
 import lowatt_enedis as le
 import lowatt_enedis.services  # noqa: register services
 
 
-@dataclass(init=True)
-class args:
-    cert_file = None
-    key_file = None
-    login = "bob"
-    homologation = False
-    output = "print"
+def args() -> argparse.Namespace:
+    return argparse.Namespace(
+        cert_file=None, key_file=None, login="bob", homologation=False, output="print"
+    )
 
 
 @contextlib.contextmanager
-def override_sys_argv(argv):
+def override_sys_argv(argv: list[str]) -> Iterator[None]:
     old, sys.argv = sys.argv, argv
     try:
         yield
     finally:
         sys.argv = old
 
 
-def test_introspection():
+def test_introspection() -> None:
     service = "RecherchePoint-v2.0"
     service_wsdl = le.wsdl(service)
     assert service_wsdl.endswith(".wsdl")
 
     client = Client(service_wsdl)
     xstype_map = le.build_xstypes_map(client)
     assert "CriteresType" in xstype_map
@@ -44,20 +43,24 @@
     assert prefix == "ns3"
 
     children_map = le.xstype_children_map(xstype)
     assert "numSiret" in children_map
     assert children_map["numSiret"].min == "0"
 
 
-def test_ws_decorator():
+def test_ws_decorator() -> None:
     service, options, handler = le.COMMAND_SERVICE["search"]
+    service_location = None
+    handler_called = False
 
     @le.register("testws", service, options)
     @le.ws(service)
-    def test_handler(client, args):
+    def test_handler(
+        client: Client, args: argparse.Namespace
+    ) -> suds.sudsobject.Object:
         nonlocal handler_called, service_location
 
         handler_called = True
 
         assert client.options.location is None
 
         headers = client.options.soapheaders
@@ -66,16 +69,14 @@
 
         for service in client.wsdl.services:
             for port in service.ports:
                 for method in port.methods.values():
                     assert service_location is None
                     service_location = method.location
 
-    handler_called = False
-    service_location = None
     le.handle_cli_command("testws", args())
     assert handler_called
     assert service_location == (b"https://sge-b2b.enedis.fr/RecherchePoint/v2.0")
 
     handler_called = False
     service_location = None
     # XXX args(homologation=True) didn't work as expected
@@ -84,50 +85,51 @@
     le.handle_cli_command("testws", _args)
     assert handler_called
     assert service_location == (
         b"https://sge-homologation-b2b.enedis.fr/RecherchePoint/v2.0"
     )
 
 
-def test_cli_help():
+def test_cli_help() -> None:
     entrypoint = pkg_resources.get_entry_info(
         "lowatt_enedis",
         "console_scripts",
         "lowatt-enedis",
     )
+    assert entrypoint is not None
     func = entrypoint.load()
     stdout = io.StringIO()
     with pytest.raises(SystemExit) as cm, override_sys_argv(
         ["lowatt-enedis", "--help"],
     ), contextlib.redirect_stdout(stdout):
         func()
     assert cm.value.code == 0
     output = stdout.getvalue()
     assert output.startswith("usage: ")
 
 
 DATA_DIR = os.path.join(os.path.dirname(__file__), "data")
 
 
-def test_detailed_measures_resp2py():
+def test_detailed_measures_resp2py() -> None:
     service, options, handler = le.COMMAND_SERVICE["details"]
     client = Client(le.wsdl(service))
     soap = SoapClient(client, client.service.consulterMesuresDetaillees.method)
     resp_file = os.path.join(DATA_DIR, "consulterMesuresDetailleesResponse.xml")
     with open(resp_file) as stream:
         resp = soap.succeeded(soap.method.binding.input, stream.read())
         data = list(le.services.detailed_measures_resp2py(resp))
         assert len(data) == 8
         assert data[0] == (
             datetime.datetime(2020, 2, 29, 23, tzinfo=le.services.UTC),
             100,
         )
 
 
-def test_measures_resp2py():
+def test_measures_resp2py() -> None:
     service, options, handler = le.COMMAND_SERVICE["measures"]
     client = Client(le.wsdl(service))
     soap = SoapClient(client, client.service.consulterMesures.method)
     resp_file = os.path.join(DATA_DIR, "consulterMesuresResponse.xml")
     with open(resp_file) as stream:
         resp = soap.succeeded(soap.method.binding.input, stream.read())
         data = list(le.services.measures_resp2py(resp))
```

### Comparing `lowatt-enedis-2.0.0/test/data/consulterMesuresDetailleesResponse.xml` & `lowatt-enedis-2.1.0/test/data/consulterMesuresDetailleesResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/test/data/consulterMesuresResponse.xml` & `lowatt-enedis-2.1.0/test/data/consulterMesuresResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/PKG-INFO` & `lowatt-enedis-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.0.0
+Version: 2.1.0
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: typing
 License-File: COPYING
 
 # lowatt-enedis
 
@@ -91,8 +92,10 @@
 ## Contributions
 
 Contribution are welcome through the [Github
 repository](https://github.com/lowatt/lowatt_enedis).
 
 Feel free to contact for more info by writing at info@lowatt.fr.
 
+## Sponsors
 
+[![QosEnergy](assets/qos-energy.png)](https://www.qosenergy.com/)
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/services.py` & `lowatt-enedis-2.1.0/lowatt_enedis/services.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,17 +17,21 @@
 """
 `lowatt_enedis.services`
 ------------------------
 
 SGE web-service mapping to plug them into the CLI.
 """
 
-from datetime import date, timedelta
+import argparse
+from datetime import date, datetime, timedelta
+from typing import Any, Iterator, Literal
 
+import suds.sudsobject
 from dateutil import tz
+from suds.client import Client
 
 from . import (
     arg_from_env,
     create_from_options,
     dict_from_dicts,
     get_option,
     register,
@@ -78,20 +82,20 @@
         },
         arg_from_env("ENEDIS_CONTRAT"),
     ),
 }
 
 
 def _accord_client(
-    client,
-    args,
-    extended=False,
-    xs_accord_type="ns3:DeclarationAccordClientType",
-    autorisation=True,
-):
+    client: Client,
+    args: argparse.Namespace,
+    extended: bool = False,
+    xs_accord_type: str = "ns3:DeclarationAccordClientType",
+    autorisation: bool = True,
+) -> suds.sudsobject.Object:
     if get_option(args, "denomination"):
         ptype = "Morale"
         who_options = {
             "denomination": "denominationSociale",
         }
         unavailable_options = {"prenom", "civilite"}
         if extended:
@@ -158,23 +162,25 @@
 MESURES_OPTIONS_MAP = {
     "from": "dateDebut",
     "to": "dateFin",
     "corrigee": "mesuresCorrigees",
 }
 
 
-def _pas(client, args, demande):
+def _pas(
+    client: Client, args: argparse.Namespace, demande: suds.sudsobject.Object
+) -> None:
     pas = get_option(args, "pas")
     if pas:
         demande.pasCdc = client.factory.create("ns1:DureeType")
         demande.pasCdc.unite = "min"
         demande.pasCdc.valeur = pas
 
 
-def _check_mesure_options_consistency(args):
+def _check_mesure_options_consistency(args: argparse.Namespace) -> None:
     if get_option(args, "pas") and get_option(args, "type") != "CDC":
         raise ValueError(
             "L'option 'pas' ne peut être  spécifiée que pour le type de "
             "mesure 'courbe de charge' (CDC).",
         )
 
 
@@ -220,28 +226,29 @@
         },
         "--insee": {
             "help": "code INSEE de la commune",
         },
     },
 )
 @ws("RecherchePoint-v2.0")
-def search_point(client, args):
+def search_point(client: Client, args: argparse.Namespace) -> suds.sudsobject.Object:
     criteria = create_from_options(
         client,
         args,
         "CriteresType",
         {
             "siret": "numSiret",
             "compteur": "matriculeOuNumeroSerie",
             "tension": "domaineTensionAlimentationCode",
             "nom": "nomClientFinalOuDenominationSociale",
             "categorie": "categorieClientFinalCode",
             "hp": "rechercheHorsPerimetre",
         },
     )
+    assert criteria is not None
     address = create_from_options(
         client,
         args,
         "AdresseInstallationType",
         {
             "etage": "escalierEtEtageEtAppartement",
             "batiment": "batiment",
@@ -267,15 +274,17 @@
             "help": "indique l'autorisation du client",
             "action": "store_true",
             "default": False,
         },
     },
 )
 @ws("ConsultationDonneesTechniquesContractuelles-v1.0")
-def point_technical_data(client, args):
+def point_technical_data(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     return client.service.consulterDonneesTechniquesContractuelles(
         get_option(args, "prm"),
         get_option(args, "login"),
         _boolean(get_option(args, "autorisation")),
     )
 
 
@@ -293,28 +302,28 @@
                 "default": False,
             },
         },
         CONTRAT_OPTIONS,
     ),
 )
 @ws("ConsultationMesures-v1.1")
-def point_measures(client, args):
+def point_measures(client: Client, args: argparse.Namespace) -> suds.sudsobject.Object:
     return client.service.consulterMesures(
         get_option(args, "prm"),
         get_option(args, "login"),
         get_option(args, "contrat"),
         _boolean(get_option(args, "autorisation")),
     )
 
 
-def parse_date(value):
+def parse_date(value: str) -> date:
     return date(*(int(part) for part in value.split("-")))
 
 
-def measures_resp2py(resp):
+def measures_resp2py(resp: suds.sudsobject.Object) -> Iterator[dict[str, Any]]:
     """Return a list of dictionaries given a response from
     ConsultationMesures web-service. Each dict contains the following keys:
     - `grille`: "frn" or "turpe",
     - `grandeurPhysique`: "EA" for active energy,
     - `classeTemporelle`: eg. "BASE", "HP", "HC",
     - `calendrier`: calendar id,
     - `unit`: "kWh",
@@ -398,28 +407,31 @@
                 "help": "demander sans l'autorisation du client (pour l'homologation seulement)",
             },
         },
         MESURES_OPTIONS,
     ),
 )
 @ws("ConsultationMesuresDetaillees-v2.0", header_ns_prefix="ns2")
-def point_detailed_measures(client, args):
+def point_detailed_measures(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     demande = create_from_options(
         client,
         args,
         "DemandeType",
         dict_from_dicts(
             {
                 "login": "initiateurLogin",
                 "prm": "pointId",
                 "type": "mesuresTypeCode",
             },
             MESURES_OPTIONS_MAP,
         ),
     )
+    assert demande is not None
     # demande.mesuresPas uniquement pour PMAX sur C5N, valeur P1D ou P1M
     if get_option(args, "type") == "PMAX":
         demande.grandeurPhysique = "PMA"
         demande.mesuresPas = "P1D"  # 'P1M'
     else:
         del demande.mesuresPas
         if get_option(args, "type") == "ENERGIE":
@@ -435,42 +447,126 @@
     demande.soutirage = _boolean(not injection)
     demande.injection = _boolean(injection)
     demande.accordClient = _boolean(not get_option(args, "no_autorisation"))
 
     return client.service.consulterMesuresDetaillees(demande)
 
 
-def detailed_measures_resp2py(resp):
+@register(
+    "detailsV3",
+    "ConsultationMesuresDetaillees-v3.0",
+    dict_from_dicts(
+        {
+            "prm": {
+                "help": "identifiant PRM du point",
+            },
+            "type": {
+                "choices": ["ENERGIE", "PMAX", "COURBE", "INDEX"],
+                "help": "type de mesure demandé : ENERGIE pour les consommations "
+                "globales quotidiennes, PMAX pour les puissances maximales "
+                "quotidiennes, COURBE pour la courbe de charge.",
+            },
+            "--courbe-type": {
+                # - PA pour récupérer les courbes de puissance active (seule
+                #   courbe disponible pour les segments C5 et P4)
+                # - PRI pour récupérer les courbes de puissance réactive
+                #   inductive
+                # - PRC pour récupérer les courbes de puissance réactive
+                #   capacitive
+                # - E pour récupérer les courbes de tension
+                # - TOUT pour récupérer les courbes disponibles
+                "choices": ["PA", "PRI", "PRC", "E", "TOUT"],
+                "default": "PA",
+                "help": "type de courbe demandé le cas échéant (Puissance Active, "
+                "Puissance Réactive Inductive, Puissance Réactive Capacitive, "
+                "tension (E), tout).",
+            },
+            "--injection": {
+                "action": "store_true",
+                "help": "demander les données en injection (soutirage par défaut).",
+            },
+            "--cadre": {
+                "choices": ["ACCORD_CLIENT", "SERVICE_ACCES", "EST_TITULAIRE"],
+                "default": "ACCORD_CLIENT",
+                "help": "Cadre d'accès à la demande, ACCORD_CLIENT par défaut.",
+            },
+        },
+        MESURES_OPTIONS,
+    ),
+)
+@ws("ConsultationMesuresDetaillees-v3.0", header_ns_prefix="ns2")
+def point_detailed_measuresV3(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
+    demande = create_from_options(
+        client,
+        args,
+        "Demande",
+        dict_from_dicts(
+            {
+                "login": "initiateurLogin",
+                "prm": "pointId",
+                "type": "mesuresTypeCode",
+            },
+            MESURES_OPTIONS_MAP,
+        ),
+    )
+    assert demande is not None
+    # demande.mesuresPas uniquement pour PMAX sur C5N, valeur P1D ou P1M
+    if get_option(args, "type") == "PMAX":
+        demande.grandeurPhysique = "PMA"
+        demande.mesuresPas = "P1D"  # 'P1M'
+    else:
+        del demande.mesuresPas
+        if get_option(args, "type") in ("ENERGIE", "INDEX"):
+            demande.grandeurPhysique = "EA"
+        elif get_option(args, "type") == "COURBE":
+            courbe_type = get_option(args, "courbe_type")
+            if not courbe_type:
+                raise ValueError(
+                    "l'option courbe-type doit être spécifié pour le type de mesure COURBE",
+                )
+            demande.grandeurPhysique = courbe_type
+    injection = get_option(args, "injection")
+    demande.sens = "INJECTION" if injection else "SOUTIRAGE"
+    demande.cadreAcces = get_option(args, "cadre")
+    return client.service.consulterMesuresDetailleesV3(demande)
+
+
+def detailed_measures_resp2py(
+    resp: suds.sudsobject.Object,
+) -> Iterator[tuple[datetime, float]]:
     """Return an iterator on (UTC tz naive datetime, value) given a response from
     ConsultationMesuresDetaillees web-service.
     """
     # start = resp.periode.dateDebut
     # end = resp.periode.dateFin
     assert len(resp.grandeur) == 1
     for point in resp.grandeur[0].mesure:
         yield (point.d.astimezone(UTC), point.v)
 
 
 def _donnees_generales(
-    client,
-    args,
-    code,
-    tag_name,
-):
+    client: Client,
+    args: argparse.Namespace,
+    code: str,
+    tag_name: str,
+) -> suds.sudsobject.Object:
     obj = create_from_options(
         client,
         args,
         tag_name,
         {
             # XXX missing: refFrn, refFrnRegroupement, affaireLieeId
             "contrat": "contratId",
             "prm": "pointId",
             "login": "initiateurLogin",
         },
     )
+    assert obj is not None
     obj.objetCode = code
     return obj
 
 
 DONNEES_GENERALES_OPTIONS = dict_from_dicts(
     {
         "prm": {
@@ -507,15 +603,15 @@
                 "default": (date.today() - timedelta(days=365 * 2)).isoformat(),
                 "help": "date de début souhaitée",
             },
         },
     ),
 )
 @ws("CommandeTransmissionHistoriqueMesures-v1.0", header_ns_prefix="ns1")
-def point_cmd_histo(client, args):
+def point_cmd_histo(client: Client, args: argparse.Namespace) -> suds.sudsobject.Object:
     _check_mesure_options_consistency(args)
 
     header = client.options.soapheaders
     header.infoFonctionnelles = client.factory.create("ns1:infoFonctionnelles")
     header.infoFonctionnelles.pointId = get_option(args, "prm")
     del header.infoFonctionnelles.affaireId
 
@@ -536,14 +632,15 @@
             MESURES_OPTIONS_MAP,
             {
                 "type": "mesureType",
                 "corrigee": "mesureCorrigee",  # override mesuresCorrigees
             },
         ),
     )
+    assert demande.historiqueMesures is not None
     _pas(client, args, demande.historiqueMesures)
     demande.historiqueMesures.declarationAccordClient = _accord_client(
         client,
         args,
         True,
         "ns0:DeclarationConsentementType",
     )
@@ -580,15 +677,17 @@
                 "help": "demander les paramètres de tarification dynamique.",
             },
         },
         ACCORD_CLIENT_OPTIONS,
     ),
 )
 @ws("CommandeTransmissionDonneesInfraJ-v1.0")
-def point_cmd_infra_j(client, args):
+def point_cmd_infra_j(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     demande = client.factory.create("ns1:DemandeType")
 
     demande.donneesGenerales = _donnees_generales(
         client,
         args,
         "AME",
         "DonneesGeneralesType",
@@ -602,22 +701,23 @@
             "injection": "injection",
             "soutirage": "soutirage",
             "cdc": "cdc",
             "idx": "idx",
             "ptd": "ptd",
         },
     )
+    assert demande.accesDonnees is not None
     demande.accesDonnees.declarationAccordClient = accord = _accord_client(
         client,
         args,
         xs_accord_type="ns1:DeclarationAccordClientType",
         autorisation=not get_option(args, "no_autorisation"),
     )
-    accord.injection = _boolean(False)
-    accord.soutirage = _boolean(False)
+    accord.injection = _boolean(get_option(args, "injection"))
+    accord.soutirage = _boolean(get_option(args, "soutirage"))
     return client.service.commanderTransmissionDonneesInfraJ(demande)
 
 
 @register(
     "subscribe",
     "CommandeCollectePublicationMesures-v3.0",
     dict_from_dicts(
@@ -666,15 +766,17 @@
                 "supérieure à la date de fin précédente lors d’un renouvellement, "
                 "un an max pour les compteurs linky",
             },
         },
     ),
 )
 @ws("CommandeCollectePublicationMesures-v3.0")
-def point_cmd_publication(client, args):
+def point_cmd_publication(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     demande = client.factory.create("ns1:DemandeType")
 
     demande.donneesGenerales = _donnees_generales(
         client,
         args,
         "AME",
         "DonneesGeneralesType",
@@ -682,22 +784,24 @@
 
     demande.accesMesures = acces = create_from_options(
         client,
         args,
         "DemandeAccesMesures",
         dict_from_dicts(MESURES_OPTIONS_MAP),
     )
+    assert demande.accesMesures is not None
+    assert acces is not None
 
     supported_actions = ["cdc_enable", "cdc", "idx"]
-    action = [a for a in supported_actions if get_option(args, a)]
+    actions = [a for a in supported_actions if get_option(args, a)]
 
-    if not action or len(action) > 1:
+    if not actions or len(actions) > 1:
         raise ValueError(f"Une action doit être selectionnée parmi {supported_actions}")
 
-    action = action[0]
+    action = actions[0]
 
     if action == "idx":
         code = "IDX"
         transmission = True
         pas = "P1D"
         period = "P1D"
     else:
@@ -739,15 +843,17 @@
 
 @register(
     "subscriptions",
     "RechercherServicesSouscritsMesures-v1.0",
     DONNEES_GENERALES_OPTIONS,
 )
 @ws("RechercherServicesSouscritsMesures-v1.0")
-def point_search_subscriptions(client, args):
+def point_search_subscriptions(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     criteria = create_from_options(
         client,
         args,
         "CriteresType",
         {
             "contrat": "contratId",
             "prm": "pointId",
@@ -769,15 +875,17 @@
             "--id": {
                 "help": "identifiant du service souscrit de mesures à arrêter",
             },
         },
     ),
 )
 @ws("CommandeArretServiceSouscritMesures-v1.0")
-def point_unsubscribe(client, args):
+def point_unsubscribe(
+    client: Client, args: argparse.Namespace
+) -> suds.sudsobject.Object:
     demande = client.factory.create("ns1:DemandeType")
 
     demande.donneesGenerales = _donnees_generales(
         client,
         args,
         "ASS",
         "DonneesGeneralesType",
@@ -789,9 +897,9 @@
         "ArretServiceSouscritType",
         {"id": "serviceSouscritId"},
     )
 
     return client.service.commanderArretServiceSouscritMesures(demande)
 
 
-def _boolean(b):
+def _boolean(b: Any) -> Literal["true", "false"]:
     return "true" if b else "false"
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/certauth.py` & `lowatt-enedis-2.1.0/lowatt_enedis/certauth.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 .. autoclass:: HTTPSClientCertTransport
 
 .. _SUDS: https://suds-py3.readthedocs.io/en/latest
 
 """
 
 import ssl
-from http.client import HTTPSConnection
-from urllib.request import HTTPSHandler, build_opener
+from http.client import HTTPResponse, HTTPSConnection
+from typing import Any
+from urllib.request import HTTPSHandler, Request, build_opener
 
 from suds.transport.http import HttpTransport
 
 
 class _HTTPSClientAuthHandler(HTTPSHandler):
-    def __init__(self, cert_file, key_file):
+    def __init__(self, cert_file: str, key_file: str):
         super().__init__()
         self.cert_file = cert_file
         self.key_file = key_file
 
-    def https_open(self, req):
-        return self.do_open(self.get_connection, req)
+    def https_open(self, req: Request) -> HTTPResponse:
+        return self.do_open(self.get_connection, req)  # type: ignore[arg-type]
 
-    def get_connection(self, host, timeout=300):
+    def get_connection(self, host: str, timeout: int = 300) -> HTTPSConnection:
         context = ssl.SSLContext()
         context.load_cert_chain(self.cert_file, self.key_file)
         return HTTPSConnection(host, context=context)
 
 
 class HTTPSClientCertTransport(HttpTransport):  # type: ignore[misc]
     """SUDS_ transport class to connect through an HTTPS connection using
@@ -63,20 +64,20 @@
             service_url,
             transport=HTTPSClientCertTransport(cert_file, key_file),
         )
 
     .. _SUDS: https://suds-py3.readthedocs.io/en/latest
     """
 
-    def __init__(self, cert_file, key_file, *args, **kwargs):
+    def __init__(self, cert_file: str, key_file: str, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.url_open = build_opener(
             _HTTPSClientAuthHandler(cert_file, key_file),
         ).open
 
-    def u2open(self, u2request):
+    def u2open(self, u2request: Request) -> HTTPResponse:
         """Open an return a connection.
 
         :param u2request: A urllib2 request.
         :return: The opened file-like urllib2 object.
         """
-        return self.url_open(u2request, timeout=self.options.timeout)
+        return self.url_open(u2request, timeout=self.options.timeout)  # type: ignore[no-any-return]
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/__main__.py` & `lowatt-enedis-2.1.0/lowatt_enedis/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with lowatt_enedis.  If not, see <https://www.gnu.org/licenses/>.
 import argparse
 import sys
+from typing import NoReturn
 
 from suds.client import Client
 
 import lowatt_enedis.services  # noqa: register services
 from lowatt_enedis import (
     COMMAND_SERVICE,
     WSException,
     handle_cli_command,
     init_cli,
     wsdl,
 )
 
 
-def _cli_parser():
+def _cli_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="CLI access to Enedis SGE web-services.",
     )
 
     subparsers = parser.add_subparsers(dest="command")
     init_cli(subparsers)
 
@@ -45,15 +46,15 @@
         "service_command",
         help="Command name.",
     )
 
     return parser
 
 
-def run():
+def run() -> NoReturn:
     parser = _cli_parser()
     args = parser.parse_args()
 
     if args.command == "wsdl":
         try:
             service_name = COMMAND_SERVICE[args.service_command][0]
         except KeyError:
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis/__init__.py` & `lowatt-enedis-2.1.0/lowatt_enedis/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,67 +17,64 @@
 """
 `lowatt_enedis`
 ---------------
 
 Command line interface to enedis SGE web-services.
 """
 
+import argparse
 import datetime
 import json
 import logging
 import os
 import sys
 from functools import wraps
 from pathlib import Path, PurePath
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Callable, Iterator, Optional, TypeVar, Union
 
 import suds.sudsobject
 from suds import WebFault
 from suds.client import Client
 from suds.plugin import DocumentPlugin
-from typing_extensions import TypedDict
 
 from .certauth import HTTPSClientCertTransport
 
+RT = TypeVar("RT")
+
 logging.basicConfig(level=logging.INFO)
 # logging.getLogger('suds.client').setLevel(logging.DEBUG)
 # logging.getLogger('suds.resolver').setLevel(logging.DEBUG)
 # logging.getLogger('suds.mx').setLevel(logging.DEBUG)
 # logging.getLogger('suds.transport').setLevel(logging.DEBUG)
 
 
 WSDL_DIR = PurePath(__file__).parent.joinpath("wsdl")
 SERVICES = {x.stem: x.resolve().as_uri() for x in Path(WSDL_DIR).glob("**/*.wsdl")}
-COMMAND_SERVICE: Dict[str, Tuple[str, Dict[str, Any], Any]] = {}
+COMMAND_SERVICE: dict[str, tuple[str, dict[str, Any], Any]] = {}
 
 
-def wsdl(service_name):
+def wsdl(service_name: str) -> str:
     """Return path to WSDL file for `service_name`."""
     try:
         return SERVICES[service_name]
     except KeyError:
         raise KeyError(
             "Unknown service name {!r}, available services are {}".format(
                 service_name,
                 ", ".join(sorted(SERVICES)),
             ),
         ) from None
 
 
-class ArgFromEnv(TypedDict):
-    default: Optional[str]
-    required: bool
-
-
-def arg_from_env(key: str) -> ArgFromEnv:
+def arg_from_env(key: str) -> dict[str, Any]:
     default = os.environ.get(key)
     return {"default": default, "required": not default}
 
 
-def init_cli(subparsers):
+def init_cli(subparsers: Any) -> None:
     """Init CLI subparsers according to registered services."""
     for command, (service, options, _) in COMMAND_SERVICE.items():
         subparser = subparsers.add_parser(
             command,
             help='Query the "{}" web-service.'.format(service),
         )
         subparser.add_argument(
@@ -118,28 +115,32 @@
     if isinstance(obj, suds.sudsobject.Object):
         return suds.sudsobject.asdict(obj)
     elif isinstance(obj, (datetime.date, datetime.datetime)):
         return obj.isoformat()
     raise TypeError(f"Object {obj!r} is not JSON serializable")
 
 
-def handle_cli_command(command, args):
+def handle_cli_command(command: str, args: argparse.Namespace) -> None:
     """Run `command` service using configuration in `args`."""
     service, _, handler = COMMAND_SERVICE[command]
     client = get_client(service, args.cert_file, args.key_file, args.homologation)
     obj = handler(client, args)
     if args.output == "xml":
-        print(client.last_received().str())  # noqa: T001
+        print(client.last_received().str())  # noqa: T201
     elif args.output == "json":
-        json.dump(obj, sys.stdout, indent=2, default=json_encode_default)
+        json.dump(
+            obj, sys.stdout, indent=2, default=json_encode_default, sort_keys=True
+        )
     else:
-        print(obj)  # noqa: T001
+        print(obj)  # noqa: T201
 
 
-def get_client(service, cert_file, key_file, homologation=False):
+def get_client(
+    service: str, cert_file: str, key_file: str, homologation: bool = False
+) -> Client:
     # Need custom plugin to handle `xs:choice` potentially expected in service
     # arguments. Non-handling this seems to be an outstanding suds bug, see
     # https://stackoverflow.com/questions/5963404/suds-and-choice-tag
     client = Client(
         wsdl(service),
         plugins=[_SetChoicePlugin()],
         transport=HTTPSClientCertTransport(cert_file, key_file),
@@ -170,61 +171,65 @@
                 b"/sge-homologation-b2b.",
             )
 
     return client
 
 
 class _SetChoicePlugin(DocumentPlugin):  # type: ignore[misc]
-    def __init__(self):
+    def __init__(self) -> None:
         self.choosen_tags = {"autorisationClient"}
 
-    def parsed(self, context):
+    def parsed(self, context: suds.plugin.DocumentContext) -> None:
         self._rec_set_choices(context.document)
 
-    def _rec_set_choices(self, document):
+    def _rec_set_choices(self, document: suds.sax.element.Element) -> None:
         for i in document.children:
             if i.name == "choice":
                 for j in i.children:
                     if j.getAttribute("name").value in self.choosen_tags:
                         i.parent.append(j)
 
             else:
                 # recursion
                 self._rec_set_choices(i)
 
 
-def register(command, service, options):
+def register(
+    command: str, service: str, options: dict[str, Any]
+) -> Callable[[Callable[..., RT]], Callable[..., RT]]:
     """Decorator registering function as a service handler for CLI `command`,
     matching `service` web-service name, accepting `options` (list of dict given
     to `argparse.ArgumentParser.add_argument`)
 
     """
 
-    def decorator(func):
+    def decorator(func: Callable[..., RT]) -> Callable[..., RT]:
         COMMAND_SERVICE[command] = (service, options, func)
         return func
 
     return decorator
 
 
 class WSException(Exception):
     pass
 
 
-def ws(service, header_ns_prefix="ns4"):
+def ws(
+    service: str, header_ns_prefix: str = "ns4"
+) -> Callable[[Callable[..., RT]], Callable[..., RT]]:
     """Decorator around sge web service call, returning a wrapper that properly set
     SOAP headers required by the service
 
     """
 
-    def decorator(func):
+    def decorator(func: Callable[..., RT]) -> Callable[..., RT]:
         service_version = service.split("-")[1][1:]
 
         @wraps(func)
-        def call_service(client, args):
+        def call_service(client: Client, args: argparse.Namespace) -> RT:
             client.xstypes_map = build_xstypes_map(client)
             header = client.factory.create("{}:entete".format(header_ns_prefix))
             header.version = service_version
             header.infoDemandeur = client.factory.create(
                 "{}:infoDemandeur".format(header_ns_prefix),
             )
             header.infoDemandeur.loginDemandeur = get_option(args, "login")
@@ -245,15 +250,20 @@
                     raise WSException("{}: {}".format(res._code, res.value))
 
         return call_service
 
     return decorator
 
 
-def create_from_options(client, args, xstype_name, options_map):
+def create_from_options(
+    client: Client,
+    args: argparse.Namespace,
+    xstype_name: str,
+    options_map: dict[str, str],
+) -> Optional[suds.sudsobject.Object]:
     """Create and return an `xstype_name` element, and fill it according to
     `options_map` {arg name: xs element name}` mapping by looking for value in
     command line `args`.
 
     """
     xstype, prefix = client.xstypes_map[xstype_name]
     children_map = xstype_children_map(xstype)
@@ -284,22 +294,24 @@
             raise ValueError("Expecting a value for {}".format(option))
 
     if has_value:
         return instance
     return None
 
 
-def get_option(args, option):
+def get_option(args: Union[dict[str, Any], argparse.Namespace], option: str) -> Any:
     if isinstance(args, dict):
         return args.get(option, None)
     else:
         return getattr(args, option)
 
 
-def build_xstypes_map(client):
+def build_xstypes_map(
+    client: Client,
+) -> dict[str, tuple[suds.xsd.sxbase.SchemaObject, str]]:
     """Return a dictionary of type names defined in the XML schema (without
     namespace nor prefix), associated to 2-uple `(type object, prefix)`.
 
     """
     assert len(client.sd) == 1, "More than one service: {}".format(client.sd)
 
     xstypes_map = {}
@@ -311,35 +323,37 @@
         prefix = service_def.getprefix(ns)
         assert xstype.name not in xstypes_map
         xstypes_map[xstype.name] = (xstype, prefix)
 
     return xstypes_map
 
 
-def xstype_children_map(xstype):
+def xstype_children_map(
+    xstype: suds.xsd.sxbase.SchemaObject,
+) -> dict[str, suds.xsd.sxbasic.Element]:
     """Return a dictionary of children tags for xstype, without namespace nor
     prefix.
 
     """
     children_map = {}
     for element, _ in xstype.children():
         children_map[element.name] = element
 
     return children_map
 
 
-def iter_methods(client):
+def iter_methods(client: Client) -> Iterator[suds.sudsobject.Facade]:
     """Return an iterator on exposerd methods suds instances."""
     for service in client.wsdl.services:
         for port in service.ports:
             for method in port.methods.values():
                 yield method
 
 
-def dict_from_dicts(*dicts):
+def dict_from_dicts(*dicts: dict[str, Any]) -> dict[str, Any]:
     """Build a dictionary from multiple dictionaries. In case of key conflict, the
     latest one wins.
 
     """
     result = {}
     for d in dicts:
         result.update(d)
```

### Comparing `lowatt-enedis-2.0.0/tox.ini` & `lowatt-enedis-2.1.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 basepython=python3
 skip_install = true
 deps =
   black
   flake8
   flake8-bugbear
   flake8-builtins
-  flake8-commas
   flake8-comprehensions
   flake8-debugger
   flake8-logging-format
   flake8-rst-docstrings
   flake8-pep3101
   flake8-string-format
   isort
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis.egg-info/PKG-INFO` & `lowatt-enedis-2.1.0/lowatt_enedis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.0.0
+Version: 2.1.0
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: typing
 License-File: COPYING
 
 # lowatt-enedis
 
@@ -91,8 +92,10 @@
 ## Contributions
 
 Contribution are welcome through the [Github
 repository](https://github.com/lowatt/lowatt_enedis).
 
 Feel free to contact for more info by writing at info@lowatt.fr.
 
+## Sponsors
 
+[![QosEnergy](assets/qos-energy.png)](https://www.qosenergy.com/)
```

### Comparing `lowatt-enedis-2.0.0/lowatt_enedis.egg-info/SOURCES.txt` & `lowatt-enedis-2.1.0/lowatt_enedis.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 lowatt_enedis/services.py
 lowatt_enedis.egg-info/PKG-INFO
 lowatt_enedis.egg-info/SOURCES.txt
 lowatt_enedis.egg-info/dependency_links.txt
 lowatt_enedis.egg-info/entry_points.txt
 lowatt_enedis.egg-info/requires.txt
 lowatt_enedis.egg-info/top_level.txt
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
 lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
 lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
@@ -49,14 +55,18 @@
 lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
 lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
 lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
 lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
 lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
 lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
 lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
+lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
+lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
+lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
 lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
 lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
 lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
 lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
 lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
 lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
 lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
@@ -65,10 +75,13 @@
 lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
 lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
 lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
 lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
 lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
 lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
 lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
+test/conftest.py
 test/test_lowatt_enedis.py
+test/test_requests.py
 test/data/consulterMesuresDetailleesResponse.xml
-test/data/consulterMesuresResponse.xml
+test/data/consulterMesuresResponse.xml
+test/data/requests.yaml
```

### Comparing `lowatt-enedis-2.0.0/README.md` & `lowatt-enedis-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,7 +71,11 @@
 
 ## Contributions
 
 Contribution are welcome through the [Github
 repository](https://github.com/lowatt/lowatt_enedis).
 
 Feel free to contact for more info by writing at info@lowatt.fr.
+
+## Sponsors
+
+[![QosEnergy](assets/qos-energy.png)](https://www.qosenergy.com/)
```

### Comparing `lowatt-enedis-2.0.0/.flake8` & `lowatt-enedis-2.1.0/.flake8`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 [flake8]
 #format = pylint
 ignore =
-  A003, # attribute overriding builtin name
-  B006, # [bugbear] Do not use mutable data structures for argument defaults (I choose by myself)
-  E123, # closing bracket does not match indentation of opening bracket's line (disagree with emacs python mode)
-  E126, # continuation line over-indented for hanging indent line (disagree with emacs python mode)
-  E226, # missing whitespace around arithmetic operator (disagree when in parameter)
-  P101, # [string-format] format string does contain unindexed parameters (don't care of py2.6)
-  P103, # [string-format] other string does contain unindexed parameters
-  P102, # [string-format] docstring does contain unindexed parameters
-  W503, # Line break occurred before a binary operator (to keep operators aligned)
+# attribute overriding builtin name
+  A003,
+# [bugbear] Do not use mutable data structures for argument defaults (I choose by myself)
+  B006,
+# closing bracket does not match indentation of opening bracket's line (disagree with emacs python mode)
+  E123,
+# continuation line over-indented for hanging indent line (disagree with emacs python mode)
+  E126,
+# missing whitespace around arithmetic operator (disagree when in parameter)
+  E226,
+# [string-format] format string does contain unindexed parameters (don't care of py2.6)
+  P101,
+# [string-format] other string does contain unindexed parameters
+  P103,
+# [string-format] docstring does contain unindexed parameters
+  P102,
+# Line break occurred before a binary operator (to keep operators aligned)
+  W503,
 max-line-length = 100
 exclude = doc/*,.tox/*,.eggs
 rst-roles =
   class,
   envvar,
   func,
   meth,
```


# Comparing `tmp/kintree-1.0.0rc0.tar.gz` & `tmp/kintree-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kintree-1.0.0rc0.tar", max compression
+gzip compressed data, was "kintree-1.0.1.tar", max compression
```

## Comparing `kintree-1.0.0rc0.tar` & `kintree-1.0.1.tar`

### file list

```diff
@@ -1,79 +1,76 @@
--rw-r--r--   0        0        0    35149 2023-03-29 19:46:31.216390 kintree-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0    14494 2023-03-29 19:46:31.216390 kintree-1.0.0rc0/README.md
--rw-r--r--   0        0        0       24 2023-03-29 19:46:31.324392 kintree-1.0.0rc0/kintree/__init__.py
--rw-r--r--   0        0        0     5304 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/part_tools.py
--rw-r--r--   0        0        0     1214 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/progress.py
--rw-r--r--   0        0        0     4852 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/common/tools.py
--rw-r--r--   0        0        0    15164 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/config_interface.py
--rw-r--r--   0        0        0       47 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_api.yaml
--rw-r--r--   0        0        0     2745 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_categories.yaml
--rw-r--r--   0        0        0      229 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_config.yaml
--rw-r--r--   0        0        0     5604 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/digikey/digikey_parameters.yaml
--rw-r--r--   0        0        0       99 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/element14/element14_api.yaml
--rw-r--r--   0        0        0      225 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/element14/element14_config.yaml
--rw-r--r--   0        0        0     1633 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/categories.yaml
--rw-r--r--   0        0        0       57 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/inventree_dev.yaml
--rw-r--r--   0        0        0       57 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/inventree_prod.yaml
--rw-r--r--   0        0        0     1019 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/parameters.yaml
--rw-r--r--   0        0        0      553 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/parameters_filters.yaml
--rw-r--r--   0        0        0     5710 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/supplier_parameters.yaml
--rw-r--r--   0        0        0      235 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/inventree/suppliers.yaml
--rw-r--r--   0        0        0       95 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/kicad/kicad.yaml
--rw-r--r--   0        0        0     1161 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/kicad/kicad_map.yaml
--rw-r--r--   0        0        0       68 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/lcsc/lcsc_api.yaml
--rw-r--r--   0        0        0      237 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/lcsc/lcsc_config.yaml
--rw-r--r--   0        0        0       25 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/mouser/mouser_api.yaml
--rw-r--r--   0        0        0      239 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/mouser/mouser_config.yaml
--rw-r--r--   0        0        0    11228 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/settings.py
--rw-r--r--   0        0        0      199 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/general.yaml
--rw-r--r--   0        0        0      183 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/internal_part_number.yaml
--rw-r--r--   0        0        0       73 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/config/user/search_api.yaml
--rw-r--r--   0        0        0    21057 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/database/inventree_api.py
--rw-r--r--   0        0        0    32757 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/database/inventree_interface.py
--rw-r--r--   0        0        0     3276 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/gui.py
--rw-r--r--   0        0        0    14401 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/common.py
--rw-r--r--   0        0        0    50767 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/main.py
--rw-r--r--   0        0        0    31898 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/gui/views/settings.py
--rw-r--r--   0        0        0        0 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/__init__.py
--rw-r--r--   0        0        0      569 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/kicad_interface.py
--rw-r--r--   0        0        0     4752 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/kicad_symbol.py
--rw-r--r--   0        0        0     7048 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/LICENSE
--rw-r--r--   0        0        0     3077 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/capacitor-polarized.kicad_sym
--rw-r--r--   0        0        0     2786 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/capacitor.kicad_sym
--rw-r--r--   0        0        0     1089 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/connector.kicad_sym
--rw-r--r--   0        0        0     2540 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/crystal-2p.kicad_sym
--rw-r--r--   0        0        0     1091 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/default.kicad_sym
--rw-r--r--   0        0        0     2647 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-led.kicad_sym
--rw-r--r--   0        0        0     2453 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-schottky.kicad_sym
--rw-r--r--   0        0        0     2251 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-standard.kicad_sym
--rw-r--r--   0        0        0     2445 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/diode-zener.kicad_sym
--rw-r--r--   0        0        0     2116 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/eeprom-sot23.kicad_sym
--rw-r--r--   0        0        0     2445 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/ferrite-bead.kicad_sym
--rw-r--r--   0        0        0     2249 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/fuse.kicad_sym
--rw-r--r--   0        0        0     2258 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/inductor.kicad_sym
--rw-r--r--   0        0        0     1089 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/integrated-circuit.kicad_sym
--rw-r--r--   0        0        0       65 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/library_template.kicad_sym
--rw-r--r--   0        0        0     2140 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/oscillator-4p.kicad_sym
--rw-r--r--   0        0        0     2451 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/protection-unidir.kicad_sym
--rw-r--r--   0        0        0     2233 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/resistor-sm.kicad_sym
--rw-r--r--   0        0        0     2233 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/resistor.kicad_sym
--rw-r--r--   0        0        0     4683 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-nfet.kicad_sym
--rw-r--r--   0        0        0     2795 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-npn.kicad_sym
--rw-r--r--   0        0        0     4986 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-pfet.kicad_sym
--rw-r--r--   0        0        0     2800 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates/transistor-pnp.kicad_sym
--rw-r--r--   0        0        0     1981 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pcb
--rw-r--r--   0        0        0     1201 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_prl
--rw-r--r--   0        0        0     6077 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pro
--rw-r--r--   0        0        0      187 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_sch
--rw-r--r--   0        0        0      227 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kintree_gui.py
--rw-r--r--   0        0        0    67605 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/kintree_gui_0.6.x.py
--rw-r--r--   0        0        0    38788 2023-03-29 19:46:31.224390 kintree-1.0.0rc0/kintree/logo.png
--rw-r--r--   0        0        0     5988 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/digikey_api.py
--rw-r--r--   0        0        0     9274 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/element14_api.py
--rw-r--r--   0        0        0     3165 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/lcsc_api.py
--rw-r--r--   0        0        0     3383 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/mouser_api.py
--rw-r--r--   0        0        0     1243 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/search_api.py
--rw-r--r--   0        0        0     4013 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/search/snapeda_api.py
--rw-r--r--   0        0        0     2028 2023-03-29 19:46:31.228390 kintree-1.0.0rc0/kintree/setup_inventree.py
--rw-r--r--   0        0        0      985 2023-03-29 19:46:31.324392 kintree-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0    15687 1970-01-01 00:00:00.000000 kintree-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 18:36:38.509469 kintree-1.0.1/LICENSE
+-rw-r--r--   0        0        0    14880 2023-04-24 18:36:38.509469 kintree-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-24 18:36:38.593470 kintree-1.0.1/kintree/__init__.py
+-rw-r--r--   0        0        0     5304 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/part_tools.py
+-rw-r--r--   0        0        0     1214 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/progress.py
+-rw-r--r--   0        0        0     4852 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/common/tools.py
+-rw-r--r--   0        0        0    16047 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/config_interface.py
+-rw-r--r--   0        0        0       47 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_api.yaml
+-rw-r--r--   0        0        0     2745 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_categories.yaml
+-rw-r--r--   0        0        0      248 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/digikey/digikey_config.yaml
+-rw-r--r--   0        0        0       99 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/element14/element14_api.yaml
+-rw-r--r--   0        0        0      244 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/element14/element14_config.yaml
+-rw-r--r--   0        0        0     1633 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/categories.yaml
+-rw-r--r--   0        0        0      104 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/inventree_dev.yaml
+-rw-r--r--   0        0        0      104 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/inventree_prod.yaml
+-rw-r--r--   0        0        0     1019 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/parameters.yaml
+-rw-r--r--   0        0        0      553 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/parameters_filters.yaml
+-rw-r--r--   0        0        0     5710 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/supplier_parameters.yaml
+-rw-r--r--   0        0        0      235 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/inventree/suppliers.yaml
+-rw-r--r--   0        0        0       95 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/kicad/kicad.yaml
+-rw-r--r--   0        0        0     1161 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/kicad/kicad_map.yaml
+-rw-r--r--   0        0        0       68 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/lcsc/lcsc_api.yaml
+-rw-r--r--   0        0        0      256 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/lcsc/lcsc_config.yaml
+-rw-r--r--   0        0        0       25 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/mouser/mouser_api.yaml
+-rw-r--r--   0        0        0      258 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/mouser/mouser_config.yaml
+-rw-r--r--   0        0        0    11301 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/settings.py
+-rw-r--r--   0        0        0      199 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/general.yaml
+-rw-r--r--   0        0        0      183 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/internal_part_number.yaml
+-rw-r--r--   0        0        0       73 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/config/user/search_api.yaml
+-rw-r--r--   0        0        0    20852 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/database/inventree_api.py
+-rw-r--r--   0        0        0    33965 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/database/inventree_interface.py
+-rw-r--r--   0        0        0     3360 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/gui.py
+-rw-r--r--   0        0        0    38788 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/logo.png
+-rw-r--r--   0        0        0    14401 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/common.py
+-rw-r--r--   0        0        0    50728 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/main.py
+-rw-r--r--   0        0        0    32917 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/gui/views/settings.py
+-rw-r--r--   0        0        0      416 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/kicad_interface.py
+-rw-r--r--   0        0        0     4598 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/kicad_symbol.py
+-rw-r--r--   0        0        0     7048 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/LICENSE
+-rw-r--r--   0        0        0     3077 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/capacitor-polarized.kicad_sym
+-rw-r--r--   0        0        0     2786 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/capacitor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/connector.kicad_sym
+-rw-r--r--   0        0        0     2540 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/crystal-2p.kicad_sym
+-rw-r--r--   0        0        0     1091 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/default.kicad_sym
+-rw-r--r--   0        0        0     2647 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-led.kicad_sym
+-rw-r--r--   0        0        0     2453 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-schottky.kicad_sym
+-rw-r--r--   0        0        0     2251 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-standard.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/diode-zener.kicad_sym
+-rw-r--r--   0        0        0     2116 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/eeprom-sot23.kicad_sym
+-rw-r--r--   0        0        0     2445 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/ferrite-bead.kicad_sym
+-rw-r--r--   0        0        0     2249 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/fuse.kicad_sym
+-rw-r--r--   0        0        0     2258 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/inductor.kicad_sym
+-rw-r--r--   0        0        0     1089 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/integrated-circuit.kicad_sym
+-rw-r--r--   0        0        0       65 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/library_template.kicad_sym
+-rw-r--r--   0        0        0     2140 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/oscillator-4p.kicad_sym
+-rw-r--r--   0        0        0     2451 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/protection-unidir.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/resistor-sm.kicad_sym
+-rw-r--r--   0        0        0     2233 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/resistor.kicad_sym
+-rw-r--r--   0        0        0     4683 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-nfet.kicad_sym
+-rw-r--r--   0        0        0     2795 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-npn.kicad_sym
+-rw-r--r--   0        0        0     4986 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-pfet.kicad_sym
+-rw-r--r--   0        0        0     2800 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates/transistor-pnp.kicad_sym
+-rw-r--r--   0        0        0     1981 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pcb
+-rw-r--r--   0        0        0     1201 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_prl
+-rw-r--r--   0        0        0     6077 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pro
+-rw-r--r--   0        0        0      187 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_sch
+-rw-r--r--   0        0        0      227 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/kintree_gui.py
+-rw-r--r--   0        0        0     6440 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/digikey_api.py
+-rw-r--r--   0        0        0     9730 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/element14_api.py
+-rw-r--r--   0        0        0     3611 2023-04-24 18:36:38.513469 kintree-1.0.1/kintree/search/lcsc_api.py
+-rw-r--r--   0        0        0     3833 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/mouser_api.py
+-rw-r--r--   0        0        0     1243 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/search_api.py
+-rw-r--r--   0        0        0     4013 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/search/snapeda_api.py
+-rw-r--r--   0        0        0     2028 2023-04-24 18:36:38.517469 kintree-1.0.1/kintree/setup_inventree.py
+-rw-r--r--   0        0        0     1003 2023-04-24 18:36:38.593470 kintree-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    16129 1970-01-01 00:00:00.000000 kintree-1.0.1/PKG-INFO
```

### Comparing `kintree-1.0.0rc0/LICENSE` & `kintree-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/README.md` & `kintree-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 # <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
-### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
+### Fast part creation for [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
-## New version (1.0) is coming soon!
-
-To install the release candidate:
-``` shell
-pip install --pre -U kintree
-```
+## :fast_forward: [Demo Video](https://youtu.be/YeWBqOCb4pw)
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
-## Demo Videos :fast_forward: [Full Demo](https://youtu.be/haSAu926BOI) :fast_forward: [KiCad Demo](https://youtu.be/NSMfCCD0uVw)
-
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
 * automate part creation of InvenTree parts
 * synchronize parts data between KiCad and InvenTree
 
 Ki-nTree works with:
@@ -40,15 +33,15 @@
 
 Ki-nTree was developped by [@eeintech](https://github.com/eeintech) for [SPARK Microsystems](https://www.sparkmicro.com/), who generously accepted to make it open-source!
 
 ## Get Started
 
 ### Requirements
 
-* Ki-nTree is currently tested for Python 3.8 to 3.10 versions.
+* Ki-nTree is currently tested for Python 3.8 to 3.11 versions.
 * Ki-nTree requires a Digi-Key **production** API instance. To create one, go to https://developer.digikey.com/. Create an account, an organization and add a **production** API to your organization. Save both Client ID and Secret keys.
 > [Here is a video](https://youtu.be/OI1EGEc0Ju0) to help with the different steps
 * Ki-nTree requires a Mouser Search API key. To request one, head over to https://www.mouser.ca/api-search/ and click on "Sign Up for Search API"
 * Ki-nTree requires an Element14 Product Search API key to fetch part information for the following suppliers: Farnell (Europe), Newark (North America) and Element14 (Asia-Pacific). To request one, head over to https://partner.element14.com/ and click on "Register"
 
 ### Installation (system wide)
 
@@ -107,15 +100,14 @@
 
 #### Advanced Configuration
 
 Configuration files are stored in the folder pointed by the `Configuration Files Folder` path in the "User Settings" window:
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_settings_user.png" width="600" height="auto">
 
-
 <details>
 <summary><b>Click here to read about configuration files</b></summary>
 <p>
 
 Ki-nTree uses a number of YAML configuration files to function. New users shouldn't need to worry about them to try out Ki-nTree (except for `categories.yaml` as mentioned in the previous section), however they can be modified to customize behavior and workflow.
 
 Below is a summary table of the different configuration files, their function and if they are updated by the GUI:
@@ -155,15 +147,18 @@
 Note that each time you enable the "Add" permission to an object, InvenTree automatically enables the "Change" permission to that object too.
 
 #### Settings
 1. With Ki-nTree GUI open, click on "Settings > Supplier > Digi-Key" and fill in both Digi-Key API Client ID and Secret keys (optional: click on "Test" to [get an API token](#get-digi-key-api-token))
 2. Click on "Settings > Supplier > Mouser" and fill in the Mouser part search API key
 3. Click on "Settings > Supplier > Element14" and fill in the Element14 product search API key (key is shared with Farnell and Newark)
 4. Click on "Settings > KiCad", browse to the location where KiCad symbol, template and footprint libraries are stored on your computer then click "Save"
-5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to get an API token)
+5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
+  a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
+  b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
+
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
 Enter your Digi-Key developper account credentials then login. The following page will appear (`user@email.com` will show your email address):
```

### Comparing `kintree-1.0.0rc0/kintree/common/part_tools.py` & `kintree-1.0.1/kintree/common/part_tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/common/progress.py` & `kintree-1.0.1/kintree/common/progress.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/common/tools.py` & `kintree-1.0.1/kintree/common/tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/config_interface.py` & `kintree-1.0.1/kintree/config/config_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,26 +94,43 @@
 
     try:
         # Use base64 encoding to make password unreadable inside the file
         user_settings['PASSWORD'] = base64.b64decode(password).decode()
     except TypeError:
         user_settings['PASSWORD'] = ''
 
+    if 'ENABLE_PROXY' not in user_settings:
+        user_settings['ENABLE_PROXY'] = False
+    proxies = user_settings.get('PROXIES', None)
+    if not proxies:
+        user_settings['PROXY'] = ''
+    else:
+        # loading the proxy independent if it is http or https
+        user_settings['PROXY'] = list(proxies.values())[0]
+
     return user_settings
 
 
-def save_inventree_user_settings(enable: bool, server: str, username: str, password: str, user_config_path: str):
+def save_inventree_user_settings(enable: bool,
+                                 server: str,
+                                 username: str,
+                                 password: str,
+                                 enable_proxy: bool,
+                                 proxies: dict,
+                                 user_config_path: str):
     ''' Save InvenTree user settings to file '''
     user_settings = {}
 
     user_settings['ENABLE'] = enable
     user_settings['SERVER_ADDRESS'] = server
     user_settings['USERNAME'] = username
     # Use base64 encoding to make password unreadable inside the file
     user_settings['PASSWORD'] = base64.b64encode(password.encode())
+    user_settings['ENABLE_PROXY'] = enable_proxy
+    user_settings['PROXIES'] = proxies
 
     return dump_file(user_settings, user_config_path)
 
 
 def load_library_path(user_config_path: str, silent=False):
     ''' Load KiCad library from KiCad settings file '''
     user_settings = load_file(user_config_path)
@@ -399,20 +416,29 @@
                     pass
 
             return False
 
     return dump_file(supplier_categories, supplier_config_path)
 
 
-def load_category_parameters(category: str, supplier_config_path: str) -> dict:
+def load_category_parameters(categories: list, supplier_config_path: str) -> dict:
     ''' Load Supplier parameters mapping from Supplier settings file '''
     try:
-        category_parameters = load_file(supplier_config_path)[category]
+        category_file = load_file(supplier_config_path)
     except:
         return None
+    category_parameters = None
+    for category in reversed(categories):
+        try:
+            category_parameters = category_file[category]
+            break
+        except:
+            pass
+    if not category_parameters:
+        return None
 
     category_parameters_inversed = {}
     for parameter in category_parameters.keys():
         if category_parameters[parameter]:
             for supplier_parameter in category_parameters[parameter]:
                 category_parameters_inversed[supplier_parameter] = parameter
```

### Comparing `kintree-1.0.0rc0/kintree/config/digikey/digikey_categories.yaml` & `kintree-1.0.1/kintree/config/digikey/digikey_categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/digikey/digikey_parameters.yaml` & `kintree-1.0.1/kintree/config/inventree/supplier_parameters.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Parameter Mapping between KiCad template symbol and Digi-Key
-# Each template parameter can match to multiple Digi-Key parameters
-# Categories (main keys) should match categories in kicad/kicad_map.yaml file
+# Parameter Mapping between InvenTree parameter template and suppliers parameters naming
+# Each template parameter can match to multiple suppliers parameters
+# Categories (main keys) should match categories in the categories.yaml file
+# Parameter template names should match those found in the parameters.yaml file
 Capacitors:
   ESR:
   - ESR (Equivalent Series Resistance)
   Package Height:
   - Height - Seated (Max)
   - Thickness (Max)
   Package Size:
```

### Comparing `kintree-1.0.0rc0/kintree/config/inventree/categories.yaml` & `kintree-1.0.1/kintree/config/inventree/categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/inventree/parameters.yaml` & `kintree-1.0.1/kintree/config/inventree/parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/inventree/parameters_filters.yaml` & `kintree-1.0.1/kintree/config/inventree/parameters_filters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/kicad/kicad_map.yaml` & `kintree-1.0.1/kintree/config/kicad/kicad_map.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/config/settings.py` & `kintree-1.0.1/kintree/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 CONFIG_SEARCH_API_PATH = os.path.join(CONFIG_USER_FILES, 'search_api.yaml')
 CONFIG_SEARCH_API = config_interface.load_file(CONFIG_SEARCH_API_PATH)
 
 # Digi-Key user configuration
 CONFIG_DIGIKEY = config_interface.load_file(os.path.join(CONFIG_USER_FILES, 'digikey_config.yaml'))
 CONFIG_DIGIKEY_API = os.path.join(CONFIG_USER_FILES, 'digikey_api.yaml')
 CONFIG_DIGIKEY_CATEGORIES = os.path.join(CONFIG_USER_FILES, 'digikey_categories.yaml')
-# CONFIG_DIGIKEY_PARAMETERS = os.path.join(CONFIG_USER_FILES, 'digikey_parameters.yaml')
 
 # Mouser user configuration
 CONFIG_MOUSER = config_interface.load_file(os.path.join(CONFIG_USER_FILES, 'mouser_config.yaml'))
 CONFIG_MOUSER_API = os.path.join(CONFIG_USER_FILES, 'mouser_api.yaml')
 
 # Element14 user configuration (includes Farnell, Newark and Element14)
 CONFIG_ELEMENT14 = config_interface.load_file(os.path.join(CONFIG_USER_FILES, 'element14_config.yaml'))
@@ -304,21 +303,25 @@
 
 
 # Server settings
 def load_inventree_settings():
     global SERVER_ADDRESS
     global USERNAME
     global PASSWORD
+    global ENABLE_PROXY
+    global PROXIES
     global PART_URL_ROOT
 
     inventree_settings = config_interface.load_inventree_user_settings(INVENTREE_CONFIG)
 
     SERVER_ADDRESS = inventree_settings.get('SERVER_ADDRESS', None)
     USERNAME = inventree_settings.get('USERNAME', None)
     PASSWORD = inventree_settings.get('PASSWORD', None)
+    ENABLE_PROXY = inventree_settings.get('ENABLE_PROXY', False)
+    PROXIES = inventree_settings.get('PROXIES', None)
     # Part URL
     if SERVER_ADDRESS:
         # If missing, append slash to root URL
         root_url = SERVER_ADDRESS
         if not SERVER_ADDRESS.endswith('/'):
             root_url = root_url + '/'
         # Set part URL
```

### Comparing `kintree-1.0.0rc0/kintree/database/inventree_api.py` & `kintree-1.0.1/kintree/database/inventree_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 
 # InvenTree
 from inventree.api import InvenTreeAPI
 from inventree.company import Company, ManufacturerPart, SupplierPart
 from inventree.part import Part, PartCategory, Parameter, ParameterTemplate
 
 
-def connect(server: str, username: str, password: str, connect_timeout=5, silent=False) -> bool:
+def connect(server: str,
+            username: str,
+            password: str,
+            connect_timeout=5,
+            silent=False,
+            proxies=None,
+            token='') -> bool:
     ''' Connect to InvenTree server and create API object '''
     from wrapt_timeout_decorator import timeout
     global inventree_api
 
     @timeout(dec_timeout=connect_timeout)
     def get_inventree_api_timeout():
-        return InvenTreeAPI(server, username=username, password=password)
+        return InvenTreeAPI(server,
+                            username=username,
+                            password=password,
+                            proxies=proxies,
+                            token=token)
 
     try:
         inventree_api = get_inventree_api_timeout()
     except:
         return False
 
     if inventree_api.token:
@@ -358,32 +368,14 @@
 
     if part:
         return part.pk
     else:
         return 0
 
 
-def delete_part(part_id: int) -> bool:
-    ''' Delete InvenTree part (only used for testing) '''
-    global inventree_api
-
-    part = Part(inventree_api, part_id)
-    if part.pk:
-        part._data['active'] = False
-        # Remove image url (API rejects it as it is not a file)
-        try:
-            del part._data['image']
-        except:
-            pass
-        part.save()
-        return part.delete()
-    else:
-        return True
-
-
 def create_company(company_name: str, manufacturer=False, supplier=False) -> bool:
     ''' Create InvenTree company '''
     global inventree_api
 
     if not manufacturer and not supplier:
         return None
```

### Comparing `kintree-1.0.0rc0/kintree/database/inventree_interface.py` & `kintree-1.0.1/kintree/database/inventree_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 category_separator = '/'
 
 
 def connect_to_server(timeout=5) -> bool:
     ''' Connect to InvenTree server using user settings '''
     connect = False
     settings.load_inventree_settings()
+    if not settings.USERNAME:
+        token = settings.PASSWORD
+    else:
+        token = ''
 
     try:
         connect = inventree_api.connect(server=settings.SERVER_ADDRESS,
                                         username=settings.USERNAME,
                                         password=settings.PASSWORD,
+                                        proxies=settings.PROXIES,
+                                        token=token,
                                         connect_timeout=timeout)
     except TimeoutError:
         pass
 
     if not connect:
         if not settings.SERVER_ADDRESS:
             cprint('[TREE]\tError connecting to InvenTree server: missing server address')
@@ -137,15 +143,15 @@
     except:
         pass
 
     # Function Filter
     if not categories[1] and function_filter:
         cprint(f'[INFO]\tSubcategory is filtered using "{filter_parameter}" parameter', silent=settings.SILENT, end='')
         # Load parameter map
-        parameter_map = config_interface.load_category_parameters(categories[0], settings.CONFIG_SUPPLIER_PARAMETERS)
+        parameter_map = config_interface.load_category_parameters(categories, settings.CONFIG_SUPPLIER_PARAMETERS)
         # Build compare list
         compare = []
         for supplier_parameter, inventree_parameter in parameter_map.items():
             if (supplier_parameter in part_info['parameters'].keys() and inventree_parameter == filter_parameter):
                 compare.append(part_info['parameters'][supplier_parameter])
 
         # Load subcategory map
@@ -257,43 +263,61 @@
     inventree_part['datasheet'] = part_info['datasheet'].replace(' ', '%20')
     # Image URL is not shown to user so force default key/value
     inventree_part['image'] = part_info['image'].replace(' ', '%20')
 
     # Load parameters map
     if category_tree:
         parameter_map = config_interface.load_category_parameters(
-            category=category_tree[0],
+            categories=category_tree,
             supplier_config_path=settings.CONFIG_SUPPLIER_PARAMETERS,
         )
     else:
         cprint('[INFO]\tWarning: Parameter map not loaded (no category selected)', silent=settings.SILENT)
 
     if not is_custom:
         # Add Parameters
         if parameter_map:
+            parameters_missing = []
             for supplier_param, inventree_param in parameter_map.items():
                 # Some parameters may not be mapped
                 if inventree_param not in inventree_part['parameters'].keys():
                     if supplier_param != 'Manufacturer Part Number':
                         try:
                             parameter_value = part_tools.clean_parameter_value(
                                 category=category_tree[0],
                                 name=supplier_param,
                                 value=part_info['parameters'][supplier_param],
                             )
                             inventree_part['parameters'][inventree_param] = parameter_value
-                        except:
-                            cprint(f'[INFO]\tWarning: Parameter "{supplier_param}" not found in supplier data', silent=settings.SILENT)
+                        except KeyError:
+                            parameters_missing.append(supplier_param)
                     else:
                         inventree_part['parameters'][inventree_param] = part_info['manufacturer_part_number']
 
-            # Check for missing parameters and fill value with dash
+            if parameters_missing:
+                msg = '[INFO]\tWarning: The following parameters were not found in supplier data:\n'
+                msg += str(parameters_missing)
+                cprint(msg, silent=settings.SILENT)
+
+            # Check for missing InvenTree parameters and fill value with dash
             for inventree_param in parameter_map.values():
                 if inventree_param not in inventree_part['parameters'].keys():
                     inventree_part['parameters'][inventree_param] = '-'
+
+            # Check for extra parameters which weren't mapped
+            parameters_unmapped = []
+            for search_param in part_info['parameters'].keys():
+                if search_param not in parameter_map.keys():
+                    parameters_unmapped.append(search_param)
+            
+            if parameters_unmapped:
+                if not settings.SILENT:
+                    msg = f'[INFO]\tThe following parameters are not mapped in {inventree_part["supplier_name"]} parameters configuration:\n'
+                    msg += str(parameters_unmapped)
+                    print(msg)
         else:
             cprint(f'[INFO]\tWarning: Parameter map for "{category_tree[0]}" does not exist or is empty', silent=settings.SILENT)
 
     return inventree_part
 
 
 def get_supplier_name(supplier: str) -> str:
@@ -541,17 +565,22 @@
             if inventree_part['image']:
                 # Add image
                 image_result = inventree_api.upload_part_image(inventree_part['image'], part_pk)
                 if not image_result:
                     cprint('[TREE]\tWarning: Failed to upload part image', silent=settings.SILENT)
 
         if kicad:
+            try:
+                symbol_name = ipn
+            except UnboundLocalError:
+                symbol_name = inventree_part.get('manufacturer_part_number')
+
             # Create symbol & footprint parameters
             if symbol:
-                symbol = f'{symbol.split(":")[0]}:{ipn}'
+                symbol = f'{symbol.split(":")[0]}:{symbol_name}'
                 inventree_part['parameters']['Symbol'] = symbol
             if footprint:
                 inventree_part['parameters']['Footprint'] = footprint
 
         if not inventree_part['parameters']:
             category_parameters = inventree_api.get_category_parameters(category_pk)
```

### Comparing `kintree-1.0.0rc0/kintree/gui/gui.py` & `kintree-1.0.1/kintree/gui/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
     page.vertical_alignment = ft.MainAxisAlignment.CENTER
     page.scroll = ft.ScrollMode.ALWAYS
     
     # Theme
     update_theme(page)
 
-    # Creating a progress bar that will be used to show the user that the app is busy doing something.
+    # Creating a progress bar that will be used
+    # to show the user that the app is busy doing something
     page.splash = ft.ProgressBar(visible=False)
 
     # Init dialogs
     page.snack_bar = ft.SnackBar(
         content=None,
         open=False,
     )
@@ -90,15 +91,20 @@
         page.views.pop()
         top_view = page.views[-1]
         if 'main' in top_view.route:
             handle_transition(page, transition=True)
         # Route and render
         page.go(top_view.route)
         if 'main' in top_view.route:
-            handle_transition(page, transition=False, update_page=True, timeout=0.3)
+            handle_transition(
+                page,
+                transition=False,
+                update_page=True,
+                timeout=0.3,
+            )
         if 'part' in top_view.route:
             part_view.partial_update()
         elif 'inventree' in top_view.route:
             inventree_view.partial_update()
 
     page.on_route_change = route_change
     page.on_view_pop = view_pop
```

### Comparing `kintree-1.0.0rc0/kintree/gui/views/common.py` & `kintree-1.0.1/kintree/gui/views/common.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/gui/views/main.py` & `kintree-1.0.1/kintree/gui/views/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 # KiCad
 from ...kicad import kicad_interface
 # SnapEDA
 from ...search import snapeda_api
 
 # Main AppBar
 main_appbar = ft.AppBar(
-    # leading=ft.Icon(ft.icons.DOUBLE_ARROW),
     leading=ft.Container(
         content=ft.Image(
-            src=os.path.join(settings.PROJECT_DIR, 'logo.png'),
+            src=os.path.join(settings.PROJECT_DIR, 'gui', 'logo.png'),
             fit=ft.ImageFit.CONTAIN,
         ),
         padding=ft.padding.only(left=10),
         expand=True,
     ),
     leading_width=40,
     title=ft.Text(f'Ki-nTree | {__version__}'),
```

### Comparing `kintree-1.0.0rc0/kintree/gui/views/settings.py` & `kintree-1.0.1/kintree/gui/views/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,19 +133,29 @@
             False,  # Browse disabled
         ],
         'Username': [
             'USERNAME',
             ft.TextField(),
             False,  # Browse disabled
         ],
-        'Password': [
+        'Password or Token': [
             'PASSWORD',
             ft.TextField(),
             False,  # Browse disabled
         ],
+        'Enable Proxy Support': [
+            'ENABLE_PROXY',
+            SwitchWithRefs(),
+            False,  # Browse disabled
+        ],
+        'Proxy': [
+            'PROXY',
+            ft.TextField(),
+            False,  # Browse disabled
+        ],
         'Default Part Revision': [
             'INVENTREE_DEFAULT_REV',
             ft.TextField(),
             False,  # Browse disabled
         ],
         'Enable Internal Part Number (IPN)': [
             'IPN_ENABLE_CREATE',
@@ -387,15 +397,18 @@
             )
         elif type(field) == ft.Dropdown:
             field.on_change = lambda _: self.save()
             column.controls.append(
                 field,
             )
         elif type(field) == ft.Switch or type(field) == SwitchWithRefs:
-            field.on_change = lambda _: self.save()
+            if 'proxy' in name.lower():
+                field.on_change = lambda _: None
+            else:
+                field.on_change = lambda _: self.save()
             field.label = name
             column.controls.append(
                 field,
             )
 
     def add_buttons(self, column, test=False) -> ft.Row:
         test_save_buttons = ft.Row()
@@ -728,21 +741,32 @@
     route = '/settings/inventree'
     settings_file = [
         global_settings.INVENTREE_CONFIG,
         global_settings.CONFIG_IPN_PATH,
     ]
 
     def save(self, file=None, dialog=True):
+        address = SETTINGS[self.title]['Server Address'][1].value
+        proxy = SETTINGS[self.title]['Proxy'][1].value
+        enable_proxy = SETTINGS[self.title]['Enable Proxy Support'][1].value
+        if not enable_proxy:
+            proxies = None
+        elif address.startswith('https'):
+            proxies = {'https': proxy}
+        else:
+            proxies = {'http': proxy}
         if file is None:
             # Save to InvenTree file
             config_interface.save_inventree_user_settings(
                 enable=global_settings.ENABLE_INVENTREE,
-                server=SETTINGS[self.title]['Server Address'][1].value,
+                server=address,
                 username=SETTINGS[self.title]['Username'][1].value,
-                password=SETTINGS[self.title]['Password'][1].value,
+                password=SETTINGS[self.title]['Password or Token'][1].value,
+                enable_proxy=enable_proxy,
+                proxies=proxies,
                 user_config_path=self.settings_file[0]
             )
             # Alert user
             if dialog:
                 self.show_dialog(
                     d_type=DialogType.VALID,
                     message=f'{self.title} successfully saved',
@@ -812,14 +836,19 @@
                 tab_content=ft.Text('Server', size=16),
                 content=ft.Container(
                     server_col,
                 )
             )
         )
 
+        # Link Proxy Switch to the input field
+        ref = ft.Ref[ft.TextField]()
+        ref.current = SETTINGS[self.title]['Proxy'][1]
+        SETTINGS[self.title]['Enable Proxy Support'][1].refs = [ref]
+
         # Create IPN fields
         ipn_fields_ref = ft.Ref[ft.Row]()
         ipn_fields_col = ft.Column(
             ref=ipn_fields_ref,
             controls=[],
         )
         for name in ipn_fields:
```

### Comparing `kintree-1.0.0rc0/kintree/kicad/kicad_symbol.py` & `kintree-1.0.1/kintree/kicad/kicad_symbol.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,12 +116,7 @@
         new_part = True
 
         # Progress Update
         if not progress.update_progress_bar(show_progress):
             pass
 
         return part_in_lib, new_part
-
-    # NOT YET SUPPORTED - REMOVE?
-    # def delete_symbol_from_lib(self, part_number):
-    #     ''' Remove symbol from KiCad library '''
-    #     pass
```

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/LICENSE` & `kintree-1.0.1/kintree/kicad/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/capacitor-polarized.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/capacitor-polarized.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/capacitor.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/capacitor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/connector.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/connector.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/crystal-2p.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/crystal-2p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/default.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/default.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/diode-led.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/diode-led.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/diode-schottky.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/diode-schottky.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/diode-standard.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/diode-standard.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/diode-zener.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/diode-zener.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/eeprom-sot23.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/eeprom-sot23.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/ferrite-bead.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/ferrite-bead.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/fuse.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/fuse.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/inductor.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/inductor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/integrated-circuit.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/integrated-circuit.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/oscillator-4p.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/oscillator-4p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/protection-unidir.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/protection-unidir.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/resistor-sm.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/resistor-sm.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/resistor.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/resistor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/transistor-nfet.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/transistor-nfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/transistor-npn.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/transistor-npn.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/transistor-pfet.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/transistor-pfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates/transistor-pnp.kicad_sym` & `kintree-1.0.1/kintree/kicad/templates/transistor-pnp.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pcb` & `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pcb`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_prl` & `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_prl`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/kicad/templates_project/templates_project.kicad_pro` & `kintree-1.0.1/kintree/kicad/templates_project/templates_project.kicad_pro`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/logo.png` & `kintree-1.0.1/kintree/gui/logo.png`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/search/digikey_api.py` & `kintree-1.0.1/kintree/search/digikey_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,14 +145,23 @@
 
     for parameter in range(len(part[parameter_key])):
         parameter_name = part[parameter_key][parameter][name_key]
         parameter_value = part[parameter_key][parameter][value_key]
         # Append to parameters dictionary
         part_info['parameters'][parameter_name] = parameter_value
 
+    # Extra search fields
+    if settings.CONFIG_DIGIKEY.get('EXTRA_FIELDS', None):
+        for extra_field in settings.CONFIG_DIGIKEY['EXTRA_FIELDS']:
+            if part.get(extra_field, None):
+                part_info['parameters'][extra_field] = part[extra_field]
+            else:
+                from ..common.tools import cprint
+                cprint(f'[INFO]\tWarning: Extra field "{extra_field}" not found in search results', silent=False)
+
     return part_info
 
 
 def test_api(check_content=False) -> bool:
     ''' Test method for API token '''
     setup_environment()
```

### Comparing `kintree-1.0.0rc0/kintree/search/element14_api.py` & `kintree-1.0.1/kintree/search/element14_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -204,14 +204,23 @@
                 parameter_name = part[parameter_key][parameter][name_key]
                 parameter_value = part[parameter_key][parameter][value_key]
                 # Append to parameters dictionary
                 part_info['parameters'][parameter_name] = parameter_value
         except TypeError:
             # Parameter list is empty
             pass
+
+    # Extra search fields
+    if settings.CONFIG_ELEMENT14.get('EXTRA_FIELDS', None):
+        for extra_field in settings.CONFIG_ELEMENT14['EXTRA_FIELDS']:
+            if part.get(extra_field, None):
+                part_info['parameters'][extra_field] = part[extra_field]
+            else:
+                from ..common.tools import cprint
+                cprint(f'[INFO]\tWarning: Extra field "{extra_field}" not found in search results', silent=False)
     
     # Append Store URL
     # Element14 support said "At this time our API is not structured to provide a URL to product pages in the selected storeInfo.id value."
     if store_url:
         part_info['store_url'] = f'https://{store_url}'
     else:
         part_info['store_url'] = f'https://{get_default_store_url(supplier)}'
```

### Comparing `kintree-1.0.0rc0/kintree/search/lcsc_api.py` & `kintree-1.0.1/kintree/search/lcsc_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,14 +95,23 @@
             parameter_value = part[parameter_key][parameter][value_key]
             # Append to parameters dictionary
             part_info['parameters'][parameter_name] = parameter_value
     except TypeError:
         # Parameter list is empty
         pass
 
+    # Extra search fields
+    if settings.CONFIG_LCSC.get('EXTRA_FIELDS', None):
+        for extra_field in settings.CONFIG_LCSC['EXTRA_FIELDS']:
+            if part.get(extra_field, None):
+                part_info['parameters'][extra_field] = part[extra_field]
+            else:
+                from ..common.tools import cprint
+                cprint(f'[INFO]\tWarning: Extra field "{extra_field}" not found in search results', silent=False)
+
     return part_info
 
 
 def test_api() -> bool:
     ''' Test method for API '''
 
     test_success = True
```

### Comparing `kintree-1.0.0rc0/kintree/search/mouser_api.py` & `kintree-1.0.1/kintree/search/mouser_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,14 +105,23 @@
 
     for parameter in range(len(part[parameter_key])):
         parameter_name = part[parameter_key][parameter][name_key]
         parameter_value = part[parameter_key][parameter][value_key]
         # Append to parameters dictionary
         part_info['parameters'][parameter_name] = parameter_value
 
+    # Extra search fields
+    if settings.CONFIG_MOUSER.get('EXTRA_FIELDS', None):
+        for extra_field in settings.CONFIG_MOUSER['EXTRA_FIELDS']:
+            if part.get(extra_field, None):
+                part_info['parameters'][extra_field] = part[extra_field]
+            else:
+                from ..common.tools import cprint
+                cprint(f'[INFO]\tWarning: Extra field "{extra_field}" not found in search results', silent=False)
+
     return part_info
 
 
 def test_api() -> bool:
     ''' Test method for API '''
 
     test_success = True
```

### Comparing `kintree-1.0.0rc0/kintree/search/search_api.py` & `kintree-1.0.1/kintree/search/search_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/search/snapeda_api.py` & `kintree-1.0.1/kintree/search/snapeda_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/kintree/setup_inventree.py` & `kintree-1.0.1/kintree/setup_inventree.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.0rc0/pyproject.toml` & `kintree-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "kintree"
-version = "1.0.0rc"
+version = "1.0.1"
 description = "Fast part creation in KiCad and InvenTree"
 authors = ["eeintech <eeintech@eeinte.ch>"]
 maintainers = ["eeintech <eeintech@eeinte.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/sparkmicro/Ki-nTree"
 repository = "https://github.com/sparkmicro/Ki-nTree"
-keywords = ["inventree", "kicad", "component", "part", "create"]
+keywords = ["inventree", "kicad", "digikey", "mouser", "component", "part", "create"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 digikey-api = "^1.0.0"
-Flet = "^0.4.2"
+flet = "0.5.2"
 thefuzz = "^0.19.0"
 inventree = "^0.10.1"
 kiutils = "^1.4.0"
 mouser = "^0.1.3"
 multiprocess = "^0.70.12"
-PyYAML = "^5.4.1"
+pyyaml = "^5.4.1"
 validators = "^0.19.0"
 wrapt_timeout_decorator = "^1.3.12"
 
 [tool.poetry.dev-dependencies]
-invoke = "^1.7.3"
+invoke = "^2.0.0"
 coveralls = "^3.3.1"
 
 [tool.poetry.scripts]
 kintree = 'kintree.kintree_gui:main'
 kintree_setup_inventree = 'kintree.setup_inventree:setup_inventree'
 
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.4.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kintree-1.0.0rc0/PKG-INFO` & `kintree-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 Metadata-Version: 2.1
 Name: kintree
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: Fast part creation in KiCad and InvenTree
 Home-page: https://github.com/sparkmicro/Ki-nTree
 License: GPL-3.0-or-later
-Keywords: inventree,kicad,component,part,create
+Keywords: inventree,kicad,digikey,mouser,component,part,create
 Author: eeintech
 Author-email: eeintech@eeinte.ch
 Maintainer: eeintech
 Maintainer-email: eeintech@eeinte.ch
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Flet (>=0.4.2,<0.5.0)
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: digikey-api (>=1.0.0,<2.0.0)
+Requires-Dist: flet (==0.5.2)
 Requires-Dist: inventree (>=0.10.1,<0.11.0)
 Requires-Dist: kiutils (>=1.4.0,<2.0.0)
 Requires-Dist: mouser (>=0.1.3,<0.2.0)
 Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
+Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: validators (>=0.19.0,<0.20.0)
 Requires-Dist: wrapt_timeout_decorator (>=1.3.12,<2.0.0)
 Project-URL: Repository, https://github.com/sparkmicro/Ki-nTree
 Description-Content-Type: text/markdown
 
 # <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/logo.png" width="auto" height="32"> Ki-nTree
-### Fast part creation in [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
+### Fast part creation for [KiCad](https://kicad.org/) and [InvenTree](https://inventree.org/) 
 [![License: GPL v3.0](https://img.shields.io/badge/license-GPL_v3.0-green.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python Versions](https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/python_versions.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/kintree)](https://pypi.org/project/kintree/)
 [![Tests | Linting | Publishing](https://github.com/sparkmicro/Ki-nTree/actions/workflows/test_deploy.yaml/badge.svg)](https://github.com/sparkmicro/Ki-nTree/actions)
 [![Coverage Status](https://coveralls.io/repos/github/sparkmicro/Ki-nTree/badge.svg?branch=main&service=github)](https://coveralls.io/github/sparkmicro/Ki-nTree?branch=main)
 
-## New version (1.0) is coming soon!
-
-To install the release candidate:
-``` shell
-pip install --pre -U kintree
-```
+## :fast_forward: [Demo Video](https://youtu.be/YeWBqOCb4pw)
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_example.png" width="auto" height="auto">
 
-## Demo Videos :fast_forward: [Full Demo](https://youtu.be/haSAu926BOI) :fast_forward: [KiCad Demo](https://youtu.be/NSMfCCD0uVw)
-
 ## Introduction
 Ki-nTree (pronounced "Key Entry" or "Key 'n' Tree") aims to:
 * automate part creation of KiCad library parts
 * automate part creation of InvenTree parts
 * synchronize parts data between KiCad and InvenTree
 
 Ki-nTree works with:
@@ -70,15 +64,15 @@
 
 Ki-nTree was developped by [@eeintech](https://github.com/eeintech) for [SPARK Microsystems](https://www.sparkmicro.com/), who generously accepted to make it open-source!
 
 ## Get Started
 
 ### Requirements
 
-* Ki-nTree is currently tested for Python 3.8 to 3.10 versions.
+* Ki-nTree is currently tested for Python 3.8 to 3.11 versions.
 * Ki-nTree requires a Digi-Key **production** API instance. To create one, go to https://developer.digikey.com/. Create an account, an organization and add a **production** API to your organization. Save both Client ID and Secret keys.
 > [Here is a video](https://youtu.be/OI1EGEc0Ju0) to help with the different steps
 * Ki-nTree requires a Mouser Search API key. To request one, head over to https://www.mouser.ca/api-search/ and click on "Sign Up for Search API"
 * Ki-nTree requires an Element14 Product Search API key to fetch part information for the following suppliers: Farnell (Europe), Newark (North America) and Element14 (Asia-Pacific). To request one, head over to https://partner.element14.com/ and click on "Register"
 
 ### Installation (system wide)
 
@@ -137,15 +131,14 @@
 
 #### Advanced Configuration
 
 Configuration files are stored in the folder pointed by the `Configuration Files Folder` path in the "User Settings" window:
 
 <img src="https://raw.githubusercontent.com/sparkmicro/Ki-nTree/main/images/doc/kintree_v1_settings_user.png" width="600" height="auto">
 
-
 <details>
 <summary><b>Click here to read about configuration files</b></summary>
 <p>
 
 Ki-nTree uses a number of YAML configuration files to function. New users shouldn't need to worry about them to try out Ki-nTree (except for `categories.yaml` as mentioned in the previous section), however they can be modified to customize behavior and workflow.
 
 Below is a summary table of the different configuration files, their function and if they are updated by the GUI:
@@ -185,15 +178,18 @@
 Note that each time you enable the "Add" permission to an object, InvenTree automatically enables the "Change" permission to that object too.
 
 #### Settings
 1. With Ki-nTree GUI open, click on "Settings > Supplier > Digi-Key" and fill in both Digi-Key API Client ID and Secret keys (optional: click on "Test" to [get an API token](#get-digi-key-api-token))
 2. Click on "Settings > Supplier > Mouser" and fill in the Mouser part search API key
 3. Click on "Settings > Supplier > Element14" and fill in the Element14 product search API key (key is shared with Farnell and Newark)
 4. Click on "Settings > KiCad", browse to the location where KiCad symbol, template and footprint libraries are stored on your computer then click "Save"
-5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to get an API token)
+5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
+  a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
+  b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
+
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
 Enter your Digi-Key developper account credentials then login. The following page will appear (`user@email.com` will show your email address):
```


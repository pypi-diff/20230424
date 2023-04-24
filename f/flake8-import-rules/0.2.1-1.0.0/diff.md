# Comparing `tmp/flake8_import_rules-0.2.1.tar.gz` & `tmp/flake8_import_rules-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_import_rules-0.2.1.tar", max compression
+gzip compressed data, was "flake8_import_rules-1.0.0.tar", max compression
```

## Comparing `flake8_import_rules-0.2.1.tar` & `flake8_import_rules-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2022-10-18 10:40:15.372192 flake8_import_rules-0.2.1/LICENCE
--rw-r--r--   0        0        0     1282 2022-10-24 11:46:42.455554 flake8_import_rules-0.2.1/README.md
--rw-r--r--   0        0        0     4674 2022-10-24 11:39:12.982817 flake8_import_rules-0.2.1/flake8_import_rules.py
--rw-r--r--   0        0        0     1169 2022-10-24 11:53:19.286083 flake8_import_rules-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 flake8_import_rules-0.2.1/setup.py
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 flake8_import_rules-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 12:08:38.916705 flake8_import_rules-1.0.0/LICENCE
+-rw-r--r--   0        0        0     2224 2023-04-24 16:10:36.557465 flake8_import_rules-1.0.0/README.md
+-rw-r--r--   0        0        0     6921 2023-04-24 14:09:21.077160 flake8_import_rules-1.0.0/flake8_import_rules.py
+-rw-r--r--   0        0        0      932 2023-04-18 19:40:21.692507 flake8_import_rules-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 flake8_import_rules-1.0.0/setup.py
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 flake8_import_rules-1.0.0/PKG-INFO
```

### Comparing `flake8_import_rules-0.2.1/LICENCE` & `flake8_import_rules-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `flake8_import_rules-0.2.1/setup.py` & `flake8_import_rules-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 modules = \
 ['flake8_import_rules']
 entry_points = \
 {'flake8.extension': ['I013 = flake8_import_rules:ImportRulesChecker']}
 
 setup_kwargs = {
     'name': 'flake8-import-rules',
-    'version': '0.2.1',
+    'version': '1.0.0',
     'description': '',
-    'long_description': "Helps to prevent import of certain modules from certain modules.\n\nIt's useful if you have many modules in your project and want to keep them kind of\nisolated.\n\nAfter installing just add `import-rules` option to your `setup.cfg` file.\n\n```\n[flake8]\n...\nimport-rules= \n\t# yaml format here\n\t- module_one: [\n\t\tallow module_two,\n\t\tdeny any\n\t]\n\t- module_two: [\n\t\tdeny module_one.sub.submodule\n\t]\n\t- module_two.sumbodule: deny module_one\n\t- module_three: allow any\n\n\t# many section for the same module are allowed\n\t# for example\n\t- module_two: [\n\t\tdeny some_other_module\n\t]\n\n\t# this will prevent any import everywhere\n\t- any: [\n\t\tdeny any\n\t]\n\n\t# default behaviour is\n\t- any: [\n\t\tallow any\n\t]\n\n...\n```\nRules are checking top-down. The Order Matters.\n\nIf current module name match section name or is submodule, then it will check all imports by rules from the section.\n\nThere can be one or more rules in section.\nThere can be one or more sections for the same module/submodule.\n\n`allow modulepath` - means allow imports from `modulepath` and its submodules\n\n`deny modulepath` - means deny imports from `modulepath` and its submodules.\n\nKeyword `any` (or `all`) - menas any module (like `*`)\n\nCAUTION. As .INI configparser ignores indentation use `[ ... , .. ]` flow for lists as in example.\n",
+    'long_description': 'Helps to prevent import of certain modules from certain modules.\n\nIt\'s useful if you have many modules in your project and want to keep them kind of\nisolated.\n\nAfter installing just add `import-rules` option to your `setup.cfg` file.\n\n```\n[flake8]\n...\nimport-rules= \n\t# yaml format here\n\t- module_one: [\n\t\tmodule_two allow,\n\t\tany deny\n\t]\n\t- module_two: [\n\t\tmodule_one.sub.submodule deny\n\t]\n\t- module_two.sumbodule: module_one deny\n\t- module_three: any allow\n\n\t# many section for the same module are allowed\n\t# for example\n\t- module_two: [\n\t\tdeny some_other_module\n\t]\n\n\t# this will prevent any import everywhere\n\t- any: [\n\t\tany deny\n\t]\n\n\t# default behaviour is\n\t- any: [\n\t\tany allow\n\t]\n\n\t# For each module (among foo bar baz) allow import from self submodules \n\t# and top module of others but not from submodules\n\t- X | Y | foo | bar | baz : [\n\t\tY.ANY deny,\n\t\tY     allow,\n\t\tX \t  allow\n\n\t]\n\n...\n```\nRules are checking top-down. The Order Matters.\n\nIf current module name match section name or is submodule, then it will check all imports by rules from the section.\n\nThere can be one or more rules in section.\nThere can be one or more sections for the same module/submodule.\n\n`modulepath allow` - means allow imports from `modulepath` and its submodules\n\n`modulepath deny` - means deny imports from `modulepath` and its submodules.\n\nKeyword `any` or `ANY` or `all` or `ALL` - menas any module (like `*`)\n\nTo combine different module paths in one rule we can use `|` symbol. For example\nto define rule for foo.hi foo.low bar.hi bar.low we can use \n`foo|bar.hi|low` . \n\nWe can "define" variable that will be valid only during one section and its rules.\n```\nA | B | foo | bar | baz : [\n\t...\n]\n```\nmeans if current module name is foo or bar or baz then A is equal to current module name\nand B will correspond other names from group foo|bar|baz without current module name.\n\nVariable name can be only single uppercase character. You can use variable name in section rule and inside section.\n\nYou can use variables for different module level for example\n\n```\nX|mod_a|mod_b.domain.Y : [\n\tX.infra.Y allow\n\tX.infra.ANY deny\n]\n```\n\n   \nCAUTION. As .INI configparser ignores indentation use `[ ... , .. ]` flow for lists as in example.\n\n',
     'author': 'VL',
     'author_email': '1844144@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'entry_points': entry_points,
```


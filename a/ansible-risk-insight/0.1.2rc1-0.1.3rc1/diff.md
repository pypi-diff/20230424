# Comparing `tmp/ansible-risk-insight-0.1.2rc1.tar.gz` & `tmp/ansible-risk-insight-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.2rc1.tar", last modified: Mon Apr 10 02:38:49 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.3rc1.tar", last modified: Mon Apr 24 08:03:28 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.2rc1.tar` & `ansible-risk-insight-0.1.3rc1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.711360 ansible-risk-insight-0.1.2rc1/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.640038 ansible-risk-insight-0.1.2rc1/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.650149 ansible-risk-insight-0.1.2rc1/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.2rc1/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.711165 ansible-risk-insight-0.1.2rc1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.662224 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-10 02:37:44.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.666080 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673412 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9100 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.673765 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7085 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.676236 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31556 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-10 01:04:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    10390 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    59635 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    73975 2023-04-10 01:06:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5452 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    40173 2023-04-10 02:35:50.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8059 2023-04-04 15:35:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.695936 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4041 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-03 07:57:55.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46105 2023-04-04 16:17:13.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38570 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.663637 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-10 02:38:49.000000 ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.2rc1/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.641546 ansible-risk-insight-0.1.2rc1/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.698915 ansible-risk-insight-0.1.2rc1/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.701207 ansible-risk-insight-0.1.2rc1/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.2rc1/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.2rc1/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706182 ansible-risk-insight-0.1.2rc1/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.2rc1/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.706828 ansible-risk-insight-0.1.2rc1/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707275 ansible-risk-insight-0.1.2rc1/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707614 ansible-risk-insight-0.1.2rc1/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.2rc1/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.2rc1/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-10 01:10:25.000000 ansible-risk-insight-0.1.2rc1/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-10 02:38:49.711431 ansible-risk-insight-0.1.2rc1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.2rc1/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.707948 ansible-risk-insight-0.1.2rc1/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.2rc1/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643942 ansible-risk-insight-0.1.2rc1/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643004 ansible-risk-insight-0.1.2rc1/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.708757 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643287 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.643774 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709171 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709470 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.709826 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644092 ansible-risk-insight-0.1.2rc1/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.644604 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710133 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710436 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-10 02:38:49.710765 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.2rc1/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.2rc1/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.217209 ansible-risk-insight-0.1.3rc1/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.161154 ansible-risk-insight-0.1.3rc1/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.166636 ansible-risk-insight-0.1.3rc1/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.3rc1/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.3rc1/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.3rc1/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-24 08:03:28.217038 ansible-risk-insight-0.1.3rc1/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.3rc1/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.176254 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-04-04 07:16:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      663 2023-04-24 08:02:04.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.180502 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.184906 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9158 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   828053 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.185082 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.189904 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31556 2023-04-06 00:58:38.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46548 2023-04-13 17:26:40.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8581 2023-03-14 05:38:52.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    10390 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-04-03 01:42:18.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    59746 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    74033 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    40317 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8092 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.204636 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4088 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4543 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2487 2023-02-15 09:31:38.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-03-03 02:42:12.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46781 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-04-20 11:06:45.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24554 2023-04-03 01:14:59.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.178798 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-04-24 08:03:28.000000 ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.3rc1/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.161925 ansible-risk-insight-0.1.3rc1/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.207631 ansible-risk-insight-0.1.3rc1/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.3rc1/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.3rc1/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.3rc1/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.3rc1/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.209634 ansible-risk-insight-0.1.3rc1/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.3rc1/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.3rc1/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.3rc1/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.3rc1/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.213069 ansible-risk-insight-0.1.3rc1/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.3rc1/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.213591 ansible-risk-insight-0.1.3rc1/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.213914 ansible-risk-insight-0.1.3rc1/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.3rc1/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.3rc1/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.214192 ansible-risk-insight-0.1.3rc1/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.3rc1/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.3rc1/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.3rc1/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      977 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.3rc1/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-04-24 08:03:28.217259 ansible-risk-insight-0.1.3rc1/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.3rc1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.214436 ansible-risk-insight-0.1.3rc1/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.3rc1/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.163117 ansible-risk-insight-0.1.3rc1/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.162646 ansible-risk-insight-0.1.3rc1/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.215305 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.162797 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.163026 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.215571 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.215760 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.216057 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.163171 ansible-risk-insight-0.1.3rc1/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.163399 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.216295 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.216502 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-04-24 08:03:28.216692 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.3rc1/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.3rc1/tox.ini
```

### Comparing `ansible-risk-insight-0.1.2rc1/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.3rc1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/.github/workflows/test.yml` & `ansible-risk-insight-0.1.3rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/.gitignore` & `ansible-risk-insight-0.1.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/CONTRIBUTING.md` & `ansible-risk-insight-0.1.3rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/LICENSE` & `ansible-risk-insight-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/README.md` & `ansible-risk-insight-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/yaml.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 # -*- mode:python; coding:utf-8 -*-
 
-# Copyright (c) 2022 IBM Corp. All rights reserved.
+# Copyright (c) 2023 IBM Corp. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2-rc1"
+import io
+from ruamel.yaml import YAML
+
+
+_yaml = YAML(typ="rt", pure=True)
+_yaml.default_flow_style = False
+_yaml.preserve_quotes = True
+_yaml.allow_duplicate_keys = True
+
+
+def load(stream: any):
+    return _yaml.load(stream)
+
+
+def dump(data: any):
+    output = io.StringIO()
+    _yaml.dump(data, output)
+    return output.getvalue()
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from copy import deepcopy
 from dataclasses import dataclass
 from typing import List
 from ansible_risk_insight.keyutil import detect_type
 from ansible_risk_insight.models import (
     ObjectList,
     Repository,
     Playbook,
@@ -98,16 +97,18 @@
             vars=_vars,
             resolved=True,  # TODO: False if not resolved
             templated=resolved_module_options,
             is_mutable=is_mutable,
         )
         taskcall.args = args
         # deep copy the history here because the context is updated by subsequent taskcalls
-        taskcall.variable_set = deepcopy(self.context.var_set_history)
-        taskcall.variable_use = deepcopy(self.context.var_use_history)
+        if self.context.var_set_history:
+            taskcall.variable_set = self.context.var_set_history.copy()
+        if self.context.var_use_history:
+            taskcall.variable_use = self.context.var_use_history.copy()
         taskcall.become = self.context.become
 
         return VariableAnnotatorResult()
 
 
 @dataclass
 class VariableAnnotatorResult(AnnotatorResult):
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         parser.add_argument("--taskfile-only", action="store_true", help="if true, don't load playbooks/roles arround the specified taskfile")
         parser.add_argument("--skip-install", action="store_true", help="if true, skip install for the specified target")
         parser.add_argument("--dependency-dir", nargs="?", help="path to a directory that have dependencies for the target")
         parser.add_argument("--collection-name", nargs="?", help="if provided, use it as a collection name")
         parser.add_argument("--role-name", nargs="?", help="if provided, use it as a role name")
         parser.add_argument("--source", help="source server name in ansible config file (if empty, use public ansible galaxy)")
         parser.add_argument("--without-ram", action="store_true", help="if true, RAM data is not used and not even updated")
+        parser.add_argument("--read-only-ram", action="store_true", help="if true, RAM data is used but not updated")
         parser.add_argument("--read-ram-for-dependency", action="store_true", help="if true, RAM data is used only for dependency")
         parser.add_argument("--update-ram", action="store_true", help="if true, RAM data is not used for scan but updated with the scan result")
         parser.add_argument("--include-tests", action="store_true", help='if true, load test contents in "tests/integration/targets"')
         parser.add_argument("--silent", action="store_true", help='if true, do not print anything"')
         parser.add_argument("--objects", action="store_true", help="if true, output objects.json to the output directory")
         parser.add_argument("--show-all", action="store_true", help="if true, show findings even if missing dependencies are found")
         parser.add_argument("--json", help="if specified, show findings in json format")
@@ -114,21 +115,28 @@
 
         read_ram = True
         write_ram = True
         read_ram_for_dependency = False
         if args.without_ram:
             read_ram = False
             write_ram = False
+        elif args.read_only_ram:
+            read_ram = True
+            write_ram = False
         elif args.update_ram:
             read_ram = False
             write_ram = True
         elif args.read_ram_for_dependency:
             read_ram_for_dependency = True
             read_ram = False
             write_ram = False
+        elif args.include_tests:
+            read_ram_for_dependency = True
+            read_ram = False
+            write_ram = False
 
         c = ARIScanner(
             root_dir=config.data_dir,
             rules_dir=rules_dir,
             do_save=args.save,
             read_ram=read_ram,
             write_ram=write_ram,
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/model_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1078,22 +1078,26 @@
 
     moduleObj.set_key()
 
     return moduleObj
 
 
 builtin_modules_file_name = "ansible_builtin_modules.json"
+builtin_modules = {}
 
 
 def load_builtin_modules():
+    global builtin_modules
+    if builtin_modules:
+        return builtin_modules
     base_path = os.path.dirname(__file__)
     data_path = os.path.join(base_path, builtin_modules_file_name)
     module_list = ObjectList.from_json(fpath=data_path)
-    module_dict = {m.name: m for m in module_list.items}
-    return module_dict
+    builtin_modules = {m.name: m for m in module_list.items}
+    return builtin_modules
 
 
 # modules in a SCM repo should be in `library` dir in the best practice case
 # https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html
 # however, it is often defined in `plugins/modules` directory,
 # so we search both the directories
 def load_modules(path, basedir="", collection_name="", module_dir_paths=[], use_ansible_doc=True, load_children=True):
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1994,14 +1994,15 @@
 class ModuleMetadata(object):
     fqcn: str = ""
     # arguments: list = field(default_factory=list)
     type: str = ""
     name: str = ""
     version: str = ""
     hash: str = ""
+    deprecated: bool = False
 
     @staticmethod
     def from_module(m: Module, metadata: dict):
         mm = ModuleMetadata()
         for key in mm.__dict__:
             if hasattr(m, key):
                 val = getattr(m, key, None)
@@ -2017,14 +2018,15 @@
     def from_routing(dst: str, metadata: dict):
         mm = ModuleMetadata()
         mm.fqcn = dst
         mm.type = metadata.get("type", "")
         mm.name = metadata.get("name", "")
         mm.version = metadata.get("version", "")
         mm.hash = metadata.get("hash", "")
+        mm.deprecated = True
         return mm
 
     @staticmethod
     def from_dict(d: dict):
         mm = ModuleMetadata()
         mm.fqcn = d.get("fqcn", "")
         mm.type = d.get("type", "")
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/ram_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import traceback
 import joblib
 import os
 import json
+import time
 import datetime
+import threading
 
 from .scanner import ARIScanner, config
 
 
 class RiskAssessmentModelGenerator(object):
     _queue: list = []
     _resume: int = -1
     _update: bool = False
 
+    start: float = None
+
     def __init__(
         self,
         target_list=[],
         resume=-1,
         update=False,
         parallel=True,
         download_only=False,
@@ -82,22 +86,27 @@
                 raise ValueError(f"target list must be a list of tuple(target_type, target_name), but got a {type(target_info)}")
             if len(target_info) != 2:
                 raise ValueError(f"target list must be a list of tuple(target_type, target_name), but got this; {target_info}")
 
             _type, _name = target_info
             input_list.append((i, num, _type, _name))
 
+        self.start = time.time()
+
         if self._parallel:
             joblib.Parallel(n_jobs=-1)(joblib.delayed(self.scan)(i, num, _type, _name) for (i, num, _type, _name) in input_list)
         else:
             for (i, num, _type, _name) in input_list:
                 self.scan(i, num, _type, _name)
 
     def scan(self, i, num, type, name):
-        print(f"[{i+1}/{num}] {type} {name}")
+        elapsed = round(time.time() - self.start, 2)
+        start_of_this_scan = time.time()
+        thread_id = threading.get_native_id()
+        print(f"[{i+1}/{num}] start {type} {name} ({elapsed} sec. elapsed) (thread: {thread_id})")
         use_src_cache = True
 
         if self.skip_scan(type, name):
             print(f"skip ram update of {type} {name}")
             return
         fail = False
         if self._update:
@@ -118,14 +127,18 @@
             )
         except Exception:
             error = traceback.format_exc()
             self._scanner.save_error(error)
             fail = True
         self.save_ram_log(type, name, fail)
 
+        elapsed_for_this_scan = round(time.time() - start_of_this_scan, 2)
+        if elapsed_for_this_scan > 60:
+            print(f"WARNING: It took {elapsed_for_this_scan} sec. to process [{i+1}/{num}] {type} {name}")
+
     def save_ram_log(self, type, name, fail):
         out_dir = os.path.join(self._scanner.root_dir, "log", type, name)
         path = os.path.join(out_dir, "ram_log.json")
 
         scan_time = datetime.datetime.utcnow().isoformat()
         new_record = {"type": type, "name": name, "succeed": not fail, "time": scan_time}
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/risk_assessment_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,14 @@
                 self.role_index = json.load(file)
 
         taskfile_index_path = os.path.join(self.root_dir, "indices", taskfile_index_name)
         if os.path.exists(taskfile_index_path):
             with open(taskfile_index_path, "r") as file:
                 self.taskfile_index = json.load(file)
 
-        self.init_findings_json_list_cache()
-
     def clear_old_cache(self):
         size = self.max_cache_size
         self._remove_old_item(self.findings_cache, size)
         self._remove_old_item(self.findings_search_cache, size)
         self._remove_old_item(self.module_search_cache, size)
         self._remove_old_item(self.role_search_cache, size)
         self._remove_old_item(self.taskfile_search_cache, size)
@@ -771,14 +769,16 @@
         search_patterns = os.path.join(self.root_dir, "roles", "findings", "*", "*", "*", "findings.json")
         findings_json_list_role = safe_glob(search_patterns)
         findings_json_list_role = sort_by_version(findings_json_list_role)
         findings_json_list = findings_json_list_coll + findings_json_list_role
         self.findings_json_list_cache = findings_json_list
 
     def list_all_ram_metadata(self):
+        if not self.findings_json_list_cache:
+            self.init_findings_json_list_cache()
         findings_json_list = self.findings_json_list_cache
 
         metadata_list = []
         for findings_path in findings_json_list:
             parts = findings_path.split("/")
 
             metadata_list.append(
@@ -788,14 +788,16 @@
                     "version": parts[-3],
                     "hash": parts[-2],
                 }
             )
         return metadata_list
 
     def search_findings(self, target_name, target_version, target_type=None):
+        if not self.findings_json_list_cache:
+            self.init_findings_json_list_cache()
         args_str = json.dumps([target_name, target_version, target_type])
         if args_str in self.findings_search_cache:
             return self.findings_search_cache[args_str]
 
         if not target_name:
             raise ValueError("target name must be specified for searching RAM data")
         if not target_version:
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/risk_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from .models import AnsibleRunContext, ARIResult, TargetResult, NodeResult, RuleResult, Rule, SpecMutation
 from .keyutil import detect_type, key_delimiter
 from .analyzer import load_taskcalls_in_trees
 from .utils import load_classes_in_dir
 
 
 rule_versions_filename = "rule_versions.json"
-rule_cache = []
 
 
 def key2name(key: str):
     _type = detect_type(key)
     if _type == "playbook":
         return os.path.basename(key.split(key_delimiter)[-1])
     elif _type == "role":
@@ -59,19 +58,14 @@
                 continue
             commit_id = d.get("commit_id")
             version_dict[rule_id] = commit_id
     return version_dict
 
 
 def load_rules(rules_dir: str = "", rule_id_list: list = [], fail_on_error: bool = False):
-    global rule_cache
-
-    if rule_cache:
-        return rule_cache
-
     if not rules_dir:
         return []
     rules_dir_list = rules_dir.split(":")
     _rules = []
     for _rules_dir in rules_dir_list:
         versions_file = os.path.join(_rules_dir, rule_versions_filename)
         versions_dict = {}
@@ -115,32 +109,34 @@
                 return len(_list)
 
         _rules = sorted(_rules, key=lambda r: index(rule_id_list, r))
 
     # sort by precedence
     _rules = sorted(_rules, key=lambda r: r.precedence)
 
-    rule_cache = _rules
-
     return _rules
 
 
 def make_subject_str(playbook_num: int, role_num: int):
     subject = ""
     if playbook_num > 0 and role_num > 0:
         subject = "playbooks/roles"
     elif playbook_num > 0:
         subject = "playbooks"
     elif role_num > 0:
         subject = "roles"
     return subject
 
 
-def detect(contexts: List[AnsibleRunContext], rules_dir: str = "", rules: list = []):
-    rules = load_rules(rules_dir, rules, False)
+def detect(contexts: List[AnsibleRunContext], rules_dir: str = "", rules: list = [], rules_cache: list = []):
+    loaded_rules = []
+    if rules_cache:
+        loaded_rules = rules_cache
+    else:
+        loaded_rules = load_rules(rules_dir, rules, False)
 
     playbook_count = {"total": 0, "risk_found": 0}
     role_count = {"total": 0, "risk_found": 0}
 
     data_report = {"summary": {}, "details": [], "ari_result": None}
     role_to_playbook_mappings = {}
 
@@ -173,15 +169,15 @@
                     role_to_playbook_mappings[role_name] = _mappings
         else:
             role_count["total"] += 1
 
         for t in ctx:
             ctx.current = t
             n_result = NodeResult(node=t)
-            for rule in rules:
+            for rule in loaded_rules:
                 if not rule.enabled:
                     continue
                 start_time = time.time()
                 r_result = RuleResult(file=t.file_info(), rule=rule.get_metadata())
                 try:
                     matched = rule.match(ctx)
                     if matched:
@@ -204,15 +200,15 @@
                 n_result.rules.append(r_result)
             t_result.nodes.append(n_result)
         ari_result.targets.append(t_result)
 
     data_report["ari_result"] = ari_result
     data_report["spec_mutations"] = spec_mutations
 
-    return data_report
+    return data_report, loaded_rules
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="risk_detector.py",
         description="Detect risks from tasks by checking rules",
         epilog="end",
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
             resolved_fqcn = task.spec.resolved_name
             suggested_fqcns = [cand[0] for cand in task.spec.possible_candidates]
             suggested_dependency = [cand[1] for cand in task.spec.possible_candidates]
 
             if not task.spec.resolved_name:
                 for suggestion in suggested_fqcns:
-                    if not suggestion.endswith(f".{task.spec.module}"):
+                    if suggestion != task.spec.module and not suggestion.endswith(f".{task.spec.module}"):
                         wrong_module_name = task.spec.module
                         break
                 if not task.spec.possible_candidates:
                     not_exist = True
                     wrong_module_name = task.spec.module
 
             if task.spec.resolved_name:
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
     findings: Findings = None
     result: ARIResult = None
 
     # the following are set by ARIScanner
     root_dir: str = ""
     rules_dir: str = ""
     rules: list = field(default_factory=list)
+    rules_cache: list = field(default_factory=list)
     persist_dependency_cache: bool = False
     spec_mutations_from_previous_scan: dict = field(default_factory=dict)
     spec_mutations: dict = field(default_factory=dict)
     use_ansible_doc: bool = True
     do_save: bool = False
     silent: bool = False
     _parser: Parser = None
@@ -623,15 +624,16 @@
 
     def apply_rules(self):
         target_name = self.name
         if self.collection_name:
             target_name = self.collection_name
         if self.role_name:
             target_name = self.role_name
-        data_report = detect(self.contexts, rules_dir=self.rules_dir, rules=self.rules)
+        data_report, rules_cache = detect(self.contexts, rules_dir=self.rules_dir, rules=self.rules, rules_cache=self.rules_cache)
+        self.rules_cache = rules_cache
         spec_mutations = data_report.get("spec_mutations", {})
         if spec_mutations:
             self.spec_mutations = spec_mutations
         metadata = {
             "type": self.type,
             "name": target_name,
             "version": self.version,
@@ -719,19 +721,20 @@
 @dataclass
 class ARIScanner(object):
     config: Config = None
 
     root_dir: str = ""
     rules_dir: str = ""
     rules: list = field(default_factory=list)
+    rules_cache: list = field(default_factory=list)
 
     ram_client: RAMClient = None
     read_ram: bool = True
     read_ram_for_dependency: bool = True
-    write_ram: bool = True
+    write_ram: bool = False
 
     persist_dependency_cache: bool = False
 
     skip_playbook_format_error: bool = (True,)
     skip_task_format_error: bool = (True,)
 
     use_ansible_doc: bool = True
@@ -752,15 +755,16 @@
 
         if not self.root_dir:
             self.root_dir = self.config.data_dir
         if not self.rules_dir:
             self.rules_dir = self.config.rules_dir
         if not self.rules:
             self.rules = self.config.rules
-        self.ram_client = RAMClient(root_dir=self.root_dir)
+        if not self.ram_client:
+            self.ram_client = RAMClient(root_dir=self.root_dir)
         self._parser = Parser(
             do_save=self.do_save,
             use_ansible_doc=self.use_ansible_doc,
             skip_playbook_format_error=self.skip_playbook_format_error,
             skip_task_format_error=self.skip_task_format_error,
         )
 
@@ -828,27 +832,28 @@
             taskfile_yaml=taskfile_yaml,
             taskfile_only=taskfile_only,
             include_test_contents=include_test_contents,
             out_dir=out_dir,
             root_dir=self.root_dir,
             rules_dir=self.rules_dir,
             rules=self.rules,
+            rules_cache=self.rules_cache,
             persist_dependency_cache=self.persist_dependency_cache,
             spec_mutations_from_previous_scan=spec_mutations_from_previous_scan,
             use_ansible_doc=self.use_ansible_doc,
             do_save=self.do_save,
             silent=self.silent,
             _parser=self._parser,
         )
         self._current = scandata
         self.record_end(time_records, "scandata_init")
 
         self.record_begin(time_records, "metadata_load")
         metdata_loaded = False
-        if self.read_ram:
+        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
             loaded, metadata, dependencies = self.load_metadata_from_ram(scandata.type, scandata.name, scandata.version)
             logger.debug(f"metadata loaded: {loaded}")
             if loaded:
                 scandata.set_metadata(metadata, dependencies)
                 metdata_loaded = True
                 if not self.silent:
                     logger.debug(f'Use metadata for "{scandata.name}" in RAM DB')
@@ -916,22 +921,24 @@
                             read_ram=read_ram_for_dependency,
                             read_ram_for_dependency=self.read_ram_for_dependency,
                             write_ram=self.write_ram,
                             use_ansible_doc=self.use_ansible_doc,
                             do_save=self.do_save,
                             silent=True,
                         )
+                        ext_target_path = os.path.join(self.root_dir, ext_path)
                         # use prepared dep dirs
                         dep_scanner.evaluate(
                             type=ext_type,
                             name=ext_name,
                             version=ext_ver,
                             hash=ext_hash,
-                            target_path=ext_path,
+                            target_path=ext_target_path,
                             dependency_dir=scandata.dependency_dir,
+                            install_dependencies=False,
                             skip_dependency=True,
                             source_repository=scandata.source_repository,
                             include_test_contents=include_test_contents,
                             load_only=True,
                         )
                         dep_scandata = dep_scanner.get_last_scandata()
                         scandata.ext_definitions[key] = dep_scandata.root_definitions
@@ -948,15 +955,15 @@
         # scandata.prm["playbooks"] = playbooks
         # scandata.prm["roles"] = roles
         # scandata.prm["modules"] = modules
         self.record_end(time_records, "prm_load")
 
         loaded = False
         self.record_begin(time_records, "target_load")
-        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE]:
+        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
             loaded, root_defs = self.load_definitions_from_ram(scandata.type, scandata.name, scandata.version, scandata.hash, allow_unresolved=True)
             logger.debug(f"spec data loaded: {loaded}")
             if loaded:
                 scandata.root_definitions = root_defs
                 if not self.silent:
                     logger.info("Use spec data in RAM DB")
         self.record_end(time_records, "target_load")
@@ -1010,24 +1017,27 @@
 
         self.record_begin(time_records, "apply_rules")
         scandata.apply_rules()
         self.record_end(time_records, "apply_rules")
         if not self.silent:
             logger.debug("apply_rules() done")
 
+        if scandata.rules_cache:
+            self.rules_cache = scandata.rules_cache
+
         scandata.add_time_records(time_records=time_records)
 
         dep_num, ext_counts, root_counts = scandata.count_definitions()
         if not self.silent:
             print("# of dependencies:", dep_num)
             # print("ext definitions:", ext_counts)
             # print("root definitions:", root_counts)
 
         # save RAM data
-        if self.write_ram:
+        if self.write_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
             self.register_findings_to_ram(scandata.findings)
             self.register_indices_to_ram(scandata.findings, include_test_contents)
 
         if scandata.out_dir is not None and scandata.out_dir != "":
             self.save_rule_result(scandata.findings, scandata.out_dir)
             if not self.silent:
                 print("The rule result is saved at {}".format(scandata.out_dir))
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,19 +488,21 @@
     def _recursive_get_calls(self, key, caller=None, handover={}, index=0, history=[]):
         obj_list = ObjectList()
         obj = self.get_object(key)
         if obj is None:
             return obj_list
         if key in history:
             return obj_list
-        _history = deepcopy(history)
+        _history = []
+        if history:
+            _history = [h for h in history]
         call_obj = call_obj_from_spec(spec=obj, caller=caller, index=index)
         if call_obj is not None:
             obj_list.add(call_obj, update_dict=False)
-            history.append(key)
+            _history.append(key)
         children_keys, from_ram, handover = self._get_children_keys(obj, handover_from_upper_node=handover)
         for i, c_key in enumerate(children_keys):
             child_objects = self._recursive_get_calls(
                 c_key,
                 call_obj,
                 handover,
                 i,
@@ -580,21 +582,15 @@
             obj = matched_obj.get("object", None)
             if obj is not None:
                 return obj
 
         return None
 
     def add_builtin_modules(self):
-        builtin_module_dict = {}
-        if self.ram_client and self.ram_client.builtin_modules_cache:
-            builtin_module_dict = self.ram_client.builtin_modules_cache
-        else:
-            builtin_module_dict = load_builtin_modules()
-            if self.ram_client:
-                self.ram_client.builtin_modules_cache = builtin_module_dict
+        builtin_module_dict = load_builtin_modules()
         builtin_modules = list(builtin_module_dict.values())
         obj_list = ObjectList(items=builtin_modules)
         self.ext_definitions["modules"].merge(obj_list)
 
     def _get_children_keys(self, obj, handover_from_upper_node={}):
         if isinstance(obj, CallObject):
             return self._get_children_keys(obj.spec)
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight/_version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,17 @@
 # -*- mode:python; coding:utf-8 -*-
 
-# Copyright (c) 2023 IBM Corp. All rights reserved.
+# Copyright (c) 2022 IBM Corp. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import io
-from ruamel.yaml import YAML
-
-
-_yaml = YAML(typ="rt", pure=True)
-_yaml.default_flow_style = False
-_yaml.preserve_quotes = True
-_yaml.allow_duplicate_keys = True
-
-
-def load(stream: any):
-    return _yaml.load(stream)
-
-
-def dump(data: any):
-    output = io.StringIO()
-    _yaml.dump(data, output)
-    return output.getvalue()
+__version__ = "0.1.3-rc1"
```

### Comparing `ansible-risk-insight-0.1.2rc1/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.3rc1/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/data-struct.txt` & `ansible-risk-insight-0.1.3rc1/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.3rc1/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.3rc1/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.3rc1/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.3rc1/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/annotation.md` & `ansible-risk-insight-0.1.3rc1/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/customize_rules.md` & `ansible-risk-insight-0.1.3rc1/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.3rc1/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.3rc1/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.3rc1/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.3rc1/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/example/readme.md` & `ansible-risk-insight-0.1.3rc1/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.3rc1/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/example/sample.py` & `ansible-risk-insight-0.1.3rc1/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/mkdocs.yml` & `ansible-risk-insight-0.1.3rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/pyproject.toml` & `ansible-risk-insight-0.1.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/test/test_scanner.py` & `ansible-risk-insight-0.1.3rc1/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.3rc1/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.2rc1/tox.ini` & `ansible-risk-insight-0.1.3rc1/tox.ini`

 * *Files identical despite different names*


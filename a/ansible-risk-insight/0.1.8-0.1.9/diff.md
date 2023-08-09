# Comparing `tmp/ansible-risk-insight-0.1.8.tar.gz` & `tmp/ansible-risk-insight-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.8.tar", last modified: Fri Jul 28 01:06:20 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.9.tar", last modified: Wed Aug  2 05:22:48 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.8.tar` & `ansible-risk-insight-0.1.9.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.252075 ansible-risk-insight-0.1.8/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.189841 ansible-risk-insight-0.1.8/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.196356 ansible-risk-insight-0.1.8/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.8/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.8/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.8/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-07-28 01:06:20.251912 ansible-risk-insight-0.1.8/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.8/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.208687 ansible-risk-insight-0.1.8/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      659 2023-07-28 01:06:04.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.211981 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.218447 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     3312 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.218664 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.221072 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-05-19 01:44:23.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31842 2023-06-05 06:59:18.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46758 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8612 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2508 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    60897 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    76012 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24418 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    44597 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8525 2023-07-28 01:05:55.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.235170 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-07-06 08:35:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6571 2023-06-05 06:59:18.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6188 2023-07-18 01:54:22.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     3036 2023-04-28 09:03:05.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    47220 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    39915 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24586 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)     1209 2023-07-28 01:05:55.000000 ansible-risk-insight-0.1.8/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.209741 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      272 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       91 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-07-28 01:06:20.000000 ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.8/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.190755 ansible-risk-insight-0.1.8/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.237780 ansible-risk-insight-0.1.8/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.8/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.8/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.8/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.8/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.239645 ansible-risk-insight-0.1.8/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.8/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.8/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.8/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.8/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.242770 ansible-risk-insight-0.1.8/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.8/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.243265 ansible-risk-insight-0.1.8/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.243574 ansible-risk-insight-0.1.8/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.8/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.8/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.247712 ansible-risk-insight-0.1.8/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.8/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.8/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.8/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      993 2023-07-27 07:55:44.000000 ansible-risk-insight-0.1.8/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-07-28 01:06:20.252128 ansible-risk-insight-0.1.8/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.8/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.248297 ansible-risk-insight-0.1.8/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.8/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.191964 ansible-risk-insight-0.1.8/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.191497 ansible-risk-insight-0.1.8/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.249055 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.191645 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.191872 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.249639 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.249880 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.250837 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.192080 ansible-risk-insight-0.1.8/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.192406 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.251051 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.251314 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-28 01:06:20.251573 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.8/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.8/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.318572 ansible-risk-insight-0.1.9/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.256755 ansible-risk-insight-0.1.9/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.263975 ansible-risk-insight-0.1.9/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.9/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.9/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.9/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2023-08-02 05:22:48.318415 ansible-risk-insight-0.1.9/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.9/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.276707 ansible-risk-insight-0.1.9/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      659 2023-08-02 05:22:40.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.281705 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.288964 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     2964 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.289171 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.291772 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-05-19 01:44:23.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31842 2023-06-05 06:59:18.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    47374 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)    10537 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15798 2023-08-02 05:17:47.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2683 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    61644 2023-08-02 05:17:47.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    80272 2023-08-02 05:17:47.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24587 2023-08-02 05:17:45.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    44716 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8376 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.306114 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-07-06 08:35:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6571 2023-06-05 06:59:18.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6188 2023-07-18 01:54:22.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3036 2023-04-28 09:03:05.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    48331 2023-08-01 08:03:03.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    41309 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24616 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1226 2023-08-02 05:20:18.000000 ansible-risk-insight-0.1.9/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.278525 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      103 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-08-02 05:22:48.000000 ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.9/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.257608 ansible-risk-insight-0.1.9/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.309814 ansible-risk-insight-0.1.9/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.9/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.9/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.9/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.9/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.311996 ansible-risk-insight-0.1.9/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.9/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.9/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.9/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.9/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.314958 ansible-risk-insight-0.1.9/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.9/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.315438 ansible-risk-insight-0.1.9/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.315714 ansible-risk-insight-0.1.9/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.9/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.9/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.315976 ansible-risk-insight-0.1.9/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.9/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.9/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.9/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1012 2023-08-01 01:36:12.000000 ansible-risk-insight-0.1.9/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-08-02 05:22:48.318617 ansible-risk-insight-0.1.9/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.9/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.316258 ansible-risk-insight-0.1.9/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.9/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.258977 ansible-risk-insight-0.1.9/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.258451 ansible-risk-insight-0.1.9/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.316858 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.258622 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.258881 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.317153 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.317357 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.317541 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.259037 ansible-risk-insight-0.1.9/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.259288 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.317745 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.317917 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-02 05:22:48.318105 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.9/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.9/tox.ini
```

### Comparing `ansible-risk-insight-0.1.8/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/.github/workflows/test.yml` & `ansible-risk-insight-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/.gitignore` & `ansible-risk-insight-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/CONTRIBUTING.md` & `ansible-risk-insight-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/LICENSE` & `ansible-risk-insight-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/README.md` & `ansible-risk-insight-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.9/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.9/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/awx_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,26 +44,14 @@
                     matched = True
                     break
     except IOError:
         return False
     return matched
 
 
-def could_be_taskfile(fpath):
-    if could_be_playbook(fpath):
-        return False
-    with codecs.open(fpath, "r", encoding="utf-8", errors="ignore") as f:
-        for n, line in enumerate(f):
-            if "- name: " in line:
-                return True
-            if "ansible.builtin." in line:
-                return True
-    return False
-
-
 # this method is based on awx code
 # awx/main/models/projects.py#L206-L217 in ansible/awx
 def search_playbooks(root_path):
     results = []
     if root_path and os.path.exists(root_path):
         for dirpath, dirnames, filenames in os.walk(root_path, followlinks=False):
             if skip_directory(dirpath):
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.9/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.9/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
 
 @dataclass
 class Dependency(object):
     dir: str = ""
     name: str = ""
     metadata: DownloadMetadata = field(default_factory=DownloadMetadata)
+    is_local_dir: bool = False
 
 
 @dataclass
 class DependencyDirPreparator(object):
     root_dir: str = ""
     source_repository: str = ""
     target_type: str = ""
@@ -293,28 +294,31 @@
                     fullpath = os.path.join(sub_dependency_dir_path, "ansible_collections", parts[0], parts[1])
                     downloaded_dep.dir = fullpath.replace(f"{self.root_dir}/", "")
                 self.dependency_dirs.append(asdict(downloaded_dep))
 
         if role_dependencies:
             for rdep in role_dependencies:
                 target_version = None
+                is_local_dir = False
                 if isinstance(rdep, dict):
                     rdep_name = rdep.get("name", None)
                     target_version = rdep.get("version", None)
                     if not rdep_name:
                         rdep_name = rdep.get("role", None)
+                    is_local_dir = rdep.get("is_local_dir", False)
                     rdep = rdep_name
                 name = rdep
                 if type(rdep) is dict:
                     name = rdep.get("name", "")
                     if name == "":
                         name = rdep.get("src", "")
                 logger.debug("prepare dir for {}".format(name))
                 downloaded_dep = Dependency(
                     name=name,
+                    is_local_dir=is_local_dir,
                 )
                 downloaded_dep.metadata.type = LoadType.ROLE
                 downloaded_dep.metadata.name = name
                 downloaded_dep.metadata.cache_enabled = cache_enabled
                 # sub_dependency_dir_path = "{}/{}".format(dependency_dir_path, rdep)
 
                 sub_dependency_dir_path = os.path.join(
@@ -322,15 +326,17 @@
                     "roles",
                     "src",
                     name,
                 )
 
                 if not os.path.exists(sub_dependency_dir_path):
                     os.makedirs(sub_dependency_dir_path)
-                if cache_enabled:
+                if is_local_dir:
+                    downloaded_dep.is_local_dir = is_local_dir
+                elif cache_enabled:
                     logger.debug("cache enabled")
                     cache_dir_path = os.path.join(
                         cache_dir,
                         "roles",
                         name,
                     )
                     download_meta_dir_path = os.path.join(
@@ -341,16 +347,19 @@
                     if os.path.exists(cache_dir_path) and len(os.listdir(cache_dir_path)) != 0:
                         logger.debug("dependency cache data found")
                         metadata_file = os.path.join(download_meta_dir_path, download_metadata_file)
                         md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
                         self.move_src(cache_dir_path, sub_dependency_dir_path)
                     else:
                         logger.debug("dependency cache data not found")
-                        install_msg = install_galaxy_target(name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository, target_version)
+                        install_msg, install_err = install_galaxy_target(
+                            name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository, target_version
+                        )
                         logger.debug("role install msg: {}".format(install_msg))
+                        logger.debug("role install msg err: {}".format(install_err))
                         metadata = self.extract_roles_metadata(install_msg)
                         if not metadata:
                             raise ValueError("failed to install {} {}".format(LoadType.ROLE, name))
                         metadata_file = self.export_data(metadata, download_meta_dir_path, download_metadata_file)
                         md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
                         # save cache
                         if not os.path.exists(cache_dir_path):
@@ -358,16 +367,17 @@
                         self.move_src(sub_dependency_dir_path, cache_dir_path)
                     if md:
                         downloaded_dep.metadata = md
                 elif name in role_dependency_dirs:
                     logger.debug("use the specified dependency dirs")
                     sub_dependency_dir_path = role_dependency_dirs[name]
                 else:
-                    install_msg = install_galaxy_target(name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository)
+                    install_msg, install_err = install_galaxy_target(name, LoadType.ROLE, sub_dependency_dir_path, self.source_repository)
                     logger.debug("role install msg: {}".format(install_msg))
+                    logger.debug("role install msg err: {}".format(install_err))
                     metadata = self.extract_roles_metadata(install_msg)
                     if not metadata:
                         raise ValueError("failed to install {} {}".format(LoadType.ROLE, name))
                     sub_download_location = os.path.join(self.download_location, "role", name)
                     metadata_file = self.export_data(metadata, sub_download_location, download_metadata_file)
                     md = self.find_target_metadata(LoadType.ROLE, metadata_file, name)
                     if md is not None:
@@ -429,18 +439,19 @@
                 metadata_file = os.path.join(metafile_location, download_metadata_file)
                 md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
                 tmp_target_dir = os.path.join(tmp_src_dir, self.target_name)
                 if not os.path.exists(tmp_target_dir):
                     os.makedirs(tmp_target_dir)
                 self.move_src(sub_download_location, tmp_target_dir)
             else:
-                install_msg = install_galaxy_target(
+                install_msg, install_err = install_galaxy_target(
                     self.target_name, self.target_type, tmp_src_dir, self.source_repository, target_version=self.target_version
                 )
                 logger.debug("role install msg: {}".format(install_msg))
+                logger.debug("role install msg err: {}".format(install_err))
                 metadata = self.extract_roles_metadata(install_msg)
                 if not metadata:
                     raise ValueError("failed to install {} {}".format(self.target_type, self.target_name))
                 metadata_file = self.export_data(metadata, metafile_location, download_metadata_file)
                 md = self.find_target_metadata(LoadType.ROLE, metadata_file, self.target_name)
                 # save cache
                 if not os.path.exists(sub_download_location):
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/dependency_finder.py`

 * *Files 22% similar despite different names*

```diff
@@ -88,14 +88,44 @@
                         metadata = yaml.safe_load(file)
                     except Exception as e:
                         logger.debug("failed to load this yaml file to read metadata; {}".format(e.args[0]))
 
                     if metadata is not None and isinstance(metadata, dict):
                         requirements["roles"] = metadata.get("dependencies", [])
                         requirements["collections"] = metadata.get("collections", [])
+
+    # remove local dependencies
+    role_reqs = requirements.get("roles", [])
+    if role_reqs:
+        updated_role_reqs = []
+        _target = target[:-1] if target[-1] == "/" else target
+        base_dir = os.path.dirname(_target)
+        for r_req in role_reqs:
+            r_req_name = ""
+            if isinstance(r_req, str):
+                r_req_name = r_req
+            elif isinstance(r_req, dict):
+                r_req_name = r_req.get("role", "")
+                if not r_req_name and "name" in r_req:
+                    r_req_name = r_req.get("name", "")
+            # if role dependency name does not have ".", it should be a local dependency
+            is_local_dir = False
+            if "." not in r_req_name:
+                r_req_dir = os.path.join(base_dir, r_req_name)
+                if os.path.exists(r_req_dir):
+                    is_local_dir = True
+            # or, it can be written as `<collection_name>.<role_name>`
+            if "." in r_req_name:
+                r_short_name = r_req_name.split(".")[-1]
+                r_req_dir = os.path.join(base_dir, r_short_name)
+                if os.path.exists(r_req_dir):
+                    r_req_name = r_short_name
+                    is_local_dir = True
+            updated_role_reqs.append({"name": r_req_name, "is_local_dir": is_local_dir})
+        requirements["roles"] = updated_role_reqs
     return requirements, main_yaml
 
 
 def find_collection_dependency(target):
     requirements = {}
     # collection dir installed by ansible-galaxy command
     manifest_json_files = safe_glob(os.path.join(target, "**", collection_manifest_json), recursive=True)
@@ -134,26 +164,50 @@
         with open(requirements_yml_path, "r") as file:
             try:
                 requirements = yaml.safe_load(file)
             except Exception as e:
                 logger.debug("failed to load requirements.yml; {}".format(e.args[0]))
     else:
         requirements, yaml_path = load_dependency_from_galaxy(path)
+    # sometimes there is empty requirements.yml
+    # if so, we set empty dict as requirements instead of `None`
+    if not requirements:
+        requirements = {}
     return requirements, yaml_path
 
 
+def is_galaxy_yml(path):
+    if not os.path.exists(path):
+        return False
+
+    metadata = None
+    try:
+        with open(path, "r") as file:
+            metadata = yaml.safe_load(file)
+    except Exception:
+        pass
+
+    if not isinstance(metadata, dict):
+        return False
+
+    if "name" in metadata and "namespace" in metadata:
+        return True
+
+    return False
+
+
 def load_dependency_from_galaxy(path):
     requirements = {}
     yaml_path = ""
     galaxy_yml_files = safe_glob(os.path.join(path, "**", galaxy_yml), recursive=True)
     galaxy_yml_files.extend(safe_glob(os.path.join(path, "**", GALAXY_yml), recursive=True))
     logger.debug("found meta files {}".format(galaxy_yml_files))
     if len(galaxy_yml_files) > 0:
         for g in galaxy_yml_files:
-            if os.path.exists(g):
+            if is_galaxy_yml(g):
                 yaml_path = g
                 metadata = {}
                 with open(g, "r") as file:
                     metadata = yaml.safe_load(file)
                     dependencies = metadata.get("dependencies", {})
                     requirements["collections"] = format_dependency_info(dependencies)
     return requirements, yaml_path
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/finder.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 
 from dataclasses import dataclass
 from pathlib import Path
 import re
 import os
 import yaml
+import traceback
 
 try:
     # if `libyaml` is available, use C based loader for performance
     import _yaml  # noqa: F401
     from yaml import CSafeLoader as Loader
 except Exception:
     # otherwise, use Python based loader
@@ -298,14 +299,26 @@
         root_path = os.path.dirname(top_playbook_path)
     return root_path
 
 
 def find_collection_name_of_repo(path):
     pattern = os.path.join(path, "**/galaxy.yml")
     found_galaxy_ymls = safe_glob(pattern, recursive=True)
+
+    # skip galaxy ymls found in collections/roles in the repository
+    _galaxy_ymls = []
+    for gpath in found_galaxy_ymls:
+        relative_path = gpath.replace(path, "", 1)
+        if "/collections/" in relative_path:
+            continue
+        if "/roles/" in relative_path:
+            continue
+        _galaxy_ymls.append(gpath)
+    found_galaxy_ymls = _galaxy_ymls
+
     my_collection_name = ""
     if len(found_galaxy_ymls) > 0:
         galaxy_yml = found_galaxy_ymls[0]
         my_collection_info = None
         with open(galaxy_yml, "r") as file:
             try:
                 my_collection_info = yaml.load(file, Loader=Loader)
@@ -313,7 +326,180 @@
                 logger.debug("failed to load this yaml file to read galaxy.yml; {}".format(e.args[0]))
         if my_collection_info is None:
             return ""
         namespace = my_collection_info.get("namespace", "")
         name = my_collection_info.get("name", "")
         my_collection_name = "{}.{}".format(namespace, name)
     return my_collection_name
+
+
+def find_all_ymls(root_dir: str):
+    patterns = [os.path.join(root_dir, "**", "*.ya?ml")]
+    ymls = safe_glob(patterns)
+    return ymls
+
+
+def _get_body_data(body: str = "", data: list = None, fpath: str = ""):
+    if fpath and not body and not data:
+        try:
+            with open(fpath, "r") as file:
+                body = file.read()
+                data = yaml.safe_load(body)
+        except Exception:
+            pass
+    elif body and not data:
+        try:
+            data = yaml.safe_load(body)
+        except Exception:
+            pass
+    return body, data, fpath
+
+
+def could_be_playbook_detail(body: str = "", data: list = None, fpath: str = ""):
+    body, data, fpath = _get_body_data(body, data, fpath)
+
+    if not body:
+        return False
+
+    if len(data) == 0:
+        return False
+
+    if not isinstance(data[0], dict):
+        return False
+
+    if "hosts" in data[0]:
+        return True
+
+    if "import_playbook" in data[0] or "ansible.builtin.import_playbook" in data[0]:
+        return True
+
+    return False
+
+
+def could_be_taskfile(body: str = "", data: list = None, fpath: str = ""):
+    body, data, fpath = _get_body_data(body, data, fpath)
+
+    if not body:
+        return False
+
+    if not data:
+        return False
+
+    if not isinstance(data, list):
+        return False
+
+    if not isinstance(data[0], dict):
+        return False
+
+    if "name" in data[0]:
+        return True
+
+    module_name = find_module_name(data[0])
+    if module_name:
+        short_module_name = module_name.split(".")[-1] if "." in module_name else module_name
+        if short_module_name == "import_playbook":
+            # if the found module name is import_playbook, the file is a playbook
+            return False
+        else:
+            return True
+
+    return False
+
+
+# this function is only for empty files
+# if a target file has some contents, it should be checked with
+# some dedicated functions like `could_be_taskfile()`.
+def label_empty_file_by_path(fpath: str):
+
+    taskfile_dir = ["/tasks/", "/handlers/"]
+    for t_d in taskfile_dir:
+        if t_d in fpath:
+            return "taskfile"
+
+    playbook_dir = ["/playbooks/"]
+    for p_d in playbook_dir:
+        if p_d in fpath:
+            return "playbook"
+
+    return ""
+
+
+def get_role_info_from_path(fpath: str):
+    patterns = [
+        "/roles/",
+        "/tests/integration/targets/",
+    ]
+    targets = [
+        "/tasks/",
+        "/handlers/",
+        "/vars/",
+        "/defaults/",
+        "/meta/",
+    ]
+    role_name = ""
+    role_path = ""
+    for p in patterns:
+        found = False
+        if p in fpath:
+            relative_path = fpath.split(p, 1)[-1]
+            for t in targets:
+                if t in relative_path:
+                    role_path = relative_path.rsplit(t, 1)[0]
+                    role_name = role_path.split("/")[-1]
+                    found = True
+                    break
+        if found:
+            break
+    return role_name, role_path
+
+
+# TODO: implement this
+def get_project_info_for_file(fpath, root_dir):
+    return os.path.basename(root_dir), root_dir
+
+
+def is_meta_yml(yml_path):
+    parts = yml_path.split("/")
+    if len(parts) > 2 and parts[-2] == "meta":
+        return True
+    return False
+
+
+def is_vars_yml(yml_path):
+    parts = yml_path.split("/")
+    if len(parts) > 2 and parts[-2] in ["vars", "defaults"]:
+        return True
+    return False
+
+
+def label_yml_file(yml_path: str):
+    body = ""
+    data = None
+    error = None
+    try:
+        with open(yml_path, "r") as file:
+            body = file.read()
+    except Exception:
+        error = {"type": "FileReadError", "detail": traceback.format_exc()}
+    if error:
+        return "others", error
+
+    try:
+        data = yaml.safe_load(body)
+    except Exception:
+        error = {"type": "YAMLParseError", "detail": traceback.format_exc()}
+    if error:
+        return "others", error
+
+    label = ""
+    if not body or not data:
+        label_by_path = label_empty_file_by_path(yml_path)
+        label = label_by_path if label_by_path else "others"
+    elif data and not isinstance(data, list):
+        label = "others"
+    elif could_be_playbook(yml_path) and could_be_playbook_detail(body, data):
+        label = "playbook"
+    elif could_be_taskfile(body, data):
+        label = "taskfile"
+    else:
+        label = "others"
+    return label, None
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/findings.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 from copy import deepcopy
 from dataclasses import dataclass, field
 import jsonpickle
 from .utils import (
     lock_file,
     unlock_file,
     remove_lock_file,
@@ -62,14 +63,17 @@
                 unlock_file(lock)
                 remove_lock_file(lock)
         return json_str
 
     def save_rule_result(self, fpath=""):
         json_str = jsonpickle.encode(self.report.get("ari_result", {}), make_refs=False, unpicklable=False)
         if fpath:
+            rule_result_dir = os.path.dirname(fpath)
+            if not os.path.exists(rule_result_dir):
+                os.makedirs(rule_result_dir, exist_ok=True)
             with open(fpath, "w") as file:
                 file.write(json_str)
         return json_str
 
     @staticmethod
     def load(fpath="", json_str=""):
         if fpath:
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/model_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,23 @@
     split_target_playbook_fullpath,
     split_target_taskfile_fullpath,
     get_module_specs_by_ansible_doc,
     get_documentation_in_module_file,
     get_class_by_arg_type,
     is_test_object,
 )
-from .awx_utils import could_be_playbook, could_be_taskfile
+from .awx_utils import could_be_playbook
+from .finder import could_be_taskfile
+
 
 # collection info direcotry can be something like
 #   "brightcomputing.bcm-9.1.11+41615.gitfab9053.info"
 collection_info_dir_re = re.compile(r"^[a-z0-9_]+\.[a-z0-9_]+-[0-9]+\.[0-9]+\.[0-9]+.*\.info$")
 
-string_module_options_re = re.compile(r"^([a-z0-9]+=(?:[^ ]*{{ [^ ]+ }}[^ ]*|[^ ])+\s?)+$")
+string_module_options_re = re.compile(r"^(?:[^ ]* )([a-z0-9_]+=(?:[^ ]*{{ [^ ]+ }}[^ ]*|[^ ])+\s?)+$")
 
 loop_task_option_names = [
     "loop",
     "with_list",
     "with_items",
     "with_dict",
     # TODO: support the following
@@ -137,14 +139,31 @@
     logger.debug("start loading playbooks")
     repoObj.playbooks = load_playbooks(repo_path, basedir=basedir, include_test_contents=include_test_contents, load_children=load_children)
     logger.debug("done ... {} playbooks loaded".format(len(repoObj.playbooks)))
     logger.debug("start loading roles")
     repoObj.roles = load_roles(
         repo_path, basedir=basedir, use_ansible_doc=use_ansible_doc, include_test_contents=include_test_contents, load_children=load_children
     )
+    # in case the target project is a role
+    if os.path.exists(os.path.join(repo_path, "tasks")):
+        role_name = os.path.basename(repo_path)
+        role = load_role(
+            path=repo_path,
+            name=role_name,
+            collection_name=my_collection_name,
+            basedir=basedir,
+            use_ansible_doc=use_ansible_doc,
+            include_test_contents=include_test_contents,
+            load_children=load_children,
+        )
+        if role:
+            if load_children:
+                repoObj.roles.append(role)
+            else:
+                repoObj.roles.append(role.defined_in)
     logger.debug("done ... {} roles loaded".format(len(repoObj.roles)))
     logger.debug("start loading modules (that are defined in this repository)")
     repoObj.modules = load_modules(
         repo_path,
         basedir=basedir,
         collection_name=repoObj.my_collection_name,
         use_ansible_doc=use_ansible_doc,
@@ -600,16 +619,16 @@
     return pbObj
 
 
 def load_playbooks(path, basedir="", skip_playbook_format_error=True, skip_task_format_error=True, include_test_contents=False, load_children=True):
     if path == "":
         return []
     patterns = [
-        os.path.join(path, "/*.ya?ml"),
-        os.path.join(path, "/playbooks/**/*.ya?ml"),
+        os.path.join(path, "*.ya?ml"),
+        os.path.join(path, "playbooks/**/*.ya?ml"),
     ]
     if include_test_contents:
         patterns.append(os.path.join(path, "tests/**/*.ya?ml"))
         patterns.append(os.path.join(path, "molecule/**/*.ya?ml"))
     candidates = safe_glob(patterns, recursive=True)
     playbooks = []
     playbook_names = []
@@ -820,15 +839,15 @@
     if include_test_contents:
         patterns.extend([tests_dir_path + "/**/*.ya?ml"])
     task_yaml_files = safe_glob(patterns, recursive=True)
 
     taskfiles = []
     for task_yaml_path in task_yaml_files:
         tf = None
-        if not could_be_taskfile(task_yaml_path):
+        if not could_be_taskfile(fpath=task_yaml_path):
             continue
         try:
             tf = load_taskfile(
                 task_yaml_path,
                 role_name=fqcn,
                 collection_name=collection_name,
                 basedir=basedir,
@@ -1200,15 +1219,22 @@
         if k == "name":
             task_name = v
         if k == module_name:
             module_options = v
         else:
             task_options.update({k: v})
 
-    taskObj.set_yaml_lines(fullpath=fullpath, yaml_lines=yaml_lines, task_name=task_name, module_name=module_name, module_options=module_options)
+    taskObj.set_yaml_lines(
+        fullpath=fullpath,
+        yaml_lines=yaml_lines,
+        task_name=task_name,
+        module_name=module_name,
+        module_options=module_options,
+        task_options=task_options,
+    )
 
     # module_options can be passed as a string like below
     #
     # - name: sample of string module options
     #   ufw: port={{ item }} proto=tcp rule=allow
     #   with_items:
     #   - 5222
@@ -1227,15 +1253,15 @@
                 unknown_key = "file"
             matched_options = string_module_options_re.findall(module_options)
             if len(matched_options) == 0:
                 new_module_options[unknown_key] = module_options
             else:
                 unknown_key_val = module_options.split(matched_options[0])[0]
                 if unknown_key_val != "":
-                    new_module_options[unknown_key] = unknown_key_val
+                    new_module_options[unknown_key] = unknown_key_val.strip()
                 for p in matched_options:
                     key = p.split("=")[0]
                     val = "=".join(p.split("=")[1:])
                     new_module_options[key] = val
             module_options = new_module_options
     executable = module_name
     executable_type = ExecutableType.MODULE_TYPE
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from collections.abc import Callable
 from tabulate import tabulate
 from ruamel.yaml.scalarstring import DoubleQuotedScalarString
 
 from copy import deepcopy
 import json
 import jsonpickle
+import Levenshtein
 import ansible_risk_insight.yaml as ariyaml
 from ansible.module_utils.parsing.convert_bool import boolean
 from .keyutil import (
     set_collection_key,
     set_module_key,
     set_play_key,
     set_playbook_key,
@@ -1068,47 +1069,129 @@
     line_num_in_file: list = field(default_factory=list)  # [begin, end]
 
     # FQCN for Module and Role. Or a file path for TaskFile.  resolved later
     resolved_name: str = ""
     # candidates of resovled_name
     possible_candidates: list = field(default_factory=list)
 
-    def set_yaml_lines(self, fullpath="", yaml_lines="", task_name="", module_name="", module_options=None):
+    # embed these data when module/role/taskfile are resolved
+    module_info: dict = field(default_factory=dict)
+    include_info: dict = field(default_factory=dict)
+
+    def set_yaml_lines(self, fullpath="", yaml_lines="", task_name="", module_name="", module_options=None, task_options=None):
         if not task_name and not module_options:
             return
-        found_line_num = -1
+
         lines = []
         if yaml_lines:
             lines = yaml_lines.splitlines()
         else:
             lines = open(fullpath, "r").read().splitlines()
+
+        # search candidates that match either of the following conditions
+        #   - task name is included in the line
+        #   - if module name is included,
+        #       - if module option is string, it is included
+        #       - if module option is dict, at least one key is included
+        candidate_line_nums = []
         for i, line in enumerate(lines):
             if task_name:
                 if task_name in line:
-                    found_line_num = i
-                    break
+                    candidate_line_nums.append(i)
             elif "{}:".format(module_name) in line:
                 if isinstance(module_options, str):
                     if module_options in line:
-                        found_line_num = i
-                        break
+                        candidate_line_nums.append(i)
                 elif isinstance(module_options, dict):
                     option_matched = False
                     for key in module_options:
                         if "{}:".format(key) in lines[i + 1]:
                             option_matched = True
                             break
                     if option_matched:
-                        found_line_num = i
-                        break
-        if found_line_num < 0:
+                        candidate_line_nums.append(i)
+        if not candidate_line_nums:
             return
-        found_line = lines[found_line_num]
+
+        # get task yaml_lines for each candidate
+        candidate_blocks = []
+        for candidate_line_num in candidate_line_nums:
+            _yaml_lines, _line_num_in_file = self._find_task_block(lines, candidate_line_num)
+            if _yaml_lines and _line_num_in_file:
+                candidate_blocks.append((_yaml_lines, _line_num_in_file))
+
+        if not candidate_blocks:
+            return
+
+        reconstructed_yaml = ""
+        best_yaml_lines = ""
+        best_line_num_in_file = []
+        sorted_candidates = []
+        if len(candidate_blocks) == 1:
+            best_yaml_lines = candidate_blocks[0][0]
+            best_line_num_in_file = candidate_blocks[0][1]
+        else:
+            # reconstruct yaml from the task data to calculate similarity (edit distance) later
+            reconstructed_data = [{}]
+            if task_name:
+                reconstructed_data[0]["name"] = task_name
+            reconstructed_data[0][module_name] = module_options
+            if isinstance(task_options, dict):
+                for key, val in task_options.items():
+                    if key not in reconstructed_data[0]:
+                        reconstructed_data[0][key] = val
+
+            try:
+                reconstructed_yaml = ariyaml.dump(reconstructed_data)
+            except Exception:
+                pass
+
+            # find best match by edit distance
+            if reconstructed_yaml:
+
+                def remove_comment_lines(s):
+                    lines = s.splitlines()
+                    updated = []
+                    for line in lines:
+                        if line.strip().startswith("#"):
+                            continue
+                        updated.append(line)
+                    return "\n".join(updated)
+
+                def calc_dist(s1, s2):
+                    us1 = remove_comment_lines(s1)
+                    us2 = remove_comment_lines(s2)
+                    dist = Levenshtein.distance(us1, us2)
+                    return dist
+
+                r = reconstructed_yaml
+                sorted_candidates = sorted(candidate_blocks, key=lambda x: calc_dist(r, x[0]))
+                best_yaml_lines = sorted_candidates[0][0]
+                best_line_num_in_file = sorted_candidates[0][1]
+            else:
+                # give up here if yaml reconstruction failed
+                # use the first candidate
+                best_yaml_lines = candidate_blocks[0][0]
+                best_line_num_in_file = candidate_blocks[0][1]
+
+        self.yaml_lines = best_yaml_lines
+        self.line_num_in_file = best_line_num_in_file
+        return
+
+    def _find_task_block(self, yaml_lines: list, start_line_num: int):
+        if not yaml_lines:
+            return None, None
+
+        if start_line_num < 0:
+            return None, None
+
+        lines = yaml_lines
+        found_line = lines[start_line_num]
         is_top_of_block = found_line.replace(" ", "").startswith("-")
-        begin_line_num = found_line_num
+        begin_line_num = start_line_num
         indent_of_block = -1
         if is_top_of_block:
             indent_of_block = len(found_line.split("-")[0])
         else:
             found = False
             found_line = ""
             _indent_of_block = -1
@@ -1127,15 +1210,15 @@
                         found = True
                         found_line = _line
                         break
                 begin_line_num -= 1
                 if begin_line_num < 0:
                     break
             if not found:
-                return
+                return None, None
             indent_of_block = len(found_line.split("-")[0])
         index = begin_line_num + 1
         end_found = False
         end_line_num = -1
         for i in range(len(lines)):
             if index >= len(lines):
                 break
@@ -1149,33 +1232,39 @@
                     break
             index += 1
             if index >= len(lines):
                 end_found = True
                 end_line_num = index
                 break
         if not end_found:
-            return
+            return None, None
         if begin_line_num < 0 or end_line_num > len(lines) or begin_line_num > end_line_num:
-            return
-        self.yaml_lines = "\n".join(lines[begin_line_num : end_line_num + 1])
-        self.line_num_in_file = [begin_line_num + 1, end_line_num + 1]
-        return
+            return None, None
+
+        yaml_lines = "\n".join(lines[begin_line_num : end_line_num + 1])
+        line_num_in_file = [begin_line_num + 1, end_line_num + 1]
+        return yaml_lines, line_num_in_file
 
     # this keeps original contents like comments, indentation
     # and quotes for string as much as possible
-    def yaml(self, original_module=""):
+    def yaml(self, original_module="", use_yaml_lines=True):
+        task_data_wrapper = None
         task_data = None
-        try:
-            task_data_wrapper = ariyaml.load(self.yaml_lines)
-            task_data = task_data_wrapper[0]
-        except Exception:
-            pass
+        if use_yaml_lines:
+            try:
+                task_data_wrapper = ariyaml.load(self.yaml_lines)
+                task_data = task_data_wrapper[0]
+            except Exception:
+                pass
 
-        if not task_data:
-            return self.yaml_lines
+            if not task_data:
+                return self.yaml_lines
+        else:
+            task_data_wrapper = []
+            task_data = {}
 
         # task name
         if self.name:
             task_data["name"] = self.name
         elif "name" in task_data:
             task_data.pop("name")
 
@@ -1209,15 +1298,18 @@
             for old_key in old_keys:
                 if old_key in ["name", self.module]:
                     continue
                 if old_key not in new_keys:
                     current_to.pop(old_key)
             options_without_name = {k: v for k, v in self.options.items() if k != "name"}
             recursive_copy_dict(options_without_name, current_to)
-        task_data_wrapper[0] = current_to
+        if len(task_data_wrapper) == 0:
+            task_data_wrapper.append(current_to)
+        else:
+            task_data_wrapper[0] = current_to
         new_yaml = ariyaml.dump(task_data_wrapper)
         return new_yaml
 
     # this makes a yaml from task contents such as spec.module,
     # spec.options, spec.module_options in a fixed format
     # NOTE: this will lose comments and indentations in the original YAML
     def formatted_yaml(self):
@@ -1337,15 +1429,15 @@
         original_new_value = deepcopy(new_value)
         need_restore = False
         keys_to_be_restored = []
         if isinstance(new_value, str):
             new_value = DoubleQuotedScalarString(new_value)
             need_restore = True
         for k, v in self._task_spec.options.items():
-            if type(v) != type(old_value):
+            if type(v).__name__ != type(old_value).__name__:
                 continue
             if v != old_value:
                 continue
             self._task_spec.options[k] = new_value
             keys_to_be_restored.append(k)
         self._yaml = self._task_spec.yaml()
         self._task_spec.yaml_lines = self._yaml
@@ -1399,15 +1491,15 @@
             new_value = DoubleQuotedScalarString(new_value)
             need_restore = True
         for k in self._task_spec.module_options:
             # if `key` is specified, skip other keys
             if key and k != key:
                 continue
             value = self._task_spec.module_options[k]
-            if type(value) == type(old_value) and value == old_value:
+            if type(value).__name__ == type(old_value).__name__ and value == old_value:
                 self._task_spec.module_options[k] = new_value
                 keys_to_be_restored.append(k)
         self._yaml = self._task_spec.yaml()
         self._task_spec.yaml_lines = self._yaml
         if need_restore:
             for k in self._task_spec.module_options:
                 if k in keys_to_be_restored:
@@ -1540,14 +1632,15 @@
 
 @dataclass
 class AnsibleRunContext(object):
     sequence: RunTargetList = field(default_factory=RunTargetList)
     root_key: str = ""
     parent: Object = None
     ram_client: any = None
+    scan_metadata: dict = field(default_factory=dict)
 
     # used by rule check
     current: RunTarget = None
     _i: int = 0
 
     # used if ram generate / other data generation by loop
     last_item: bool = False
@@ -1572,57 +1665,73 @@
         self._i += 1
         return t
 
     def __getitem__(self, i):
         return self.sequence[i]
 
     @staticmethod
-    def from_tree(tree: ObjectList, parent: Object = None, last_item: bool = False, ram_client=None):
+    def from_tree(tree: ObjectList, parent: Object = None, last_item: bool = False, ram_client=None, scan_metadata=None):
         if not tree:
             return AnsibleRunContext(parent=parent, last_item=last_item)
         if len(tree.items) == 0:
             return AnsibleRunContext(parent=parent, last_item=last_item)
 
         root_key = tree.items[0].spec.key
         sequence_items = []
         for item in tree.items:
             if not isinstance(item, RunTarget):
                 continue
             sequence_items.append(item)
         tl = RunTargetList(items=sequence_items)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client)
+        return AnsibleRunContext(
+            sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client, scan_metadata=scan_metadata
+        )
 
     @staticmethod
-    def from_targets(targets: List[RunTarget], root_key: str = "", parent: Object = None, last_item: bool = False, ram_client=None):
+    def from_targets(
+        targets: List[RunTarget], root_key: str = "", parent: Object = None, last_item: bool = False, ram_client=None, scan_metadata=None
+    ):
         if not root_key:
             if len(targets) > 0:
                 root_key = targets[0].spec.key
         tl = RunTargetList(items=targets)
-        return AnsibleRunContext(sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client)
+        return AnsibleRunContext(
+            sequence=tl, root_key=root_key, parent=parent, last_item=last_item, ram_client=ram_client, scan_metadata=scan_metadata
+        )
 
     def find(self, target: RunTarget):
         for t in self.sequence:
             if t.key == target.key:
                 return t
         return None
 
     def before(self, target: RunTarget):
         targets = []
         for rt in self.sequence:
             if rt.key == target.key:
                 break
             targets.append(rt)
         return AnsibleRunContext.from_targets(
-            targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+            targets,
+            root_key=self.root_key,
+            parent=self.parent,
+            last_item=self.last_item,
+            ram_client=self.ram_client,
+            scan_metadata=self.scan_metadata,
         )
 
     def search(self, cond: AnnotationCondition):
         targets = [t for t in self.sequence if t.type == RunTargetType.Task and t.has_annotation_by_condition(cond)]
         return AnsibleRunContext.from_targets(
-            targets, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+            targets,
+            root_key=self.root_key,
+            parent=self.parent,
+            last_item=self.last_item,
+            ram_client=self.ram_client,
+            scan_metadata=self.scan_metadata,
         )
 
     def is_end(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[-1].key
 
@@ -1637,15 +1746,20 @@
     def is_begin(self, target: RunTarget):
         if len(self) == 0:
             return False
         return target.key == self.sequence[0].key
 
     def copy(self):
         return AnsibleRunContext.from_targets(
-            targets=self.sequence.items, root_key=self.root_key, parent=self.parent, last_item=self.last_item, ram_client=self.ram_client
+            targets=self.sequence.items,
+            root_key=self.root_key,
+            parent=self.parent,
+            last_item=self.last_item,
+            ram_client=self.ram_client,
+            scan_metadata=self.scan_metadata,
         )
 
     @property
     def info(self):
         if not self.root_key:
             return {}
         return get_obj_info_by_key(self.root_key)
@@ -1809,14 +1923,17 @@
     roles: list = field(default_factory=list)
     module_defaults: dict = field(default_factory=dict)
     options: dict = field(default_factory=dict)
     collections_in_play: list = field(default_factory=list)
     become: BecomeInfo = None
     variables: dict = field(default_factory=dict)
 
+    # embed this data when role is resolved
+    roles_info: list = field(default_factory=list)
+
     def set_key(self, parent_key="", parent_local_key=""):
         set_play_key(self, parent_key, parent_local_key)
 
     def children_to_key(self):
         pre_task_keys = [t.key if isinstance(t, Task) else t for t in self.pre_tasks]
         self.pre_tasks = pre_task_keys
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,17 @@
                     basedir=ld.path,
                     use_ansible_doc=self.use_ansible_doc,
                     skip_playbook_format_error=self.skip_playbook_format_error,
                     skip_task_format_error=self.skip_task_format_error,
                     include_test_contents=ld.include_test_contents,
                     load_children=False,
                 )
+                # use fqcn as role_name when the original target_name is a local path
+                if role_name != obj.fqcn:
+                    role_name = obj.fqcn
             except PlaybookFormatError:
                 if not self.skip_playbook_format_error:
                     raise
             except TaskFormatError:
                 if not self.skip_task_format_error:
                     raise
             except Exception:
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/risk_assessment_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,15 @@
         # check if the module is builtin
         matched_builtin_modules = self.search_builtin_module(name, used_in)
         if len(matched_builtin_modules) > 0:
             self.module_search_cache[args_str] = matched_builtin_modules
             return matched_builtin_modules
 
         short_name = name
+        search_name = name
         if "." in name:
             short_name = name.split(".")[-1]
 
         from_indices = False
         found_index = None
         if short_name in self.module_index and self.module_index[short_name]:
             from_indices = True
@@ -437,14 +438,15 @@
             _type = found_index.get("type", "")
             _name = found_index.get("name", "")
             _version = found_index.get("version", "")
             _hash = found_index.get("hash", "")
             findings_path = os.path.join(self.root_dir, _type + "s", "findings", _name, _version, _hash, "findings.json")
             if os.path.exists(findings_path):
                 modules_json_list.append(findings_path)
+            search_name = found_index.get("fqcn", "")
         else:
             # Do not search a module from all findings
             # when it is not found in the module index.
             # Instead, just return nothing in the case.
             pass
         matched_modules = []
         search_end = False
@@ -458,18 +460,18 @@
                     continue
                 definitions = f.root_definitions.get("definitions", {})
                 modules = definitions.get("modules", [])
                 self.findings_cache[findings_json] = definitions
             for m in modules:
                 matched = False
                 if exact_match:
-                    if m.fqcn == name:
+                    if m.fqcn == search_name:
                         matched = True
                 else:
-                    if m.fqcn == name or m.fqcn.endswith(f".{name}"):
+                    if m.fqcn == search_name or m.fqcn == name or m.fqcn.endswith(f".{short_name}"):
                         matched = True
                 if matched:
                     parts = findings_json.split("/")
 
                     matched_modules.append(
                         {
                             "type": "module",
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/risk_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 from .utils import load_classes_in_dir
 
 
 rule_versions_filename = "rule_versions.json"
 
 
 def key2name(key: str):
-    _type = detect_type(key)
-    if _type == "playbook":
-        return os.path.basename(key.split(key_delimiter)[-1])
-    elif _type == "role":
-        return key.split(key_delimiter)[-1]
+    return key.split(key_delimiter)[-1]
 
 
 def load_rule_versions_file(filepath: str):
     if not os.path.exists(filepath):
         return {}
 
     version_dict = {}
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,15 +594,21 @@
 
     def resolve_variables(self, ram_client=None):
         taskcalls_in_trees = resolve(self.trees, self.additional)
         self.taskcalls_in_trees = taskcalls_in_trees
 
         for i, tree in enumerate(self.trees):
             last_item = i + 1 == len(self.trees)
-            ctx = AnsibleRunContext.from_tree(tree=tree, parent=self.target_object, last_item=last_item, ram_client=ram_client)
+            scan_metadata = {
+                "type": self.type,
+                "name": self.name,
+            }
+            ctx = AnsibleRunContext.from_tree(
+                tree=tree, parent=self.target_object, last_item=last_item, ram_client=ram_client, scan_metadata=scan_metadata
+            )
             self.contexts.append(ctx)
 
         if self.do_save:
             root_def_dir = self.__path_mappings["root_definitions"]
             tasks_in_t_path = os.path.join(root_def_dir, "tasks_in_trees.json")
             tasks_in_t_lines = []
             for d in taskcalls_in_trees:
@@ -853,15 +859,18 @@
             _parser=self._parser,
         )
         self._current = scandata
         self.record_end(time_records, "scandata_init")
 
         self.record_begin(time_records, "metadata_load")
         metdata_loaded = False
-        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
+        read_root_from_ram = (
+            self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT] and not is_local_path(scandata.name)
+        )
+        if read_root_from_ram:
             loaded, metadata, dependencies = self.load_metadata_from_ram(scandata.type, scandata.name, scandata.version)
             logger.debug(f"metadata loaded: {loaded}")
             if loaded:
                 scandata.set_metadata(metadata, dependencies)
                 metdata_loaded = True
                 if not self.silent:
                     logger.debug(f'Use metadata for "{scandata.name}" in RAM DB')
@@ -883,35 +892,50 @@
                 [
                     (
                         d.get("metadata", {}).get("type", ""),
                         d.get("metadata", {}).get("name", ""),
                         d.get("metadata", {}).get("version", ""),
                         d.get("metadata", {}).get("hash", ""),
                         d.get("dir"),
+                        d.get("is_local_dir", False),
                     )
                     for d in scandata.loaded_dependency_dirs
                 ]
             )
             ext_count = len(ext_list)
 
             # Start ARI Scanner main flow
             self.record_begin(time_records, "dependency_load")
-            for i, (ext_type, ext_name, ext_ver, ext_hash, ext_path) in enumerate(ext_list):
+            for i, (ext_type, ext_name, ext_ver, ext_hash, ext_path, is_local_dir) in enumerate(ext_list):
                 if not self.silent:
                     if i == 0:
                         logger.info("start loading {} {}(s)".format(ext_count, ext_type))
                     logger.info("[{}/{}] {} {}".format(i + 1, ext_count, ext_type, ext_name))
 
                 # avoid infinite loop
                 is_root = False
                 if scandata.type == ext_type and scandata.name == ext_name:
                     is_root = True
 
+                ext_target_path = os.path.join(self.root_dir, ext_path)
+                role_name_for_local_dep = ""
+                # if a dependency is a local role, set the local path
+                if scandata.type == LoadType.ROLE and ext_type == LoadType.ROLE:
+                    if is_local_dir and is_local_path(scandata.name) and scandata.name != ext_name:
+                        root_role_path = scandata.name[:-1] if scandata.name[-1] == "/" else scandata.name
+                        role_base_dir = os.path.dirname(root_role_path)
+                        dep_role_path = os.path.join(role_base_dir, ext_name)
+                        role_name_for_local_dep = ext_name
+                        ext_name = dep_role_path
+                        ext_target_path = dep_role_path
+
                 if not is_root:
                     key = "{}-{}".format(ext_type, ext_name)
+                    if role_name_for_local_dep:
+                        key = "{}-{}".format(ext_type, role_name_for_local_dep)
                     read_ram_for_dependency = self.read_ram or self.read_ram_for_dependency
 
                     dep_loaded = False
                     if read_ram_for_dependency:
                         # searching findings from ARI RAM and use them if found
                         dep_loaded, ext_defs = self.load_definitions_from_ram(ext_type, ext_name, ext_ver, ext_hash)
                         if dep_loaded:
@@ -929,15 +953,14 @@
                             read_ram=read_ram_for_dependency,
                             read_ram_for_dependency=self.read_ram_for_dependency,
                             write_ram=self.write_ram,
                             use_ansible_doc=self.use_ansible_doc,
                             do_save=self.do_save,
                             silent=True,
                         )
-                        ext_target_path = os.path.join(self.root_dir, ext_path)
                         # use prepared dep dirs
                         dep_scanner.evaluate(
                             type=ext_type,
                             name=ext_name,
                             version=ext_ver,
                             hash=ext_hash,
                             target_path=ext_target_path,
@@ -964,15 +987,15 @@
         # scandata.prm["playbooks"] = playbooks
         # scandata.prm["roles"] = roles
         # scandata.prm["modules"] = modules
         self.record_end(time_records, "prm_load")
 
         loaded = False
         self.record_begin(time_records, "target_load")
-        if self.read_ram and scandata.type not in [LoadType.PLAYBOOK, LoadType.TASKFILE, LoadType.PROJECT]:
+        if read_root_from_ram:
             loaded, root_defs = self.load_definitions_from_ram(scandata.type, scandata.name, scandata.version, scandata.hash, allow_unresolved=True)
             logger.debug(f"spec data loaded: {loaded}")
             if loaded:
                 scandata.root_definitions = root_defs
                 if not self.silent:
                     logger.info("Use spec data in RAM DB")
         self.record_end(time_records, "target_load")
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     Role,
     Task,
     TaskFile,
     ExecutableType,
     LoadType,
     CallObject,
     TaskCall,
+    PlayCall,
+    RoleCall,
     call_obj_from_spec,
 )
 from .model_loader import load_builtin_modules
 from .risk_assessment_model import RAMClient
 from .variable_manager import VariableManager
 
 
@@ -548,26 +550,54 @@
                     if taskcall.spec.executable_type == ExecutableType.MODULE_TYPE:
                         taskcall.module = c_obj.spec
                         if c_key in from_ram:
                             req_info = from_ram[c_key]
                             taskcall.spec.possible_candidates = [(c_obj.spec.fqcn, req_info)]
                         else:
                             taskcall.spec.resolved_name = c_obj.spec.fqcn
+                        taskcall.spec.module_info = {
+                            "collection": c_obj.spec.collection,
+                            "short_name": c_obj.spec.name,
+                            "fqcn": c_obj.spec.fqcn,
+                            "key": c_obj.spec.key,
+                        }
                     elif taskcall.spec.executable_type == ExecutableType.ROLE_TYPE:
                         if c_key in from_ram:
                             req_info = from_ram[c_key]
                             taskcall.spec.possible_candidates = [(c_obj.spec.fqcn, req_info)]
                         else:
                             taskcall.spec.resolved_name = c_obj.spec.fqcn
+                        taskcall.spec.include_info = {
+                            "type": "role",
+                            "fqcn": c_obj.spec.fqcn,
+                            "path": c_obj.spec.defined_in,
+                            "key": c_obj.spec.key,
+                        }
                     elif taskcall.spec.executable_type == ExecutableType.TASKFILE_TYPE:
                         if c_key in from_ram:
                             req_info = from_ram[c_key]
                             taskcall.spec.possible_candidates = [(c_obj.spec.key, req_info)]
                         else:
                             taskcall.spec.resolved_name = c_obj.spec.key
+                        taskcall.spec.include_info = {
+                            "type": "taskfile",
+                            "path": c_obj.spec.defined_in,
+                            "key": c_obj.spec.key,
+                        }
+            elif isinstance(call_obj, PlayCall):
+                playcall = call_obj
+                if len(child_objects.items) > 0:
+                    c_obj = child_objects.items[0]
+                    if isinstance(c_obj, RoleCall):
+                        role_info = {
+                            "fqcn": c_obj.spec.fqcn,
+                            "path": c_obj.spec.defined_in,
+                            "key": c_obj.spec.key,
+                        }
+                        playcall.spec.roles_info.append(role_info)
             for c_obj in child_objects.items:
                 obj_list.add(c_obj)
         return obj_list
 
     def _recursive_make_graph(self, key, graph, _objects, caller=None):
         current_graph = [g for g in graph]
         # if this key is already in the graph src, no need to trace children
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "ansible-galaxy {} install {} {} -p {}".format(target_type, target_name, server_option, output_dir),
         shell=True,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         text=True,
     )
-    return proc.stdout
+    return proc.stdout, proc.stderr
 
 
 def install_github_target(target, output_dir):
     proc = subprocess.run(
         "git clone {} {}".format(target, output_dir),
         shell=True,
         stdin=subprocess.PIPE,
@@ -568,15 +568,15 @@
     if proc.stderr and not proc.stdout:
         logger.debug(f"error while getting the documentation for modules `{fqcn_list_str}`: {proc.stderr}")
         return ""
     wrapper_dict = json.loads(proc.stdout)
     specs = {}
     for fqcn in wrapper_dict:
         doc_dict = wrapper_dict[fqcn].get("doc", {})
-        doc = yaml.safe_dump(doc_dict)
+        doc = yaml.safe_dump(doc_dict, sort_keys=False)
         examples = wrapper_dict[fqcn].get("examples", "")
         specs[fqcn] = {
             "doc": doc,
             "examples": examples,
         }
     return specs
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.9/ansible_risk_insight/yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 
 
 _yaml: ContextVar[YAML] = ContextVar("yaml")
 
 
 def _set_yaml():
     if not _yaml.get(None):
-        _yaml.set(YAML(typ="rt", pure=True))
-        _yaml.default_flow_style = False
-        _yaml.preserve_quotes = True
-        _yaml.allow_duplicate_keys = True
+        yaml = YAML(typ="rt", pure=True)
+        yaml.default_flow_style = False
+        yaml.preserve_quotes = True
+        yaml.allow_duplicate_keys = True
+        _yaml.set(yaml)
 
 
 def load(stream: any):
     _set_yaml()
     yaml = _yaml.get()
     return yaml.load(stream)
```

### Comparing `ansible-risk-insight-0.1.8/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.9/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/data-struct.txt` & `ansible-risk-insight-0.1.9/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.9/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.9/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.9/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.9/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/annotation.md` & `ansible-risk-insight-0.1.9/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/customize_rules.md` & `ansible-risk-insight-0.1.9/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.9/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.9/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.9/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.9/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/example/readme.md` & `ansible-risk-insight-0.1.9/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.9/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/example/sample.py` & `ansible-risk-insight-0.1.9/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/mkdocs.yml` & `ansible-risk-insight-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/pyproject.toml` & `ansible-risk-insight-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "PyYAML",
     "smmap",
     "tabulate",
     "requests",
     "ansible",
     "ruamel.yaml",
     "filelock",
+    "Levenshtein",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ansible_risk_insight._version.__version__"}
 
 [project.scripts]
```

### Comparing `ansible-risk-insight-0.1.8/test/test_scanner.py` & `ansible-risk-insight-0.1.9/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.9/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.8/tox.ini` & `ansible-risk-insight-0.1.9/tox.ini`

 * *Files identical despite different names*

